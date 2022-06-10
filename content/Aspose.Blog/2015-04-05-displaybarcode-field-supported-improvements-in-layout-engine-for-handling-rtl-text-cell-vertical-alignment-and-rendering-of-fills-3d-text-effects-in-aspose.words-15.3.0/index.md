---
title: 'Layout Engine for Handling RTL Text in Aspose.Words'
date: Sun, 05 Apr 2015 07:08:46 +0000
draft: false
url: /2015/04/05/displaybarcode-field-supported-improvements-in-layout-engine-for-handling-rtl-text-cell-vertical-alignment-and-rendering-of-fills-3d-text-effects-in-aspose.words-15.3.0/
author: Awais Hafeez
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---

[](http://www.aspose.com/.net/word-component.aspx)Aspose.Words 15.3.0 has been released. This month’s release contains over 138 useful new features, enhancements and bug fixes to the Aspose.Words products.

You can download the latest releases of Aspose.Words from the following links:

*   [Aspose.Words for .NET 15.3.0][1]
*   [Aspose.Words for Java 15.3.0][2]

Here is a look at just a few of the biggest features and API changes in this month’s release. For a full list of bug fixes and improvements please refer to the download pages in the links above.

*   Improvements in the layout engine for handling RTL text, text boxes, cell vertical alignment and others.
*   Improvements in import/export for all file formats.
*   Optimized output size of PDF documents for some cases.
*   Document.WarningCallback property can now send you loss of formatting warnings at anytime during document lifetime, not only during saving.
*   Fields are now updated inside DrawingML shapes.
*   ShapeRenderer.OpaqueBoundsInPoints returns the "real" shape bounds.
*   Improvements in rendering of fills, 3D text effects and others.
*   The DISPLAYBARCODE field is supported now so you can add a custom barcode generator.

## Public BarCode Generation API Introduced

The DISPLAYBARCODE field is now supported. We have introduced following entities in Aspose.Words API:

*   Added the IBarcodeGenerator interface
*   Added the BarcodeParameters class
*   Added the FieldOptions.BarcodeGenerator property.

### Usage Examples

You can find usage examples for this new "custom BarCode image generation for DISPLAYBARCODE field" feature in Aspose.Words documentation page: How to Generate a Custom BarCode Image for DISPLAYBARCODE Field

## InsertDocument Method Added to DocumentBuilder Class

The following new method inserts content of the document into the current position of DocumentBuilder's cursor

```
public Node InsertDocument(Document, ImportFormatMode);

```

### Usage Examples

You can find usage examples for this new "custom BarCode image generation for DISPLAYBARCODE field" feature in Aspose.Words documentation page: Inserting content of the Document

## DocumentBase.WarningCallback Property Added

The Document can raise warnings at an any stage of its life cycle. So, to be able to receive all the warnings, a new property was added into DocumentBase class.

```
public IWarningCallback WarningCallback

```

At the same time SaveOptions.WarningCallback is now obsolete and its usage in new code should be avoided.

## OpaqueBoundsInPoints Property and GetOpaqueRectangleInPixels Method Added to ShapeRenderer Class

New property OpaqueBoundsInPoints and method GetOpaqueRectangleInPixels have been added to ShapeRenderer class. They allow to get opaque bounds of the shape in points. Before this option was introduced it had been needed to work with raw pixel data to get this bound. This is how it works now:

```
public static void RenderNode(Node node, string filePath, ImageSaveOptions imageOptions)
{
    // This code is taken from public API samples of AW.
    // Previously to find opaque bounds of the shape the function
    // that checks every pixel of the rendered image was used.
    // For now opaque bounds is got using ShapeRenderer.GetOpaqueRectangleInPixels method.

    // If no image options are supplied, create default options.
    if (imageOptions == null)
        imageOptions = new ImageSaveOptions(FileFormatUtil.ExtensionToSaveFormat(Path.GetExtension(filePath)));

    // Store the paper color to be used on the final image and change to transparent.
    // This will cause any content around the rendered node to be removed later on.
    Color savePaperColor = imageOptions.PaperColor;
    imageOptions.PaperColor = Color.Transparent;

    // There a bug which affects the cache of a cloned node. To avoid this we instead clone the entire document including all nodes,
    // find the matching node in the cloned document and render that instead.
    Document doc = (Document)node.Document.Clone(true);
    node = doc.GetChild(NodeType.Any, node.Document.GetChildNodes(NodeType.Any, true).IndexOf(node), true);

    // Create a temporary shape to store the target node in. This shape will be rendered to retrieve
    // the rendered content of the node.
    Shape shape = new Shape(doc, ShapeType.TextBox);
    Section parentSection = (Section)node.GetAncestor(NodeType.Section);

    // Assume that the node cannot be larger than the page in size.
    shape.Width = parentSection.PageSetup.PageWidth;
    shape.Height = parentSection.PageSetup.PageHeight;
    shape.FillColor = Color.Transparent; // We must make the shape and paper color transparent.

    // Don't draw a surronding line on the shape.
    shape.Stroked = false;

    // Move up through the DOM until we find node which is suitable to insert into a Shape (a node with a parent can contain paragraph, tables the same as a shape).
    // Each parent node is cloned on the way up so even a descendant node passed to this method can be rendered.
    // Since we are working with the actual nodes of the document we need to clone the target node into the temporary shape.
    Node currentNode = node;
    while (!(currentNode.ParentNode is InlineStory || currentNode.ParentNode is Story || currentNode.ParentNode is ShapeBase))
    {
        CompositeNode parent = (CompositeNode)currentNode.ParentNode.Clone(false);
        currentNode = currentNode.ParentNode;
        parent.AppendChild(node.Clone(true));
        node = parent; // Store this new node to be inserted into the shape.
    }

    // We must add the shape to the document tree to have it rendered.
    shape.AppendChild(node.Clone(true));
    parentSection.Body.FirstParagraph.AppendChild(shape);

    // Render the shape to stream so we can take advantage of the effects of the ImageSaveOptions class.
    // Retrieve the rendered image and remove the shape from the document.
    MemoryStream stream = new MemoryStream();
    ShapeRenderer renderer = shape.GetShapeRenderer();
    renderer.Save(stream, imageOptions);
    shape.Remove();

    Rectangle crop = renderer.GetOpaqueRectangleInPixels(imageOptions.Scale, imageOptions.Resolution);

    // Load the image into a new bitmap.
    using (Bitmap renderedImage = new Bitmap(stream))
    {
        Bitmap croppedImage = new Bitmap(crop.Width, crop.Height);
        croppedImage.SetResolution(imageOptions.Resolution, imageOptions.Resolution);

        // Create the final image with the proper background color.
        using (Graphics g = Graphics.FromImage(croppedImage))
        {
            g.Clear(savePaperColor);
            g.DrawImage(renderedImage, new Rectangle(0, 0, croppedImage.Width, croppedImage.Height), crop.X, crop.Y, crop.Width, crop.Height, GraphicsUnit.Pixel);

            croppedImage.Save(filePath);
        }
    }
}

```




[1]: http://www.aspose.com/community/files/51/.net-components/aspose.words-for-.net/default.aspx
[2]: http://www.aspose.com/community/files/72/java-components/aspose.words-for-java/default.aspx





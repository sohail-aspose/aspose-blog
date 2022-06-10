---
title: 'Shape, DrawingML Classes Merged into Shape and Word Document Comparison Feature Introduced in Aspose.Words 15.2.0'
date: Wed, 11 Mar 2015 08:53:20 +0000
draft: false
url: /2015/03/11/shape-drawingml-classes-merged-into-shape-and-word-document-comparison-feature-introduced-in-aspose.words-15.2.0/
author: Awais Hafeez
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---



{{< figure align=center src="images/aspose-Words-for-net-e1378287014402.png" alt="Aspose.Words for .NET logo">}}


Aspose.Words 15.2.0 has been released. This month’s release contains over 127 useful new features, enhancements and bug fixes to the Aspose.Words products.

You can download the latest releases of Aspose.Words from the following links:

*   [Aspose.Words for .NET 15.2.0][1]
*   [Aspose.Words for Java 15.2.0][2]

Here is a look at just a few of the biggest features and API changes in this month’s release. For a full list of bug fixes and improvements please refer to the download pages in the links above.

*   Document comparison feature is introduced, see Document.Compare
*   DrawingML API breaking changes (Shape and DrawingML classes merged into Shape)
*   Implemented text justification for multiline WordArt objects
*   Implemented multi line text rendering in DrawingML text boxes, SmartArt and charts
*   Middle East languages are now rendered correctly in SmartArt and charts
*   Improved positioning of comment's balloons during rendering
*   Improved vertical text inside text boxes during rendering

## Word Document Comparison Feature Introduced

We have added Document.Compare Method in Aspose.Words 15.2.0 which compares this document with another document producing changes as number of edit and format revisions Revision. However, StructuredDocumentTag and CustomXmlMarkup document nodes are not compared at the moment. Also, Documents must not have Revisions before comparison.

### Usage Examples

You can find usage examples for this new Word document comparison feature in Aspose.Words documentation page: [How to Compare Two Word Documents][3].

## LayoutCollector will not Automatically Update Fields in Document

Fix of WORSDNET-10305 has changed behavior of layout collector class. It will not automatically update fields in the document. If user wants field updations, then this can be achieved by adding Document.UpdateFields Method after the call to layout collector class constructor.

## Aspose.Words Drawing API Changes

Aspose.Words introduces new API changes to make your life easier during working with graphic objects:

**1\.** The hugest one is removing DrawingML from the API. Now you do not need to think about graphic object markup language, Vml or DrawingML, now both of them are available through the Shape or GroupShape object in Aspose.Words document model.

Previously to loop through all single graphic objects inside your document you have to loop through two different collections of Shapes and DrawingMLs, but now everything is much easier, you need just one collection, which already contains all graphics. However, if you still need to find out the shape markup language, you can do it using public property Shape.MarkupLanguage, and depending on shape, you will get ShapeMarkupLanguage.Dml or ShapeMarkupLanguage.Vml.

Please see the following example:

```
Document doc = new Document("Document_With_Dml_And_Vml_Shapes.docx");
 
// Loop through all single shapes inside document.
foreach (Shape shape in doc.GetChildNodes(NodeType.Shape, true))
{
   Console.WriteLine(shape.MarkupLanguage);
}
 
// Loop through all group shapes inside document.
foreach (GroupShape groupShape in doc.GetChildNodes(NodeType.GroupShape, true))
{
   Console.WriteLine(groupShape.MarkupLanguage);
}
```

**1.1.** NodeType.DrawingML was removed, all graphic objects have NodeType.Shape or NodeType.GroupShape.

**1.2.** DrawingMLImageData was unified with ImageData. All that you need to do in your code it is replace DrawingMLImageData with ImageData.

**1.3.** DocumentVisitor.VisitDrawingMLStart and VisitDrawingMLEnd were removed. All that you need to do in your code it is replace them with VisitShapeStart/VisitShapeEnd.

**1.4.** DrawingML shape had Size property but now you have to use SizeInPoints like for Vml shape. Please replace DrawingML.Size with Shape.SizeInPoints.

**2\.** All shapes properties are available for Dml shapes now. Therefore, you are able to modify Dml and Vml shapes using exactly the same code:

```
NodeCollection shapes = doc.GetChildNodes(NodeType.Shape, true);
Shape shape = (Shape)doc.GetChild(NodeType.Shape, 1, true);
 
// Set some properties.
shape.FlipOrientation = FlipOrientation.Vertical;
 
shape.Rotation = 30;
```

**2.1.** Change stroke properties using the following code:

```
 // Set stroke attrs.
Stroke stroke = shape.Stroke;
stroke.On = true;
stroke.Weight = 5;
stroke.Color = Color.Red;
stroke.DashStyle = DashStyle.ShortDashDotDot;
stroke.Opacity = 0.3;
stroke.JoinStyle = JoinStyle.Miter;
stroke.EndCap = EndCap.Square;
stroke.LineStyle = ShapeLineStyle.Triple;
// Etc.
```

**2.2.** Change fill properties using the following code:

```
 Fill fill = shape.Fill;
 
// Set new colors.
fill.Color = Color.Green;
fill.Color2 = Color.Black;
 
// Etc.
```

**2.3.** Change font properties using the following code:

```
 // Get shape and work with its font props.
Shape shape = (Shape)doc.GetChild(NodeType.Shape, 1, true);
 
Font shapeFont = shape.Font;
shapeFont.Name = "Blackoak Std";
shapeFont.Size = 10;
 
// Etc.
```

**3\.** As you already know MS Word inserts new graphic objects to the document using Dml markup language, Aspose.Words does the same now. But, for backward compatibility you can use doc.CompatibilityOptions.OptimizeFor method to specify needed MS Word version. And if MS Word version is higher than Word2007 or not specified Aspose.Words inserts image using ShapeMarkupLanguage.Dml, in other cases using ShapeMarkupLanguage.Vml.

```
 Document doc = new Document();
 
DocumentBuilder builder = new DocumentBuilder(doc);
 
string testImage = TestUtil.BuildTestFileName("TestPng.png");
 
// MsWordVersion.Unspecified - shape will be inserted as Dml shape.
Shape shape = builder.InsertImage(testImage);
 
// MsWordVersion.Word2003 - shape will be inserted as Vml shape.
doc.CompatibilityOptions.OptimizeFor(MsWordVersion.Word2003);
 
shape = builder.InsertImage(testImage);
 
// MsWordVersion.Word2010 - shape will be inserted as Dml shape.
doc.CompatibilityOptions.OptimizeFor(MsWordVersion.Word2010);
 
shape = builder.InsertImage(testImage);
```

But actually, you do not need even to think about this too, because Aspose.Words smartly converts your Dml markup shape to Vml in case of using old MS Word formats.




[1]: https://downloads.aspose.com/words/net
[2]: https://downloads.aspose.com/words/java
[3]: https://docs.aspose.com/display/wordsnet/Working+with+Document#WorkingwithDocument-HowtoCompareTwoWordDocuments





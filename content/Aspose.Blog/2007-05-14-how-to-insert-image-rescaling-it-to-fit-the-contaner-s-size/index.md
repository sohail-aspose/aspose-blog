---
title: 'How to insert image, rescaling it to fit the container''s size'
date: Mon, 14 May 2007 18:57:00 +0000
draft: false
url: /2007/05/14/how-to-insert-image-rescaling-it-to-fit-the-contaner-s-size/
author: Miklovan
summary: ''
tags: ['Aspose.Words', 'fit image to container', 'fit image to table cell', 'fit image to textbox', 'scale image fit to container', 'stretch image to fit container']
categories: ['Aspose.Words Product Family']
---

Sometimes, there is a need to rescale the images so that they could comply with the overall design of the document or simply fit to page size.

The best way to do it is creating a container having the desired size and putting it to the document. The two possible candidates for containers are **table cell** or **textbox**. And the best way to mark up the place for image insertion is an image **merge field** (the filed that has the "Image:" prefix in its name).

Let's imagine that we have a document which has some table cells and texboxes, having different sizes and containing «Image:Image1» merge fields.

Now, that we have such a template -  how we can insert the images to it, so that they could be rescaled to fit the container's sizes? I have made the following simple function to assist in this process:  
`` `[C#]` ``

```
/// <summary>

/// Replace merge field of the specified name with image.

/// </summary>

/// <param name="mergefieldName">Name of the merge field, where the image should be inserted.

/// The merge field itself is destroyed in the process.

/// If the merge field name is prefixed (e.g. "Image:Image1"),

/// then the name should be specified without prefix (e.g. "Image1").</param>

/// <param name="imageFileName">fully qualified name image file.

/// <param name="builder">DocumentBuilder.</param>

/// <returns>Returns true, if the merge field with the specified name was found in the document,

/// false - if no such filed exists in the document.</returns>

private bool InsertImage(string mergeFieldName, string imageFileName, DocumentBuilder builder)

{

      // Move builder to merge field (merge field is automatically removed).

      if (builder.MoveToMergeField(mergeFieldName))

      {

            // No image resize by default.

            // (Setting size to negative values makes image to be inserted without resizing.)

            double width = -1;

            double height = -1;

 

            // Check if the image is inserted into table cell.

            Cell cell = (Cell)builder.CurrentParagraph.GetAncestor(typeof(Aspose.Words.Cell));

 

            if (cell != null)

            {

                  // Set the cell properties so that the inserted image could occupy the cell space exactly.

                  cell.CellFormat.LeftPadding = 0;

                  cell.CellFormat.RightPadding = 0;

                  cell.CellFormat.TopPadding = 0;

                  cell.CellFormat.BottomPadding = 0;

                  cell.CellFormat.WrapText = false;

                  cell.CellFormat.FitText = true;

 

                  // Get cell dimensions.

                  width = cell.CellFormat.Width;

                  height = cell.ParentRow.RowFormat.Height;

            }

 

            // Check if the image is inserted into a textbox.

            Shape shape = (Shape)builder.CurrentParagraph.GetAncestor(typeof(Aspose.Words.Drawing.Shape));

 

            if ((shape != null) && (shape.ShapeType == ShapeType.TextBox))

            {

                  // Set the textbox properties so that the inserted image could occupy the textbox space exactly.

                  shape.TextBox.InternalMarginTop = 0;

                  shape.TextBox.InternalMarginLeft = 0;

                  shape.TextBox.InternalMarginBottom = 0;

                  shape.TextBox.InternalMarginRight = 0;

 

                  // Get cell dimensions.

                  width = shape.Width;

                  height = shape.Height;

            }

 

            // Insert image with or without rescaling, based on the previously done analysis.

            builder.InsertImage(imageFileName, width, height);

 

            // Signal the caller that the image was succesfully inserted at merge field position.

            return true;

      }

      else

      {

            // Signal the caller that no merge field with the specified name could be found in the document.

            return false;

      }

}
```

As you can see this function is universal. If it discovers that image merge field is contained inside table cell - it rescales image to fit the table cell size. The table cell formatting properties are also modified, removing margins, etc., so that the inserted image could take all space inside the table cell. The same is done if the container is the textbox. If no container is found then image is inserted without rescaling, as is.

This function can generally be used in two ways - direct call like this:

```
while (InsertImage(“Image1”, imageFileName, builder));
```

Or using MailMerge process like this:

`[C#]`

```
private void MailMerge_MergeImageField(object sender, MergeImageFieldEventArgs e)
{
DocumentBuilder builder = new DocumentBuilder(e.Document);
// The code below should be adapted to your application specifics.
string imageFileName = TestUtil.BuildTestFileName("Aspose.Words.jpg");
InsertImage(e.FieldName, imageFileName, builder);
}
```

The code of **InsertImage** function can be further improved to allow different fitting policies to be applied. For example, fit width, fit height, touch container borders from inside, touch container borders from outside, fit size, shrink to fit, enlarge to fit, etc. I hope it won't present too many difficulties to implement that kind of fitting if necessary.









---
title: 'Extract Text based on Columns and Identify Image Type within PDF in C# with Aspose.PDF for .NET 9.9.0'
date: Mon, 22 Dec 2014 11:45:23 +0000
draft: false
url: /2014/12/22/extract-text-based-on-columns-from-pdf-using-csharp-asp.net/
author: Codewarior
summary: ''
tags: ['Nayyer Shahbaz', 'Aspose.Pdf for .NET', 'Extract table border in PDF', 'Extract text from multi column PDF document', 'Identify image color in PDF document']
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/aspose-Pdf-for-net_100.png" alt="Extract text from columns in PDF document">}}


We are very much excited to announce the release of [Aspose.PDF for .NET 9.9.0][1] which provides new features and empowers the developers to extract text from PDF documents. You can also extract text from multi-column PDF documents using C#. In addition, you can now extract the table borders and identify images in PDF documents. The following are some of the exciting features introduced in this release.

## Extract Text based on Columns from PDF in C#

In case we have a PDF document with more than one column (multi-column) PDF document and we need to extract the page contents while honoring the same layout, then Aspose.Pdf for .NET is the right choice to accomplish this requirement. One approach is to reduce the font size of contents inside PDF documents and then perform text extraction. The following code snippet shows how to extract text from columns in PDF using C#.

```
string path = "D:\\Temp\\";
InitLicense();
Document pdfDocument = new Document(path + "net_New-age NED's.pdf");

TextFragmentAbsorber tfa = new TextFragmentAbsorber();
pdfDocument.Pages.Accept(tfa);
TextFragmentCollection tfc = tfa.TextFragments;
foreach (TextFragment tf in tfc)
{
    //need to reduce font size at least for 70%
    tf.TextState.FontSize = tf.TextState.FontSize * 0.7f;
}
Stream st = new MemoryStream();
pdfDocument.Save(st);
pdfDocument = new Document(st);

TextAbsorber textAbsorber = new TextAbsorber();
pdfDocument.Pages.Accept(textAbsorber);
String extractedText = textAbsorber.Text;
textAbsorber.Visit(pdfDocument);

System.IO.File.WriteAllText(path + "Extracted.txt", extractedText); 
```

In this new release, we also have introduced several improvements in TextAbsorber and in the internal text formatting mechanism. So now during the text extraction using 'Pure' mode, you may specify the ScaleFactor option and it can be another approach to extract text from multi-column PDF document besides the above stated approach. This scale factor may be set to adjust grid which is used for the internal text formatting mechanism during text extraction. Specifying the ScaleFactor values between 1 and 0.1 (including 0.1) has the same effect as font reduction.

Specifying the ScaleFactor values between 0.1 and -0.1 is treated as zero value, but it makes the algorithm to calculate scale factor needed during extracting text automatically. The calculation is based on average glyph width of the most popular font on the page, but we cannot guarantee that in extracted text no string of column reaches the start of the next column. Please note that if ScaleFactor value is not specified, the default value of 1.0 will be used. It means no scaling will be carried out. If the specified ScaleFactor value is more than 10 or less than -0.1, the default value of 1.0 will be used.

We propose the usage of auto-scaling (ScaleFactor = 0) when processing large number of PDF files for text content extraction. Or manually set redundant reducing of grid width ( about ScaleFactor = 0.5). However, you must not determine whether scaling is necessary for concrete documents or not. If You set redundant reducing of grid width for the document (that doesn't need in it), the extracted text content will remain fully adequate. Please take a look over the following code snippet.

```
Document pdfDocument = new Document(inputFile);

TextAbsorber textAbsorber = new TextAbsorber();
textAbsorber.ExtractionOptions = new TextExtractionOptions(TextExtractionOptions.TextFormattingMode.Pure);
//Setting scale factor to 0.5 is enough to split columns in the majority of documents
//Setting of zero allows to algorithm choose scale factor automatically
textAbsorber.ExtractionOptions.ScaleFactor = 0.5; /* 0; */
pdfDocument.Pages.Accept(textAbsorber);
String extractedText = textAbsorber.Text;

System.IO.File.WriteAllText(outFile, extractedText); 
```

Please note that there is no direct correspondence between new ScaleFactor and the old coefficient of manually font reducing. However, by default algorithm takes into account the value of font size that have already reduced due to some internal reasons. For example, reducing font size from 10 to 7 has the same effect as setting scale factor to 5/8 (= 0.625).

## Identify if Image in PDF is Colored or Black & White

Different type of compression can be applied over images to reduce their size. The type of compression being applied over image depends upon the ColorSpace of source image i.e. if image is Color (RGB), then apply JPEG2000 compression, and if it is Black & White, then JBIG2/JBIG2000 compression should be applied. Therefore identifying each image type and using an appropriate type of compression will create best/optimized output. The following code snippet can be used to identify if the images inside PDF file are Colored or Black & White. For further information, you may visit [Identify if image inside PDF is Colored or Black & White][2]

```
// The path to the documents directory.
string dataDir = RunExamples.GetDataDir_AsposePdf_Images();

// Counter for grayscale images
int grayscaled = 0;
// Counter for RGB images
int rgd = 0;

using (Document document = new Document(dataDir + "ExtractImages.pdf"))
{
    foreach (Page page in document.Pages)
    {
        Console.WriteLine("--------------------------------");
        ImagePlacementAbsorber abs = new ImagePlacementAbsorber();
        page.Accept(abs);
        // Get the count of images over specific page
        Console.WriteLine("Total Images = {0} over page number {1}", abs.ImagePlacements.Count, page.Number);
        // Document.Pages[29].Accept(abs);
        int image_counter = 1;
        foreach (ImagePlacement ia in abs.ImagePlacements)
        {
            ColorType colorType = ia.Image.GetColorType();
            switch (colorType)
            {
                case ColorType.Grayscale:
                    ++grayscaled;
                    Console.WriteLine("Image {0} is GrayScale...", image_counter);
                    break;
                case ColorType.Rgb:
                    ++rgd;
                    Console.WriteLine("Image {0} is RGB...", image_counter);
                    break;
            }
            image_counter += 1;
        }
    }
}
```

## Setting Header/Footer for whole PDF

Header and Footer are very important elements inside PDF documents. They are used to show some important information related to PDF document i.e. Document Tile, company logo, Confidential Notice, page count, etc. When creating a PDF document, we can add a Header/Footer element for each page. However in order to have optimized performance, another approach is to first create a PDF document with all required elements, create Header/Footer instance, iterate through all PDF pages and add the newly created Header/Footer object to each page of the document. The following code snippet shows the steps to create a Table object, add sample information inside the table, create Header/Footer object, add the table to paragraphs collection of Footer object and then set Footer object as a footer for each page of the document.

```
string inFile = "input.pdf";
string outFile = "34055.pdf";
// load input PDF file
Document doc = new Document(inFile);
// create table instance
Aspose.Pdf.Table table = new Aspose.Pdf.Table();
table.ColumnWidths = "50 50";
// create row object
Aspose.Pdf.Row row = new Aspose.Pdf.Row();
// add table cell in first row of PDF
row.Cells.Add("row1 cell 1");
row.Cells.Add("row1 cell 2");
// add first row to table instance
table.Rows.Add(row);
// create another row object
row = new Aspose.Pdf.Row();
row.Cells.Add("row2 cell 1");
row.Cells.Add("row2 cell 2");
table.Rows.Add(row);
// create Footer object
Aspose.Pdf.HeaderFooter footer = new Aspose.Pdf.HeaderFooter();
// add table to paragraphs collection of footer object
footer.Paragraphs.Add(table);
// itterat through each page of PDF file
foreach (Page page in doc.Pages)
    // set footer of page as recently created footer instance
    page.Footer = footer;
// save PDF document
doc.Save(outFile); 
```

## Extract Table Border as Image from PDF in C#

The page borders are path drawing operations. Therefore the Pdf->Html processing logic just performs drawing instructions and places the background behind the text. So, to repeat the logic, you has to process contents operators manually and draw the graphics yourself. Also please note that following code snippet might not work accurately for various PDF files but if you encounter any issue, please feel free to contact. This code was developed for specific PDF files.

```
Document doc = new Document(inFile);

int defaultResolution = 72;
Stack graphicsState = new Stack();
System.Drawing.Bitmap bitmap = new System.Drawing.Bitmap((int)doc.Pages[1].PageInfo.Width, (int)doc.Pages[1].PageInfo.Height);
System.Drawing.Drawing2D.GraphicsPath graphicsPath = new System.Drawing.Drawing2D.GraphicsPath();
// default ctm matrix value is 1,0,0,1,0,0
System.Drawing.Drawing2D.Matrix lastCTM = new System.Drawing.Drawing2D.Matrix(1, 0, 0, -1, 0, 0);
// System.Drawing coordinate system is top left based, while pdf coordinate system is low left based, so we have to apply the inversion matrix
System.Drawing.Drawing2D.Matrix inversionMatrix = new System.Drawing.Drawing2D.Matrix(1, 0, 0, -1, 0, (float)doc.Pages[1].PageInfo.Height);
System.Drawing.PointF lastPoint = new System.Drawing.PointF(0, 0);
System.Drawing.Color fillColor = System.Drawing.Color.FromArgb(0, 0, 0);
System.Drawing.Color strokeColor = System.Drawing.Color.FromArgb(0, 0, 0);

using (System.Drawing.Graphics gr = System.Drawing.Graphics.FromImage(bitmap))
{
    gr.SmoothingMode = SmoothingMode.HighQuality;
    graphicsState.Push(new System.Drawing.Drawing2D.Matrix(1, 0, 0, 1, 0, 0));

    // process all the contents commands
    foreach (Operator op in doc.Pages[1].Contents)
    {
        Operator.GSave opSaveState = op as Operator.GSave;
        Operator.GRestore opRestoreState = op as Operator.GRestore;
        Operator.ConcatenateMatrix opCtm = op as Operator.ConcatenateMatrix;
        Operator.MoveTo opMoveTo = op as Operator.MoveTo;
        Operator.LineTo opLineTo = op as Operator.LineTo;
        Operator.Re opRe = op as Operator.Re;
        Operator.EndPath opEndPath = op as Operator.EndPath;
        Operator.Stroke opStroke = op as Operator.Stroke;
        Operator.Fill opFill = op as Operator.Fill;
        Operator.EOFill opEOFill = op as Operator.EOFill;
        Operator.SetRGBColor opRGBFillColor = op as Operator.SetRGBColor;
        Operator.SetRGBColorStroke opRGBStrokeColor = op as Operator.SetRGBColorStroke;

        if (opSaveState != null)
        {
            // save previous state and push current state to the top of the stack
            graphicsState.Push(((System.Drawing.Drawing2D.Matrix)graphicsState.Peek()).Clone());
            lastCTM = (System.Drawing.Drawing2D.Matrix)graphicsState.Peek();
        }
        else if (opRestoreState != null)
        {
            // throw away current state and restore previous one
            graphicsState.Pop();
            lastCTM = (System.Drawing.Drawing2D.Matrix)graphicsState.Peek();
        }
        else if (opCtm != null)
        {
            System.Drawing.Drawing2D.Matrix cm = new System.Drawing.Drawing2D.Matrix(
                (float)opCtm.Matrix.A,
                (float)opCtm.Matrix.B,
                (float)opCtm.Matrix.C,
                (float)opCtm.Matrix.D,
                (float)opCtm.Matrix.E,
                (float)opCtm.Matrix.F);

            // multiply current matrix with the state matrix
            ((System.Drawing.Drawing2D.Matrix)graphicsState.Peek()).Multiply(cm);
            lastCTM = (System.Drawing.Drawing2D.Matrix)graphicsState.Peek();
        }
        else if (opMoveTo != null)
        {
            lastPoint = new System.Drawing.PointF((float)opMoveTo.X, (float)opMoveTo.Y);
        }
        else if (opLineTo != null)
        {
            System.Drawing.PointF linePoint = new System.Drawing.PointF((float)opLineTo.X, (float)opLineTo.Y);
            graphicsPath.AddLine(lastPoint, linePoint);

            lastPoint = linePoint;
        }
        else if (opRe != null)
        {
            System.Drawing.RectangleF re = new System.Drawing.RectangleF((float)opRe.X, (float)opRe.Y, (float)opRe.Width, (float)opRe.Height);
            graphicsPath.AddRectangle(re);
        }
        else if (opEndPath != null)
        {
            graphicsPath = new System.Drawing.Drawing2D.GraphicsPath();
        }
        else if (opRGBFillColor != null)
        {
            fillColor = opRGBFillColor.getColor();
        }
        else if (opRGBStrokeColor != null)
        {
            strokeColor = opRGBStrokeColor.getColor();
        }
        else if (opStroke != null)
        {
            graphicsPath.Transform(lastCTM);
            graphicsPath.Transform(inversionMatrix);
            gr.DrawPath(new System.Drawing.Pen(strokeColor), graphicsPath);
            graphicsPath = new System.Drawing.Drawing2D.GraphicsPath();
        }
        else if (opFill != null)
        {
            graphicsPath.FillMode = FillMode.Winding;
            graphicsPath.Transform(lastCTM);
            graphicsPath.Transform(inversionMatrix);
            gr.FillPath(new System.Drawing.SolidBrush(fillColor), graphicsPath);
            graphicsPath = new System.Drawing.Drawing2D.GraphicsPath();
        }
        else if (opEOFill != null)
        {
            graphicsPath.FillMode = FillMode.Alternate;
            graphicsPath.Transform(lastCTM);
            graphicsPath.Transform(inversionMatrix);
            gr.FillPath(new System.Drawing.SolidBrush(fillColor), graphicsPath);
            graphicsPath = new System.Drawing.Drawing2D.GraphicsPath();
        }
    }
}
bitmap.Save(outFile, ImageFormat.Png); 
```

## Improve On-fly Resources Optimization

The Document class has **OptimizeResources(..)** which takes **Document.OptimizationOptions** object to optimize the size of the input document. The Document class also has a property named **OptimizeSize** which Gets or sets optimization flag. When pages are added to document, equal resource streams in the resultant file are merged into one PDF object if this flag set. This allows us to decrease resultant file size but may cause slower execution and larger memory requirements. The default value is false. When this option is turned off, newly added pages are scanned and if duplicate resources are found, they are "merged" with existing resources (provided they are the same). However recently we have observed that this works with stream objects only (i.e. contents of the pictures or font files). Therefore we started to investigate the possibility of optimization for dictionary objects which will allow using shared font dictionaries. Some customers have recently reported that they experienced serious size expansion issues. Therefore in this new release, the Optimization is improved in order to merge streams and dictionaries of the resources (fonts, images, etc). Nevertheless, **OptimizationOptions.AllowPageReuse** property is added to enable/disable pages merging.

## Setting Printer Driver Settings

We investigated the enhancement requested earlier to set printer driver settings and as per our observations, the printer driver settings are very specific to particular printer. The .Net Framework provides extra printing features in WPF (Presentation Foundation), but Aspose.Pdf.dll cannot use it and I am afraid we do not have any plans to introduce its dependency in a short time period.

Another option is used WinAPI functionality, but this is not an option because it is not safe and non-cross-platform.

You may also consider using DEVMODE setting with printerSettings which are provided to PdfViewer.PrintDocumentWithSettings method.

## Miscellaneous Fixes

As well as the enhancements and features discussed above, there have been numerous fixes related to HTML to PDF conversion, PDF to Excel conversion, XPS to PDF conversion, PDF to TIFF conversion, conversion of PDF to PDF/A compliant documents, text replacement, rendering PDF files to XPS, creating TOCs in PDF files, and printing PDFs with embedded fonts. Please download and try the latest release of [Aspose.PDF for .NET 9.9.0][3].




[1]: http://products.aspose.com/pdf/net
[2]: https://docs.aspose.com/display/pdfnet/Manipulate+Images#ManipulateImages-IdentifyifimageinsidePDFisColoredorBlack&White
[3]: https://downloads.aspose.com/pdf/net





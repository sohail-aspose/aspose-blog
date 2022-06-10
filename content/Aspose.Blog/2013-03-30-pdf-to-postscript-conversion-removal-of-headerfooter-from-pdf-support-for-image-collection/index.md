---
title: 'Convert PDF to PostScript and Remove Header/Footer from PDF in C#'
date: Sat, 30 Mar 2013 21:30:10 +0000
draft: false
url: /2013/03/30/pdf-to-postscript-conversion-removal-of-headerfooter-from-pdf-support-for-image-collection/
author: Codewarior
summary: ''
tags: ['Nayyer Shahbaz', 'PDF to PS', 'PDF to PostScript in Csharp', 'Remove Header Footer in PDF']
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/aspose-Pdf-for-net_100.png" alt="">}}


We are always enthusiastic about adding new features and excited to introduce the enhancements to our products. Furthermore, we have always tried our level best to fix the issues and bugs reported in earlier versions because it helps us gain customer's confidence in our products. Keeping the tradition alive, we are very much excited to announce the release of [Aspose.PDF for .NET 7.8.0][1]. During the preparation of this release, we have introduced many new features and enhancement and also fixed many of the issues reported earlier.

## Convert PDF to PostScript in C#

One of the salient features of [Aspose.PDF for .NET 7.8.0][2] is support for rendering PDF document to PostScript (PS) format. Accomplishing this requirement has been made very easy by introducing support in the PdfViewer class. Now you simply need to install PostScript drivers on your system, use the PdfViewer class and you are good to go with the conversion.

{{< gist aspose-pdf 4a12f0ebd453e7f0d552ed6658ed3253 "Examples-CSharp-AsposePdfFacades-Printing-PdfToPostScript-PdfToPostScript.cs" >}}

Please check out the related article for further details on [PDF to PostScript conversion][3].

## Image Collection Support

As per the Document Object Model (DOM) approach, each object inside a PDF file can be individually accessed and manipulated. Therefore taking benefit of this mechanism, we have introduced Image Collection support. Please take a look over the following simple code to add images to a PDF file's collection object.

```
// Instantiate Document object 
Document doc = new Document();
// Initialize collections object for Document object 
doc.Collection = new Collection();
// Load source Image file 
Aspose.Pdf.FileSpecification fs = new Aspose.Pdf.FileSpecification("AsposeDependency.PNG");
// Add description for loaded image file 
fs.Description = "PNG file1";
// Add image to collection of PDF file 
doc.Collection.Add(fs);
// Load another image file
fs = new FileSpecification("sampleImage.jpg");
fs.Description = "JPEG file1";
// Add image to collection of PDF file
doc.Collection.Add(fs);
// Load third image file
fs = new FileSpecification("1.png");
// Description for image file
fs.Description = "PNG file2";
doc.Collection.Add(fs);
// Save the document
doc.Save("c:/pdftest/Image_Collection.pdf"); 
```



{{< figure align=center src="images/Images_Collection.png" alt="Image Collection inside PDF document">}}


  
The above snapshot shows the Image collection inside the PDF document

## Remove Header or Footer from PDF File

Recently we have worked on a requirement to remove headers and footers from PDF files.  To fulfill this requirement, we've added the PdfFileStamp.StampId property. This property allows you to set an identifier for new stamps (including header, footer, page number). The added stamp may be removed using the PdfContentEditor: add header, footer and page number while assigning them arbitrary IDs, and later remove them with those IDs.

```
PdfFileStamp pfe = new PdfFileStamp("Input.pdf"," PDF_With_Header_Footer.pdf");
// 100 is the stampId for footer
pfe.StampId = 100;
pfe.AddFooter(new FormattedText("Footer"), 10);
// 200 is the stampId for header
pfe.StampId = 200;
pfe.AddHeader(new FormattedText("Header"), 10);
// 300 if  the stampId for page number
pfe.StampId = 300;
pfe.AddPageNumber(new FormattedText(" Page #", System.Drawing.Color.Red, System.Drawing.Color.Blue));
pfe.Close();

PdfContentEditor pce = new PdfContentEditor();
pce.BindPdf("PDF_With_Header_Footer.pdf");
StampInfo[] stamps = pce.GetStamps(1);
Console.WriteLine(stamps.Length);
Assert.AreEqual(3, stamps.Length);
// Show found stamps IDs
foreach (StampInfo info in stamps)

{ Console.WriteLine(info.StampId); }
// Remove header, footer and page number
pce.DeleteStampById(100);
pce.DeleteStampById(200);
pce.DeleteStampById(300);
pce.Save("No_Header-Footer.pdf"); 
```

## Use CMYK Colorspace to Set ForegroundColor and BackgroundColor

Prior to the release of Aspose.PDF for .NET 7.8.0, we supported using the **System.Drawing.Color** object to set the foreground and background color of text, stamps, and similar objects. With the release of this version, we have enhanced the capabilities of our product so you can set the color from the CMYK, gray and RGB color spaces. The **TextState** and **TextFragmentState** objects have properties to set BackgroundColor and ForegroundColor. To set background or foreground color from the CMYK colorspace, please try using the following code snippet.

```
TextStamp stamp = new TextStamp("Test");
stamp.TextState.ForegroundColor = Aspose.Pdf.Color.FromCmyk(0.1, 0.2, 0.3, 0.5);
stamp.TextState.BackgroundColor = Aspose.Pdf.Color.FromCmyk(0.3, 0.2, 0.1, 0.3);
// Save updated document
```

### Code Migration Scenarios

Previously valid code:

*   TextState.BackgroundColor = System.Drawing.Color.Brown

Valid code from Aspose.Pdf for .NET 7.8.0:

*   TextState.BackgroundColor = Aspose.Pdf.Color.FromRgb(System.Drawing.Color.Brown);

Besides the above stated enhancements, we have also made many improvements in terms of performance while converting TIFF to PDF, PDF to TIFF, HTML to PDF, XPS to PDF, PDF to XPS, PDF printing, image replacement, image extraction, text watermarking, image stamping and much more. Please visit the following link for further details on what's new & fixed in **Aspose.PDF for .NET 7.8.0.**




[1]: https://downloads.aspose.com/pdf/net
[2]: https://downloads.aspose.com/pdf/net
[3]: https://docs.aspose.com/display/pdfnet/Working+with+PDF+printing+-+Facades#WorkingwithPDFprinting-Facades-PDFtoPostScriptconversion





---
title: 'Print PDF Documents using PrintController and Add FlateDecode Images in XImageCollection of a Document'
date: Sun, 13 Jan 2019 20:18:05 +0000
draft: false
url: /2019/01/13/print-pdf-documents-using-printcontroller-and-add-flatedecode-images-in-ximagecollection-of-a-document/
author: Asad Ali
summary: ''
tags: ['.NET PDF API', 'Asad Ali', 'Print PDF documents']
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/aspose-Pdf-for-net.png" alt="">}}


We at Aspose are honored announcing December Release i.e. [Aspose.PDF for .NET 18.12][1] which is available for download and to be used in .NET applications. This new release of API contains a number of new features, enhancements and bug fixes for the issues reported in the previous version(s) of the API. In order to have an insight into what has been introduced new and changed in the latest release, it is recommended to go through the detailed release notes page in the API documentation. The [release notes page][2] contains complete information about public API Changes in this release of the API.

Following sections provides insights into worth mentioning and useful features/enhancements in December revision of Aspose.PDF for .NET.

## Print PDF Documents using PrintController of Aspose.PDF

The latest release of the API offers **PrintController** Class which helps to save a **System.Drawing.Printing.PrintDocument** as PDF format. Following is a simple example to use **PrintController** Class and its functionality:

```
public void PDFNEWNET\_45624()
{
 string outFile = GetOutputPath("45624.pdf");
 PrintDocument doc = new PrintDocument();
 doc.PrintPage += new PrintPageEventHandler(mPrintDoc\_PrintPage);
 Aspose.Pdf.PrintController printController = new Aspose.Pdf.PrintController();
 printController.FileName = outFile;
 doc.PrintController = printController;
 doc.Print();
}  
private void mPrintDoc\_PrintPage(object sender  
, System.Drawing.Printing.PrintPageEventArgs e)  
{  
 e.Graphics.DrawRectangle(new Pen(System.Drawing.Color.Red), 0, 0, 100, 100);  
 e.Graphics.FillEllipse(new SolidBrush(System.Drawing.Color.Blue), 100, 100, 200, 200);  
}
```

## Store FlateDecode Images in XImageCollection

With the latest release of the API, the FlateDecode filter is supported for adding images into PDF Pages. You can consider the following code snippet in order to achieve this functionality:

```
Aspose.Pdf.Document document = new Document();
document.Pages.Add();
Page page = document.Pages\[1\];
FileStream imageStream = new FileStream(@"c:\\1.jpg", FileMode.Open);
page.Resources.Images.Add(imageStream, ImageFilterType.Flate); // New FilterType
XImage ximage = page.Resources.Images\[page.Resources.Images.Count\];
page.Contents.Add(new Operators.GSave());
```

For internal usage, you can pass **ImageFilterType** parameter **Flate**:

```
// XImageCollection  
internal IPdfObject add(Stream stream, int quality  
, bool isBlackWhite, ImageFilterType filterType, bool isMasked  
, Stream predefinedStream = null)  
{  
 stream = IsMetafile(stream);  
 return AddOrReplace(-1, stream, quality, isBlackWhite, filterType, isMasked  
 , predefinedStream);  
}
```

## Miscellaneous Fixes

As mentioned above the December release of the API has come with quite exciting features and enhancements. However, the following are some useful fixes and improvements which have been included in this release to improve its performance and usability:

*   PDF/UA functionality has been enhanced in terms of:
    *   Validating Text
    *   Creating ITaggedContent Interface
    *   Creating Factory of Structure Elements
    *   Managing Logical Tree of Elements
    *   Setting up Title and Language of Tagged PDF Documents
*   Enhanced PDF Optimization
*   Descriptive Exception is added for non-existing fonts in PDF to HTML Conversion Scenario
*   Performance has been improved for PDF to PNG Conversion
*   Various fixes have been made for text adding/editing scenarios
*   Following Conversion Engines have been improved further:
    *   JPG to PDF
    *   PDF to TIFF
    *   PDF to JPEG
    *   PDF to PNG
    *   PDF to PDF/A-1B
    *   PDF to PDF/UA
*   Improvements regarding Table data extraction have been made

## Aspose.PDF for .NET Resources

As it is always recommended to use latest releases of our API’s, so we suggest you please download the latest release [Aspose.PDF for .NET 18.12][3] and check following resources which will help you working with API:

*   [Home page for Aspose.PDF for .NET][4]
*   [Download Aspose.PDF for .NET 18.12][5]
*   [Aspose.PDF product family forum][6]– Post your technical questions and queries, or any other problem you faced while running Aspose.PDF APIs.
*   [Aspose.PDF for .NET online documentation][7]– help documentation and API reference documents.
*   [Enable Blog Subscription][8]– Do not limit yourself, you can keep yourself updated with the latest news on Aspose.PDF APIs, new features, fixes and other API related topics by subscribing to Aspose.PDF blog.
*   [Aspose.PDF for .NET Examples][9] – We have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: https://www.nuget.org/packages/Aspose.Pdf/18.12.0
[2]: https://docs.aspose.com/display/pdfnet/Aspose.PDF+for+.NET+18.12+Release+Notes
[3]: https://www.nuget.org/packages/Aspose.Pdf/18.12.0
[4]: https://products.aspose.com/pdf/net
[5]: https://www.nuget.org/packages/Aspose.Pdf/18.12.0
[6]: https://forums.aspose.com/c/pdf
[7]: https://docs.aspose.com/display/pdfnet/Home
[8]: https://blog.aspose.com/category/aspose-products/aspose-pdf-product-family/
[9]: https://github.com/aspose-pdf/Aspose.PDF-for-.NET





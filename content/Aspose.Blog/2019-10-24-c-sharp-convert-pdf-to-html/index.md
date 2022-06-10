---
title: 'Convert PDF to HTML using C# .NET'
date: Thu, 24 Oct 2019 01:08:00 +0000
draft: false
url: /2019/10/24/c-sharp-convert-pdf-to-html/
author: Kashif Iqbal
summary: ''
tags: ['Convert PDF to HTML Csharp', 'PDF to HTML', 'convert PDF files', 'convert PDF to HTML']
categories: ['Aspose.PDF Product Family']
---

In this post, we’ll explore and demonstrate how to read and convert a PDF to HTML in C# with various customization options.



{{< figure align=center src="images/aspose_pdf-for-net.jpg" alt="Convert PDF to HTML C#">}}


[PDF][1] is one of the most popular document formats these days which is used by a variety of applications as the final output. Due to its support for a wide range of data types and portability, it is the format of choice for creating and sharing content. As a .NET application developer who is interested in developing document management applications, you may want to embed processing features to read and convert PDF documents to other file formats such as [HTML][2].

This article covers the following PDF to HTML conversion scenarios:

*   Convert PDF to HTML using C#
*   Convert PDF to HTML with Embedded Resources in C#
*   Save Images to Specific Folder in PDF to HTML Conversion
*   Convert PDF to Multipage HTML in C#

## C# PDF to HTML Converter Library

[Aspose.PDF for .NET][3] is a powerful PDF library that also provides an efficient PDF to HTML converter. It lets you read and convert PDF files to HTML using C# or VB.NET within your .NET applications. You can [download][4] Aspose.PDF for .NET or add it in your project using [NuGet Package Manager][5].

## Convert PDF to HTML using C#

Converting a PDF document to HTML is as simple as pie and you can do it in a couple of lines of code. Simply load the PDF document using [Document][6] class and save it as HTML using _.html_ extension. The following code sample shows how to convert a PDF document to HTML in C#.

```
// Open the source PDF document
Document pdfDocument = new Document("PDFToHTML.pdf");

// Save the file into MS document format
pdfDocument.Save("output_out.html", SaveFormat.Html);
```

The API takes care of reading all the internal details of the PDF format and converts it to HTML. Interestingly, you don’t need to have PDF reader programs installed at your end or any other computer where your application will finally run.

## Convert PDF to HTML with Embedded Resources in C#

You can also convert PDF to HTML with all the resources as part of the output HTML. This will result in making all the elements of a PDF file (images, CSS, and fonts) embedded into the output HTML. This is achieved by using the [HtmlSaveOptions.PartsEmbeddingMode][7] enumerator. The following code sample shows how to convert PDF to HTML with embedded resources using C#.

```
// Load source PDF file
Document doc = new Document("input.pdf");
// Instantiate HTML Save options object
HtmlSaveOptions newOptions = new HtmlSaveOptions();

// Enable option to embed all resources inside the HTML
newOptions.PartsEmbeddingMode = HtmlSaveOptions.PartsEmbeddingModes.EmbedAllIntoHtml;

// This is just optimization for IE and can be omitted 
newOptions.LettersPositioningMethod = HtmlSaveOptions.LettersPositioningMethods.UseEmUnitsAndCompensationOfRoundingErrorsInCss;
newOptions.RasterImagesSavingMode = HtmlSaveOptions.RasterImagesSavingModes.AsEmbeddedPartsOfPngPageBackground;
newOptions.FontSavingMode = HtmlSaveOptions.FontSavingModes.SaveInAllFormats;
// Output file path 
string outHtmlFile = "SingleHTML_out.html";
doc.Save(outHtmlFile, newOptions);
```

## Saving Images to Specific Folder

A PDF document can contain images in addition to textual details. On the other hand, an HTML file can also contain images that are based-64 encoded inside the HTML or referenced from a folder where these images are located. Aspose.PDF for .NET has rich features of saving images to a user-specified folder on disc. The following code sample shows how to save images to a specific folder during the conversion of PDF file to HTML in C#.

```
// Load source PDF file
Document doc = new Document("input.pdf");

// Create HtmlSaveOption with tested feature
HtmlSaveOptions newOptions = new HtmlSaveOptions();

// Specify the separate folder to save images
newOptions.SpecialFolderForAllImages = "MyFolder";

// Output file path 
string outHtmlFile = "HTML.html";
doc.Save(outHtmlFile, newOptions);
```

## Convert PDF to Multipage HTML using C#

The API doesn’t stop you here as it has a lot of options to customize the conversion. For example, you can split the HTML in the above step into multiple pages during PDF to HTML conversion. The following code sample shows how to convert PDF to a multipage HTML using C#.

```
// Open the source PDF document
Document pdfDocument = new Document("PDFToHTML.pdf");

// Instantiate HTML SaveOptions object
HtmlSaveOptions htmlOptions = new HtmlSaveOptions();

// Specify to split the output into multiple pages
htmlOptions.SplitIntoPages = true;

// Save the document
pdfDocument.Save(@"MultiPageHTML_out.html", htmlOptions);
```

Setting the _[SplitIntoPages][8]_ flag to true takes care of everything for you and the output HTML consists of multiple pages instead of a single page.

## Conclusion

This article covered various scenarios of how to convert PDF to HTML programmatically using C#. It also demonstrated how to customize the conversion using different options.

Still want more? You can head-on to the APIs documentation section, [PDF to HTML][9] that lists some advanced level features for applying more options during conversion.

Download your free copy of [Aspose.PDF for .NET][10] and you can get started in no time by following the API documentation. If you have any queries, feel free to post to [Aspose.PDF forum][11]. We'll be glad to assist you with your queries and inquiries.

## Related Articles

*   [Convert HTML Files to PDF in C# .NET][12]




[1]: https://wiki.fileformat.com/view/pdf/
[2]: https://wiki.fileformat.com/web/html/
[3]: https://products.aspose.com/pdf/net
[4]: https://downloads.aspose.com/pdf/net
[5]: https://nuget.org/packages/Aspose.pdf
[6]: https://apireference.aspose.com/pdf/net/aspose.pdf/document
[7]: https://apireference.aspose.com/pdf/net/aspose.pdf/htmlsaveoptions/fields/partsembeddingmode
[8]: https://apireference.aspose.com/net/pdf/aspose.pdf/htmlsaveoptions/properties/splitintopages
[9]: https://docs.aspose.com/display/pdfnet/Convert+PDF+File+into+HTML+Format
[10]: https://downloads.aspose.com/pdf/net
[11]: https://forum.aspose.com/c/pdf
[12]: https://blog.aspose.com/2020/02/28/convert-html-to-pdf-programmatically-in-csharp-net/





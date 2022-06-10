---
title: 'Font Handling and Rendering HTML Tags inside Table'
date: Sun, 20 May 2018 21:07:05 +0000
draft: false
url: /2018/05/20/font-handling-and-rendering-html-tags-inside-table-using-aspose.pdf-for-.net/
author: Asad Ali
summary: ''
tags: ['Asad Ali']
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/aspose-Pdf-for-net.png" alt="">}}


We at Aspose are very much excited to announce May release of Aspose.PDF for .NET. [Aspose.PDF for .NET 18.5][1] is available on NuGet Gallery for download. We have introduced excited features in this release of the API in order to improve the usability and performance of the API. Along with that several bugs, which were reported for earlier version(s) of the API, are also fixed in this release. [Release notes of Aspose.PDF for .NET 18.5][2], contains detailed information regarding improvements and public API Changes in this version.

## Set Default Font Name

As per the default behavior of the API, Aspose.PDF for .NET used to replace fonts with default font when these fonts (used in the PDF) were not available in the document itself and on the device where API was being used. However, we have investigated for; when a font is installed/present in the device or embedded into the document, the output PDF document should have same font rather than being replaced with default font. In order to implement the behavior we have introduced a [DefaultFontName][3] Property in **PdfSaveOptions** Class, which can be used to specify the default font name while saving a PDF document as PDF format. A demonstration of the feature with code snippet is also presented in the following article of API documentation:

*   [Set Default Font Name while Saving PDF][4]

## Get all Fonts from PDF file

One of the excited features in [Aspose.PDF for .NET 18.5][5] is to get all fonts from PDF document programmatically. With this release of the API, you can get all fonts by using [GetAllFonts()][6] method provided by **FontUtilities** interface. An example with complete code snippet is given at following link of the API documentation:

*   [Get all Fonts from PDF Document][7]

## Support for HTML Tags inside Table

In earlier version(s) of the API, **Table.ImportDataTable()** was being used, in order to fetch DataTable content inside a Table in PDF document. However, we have enhanced this method and now if you have a requirement to fetch content from database containing HTML Tags in it, [ImportDataTable()][8] method can render those HTML Tags accordingly inside PDF document. You can check further details and code snippet in API documentation at given link:

*   [Add HTML Tags inside Table][9]

## Miscellaneous

As it is always recommended to use latest release of our API’s, so we suggest you to please download the latest release[Aspose.PDF for .NET 18.5][10] and check following resources which will help you working with API:

*   [Home page for Aspose.PDF for .NET][11]
*   [Download Aspose.PDF for .NET 18.5][12]
*   [Aspose.PDF product family forum][13]– Post your technical questions and queries, or any other problem you faced while running Aspose.PDF APIs.
*   [Aspose.PDF for .NET online documentation][14]– help documentation and API reference documents.
*   [Enable Blog Subscription][15]– Do not limit yourself, you can keep yourself updated with the latest news on Aspose.PDF APIs, new features, fixes and other API related topics by subscribing to Aspose.PDF blog.
*   [Aspose.PDF for .NET Examples][16]– We have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: https://www.nuget.org/packages/Aspose.Pdf/18.5.0 "Aspose.PDF for .NET 18.5"
[2]: https://docs.aspose.com/display/pdfnet/Aspose.PDF+for+.NET+18.5+Release+Notes "Aspose.PDF for .NET 18.5 Release Notes"
[3]: https://apireference.aspose.com/net/pdf/aspose.pdf/pdfsaveoptions/properties/defaultfontname "DefaultFontName Property"
[4]: https://docs.aspose.com/display/pdfnet/Formatting+PDF+Document#FormattingPDFDocument-SetDefaultFontNamewhileSavingPDF "Set Default Font Name while Saving PDF"
[5]: https://www.nuget.org/packages/Aspose.Pdf/18.5.0 "Aspose.PDF for .NET 18.5"
[6]: https://apireference.aspose.com/net/pdf/aspose.pdf.document/idocumentfontutilities/methods/getallfonts "GetAllFonts Method"
[7]: https://docs.aspose.com/display/pdfnet/Formatting+PDF+Document#FormattingPDFDocument-GetAllFontsfromPDFDocument "Get all Fonts from PDF Document"
[8]: https://apireference.aspose.com/net/pdf/aspose.pdf/table/methods/importdatatable "ImportDataTable Method"
[9]: https://docs.aspose.com/display/pdfnet/Add+and+Extract+a+Table#AddandExtractaTable-AddHTMLTagsinsideTable "Add HTML Tags inside Table"
[10]: https://www.nuget.org/packages/Aspose.Pdf/18.5.0 "Download API"
[11]: https://products.aspose.com/pdf/net "Aspose.PDF API home page"
[12]: https://www.nuget.org/packages/Aspose.Pdf/18.5.0 "API Download Section"
[13]: https://forums.aspose.com/c/pdf "Support Forum"
[14]: https://docs.aspose.com/display/pdfnet/Home "Online Documentation"
[15]: https://blog.aspose.com/category/aspose-products/aspose-pdf-product-family/ "Blog Subscription"
[16]: https://github.com/aspose-pdf/Aspose.PDF-for-.NET "GitHub examples repository"





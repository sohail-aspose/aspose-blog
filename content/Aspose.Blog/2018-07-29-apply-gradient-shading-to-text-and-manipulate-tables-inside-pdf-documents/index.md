---
title: 'Apply Gradient Shading to Text and Manipulate Tables in PDF Documents in C# .NET'
date: Sun, 29 Jul 2018 22:51:40 +0000
draft: false
url: /2018/07/29/apply-gradient-shading-to-text-and-manipulate-tables-inside-pdf-documents/
author: Asad Ali
summary: ''
tags: ['Add or extract table in PDF document', 'Apply gradient shading to text in PDF', 'Apply pattern colorspace to text in PDF', 'Asad Ali']
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/aspose-Pdf-for-net.png" alt="">}}


We are very much excited to announce the release of [Aspose.PDF for .NET 18.7][1], which is available over NuGet Gallery for download and to be used in .NET Applications. This new release has been rolled out with quite excited features and enhancements. Several fixes to the bugs reported in earlier versions of the API, have also been included in latest release of the API. In case you are planning to use latest version, we strongly recommend you to go through the [release notes][2] page of the API in official documentation. All public API Changes including improvements and new features have been mentioned in the release notes. However, following are some major features which have been offered with new release of Aspose.PDF for .NET.

## Add Text with Gradient Shading

In text editing scenarios, applying gradient shading or pattern colorspace to the text is now available in latest release of the API. **Aspose.Pdf.Color** Class has further been enhanced by introducing new property of **PatternColorSpace**, which can be used to specify shading colors for the text. An example demonstrating the usage of mentioned feature can be checked at following link in API documentation:

*   [Apply Gradient Shading to the Text][3]

## Manipulate Table inside PDF document

Earlier it was achievable to add table inside PDF document as well as extract it using **TableAbsorber** Class. However, new features have been added to the API in order to remove as well as replace existing tables with new ones. Existing **TableAbsorber** Class has further been enhanced by introducing following new methods:

*   **Remove(AbsorbedTable table)**
*   **Replace(Page page, AbsorbedTable oldTable, Table newTable)**

In order to use above mentioned methods to remove and replace tables inside PDF document, please check following articles in API documentation:

*   [Remove Table from PDF document][4]
*   [Remove Multiple Tables from PDF document][5]
*   [Replace old Table with new one in PDF document][6]

## Remove Text from PDF document

Existing **TextFragmentAbsober** Class has further been enhanced by adding new method i.e. **RemoveAllText()**. You can remove text from particular page as well as from whole PDF document using this method. In particular scenarios where text removal from PDF is an important requirement, this new method works quite efficiently and fast. Following example in API documentation demonstrate usage of this method:

*   [Remove All Text using TextFragmentAbsorber][7]

## Support for Tagged PDF documents

Since functionality to generate Tagged PDF documents has been under development, completed features have also been included in this release of the API. Following is the list of features related to Tagged (PDF/UA) PDF documents:

*   Validation for Tagged of Real Content has been implemented
*   Implemented validation for Artifacts
*   Implemented Recognition of Natural Language
*   Added Support of Graphics Operators in Content Sequence Classes
*   Validation of Graphics has been added
*   Added Support for images in tagged content
*   Bounding box for images has been added
*   Image attributes are supported for tagged PDF

## Miscellaneous Fixes

Along with the above mentioned features, 25 fixes have also been incorporated in Aspose.PDF for .NET 18.7. Some important fixes and improvements include:

*   Worked to improve heading formatting inside PDF document
*   Improved functionality of **TextFragmentAbsorber** Class
*   Text replacement operations have further been improved
*   Inter-File Format conversions have been improved further for compliance tests
*   Image rendering inside PDF has been improved
*   Text rendering inside tables has been improved
*   PDF to image conversions has been further improved and enhanced

## Aspose.PDF for .NET Resources

As it is always recommended to use latest releases of our API’s, so we suggest you to please download the latest release [Aspose.PDF for .NET 18.7][8] and check following resources which will help you working with API:

*   [Home page for Aspose.PDF for .NET][9]
*   [Download Aspose.PDF for .NET 18.7][10]
*   [Aspose.PDF product family forum][11]– Post your technical questions and queries, or any other problem you faced while running Aspose.PDF APIs.
*   [Aspose.PDF for .NET online documentation][12]– help documentation and API reference documents.
*   [Enable Blog Subscription][13]– Do not limit yourself, you can keep yourself updated with the latest news on Aspose.PDF APIs, new features, fixes and other API related topics by subscribing to Aspose.PDF blog.
*   [Aspose.PDF for .NET Examples][14] – We have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: https://www.nuget.org/packages/Aspose.Pdf/18.7.0
[2]: https://docs.aspose.com/display/pdfnet/Aspose.PDF+for+.NET+18.7+Release+Notes
[3]: https://docs.aspose.com/display/pdfnet/Text+Formatting+inside+PDF#TextFormattinginsidePDF-ApplyGradientShadingtotheText
[4]: https://docs.aspose.com/display/pdfnet/Manipulate+and+Integrate+Table#ManipulateandIntegrateTable-RemoveTablefromPDFdocument
[5]: https://docs.aspose.com/display/pdfnet/Manipulate+and+Integrate+Table#ManipulateandIntegrateTable-RemoveMultipleTablesfromPDFdocument
[6]: https://docs.aspose.com/display/pdfnet/Manipulate+and+Integrate+Table#ManipulateandIntegrateTable-ReplaceoldTablewithnewoneinPDFdocument
[7]: https://docs.aspose.com/display/pdfnet/Replace+Text+in+a+PDF+Document#ReplaceTextinaPDFDocument-RemoveAllTextusingTextFragmentAbsober
[8]: https://www.nuget.org/packages/Aspose.Pdf/18.7.0
[9]: https://products.aspose.com/pdf/net
[10]: https://www.nuget.org/packages/Aspose.Pdf/18.7.0
[11]: https://forums.aspose.com/c/pdf
[12]: https://docs.aspose.com/display/pdfnet/Home
[13]: https://blog.aspose.com/category/aspose-products/aspose-pdf-product-family/
[14]: https://github.com/aspose-pdf/Aspose.PDF-for-.NET





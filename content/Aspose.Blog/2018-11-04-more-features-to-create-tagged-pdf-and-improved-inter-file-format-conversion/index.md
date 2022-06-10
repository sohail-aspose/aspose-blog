---
title: 'More Features to Create Tagged PDF and Improved Inter-File Format Conversion'
date: Sun, 04 Nov 2018 19:23:41 +0000
draft: false
url: /2018/11/04/more-features-to-create-tagged-pdf-and-improved-inter-file-format-conversion/
author: Asad Ali
summary: ''
tags: ['Asad Ali', 'Create tagged PDF files', 'Create tagged PDF with Link Annotation', 'Create tagged PDF with PDF/UA validations']
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/aspose-Pdf-for-net.png" alt="">}}


We are excited to announce a new release of [Aspose.PDF for .NET 18.10][1] which is available for download on NuGet Gallery and to be used in .NET applications. As per the regular monthly update process, we have incorporated new features and enhancements in the API, as well as several fixes to the reported bugs, which have also been included in the latest release. Before using the latest version of the API, we strongly recommend you visit the [release notes page of Aspose.PDF for .NET 18.10][2] in order to know what has been changed and introduced new in the API.

The following section provides insights into worth mentioning features that have been introduced in the latest release of the API.

## Support for Link Annotation in Tagged PDF

The latest version of the API has been released with the support of Link Annotation in Tagged PDFs. This support includes various functionalities i.e. adding tagged content with link tag, adding decorated link text content and get rectangles that bounds link content. We have been working over providing full support for creating Tagged PDF content and hopefully new features would also be a part of the next release.

## PDF/UA Validations

Some validations for PDF/UA Format of PDF documents have also been implemented in the latest release of the API as follows:

*   XObjects Validations
*   Actions Validations

## Determine if Text has Underline

In order to determine if the text has underlined, the getter for **Underline** property of **TextState** of **TextFragment** has been implemented. However, in the case Underline property was not previously set (the typical situation for searching text in an existing document) following option should be set:

```
textFragmentAbsorber.TextEditOptions = new TextEditOptions(true)
{
    ToAttemptGetUnderlineFromSource = true
};
```

There are several serious reasons for using the above option because explicit instruction must be set for searching underlines in the document. As implementation of text underlining is not described in PDF specification, it means a great number of ways exist how text underlining may be implemented in third party documents. Therefore, we cannot give warranties that the underlining of text will be found in all cases in the source document.

## Miscellaneous Fixes

Along with the features mentioned above, the following are useful improvements and enhancements included in the latest release of the API:

*   Tooltips for WebHyperlink have been improved to show correct behavior
*   Subscript in LatexFagment has been further improved
*   Non-English characters rendering in PDF document is improved
*   PDF to PPTX conversion is improved
*   Text searching scenarios have been taken care of in terms of coordinates extraction
*   Font handling has been improved
*   PDF to TIFF Conversion Engine has further been improved
*   Image rendering while HTML to PDF Conversion is further improved
*   Various improvements have been made for PDF to PDF/A conversion
*   Memory consumption has further been improvised

## Aspose.PDF for .NET Resources

As it is always recommended to use latest releases of our API’s, so we suggest you please download the latest release [Aspose.PDF for .NET 18.10][3] and check following resources which will help you working with API:

*   [Home page for Aspose.PDF for .NET][4]
*   [Download Aspose.PDF for .NET 18.10][5]
*   [Aspose.PDF product family forum][6]– Post your technical questions and queries, or any other problem you faced while running Aspose.PDF APIs.
*   [Aspose.PDF for .NET online documentation][7]– help documentation and API reference documents.
*   [Enable Blog Subscription][8]– Do not limit yourself, you can keep yourself updated with the latest news on Aspose.PDF APIs, new features, fixes and other API related topics by subscribing to Aspose.PDF blog.
*   [Aspose.PDF for .NET Examples][9] – We have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: https://www.nuget.org/packages/Aspose.Pdf/18.10.0
[2]: https://docs.aspose.com/display/pdfnet/Aspose.PDF+for+.NET+18.10+Release+Notes
[3]: https://www.nuget.org/packages/Aspose.Pdf/18.10.0
[4]: https://products.aspose.com/pdf/net
[5]: https://www.nuget.org/packages/Aspose.Pdf/18.10.0
[6]: https://forums.aspose.com/c/pdf
[7]: https://docs.aspose.com/display/pdfnet/Home
[8]: https://blog.aspose.com/category/aspose-products/aspose-pdf-product-family/
[9]: https://github.com/aspose-pdf/Aspose.PDF-for-.NET





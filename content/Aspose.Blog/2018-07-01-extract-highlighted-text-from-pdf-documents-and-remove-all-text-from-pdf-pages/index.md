---
title: 'Extract Highlighted Text from PDF Documents and Remove all Text from PDF Pages'
date: Sun, 01 Jul 2018 20:47:34 +0000
draft: false
url: /2018/07/01/extract-highlighted-text-from-pdf-documents-and-remove-all-text-from-pdf-pages/
author: Asad Ali
summary: ''
tags: ['Asad Ali', 'Extract Highlighted Text from PDF in C#', 'Remove Text from PDF in C#']
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/aspose-Pdf-for-net.png" alt="Extract Highlighted Text from PDF">}}


As per the regular monthly update process, we are pleased to announce the new release of Aspose.PDF for .NET. [Aspose.PDF for .NET 18.6][1] has been published and available on NuGet Gallery, to be used in .NET applications. In Aspose.PDF for .NET 18.6, we have introduced new features related to text manipulations and PDF/UA validation. Along with that, we have also made some fixes to the bugs, reported in earlier versions of the API. An overview of public API changes and improvement in this release of the API has been given over the [release notes][2] page of [Aspose.PDF for .NET 18.6][3]. In case you are about to use the latest version of the API, we strongly recommend you please check the release notes section before downloading the API.

## Extract Highlighted Text from PDF Documents

It has been an essential requirement to extract highlighted text from PDF documents. Earlier it was possible to extract text from PDF documents on the basis of some specific regular expressions or by specifying a string to be searched. **TextFragmentAbsorber** and **TextAbsorber** classes of the API have been being used quite often and efficiently to serve the purpose.

However, regarding the requirement of extracting highlighted text from PDF document, we have investigated the feature and introduced **TextMarkupAnnotation.GetMarkedText()** and **TextMarkupAnnotation.GetMarkedTextFragments()** methods in API. You can extract highlighted text from PDF document by filtering **TextMarkupAnnotation** and using the mentioned methods. An example, demonstrating the feature usage has also been showcased at following link of API documentation:

*   [Extract Highlighted Text from PDF][4]

## Remove All Text from PDF Document

While removing text from PDF documents using earlier versions of the API, you needed to set found text as an empty string. The performance overhead, in this case, was, to invoke a number of checks and adjustment operations of text position. Which was why several performance issues were observed while performing such operations. We could not minimize the number of checks and adjustment operations, as they are essential in text editing scenarios. Moreover, you cannot determine, how many text fragments will be removed and adjusted when they are processed in a loop.

In Aspose.PDF for .NET 18.6, new Aspose.Pdf.Operators.TextShowOperator() method has been introduced, in order to remove all text from PDF pages. Therefore, we recommend using this method to remove all text from PDF documents, as it surely minimizes the time and works very fast. You can please check code sample in our API documentation, for using this feature of the API:

*   [Remove All Text from PDF Pages][5]

## Important API Changes

In the latest release of Aspose.PDF for .NET, all descendants of **Aspose.Pdf.Operator** were moved into namespace **Aspose.Pdf.Operators**. Thus 'new Aspose.Pdf.Operators.GSave()' should be used, instead of 'new Aspose.Pdf.Operator.GSave()'. While upgrading to the latest version of the API, you will need to upgrade your existing code where you have used previous **Aspose.Pdf.Operator** namespace.

## Miscellaneous

In Aspose.PDF for .NET 18.6, we have also worked for introducing Accessibility Features, thus introduced new features as part of work on 508 compliance (WCAG):

*   PDF/UA validation feature was added.
*   Tagged PDF support was added.

The above-listed features are under further development and currently they are available in [Aspose.PDF for .NET 18.6][6], as a beta version.

As it is always recommended to use the latest releases of our API’s, so we suggest you please download the latest release Aspose.PDF for .NET 18.6 and check the following resources which will help you working with API:

*   [Home page for Aspose.PDF for .NET][7]
*   [Download Aspose.PDF for .NET 18.6][8]
*   [Aspose.PDF product family forum][9]– Post your technical questions and queries, or any other problem you faced while running Aspose.PDF APIs.
*   [Aspose.PDF for .NET online documentation][10]– help documentation and API reference documents.
*   [Enable Blog Subscription][11]– Do not limit yourself, you can keep yourself updated with the latest news on Aspose.PDF APIs, new features, fixes and other API related topics by subscribing to Aspose.PDF blog.
*   [Aspose.PDF for .NET Examples][12] – We have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: https://www.nuget.org/packages/Aspose.Pdf/18.6.0
[2]: https://docs.aspose.com/display/pdfnet/Aspose.PDF+for+.NET+18.6+Release+Notes
[3]: https://www.nuget.org/packages/Aspose.Pdf/18.6.0
[4]: https://docs.aspose.com/display/pdfnet/Extract+Text+from+PDF#ExtractTextfromPDF-ExtractHighlightedTextfromPDFDocument
[5]: https://docs.aspose.com/display/pdfnet/Replace+Text+in+a+PDF+Document#ReplaceTextinaPDFDocument-RemoveAllTextfromPDFDocument
[6]: https://www.nuget.org/packages/Aspose.Pdf/18.6.0
[7]: https://products.aspose.com/pdf/net
[8]: https://www.nuget.org/packages/Aspose.Pdf/18.6.0
[9]: https://forums.aspose.com/c/pdf
[10]: https://docs.aspose.com/display/pdfnet/Home
[11]: https://blog.aspose.com/category/aspose-products/aspose-pdf-product-family/
[12]: https://github.com/aspose-pdf/Aspose.PDF-for-.NET





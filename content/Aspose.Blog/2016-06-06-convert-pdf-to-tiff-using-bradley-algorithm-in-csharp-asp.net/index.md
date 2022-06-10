---
title: 'C# PDF to TIFF Conversion using Bradley Algorithm'
date: Mon, 06 Jun 2016 02:54:06 +0000
draft: false
url: /2016/06/06/convert-pdf-to-tiff-using-bradley-algorithm-in-csharp-asp.net/
author: Codewarior
summary: ''
tags: ['Nayyer Shahbaz', 'PDF to TIFF', 'PDF to TIFF using Bradley Algorithm']
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/aspose-Pdf-for-net_100.png" alt="Aspose.Pdf for .NET logo">}}


The new release of Aspose.Pdf for .NET 11.6.0 has already been published with significant improvements in PDF to PDF/A, PDF to TIFF/JPEG and HTML to PDF features. The API has also been greatly improved to handle various complex scenarios that were causing issues in earlier release versions. Indeed, this version is a better and stable release, as compared to earlier versions.

## Convert PDF to TIFF using Bradley Algorithm

Aspose.PDF for .NET has been supporting the feature to convert PDF to TIF using LZW compression and then with the use of AForge, Binarization can be applied. However, one of the customers requested that for some images, they need to get the Threshold using Otsu, so they also would like to use Bradley. For further details, please visit [Convert PDF files to TIFF using Bradley algorithm.][1]

{{< gist aspose-pdf 7e1330795d76012fcb04248bb81d45b3 "Examples-CSharp-AsposePDF-Images-BradleyAlgorithm-BradleyAlgorithm.cs" >}}

## Custom Numbering Style for PageNumberStamp

The PageNumberStamp class offers the feature to add Page Number information as stamp object inside PDF document. Prior to this release, the class only supported 1,2,3,4 as page numbering style. However, there has been a requirement from the customers to use custom numbering style when placing page number stamp inside PDF document. In order to accomplish this requirement, **NumberingStyle** property has been introduced, which accepts the values from **NumberingStyle** enumeration. Specified below are values offered in this enumeration.

*   LettersLowercase
*   LettersUppercase
*   NumeralsArabic
*   NumeralsRomanLowercase
*   NumeralsRomanUppercase

### DOM Approach

{{< gist aspose-pdf 7e1330795d76012fcb04248bb81d45b3 "Examples-CSharp-AsposePDF-Stamps-Watermarks-PageNumberStamps-PageNumberStamps.cs" >}}

### Facades Approach

{{< gist aspose-pdf 4a12f0ebd453e7f0d552ed6658ed3253 "Examples-CSharp-AsposePdfFacades-Stamps-Watermarks-AddPageNumber-CustomNumberStyle.cs" >}}

## Miscellaneous fixes

As well as the enhancements and features discussed above, there have been specific improvements regarding PDF to PDF/A, PDF to HTML, XPS to PDF, PDF to XPS, HTML to PDF, RedactionAnnotation, Text manipulation, and Image placement/manipulation in PDF document. Please download and try the latest release of [Aspose.PDF for .NET 11.6.0][2].




[1]: https://docs.aspose.com/
[2]: http://downloads.aspose.com/pdf/net





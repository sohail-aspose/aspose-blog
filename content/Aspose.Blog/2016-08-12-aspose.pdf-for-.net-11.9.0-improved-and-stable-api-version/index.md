---
title: 'Aspose.Pdf for .NET 11.9.0, improved and stable API version'
date: Fri, 12 Aug 2016 09:57:22 +0000
draft: false
url: /2016/08/12/aspose.pdf-for-.net-11.9.0-improved-and-stable-api-version/
author: Tilal Ahmad
summary: ''
tags: []
categories: ['Aspose.PDF Product Family']
---

[![][1]](https://blog.aspose.com/wp-content/uploads/sites/2/2016/08/aspose_pdf-for-net.jpg)We are pleased to announce the release of [Aspose.Pdf for .NET 11.9.0][2]. Mainly, it is a maintenance release where we have improved the API functionality by fixing a number of bugs, reported by our valued customers in previous versions. This adds further value to API stability and prove it more reliable for manipulation of PDF documents as compared to other APIs, available in the market. There are no major API changes in this release.

## Improvements

**PDF to PDFA conversion:** Some PDF document includes images with transparency settings and it is lost in PDFA conversion. We can fix graphical subsystem using Convert() method with ConvertTransparencyAction parameter.

**PDF to DOCX:** In this month's release we have fixed glyphs of font with incorrect width and document orientation issues in PDF to DOCX conversion, It improved the PDF to DOCX conversion feature.

**XFA to Standard Form conversion:** Dynamic form(XFA) to Standard form conversion feature is improved in this release. We have improved algorithm that reads XFA configuration sections, also several issues with positioning and rendering of XFA Draw elements were fixed.

In addition to above improvements, this version also includes some other important bug fixes as well. There have been specific improvements regarding HTML to PDF, PDF to HTML, XML to PDF and PDF to PPTX. Please check release notes of Aspose.Pdf for .NET 11.9.0 for complete list of bug fixed.

## Public API Changes

The basic API change in this release is removal of Interfaces namespace.

**Added APIs:**

*   Interface Aspose.Pdf.GroupProcessor.IDocumentPageTextExtractor
*   Property Aspose.Pdf.GroupProcessor.IDocumentPageTextExtractor.PageCount
*   Method Aspose.Pdf.GroupProcessor.IDocumentPageTextExtractor.ExtractPageText(System.Int32)
*   Interface Aspose.Pdf.GroupProcessor.IDocumentTextExtractor
*   Method Aspose.Pdf.GroupProcessor.IDocumentTextExtractor.ExtractAllText
*   Interface Aspose.Pdf.GroupProcessor.IPdfTypeExtractor
*   Property Aspose.Pdf.GroupProcessor.IPdfTypeExtractor.PageCount
*   Property Aspose.Pdf.GroupProcessor.IPdfTypeExtractor.Version
*   Property Aspose.Pdf.GroupProcessor.IPdfTypeExtractor.IsFastExtractionUsed
*   Method Aspose.Pdf.GroupProcessor.IPdfTypeExtractor.ExtractAllText
*   Method Aspose.Pdf.GroupProcessor.IPdfTypeExtractor.ExtractPageText(System.Int32)
*   Method Aspose.Pdf.GroupProcessor.IPdfTypeExtractor.Dispose

**Removed APIs:**

*   Interface Aspose.Pdf.GroupProcessor.Interfaces.IDocumentPageTextExtractor
*   Property Aspose.Pdf.GroupProcessor.Interfaces.IDocumentPageTextExtractor.PageCount
*   Method Aspose.Pdf.GroupProcessor.Interfaces.IDocumentPageTextExtractor.ExtractPageText(System.Int32)
*   Interface Aspose.Pdf.GroupProcessor.Interfaces.IDocumentTextExtractor
*   Method Aspose.Pdf.GroupProcessor.Interfaces.IDocumentTextExtractor.ExtractAllText
*   Interface Aspose.Pdf.GroupProcessor.Interfaces.IPdfTypeExtractor
*   Property Aspose.Pdf.GroupProcessor.Interfaces.IPdfTypeExtractor.PageCount
*   Property Aspose.Pdf.GroupProcessor.Interfaces.IPdfTypeExtractor.Version
*   Property Aspose.Pdf.GroupProcessor.Interfaces.IPdfTypeExtractor.IsFastExtractionUsed
*   Method Aspose.Pdf.GroupProcessor.Interfaces.IPdfTypeExtractor.ExtractAllText
*   Method Aspose.Pdf.GroupProcessor.Interfaces.IPdfTypeExtractor.ExtractPageText(System.Int32)
*   Method Aspose.Pdf.GroupProcessor.Interfaces.IPdfTypeExtractor.Dispose

## Aspose.Pdf for .NET Resources

The following resources will help you work with Aspose.Pdf for .NET:

*   [Home page for Aspose.Pdf for .NET][3]
*   [Download Aspose.Pdf for .NET][4]
*   [Aspose.Pdf product family forum][5] – Post your technical questions and queries, or any other problem you faced while running Aspose.Pdf APIs.
*   Aspose.Pdf for .NET online documentation – help documentation.
*   [Aspose.Pdf for .NET online API reference][6] - API reference documents.
*   [Enable Blog Subscription][7] – Do not limit yourself, you can keep yourself updated with the latest news on Aspose.Pdf APIs, new features, fixes and other API related topics by subscribing to Aspose.Pdf blog.
*   [Aspose.Pdf for .NET Examples][8] – We have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: https://blog.aspose.com/wp-content/uploads/sites/2/2016/08/aspose_pdf-for-net.jpg "aspose_pdf-for-net"
[2]: http://www.aspose.com/downloads/pdf/net/new-releases/aspose.pdf-for-.net-11.9.0/
[3]: http://www.aspose.com/products/pdf/net
[4]: http://www.aspose.com/downloads/pdf/net
[5]: http://www.aspose.com/community/forums/aspose.pdf-product-family/20/showforum.aspx
[6]: http://www.aspose.com/api/net/pdf
[7]: https://blog.aspose.com/
[8]: https://github.com/aspose-pdf/Aspose.Pdf-for-.NET





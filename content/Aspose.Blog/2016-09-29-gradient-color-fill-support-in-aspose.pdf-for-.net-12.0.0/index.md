---
title: 'Fill Graph Objects with Gradient Colors in PDF using C# or VB.NET'
date: Thu, 29 Sep 2016 06:34:04 +0000
draft: false
url: /2016/09/29/gradient-color-fill-support-in-aspose.pdf-for-.net-12.0.0/
author: Tilal Ahmad
summary: ''
tags: []
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/aspose_pdf-for-net2.jpg" alt="">}}


We are pleased to announce the release of [Aspose.PDF for .NET 12.0.0][1]. This release includes number of improvements along with a new Gradient color fill feature. Now we can fill Graph objects with gradient color with the release of this version. We have improved TableAbsorber class along with other bug fixes, reported in earlier releases, that improved the quality of Aspose.Pdf for .NET API. Please check the detailed [release notes of Aspose.PDF for .NET 12.0.0][2], in order to get an idea about the new features and improvements made in this release of Aspose.Pdf for .NET. The following sections describe some details regarding these newly added features/enhancements.

## Fill Graphs with Gradient Color in PDF

In this release we have introduce gradient color fill feature. We can [fill Graph objects with gradient colors][3] using PatterColorSpace and GradientAxialShading objects as following:

{{< gist aspose-com-gists 63473b1ba28e09e229cfbf4430eabd8a "Examples-CSharp-AsposePDF-Graphs-AddDrawingWithGradientFill-AddDrawingWithGradientFill.cs" >}}

## Convert PDF to DOCX

Some of the customers are complaining the rendering quality of contents of resultant DOC(X). So in this release we have set default ImageResolution to 300 dpi. It will increase the resultant file size, as rendering quality is more important than file size for the customers. We can change the resolution as per our requirements.

```
Aspose.Pdf.DocSaveOptions saveOptions = new Aspose.Pdf.DocSaveOptions();

saveOptions.Format = Aspose.Pdf.DocSaveOptions.DocFormat.Doc;

saveOptions.Mode = Aspose.Pdf.DocSaveOptions.RecognitionMode.Flow;

saveOptions.RecognizeBullets = (true);

saveOptions.ImageResolutionX = 150;

saveOptions.ImageResolutionY = 150;
```

## Improvements

**Working with tables in existing PDF documents:** We have improved TableAbsorber object, it improved the Table manipulation feature of Aspose.Pdf for .NET.

**PDF to PDFA conversion:** We have fixed number of issues related to PDF to PDFA conversion in this release. It added a great value to stability and reliability of the API.

In addition to the above-stated improvements, this version also includes some other important bug fixes as well. There have been specific improvements regarding PDF to HTML, PDF to Images and PDF to XPS. Please check [release notes of Aspose.PDF for .NET 12.0.0][4] for a complete list of bug fixed.

## Public API Changes

If you are planning to upgrade the API from any previous version, we strongly suggest you to check the Public API Changes section of current release and other intermediate releases, to know what has been changed since your current revision of the API.

## Aspose.Pdf for .NET Resources

The following resources will help you work with Aspose.Pdf for .NET:

*   [Home page for Aspose.Pdf for .NET][5]
*   [Download Aspose.Pdf for .NET][6]
*   [Aspose.Pdf product family forum][7] – Post your technical questions and queries, or any other problem you faced while running Aspose.Pdf APIs.
*   Aspose.Pdf for .NET online documentation – help documentation.
*   [Aspose.Pdf for .NET online API reference][8] - API reference documents.
*   [Enable Blog Subscription][9] – Do not limit yourself, you can keep yourself updated with the latest news on Aspose.Pdf, APIs, new features, fixes and other API related topics by subscribing to Aspose.Pdf blog.
*   [Aspose.Pdf for .NET Examples][10] – We have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: https://downloads.aspose.com/pdf/net
[2]: https://docs.aspose.com/display/pdfnet/Aspose.Pdf+for+.NET+12.0.0+Release+Notes
[3]: https://docs.aspose.com/display/pdfnet/Working+with+Graphs#WorkingwithGraphs-AddDrawingwithGradientFill
[4]: https://docs.aspose.com/display/pdfnet/Aspose.Pdf+for+.NET+12.0.0+Release+Notes
[5]: http://www.aspose.com/products/pdf/net
[6]: http://www.aspose.com/downloads/pdf/net
[7]: http://www.aspose.com/community/forums/aspose.pdf-product-family/20/showforum.aspx
[8]: http://www.aspose.com/api/net/pdf
[9]: https://blog.aspose.com/
[10]: https://github.com/aspose-pdf/Aspose.Pdf-for-.NET





---
title: 'Convert PDF documents into other File Formats and Optimize Resources with Aspose.PDF'
date: Sun, 23 Dec 2018 19:43:04 +0000
draft: false
url: /2018/12/23/convert-pdf-documents-into-other-file-formats-and-optimize-resources-with-aspose.pdf/
author: Asad Ali
summary: ''
tags: ['Asad Ali', 'Resource optimization of PDF documents']
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/aspose-Pdf-for-net.png" alt="Optimize resources in PDF documents">}}


It is our pleasure to announce November Release of Aspose.PDF API which has been launched for .NET and Java Platforms and available for download. In this revision of the API, conversion engines have been further improved in order to convert PDF documents into other file formats. Several bugs which were reported in earlier version(s) of the API have also been rectified. Along with that, resource optimization of PDF documents has been improved in terms of performance. In case you are planning to download and use this release of the API, you may please use following links in order to download it as per your platform e.g. .NET/Java:

*   [Aspose.PDF for .NET 18.11][1]
*   [Aspose.PDF for Java 18.11][2]

It is also recommended to go through the release notes pages of these releases before downloading and using it in your environment. Release notes are present in respective API documentation over below links:

*   [Release Notes of Aspose.PDF for .NET 18.11][3]
*   [Release Notes of Aspose.PDF for Java 18.11][4]

Following section includes insights into worth mentioning features in this release of Aspose.PDF API.

## Optimize PDF Resources

It was observed that execution time of **OptimizeResources** method was slow in earlier version(s) of the API which was due to slow image compression. In this release of the API, new image compression algorithms have been implemented which work faster and you can optimize PDF documents in an improved and faster way. Following sample code snippet can be used to optimize PDF resources using new implemented properties:

**\[C#.NET\]**

```
Document doc = new Document("source.pdf");
Aspose.Pdf.Optimization.OptimizationOptions opt =
new Aspose.Pdf.Optimization.OptimizationOptions(); 
opt.LinkDuplcateStreams = true; 
opt.RemoveUnusedObjects = false; 
opt.AllowReusePageContent = true; 
opt.RemoveUnusedStreams = true; 
opt.UnembedFonts = false; 
opt.ImageCompressionOptions.CompressImages = true; opt.ImageCompressionOptions.ImageQuality = 50; opt.ImageCompressionOptions.ResizeImages = false; opt.ImageCompressionOptions.Version = ImageCompressionVersion.Fast; doc.OptimizeResources(opt);
```

**\[Java\]  
**

```
Document doc = new Document("source.pdf");
com.aspose.pdf.optimization.OptimizationOptions opt =
new com.aspose.pdf.optimization.OptimizationOptions();
opt.setLinkDuplcateStreams(true);
opt.setRemoveUnusedObjects(false);
opt.setAllowReusePageContent(true);
opt.setRemoveUnusedStreams(true);
opt.setUnembedFonts(false);
opt.getImageCompressionOptions().setCompressImages(true);
opt.getImageCompressionOptions().setImageQuality(50);
opt.getImageCompressionOptions().setResizeImages(false);
opt.getImageCompressionOptions().setVersion(ImageCompressionVersion.Fast);
doc.optimizeResources(opt);
```

## Miscellaneous Fixes

Along with the features mentioned above, following are some useful improvement which have been included in this release of the API:

*   Implemented precise coordinate calculations for characters
*   Improvements have been made for working with Form Fields
*   Hyperlink Alignment issues have been rectified
*   Improved PDF Printing time taken by the API
*   Color corrections have been made during PDF to TIFF conversion
*   Table Extraction and Manipulation algorithms have further been enhanced
*   Functionality to support text and fonts has been added for PDF/UA format

## Aspose.PDF for .NET and Java Resources

**The following resources will help you work with Aspose.PDF for .NET and Java:**

*   [Home page for Aspose.PDF API][5].
*   Aspose.PDF for [.NET][6] and [Java][7] wiki docs – Help documentation and API reference documents.
*   [Aspose.PDF product family forum ][8]– Post your technical questions, queries and any other problem you faced while running Aspose.PDF APIs.
*   [Enable Email Subscription ][9]– Do not limit yourself, stay up-to-date with the latest news about the Aspose.PDF APIs and new features, fixes, plus other API related topics by subscribing to Aspose.PDF blog.
*   [Aspose.PDF for .NET Examples ][10]– We have published our code examples on the social coding website GitHub.com. Anyone can explore the code examples for learning purposes.
*   [Aspose.PDF for Java Examples][11] – We have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.
*   Release Notes ([.NET][12] and [Java][13] – For details on API fixes, please check Release Notes having a complete list of the new features.




[1]: https://www.nuget.org/packages/Aspose.Pdf/18.11.0
[2]: https://artifact.aspose.com/repo/com/aspose/aspose-pdf/18.11/
[3]: https://docs.aspose.com/display/pdfnet/Aspose.PDF+for+.NET+18.11+Release+Notes
[4]: https://docs.aspose.com/display/pdfjava/Aspose.PDF+for+Java+18.11+Release+Notes
[5]: http://products.aspose.com/pdf
[6]: https://docs.aspose.com/display/pdfnet/Home
[7]: https://docs.aspose.com/display/pdfjava/Home
[8]: https://forum.aspose.com/c/pdf
[9]: https://blog.aspose.com/category/aspose-products/aspose-pdf-product-family/
[10]: https://github.com/aspose-pdf/Aspose.Pdf-for-.NET
[11]: https://github.com/aspose-pdf/Aspose.Pdf-for-java
[12]: https://docs.aspose.com/display/pdfnet/Aspose.Pdf+for+.NET+18.11+Release+Notes
[13]: https://docs.aspose.com/display/pdfjava/Aspose.PDF+for+Java+18.11+Release+Notes)





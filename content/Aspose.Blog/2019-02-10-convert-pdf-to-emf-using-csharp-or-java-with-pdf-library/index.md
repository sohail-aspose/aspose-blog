---
title: 'Convert PDF to EMF using C# or Java'
date: Sun, 10 Feb 2019 20:55:39 +0000
draft: false
url: /2019/02/10/convert-pdf-to-emf-using-csharp-or-java-with-pdf-library/
author: Asad Ali
summary: ''
tags: ['Asad Ali', 'Convert PDF to EMF using Csharp', 'Convert PDF to EMF using Java']
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/aspose-Pdf-for-net.png" alt="">}}


We are honored to announce 19.1 version of Aspose.PDF API which has been rolled out with a lot of improvements in terms of performance and usability. API has already been published and is available for download and to be used in both .NET and Java Applications. In this release of API, more than 30 improvements have been included along with various enhancement in existing functionalities. In case you are planning to download and consume this revision of the API, you may please navigate over following links in order to download it as per your platform e.g. .NET/Java:

*   [Aspose.PDF for .NET 19.1][1]
*   [Aspose.PDF for Java 19.1][2]

While using the latest release of the API, it is always recommended to have a detailed look over its release notes. Release notes of the API contain complete information of new improvements in the API as well as Public API Changes which are part of new revision. Following links will take you to the release notes page(s) of the API in documentation:

*   [Release Notes of Aspose.PDF for .NET 19.1][3]
*   [Release Notes of Aspose.PDF for Java 19.1][4]

The following section offers highlights of worth mentioning enhancements in this release of the API.

## Convert PDF into EMF

Converting PDF into EMF was already supported in Aspose.PDF API. However, using new revision of the API, you can achieve better results as new improvements have been made to PDF to EMF Conversion Engine to produce fine images. Following code snippet shows usage of this conversion feature:

**\[C#.NET\]**

```
Document doc = new Document("c:/pdftest/document\_with\_table.pdf");  
Aspose.Pdf.Devices.EmfDevice emf =   
new EmfDevice(new Aspose.Pdf.Devices.Resolution(300));  
emf.Process(doc.Pages\[1\], "c:/pdftest/document\_with\_table.emf");
```

## Improvements in Aspose.PDF v19.1

As mentioned above, there are various improvements which have been included in this release of the API to increase its usability factor and performance. Following list shows some highlights about these improvements:

*   Following Conversion Engines have been improved further:
    *   PDF to TIFF
    *   PDF to Image
    *   HTML to PDF
    *   PDF to SVG
    *   PDF to PPTX
    *   PDF to HTML
    *   PDF to PDF/UA
    *   PDF to PDF/A
    *   PCL to PDF
*   Improvements have been made for Text editing and replacement scenarios
*   PDF Security features have been optimized
*   Memory consumption has been improved further
*   PDF Flattening feature has been further improved
*   Concatenation operations of PDF Documents have been optimized for better performance

## Aspose.PDF for .NET and Java Resources

**The following resources will help you work with Aspose.PDF for .NET and Java:**

*   [Home page for Aspose.PDF API][5].
*   Aspose.PDF for [.NET][6] and [Java][7] wiki docs – Help documentation and API reference documents.
*   [Aspose.PDF product family forum ][8]– Post your technical questions, queries and any other problem you faced while running Aspose.PDF APIs.
*   [Enable Email Subscription ][9]– Do not limit yourself, stay up-to-date with the latest news about the Aspose.PDF APIs and new features, fixes, plus other API related topics by subscribing to Aspose.PDF blog.
*   [Aspose.PDF for .NET Examples ][10]– We have published our code examples on the social coding website GitHub.com. Anyone can explore the code examples for learning purposes.
*   [Aspose.PDF for Java Examples][11] – We have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.
*   Release Notes ([.NET][12] and [Java][13] – For details on API fixes, please check Release Notes having a complete list of the new features.




[1]: https://www.nuget.org/packages/Aspose.Pdf/19.1.0
[2]: https://repository.aspose.com/repo/com/aspose/aspose-pdf/19.1/
[3]: https://docs.aspose.com/display/pdfnet/Aspose.PDF+for+.NET+19.1+Release+Notes
[4]: https://docs.aspose.com/display/pdfjava/Aspose.PDF+for+Java+19.1+Release+Notes
[5]: http://products.aspose.com/pdf
[6]: https://docs.aspose.com/display/pdfnet/Home
[7]: https://docs.aspose.com/display/pdfjava/Home
[8]: https://forum.aspose.com/c/pdf
[9]: https://blog.aspose.com/category/aspose-products/aspose-pdf-product-family/
[10]: https://github.com/aspose-pdf/Aspose.Pdf-for-.NET
[11]: https://github.com/aspose-pdf/Aspose.Pdf-for-java
[12]: https://docs.aspose.com/display/pdfnet/Aspose.Pdf+for+.NET+19.1+Release+Notes
[13]: https://docs.aspose.com/display/pdfjava/Aspose.PDF+for+Java+19.1+Release+Notes)





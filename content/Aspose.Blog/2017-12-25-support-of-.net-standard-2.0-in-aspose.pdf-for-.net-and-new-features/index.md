---
title: 'C# PDF API for .NET Standard 2.0 - Aspose.PDF for .NET with New Features'
date: Mon, 25 Dec 2017 21:21:53 +0000
draft: false
url: /2017/12/25/support-of-.net-standard-2.0-in-aspose.pdf-for-.net-and-new-features/
author: Asad Ali
summary: ''
tags: ['.NET Core PDF API', '.NET Core PDF Library', '.NET standard PDF library', 'Asad Ali', 'Generate PDF in .NET Core', 'Generate PDF in .NET Standard', 'PDF API for ASP.NET Core']
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/aspose-Pdf-for-net.png" alt="PDF Library for .NET Standard 2.0">}}


We are pleased to announce the new release of [Aspose.PDF for .NET 17.12][1]. The latest release has the compatibility to work with **.NET Standard 2.0**. So you can now create, edit, manipulate and convert PDF documents in **.NET Standard 2.0** or **.NET Core 2.0** applications. In case you are planning to upgrade your existing version of the API to the latest version, we would strongly recommend you to please check [release notes][2] of Aspose.PDF for .NET 17.12 for an overview of API changes and improvements.

## Support of .NET Standard 2.0

Starting from Aspose.PDF for .NET 17.12, this API includes **.NET Standard 2.0** version. Our product team has ported complete functionality of regular .NET version of Aspose.Pdf, into .NET Standard 2.0 version. Since this is the first version with .NET Standard 2.0 support, so in the features related to graphics, there may be some problems and our product team has been working hard to fix them.

## Add Text with Gradient Fill in PDF

We have implemented support of gradient fill for text adding scenarios. Setting gradient fill to TextFragment/TextSegment’s foreground color is going to be operable in Aspose.PDF for .NET 17.12. Following code snippet can be used to set foreground color with gradient fill:

```
// Create new color with pattern colorspace
textFragment.TextState.ForegroundColor = new Aspose.Pdf.Color
{
    // Set PatternColorSpace to linear gradient with 
    // red starting color and blue ending color
    PatternColorSpace = 
    new GradientAxialShading(Color.Red, Color.Blue)
};
```

## Hide Page Numbers in TOC in PDF

While adding TOC (Table of Contents) in the PDF documents, usually headings in the list, are showed with page numbers where they navigate you after clicking them. Sometimes, you want to display only text without page numbers in the table of contents. In Aspose.PDF for .NET 17.12 release, you will be able to hide page numbers in table of contents by using new boolean property [IsShowPageNumbers][3] of [TocInfo][4] class.

## Use SVG Image in Stamp Annotation in PDF

In the earlier version(s) of Aspose.PDF for .NET, [StampAnnotation][5] class supported JPEG and PNG images for stamps – whereas in new 17.12 version of the API, it is feasible to use SVG image in Stamp Annotation:

```
Document doc = new Document();
doc.Pages.Add();
Aspose.Pdf.Annotations.StampAnnotation stamp = 
new Aspose.Pdf.Annotations.StampAnnotation(doc.Pages[1], 
new Aspose.Pdf.Rectangle(10,10,100,100));
stamp.Image = 
new FileStream("c:/pdftest/CHRISTMAS_004.svg", FileMode.Open);
doc.Pages[1].Annotations.Add(stamp);
doc.Save("c:/pdftest/stampannotation.pdf");
```

## Miscellaneous Fixes

Apart from the above-mentioned enhancements and features, we have also provided fixes against many issues. In order to check the complete list of issues that have been fixed in this release of Aspose.PDF for .NET, please check the [Release Notes][6] section of Aspose.PDF for .NET 17.12.

As it is always recommended to use the latest release of our API’s, so we suggest you to please download the latest release [Aspose.PDF for .NET 17.12 and check the][7] following resources which will help you working with API:

*   [Home page for Aspose.PDF for .NET][8]
*   [Download Aspose.PDF for .NET][9]
*   [Aspose.PDF product family forum][10]– Post your technical questions and queries, or any other problem you faced while running Aspose.Pdf APIs.
*   [Aspose.PDF for .NET online documentation][11]– help documentation and API reference documents.
*   [Enable Blog Subscription][12]– Do not limit yourself, you can keep yourself updated with the latest news on Aspose.Pdf APIs, new features, fixes and other API related topics by subscribing to Aspose.Pdf blog.
*   [Aspose.PDF for .NET Examples][13] – We have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: https://www.nuget.org/packages/Aspose.Pdf/17.12.0
[2]: https://docs.aspose.com/display/pdfnet/Aspose.Pdf+for+.NET+17.12+Release+Notes
[3]: https://apireference.aspose.com/net/pdf/aspose.pdf/tocinfo/properties/isshowpagenumbers
[4]: https://apireference.aspose.com/net/pdf/aspose.pdf/tocinfo
[5]: https://apireference.aspose.com/net/pdf/aspose.pdf.annotations/stampannotation/
[6]: https://docs.aspose.com/display/pdfnet/Aspose.Pdf+for+.NET+17.12+Release+Notes
[7]: https://www.nuget.org/packages/Aspose.Pdf/17.12.0
[8]: https://products.aspose.com/pdf/net
[9]: https://www.nuget.org/packages/Aspose.Pdf/
[10]: https://forums.aspose.com/c/pdf
[11]: https://docs.aspose.com/display/pdfnet/Home
[12]: https://blog.aspose.com/category/pdf/
[13]: https://github.com/aspose-pdf/Aspose.Pdf-for-.NET





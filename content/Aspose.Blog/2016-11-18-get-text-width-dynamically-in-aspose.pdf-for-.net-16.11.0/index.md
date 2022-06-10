---
title: 'Get Text Width Dynamically in Aspose.PDF for .NET 16.11.0'
date: Fri, 18 Nov 2016 18:40:40 +0000
draft: false
url: /2016/11/18/get-text-width-dynamically-in-aspose.pdf-for-.net-16.11.0/
author: Tilal Ahmad
summary: ''
tags: ['C# PDF API', 'Get text width dynamically in PDF', 'Search Text in PDF']
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/aspose_pdf-for-net.jpg" alt="">}}


We are pleased to announce the release of [Aspose.PDF for .NET 16.11.0][1]. This release includes a number of improvements along with a new feature to get text width dynamically. We have received a number of requests to provide some functionality to get text width dynamically in public API, and we have implemented this feature in the current release. We have improved PDF to PDFA conversion, PDF to DOC/DOCX conversion along with many other bug fixes, reported in earlier releases, that improved the quality of Aspose.Pdf for .NET API to make it more stable. Please check the detailed [release notes of Aspose.PDF for .NET 16.11.0][2], in order to get an idea about the new features and improvements made in this release of Aspose.Pdf for .NET.

Please note If you are planning to upgrade the API from any previous version, we strongly recommend you to check the Public API Changes Section of other intermediate releases from release notes pages, to know what has been changed since your current revision of the API.

The following sections describe some details regarding these newly added features/enhancements.

## Features

**Text width dynamically:** With the release of this version, now we can [get text width dynamically][3] with the use of MeasureString() method. We can invoke MeasureString() method of Aspose.PDF.Text.Font or Aspose.Pdf.Text.TextState classes (or both):

```
Aspose.Pdf.Text.Font font = FontRepository.FindFont("Arial");
Console.WriteLine(font.MeasureString("Sample text", 14));
TextState ts = new TextState();
ts.Font = font;
ts.FontSize = 14;
Console.WriteLine(ts.MeasureString("Sample text"));
for (char c = 'A'; c <= 'z'; c++)
{
double fnMeasure = font.MeasureString(c.ToString(), 14);
double tsMeasure = ts.MeasureString(c.ToString());
Console.WriteLine(String.Format("{0} - font measure {1}", c, fnMeasure));
Console.WriteLine(String.Format("{0} - text state measure {1}", c, tsMeasure));
}
```

**Text Searching :** We have improved the text searching procedure. From Aspose.Pdf 16.10 TextFragmentAbsorber returns text under rectangle more accurate. The rectangle may be specified with TextFragmentAbsorber.TextSearchOptions.Rectangle property.

```
 //create TextAbsorber object to find all instances of the input search phrase
TextFragmentAbsorber textFragmentAbsorber = new TextFragmentAbsorber();
textFragmentAbsorber.TextSearchOptions.LimitToPageBounds = true;
textFragmentAbsorber.TextSearchOptions.Rectangle = new Aspose.Pdf.Rectangle(100, 700, 195, 650);
//accept the absorber for all the pages
document.Pages.Accept(textFragmentAbsorber);
```

## Improvements

**PDF to PDFA conversion:** This feature is very much improved in this release, as we have fixed number of PDFA related issues in Aspose.Pdf for .NET 16.11.0.

**PDF to DOC/DOCX:** PDF to DOC/DOCX conversion is a key feature of our API. We have resolved some issues in this release that enhanced the feature reliability.

In addition to the above-stated improvements, this version also includes some other important bug fixes as well. There have been specific improvements regarding HTML to PDF, PDF to HTML, Text Replacement and  PDF to XPS. Please check release notes of Aspose.PDF for .NET 16.11.0 for a complete list of bug fixed.

## Aspose.Pdf for .NET Resources

The following resources will help you work with Aspose.Pdf for .NET:

*   [Home page for Aspose.PDF for .NET][4]
*   [Download Aspose.PDF for .NET][5]
*   [Aspose.PDF product family forum][6] – Post your technical questions and queries, or any other problem you faced while running Aspose.Pdf APIs.
*   Aspose.PDF for .NET online documentation – help documentation.
*   [Aspose.PDF for .NET online API reference][7] - API reference documents.
*   [Enable Blog Subscription][8] – Do not limit yourself, you can keep yourself updated with the latest news on Aspose.Pdf, APIs, new features, fixes and other API related topics by subscribing to Aspose.Pdf blog.
*   [Aspose.PDF for .NET Examples][9] – We have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: https://downloads.aspose.com/pdf/net
[2]: https://docs.aspose.com/display/pdfnet/Aspose.PDF+for+.NET+16.11.0+Release+Notes
[3]: https://docs.aspose.com/display/pdfnet/Add+Text+to+a+PDF+file#AddTexttoaPDFfile-GetTextWidthDynamically
[4]: https://products.aspose.com/pdf/net
[5]: http://downloads.aspose.com/pdf/net
[6]: https://forum.aspose.com/c/pdf
[7]: https://apireference.aspose.com/net/pdf
[8]: https://blog.aspose.com/
[9]: https://github.com/aspose-pdf/Aspose.Pdf-for-.NET





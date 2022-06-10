---
title: 'Process Line Breaking and Create Clones of TextFragments with Aspose.PDF for .NET 18.4'
date: Mon, 23 Apr 2018 00:37:25 +0000
draft: false
url: /2018/04/23/process-line-breaking-and-create-clones-of-textfragments-with-aspose.pdf-for-.net-18.4/
author: Asad Ali
summary: ''
tags: ['Asad Ali']
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/aspose-Pdf-for-net.png" alt="">}}


As per the monthly update process of Aspose APIs, we are pleased to announce the new April Release of Aspose.PDF for .NET. [Aspose.PDF for .NET 18.4][1] is available on NuGet Gallery for download and to be used in .NET applications. Like every new release of the API, [Aspose.PDF for .NET 18.4][2] has been launched with exciting features and enhancements. In order to have an overview of improvements and changes in this release of the API, we recommend you visit the [release notes][3] page of Aspose.PDF for .NET 18.4.

## Determine Line Break

In particular scenarios of PDF generations, sometimes you may come up with a requirement to identify the points/positions where an Enter/Line Break was added to create a new line or contents of a line were moved to the subsequent line after content reaching to the edge of the page. We have implemented logging (tracking) background processing (line breaking) of multi-line text fragments in text adding scenarios. You can use [GetNotifications()][4], a new method of Page Class in order to achieve the functionality. An example of such functionality has been provided in API documentation on the following link:

*   [Track Line Breaking of Multi-Line TextFragments][5]

Since we have already planned to improve the feature to support of such scenarios, we are working over adding the functionalities for editing existing PDF documents. We hope to provide more enhancements in API regarding this feature in upcoming versions. For now, only notifications about paragraph events in text adding scenarios are supported.

## Clone TextFragments with Identical Formatting

One of the interesting enhancements in Aspose.PDF for .NET 18.4 is, you can clone a TextFragment with segments formatting identical to the original fragment. You can use [TextFragment.Clone()][6] method in order to achieve this. Following code snippet shows how you can implement this feature in your application:

```
Document doc = new Document();
Page page = doc.Pages.Add();
TextFragment text = new TextFragment("some text");
TextSegment segment = new TextSegment("some segment");
segment.TextState.FontSize = 40;
text.Segments.Add(segment);
text = text.Clone() as TextFragment;
page.Paragraphs.Add(text);
doc.Save(outFile);
```

## Miscellaneous

As it is always recommended to use the latest release of our API’s, so we suggest you please download the latest release [Aspose.PDF for .NET 18.4][7] and check following resources which will help you working with API:

*   [Home page for Aspose.PDF for .NET][8]
*   [Download Aspose.PDF for .NET 18.4][9]
*   [Aspose.PDF product family forum][10]– Post your technical questions and queries, or any other problem you faced while running Aspose.PDF APIs.
*   [Aspose.PDF for .NET online documentation][11]– help documentation and API reference documents.
*   [Enable Blog Subscription][12]– Do not limit yourself, you can keep yourself updated with the latest news on Aspose.PDF APIs, new features, fixes and other API related topics by subscribing to Aspose.PDF blog.
*   [Aspose.PDF for .NET Examples][13] – We have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: https://www.nuget.org/packages/Aspose.Pdf/18.4.1
[2]: https://www.nuget.org/packages/Aspose.Pdf/18.4.1
[3]: https://docs.aspose.com/display/pdfnet/Aspose.PDF+for+.NET+18.4+Release+Notes
[4]: https://apireference.aspose.com/net/pdf/aspose.pdf/page/methods/getnotifications
[5]: https://docs.aspose.com/display/pdfnet/Determine+Line+Break#DetermineLineBreak-TrackLineBreakingofMulti-LineTextFragment
[6]: https://apireference.aspose.com/net/pdf/aspose.pdf.text/textfragment/methods/clone
[7]: https://www.nuget.org/packages/Aspose.Pdf/18.4.1
[8]: https://products.aspose.com/pdf/net
[9]: https://www.nuget.org/packages/Aspose.Pdf/18.4.1
[10]: https://forums.aspose.com/c/pdf
[11]: https://docs.aspose.com/display/pdfnet/Home
[12]: https://blog.aspose.com/category/aspose-products/aspose-pdf-product-family/
[13]: https://github.com/aspose-pdf/Aspose.PDF-for-.NET





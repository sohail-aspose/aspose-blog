---
title: 'Set TOC Line Style to None in PDF using C#'
date: Tue, 25 Oct 2016 17:49:52 +0000
draft: false
url: /2016/10/25/set-toc-line-style-to-none-wrap-lines-implementation-and-calculate-text-index-in-textfragment-with-aspose.pdf-for-.net-16.10.0/
author: Tilal Ahmad
summary: ''
tags: []
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/aspose_pdf-for-net.jpg" alt="">}}


[Aspose.PDF for .NET 16.10.0][1] has been released. This month's release includes the features to set TOC line style to None, wrap lines as well as some other important enhancements. It also contains a number of fixes of bugs reported in previous versions by our valued customers, which makes it a more stable and reliable release as compared to previous releases. Please check the detailed [release notes of Aspose.PDF for .NET 16.10.0][2] to have an idea about the new features and improvements made in this release of Aspose.PDF for .NET.

The following sections describe some details regarding these newly added features/enhancements.

## Set TOC Line Style to None in PDF

Some customers have a business requirement to create TOC elements without any line style. So we have introduced a new LiesDash property in TocInfo class to set TOC dash line style to none in Aspose.PDF for .NET 16.10.0. Please check following code snippet to set LineDash value to None from TabLeaderType enum:

```
// Set the title for TOC
tocInfo.Title = title;
// Set TOC line dash style
tocInfo.LineDash = TabLeaderType.None;
tocPage.TocInfo = tocInfo;
```

## Remove XFA Data Structure of Dynamic Form in PDF

We have received a requirement to completely remove the XFA structure of a dynamic form instead of converting it to AcroForm. Now we can achieve this goal by converting the dynamic form to Standard AcroFrom and later flatten the form as follows. It will remove the XFA data structure from Dynamic Form.

```
Document doc = new Document("source.pdf");
doc.Form.Type = FormType.Standard;
doc.Form.Flatten();
doc.Save("result.pdf");
```

## Support of Wrap line in New Generator

We have introduced the Wrap line feature in the TextFragment class of the new generator. We can use this feature in all the Objects those support Paragraph object e.g. Page, Table object. We can accomplish this task by setting the desired value of WrapLinesCount property of TextFragment object as following:

```
string outFile = "WrapLine_Test.pdf";
Document doc = new Document();
Page page = doc.Pages.Add();
TextFragment title = new TextFragment("In process to move from Aspose.Pdf.Generator to Aspose.Pdf I need to Move from Text to TextFragment. I am not sure how i can wrap lines in TextFragment. I am not sure how I can wrap lines in TextFragment");
title.WrapLinesCount = 1;
page.Paragraphs.Add(title);
doc.Save(outFile); 
```

## Improvements

We have improved SVG to PDF conversion feature in this release by resolving some important issues. PDF to HTML conversion feature became more stable with this release, as we have fixed a number of issues related to PDF to HTML conversion. Especially font handling and local links rendering, that improve the text rendering quality in this conversion feature.

In addition to the above-stated improvements, this version also includes some other important bug fixes as well. There have been specific improvements regarding XFA to AcroFrom conversion, XPS to PDF, HTML to PDF, PDF to PDFA and PDF to Image conversion. Please check release notes of Aspose.PDF for .NET 16.10.0 for a complete list of bug fixed.

## Aspose.PDF for .NET Resources

The following resources will help you work with Aspose.PDF for .NET:

*   [Home page for Aspose.PDF for .NET][3]
*   [Download Aspose.PDF for .NET][4]
*   [Aspose.PDF product family forum][5] – Post your technical questions and queries, or any other problem you faced while running Aspose.PDF APIs.
*   [Aspose.PDF for .NET online documentation][6] – help documentation.
*   [Aspose.PDF for .NET online API reference][7] - API reference documents.
*   [Enable Blog Subscription][8] – Do not limit yourself, you can keep yourself updated with the latest news on Aspose.PDF, APIs, new features, fixes, and other API related topics by subscribing to Aspose.PDF blog.
*   [Aspose.PDF for .NET Examples][9] – We have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: https://downloads.aspose.com/pdf/net
[2]: http://docs.aspose.com/display/pdfnet/Aspose.Pdf+for+.NET+16.10.0+Release+Notes
[3]: http://products.aspose.com/pdf/net
[4]: http://downloads.aspose.com/pdf/net
[5]: http://forum.aspose.com
[6]: http://docs.aspose.com/display/pdfnet/Home
[7]: https://apireference.aspose.com/pdf/net
[8]: https://blog.aspose.com/aspose-products/aspose-pdf-product-family
[9]: https://github.com/aspose-pdf/Aspose.Pdf-for-.NET





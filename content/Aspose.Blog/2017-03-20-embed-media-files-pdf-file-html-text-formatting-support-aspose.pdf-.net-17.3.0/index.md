---
title: 'Embed Media Files in PDF File using Aspose.PDF for .NET 17.3.0'
date: Mon, 20 Mar 2017 04:27:45 +0000
draft: false
url: /2017/03/20/embed-media-files-pdf-file-html-text-formatting-support-aspose.pdf-.net-17.3.0/
author: Tilal Ahmad
summary: ''
tags: ['Calculate table width in PDF in Csharp', 'Embed media files in PDF Csharp', 'Format HTML text in PDF']
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/aspose_pdf-for-net.jpg" alt="">}}


We are pleased to announce a new release [Aspose.PDF for .NET 17.3.0][1]. This month's release includes a new feature to [calculate Table width][2] and [embed media files(audio and video) in PDF document][3] along with some other important features. We have also enhanced the Footnote feature and HTML text support in this version in addition to many other bug fixes reported in old releases that improve the APIs functionality. Please check the detailed [release notes of this version][4] to get an idea about the new features/enhancements and fixes made in this release.

Furthermore, If you are planning to upgrade the API from any previous version, we strongly recommend you to check the [Public API Changes section][5] of other intermediate releases from [release notes folder][6], to know what has been changed since your current revision of the API.

The following sections describe some details regarding these newly added enhancements.

## Embed Media files in PDF Document

We have implemented a [new annotation RichMediaAnnotation][7] in Aspose.PDF for .NET 17.3.0. It is used to embed media files within PDF documents. In fact, RichMediaAnnotation is the container for the SWF (Flash) script. Due to license restriction, we cannot include third-party flash scripts in our product, so you should provide your own script for playing video or audio. For example, you can use VideoPlayer and AudioPlayer shipped with Adobe Acrobat. Please check the [documentation link][8] for sample code and details to embed video/audio files in PDF document using RichMediaAnnotation.

## Calculate Table Width

In some scenarios, you have not hardcoded the Table width in PDF document and later you want to know its width for some post-processing. We have introduced a new method GetWidth() to calculate Table width in this release. It renders the table and gets its width as follows:

```
Aspose.Pdf.Table table = new Aspose.Pdf.Table();
table.ColumnAdjustment = ColumnAdjustment.AutoFitToContent;
Aspose.Pdf.Row row = table.Rows.Add();
Aspose.Pdf.Cell cell1 = row.Cells.Add("Cell 1");
Aspose.Pdf.Cell cell2 = row.Cells.Add("Cell 2 text");
// get Table width
Console.WriteLine(table.GetWidth());
// get cell width
Console.WriteLine(cell1.Width);
```

## HTML Text Formatting

Aspose.PDF supports the insertion of HTML string in PDF document. If HTML specified fonts are available on the host system then it uses the same fonts, otherwise, it uses system default fonts for HTML string. We have received some requirements to support font overriding feature for HTML string. We have implemented TextState object in HtmlFramgent class, now you can override font details of HTML string as follows:

```
Aspose.Pdf.Document doc = new Aspose.Pdf.Document();
Page page = doc.Pages.Add();
HtmlFragment html = new HtmlFragment("some text");
html.TextState = new TextState();
html.TextState.Font = FontRepository.FindFont("Calibri");
page.Paragraphs.Add(html);
doc.Save(myDir+"test.pdf");
```

## FootNote Color

In the current release, we have also added support to set the color of the FootNote label(node identifier). We have implemented a TextState object in the FootNote class. You can set FootNote label color using TextState as following:

```
Aspose.Pdf.Document doc = new Aspose.Pdf.Document();
Page page = doc.Pages.Add();
Aspose.Pdf.GraphInfo graph = new Aspose.Pdf.GraphInfo();
graph.LineWidth = 2;
graph.Color = Aspose.Pdf.Color.Red;
graph.DashArray = new int[] { 3 };
graph.DashPhase = 1;
page.NoteLineStyle = graph;
TextFragment text = new TextFragment("test text 1");
text.FootNote = new Note("foot note for test text 1");
text.FootNote.Text = "21";
text.FootNote.TextState = new TextState();
text.FootNote.TextState.ForegroundColor = Aspose.Pdf.Color.Blue;
text.FootNote.TextState.FontStyle = FontStyles.Italic;
page.Paragraphs.Add(text);
doc.Save(myDir + "footnote.pdf");
```

## Aspose.Pdf for .NET Resources

The following resources will help you work with Aspose.PDF for .NET:

*   [Home page for Aspose.PDF for .NET][9]
*   [Download Aspose.PDF for .NET][10]
*   [Forum][11]– Post your technical questions and queries, or any other problem you faced while running Aspose.PDF APIs.
*   [Online documentation][12]– help documentation.
*   [API reference][13] - API reference documents.
*   [Enable Blog Subscription][14]– Do not limit yourself, you can keep yourself updated with the latest news on Aspose.PDF, APIs, new features, fixes and other API related topics by subscribing to Aspose.PDF blog.
*   [Aspose.PDF for .NET Examples][15] – We have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: https://downloads.aspose.com/pdf/net/new-releases/aspose.pdf-for-.net-17.3.0/
[2]: https://docs.aspose.com/display/pdfnet/Add+and+Extract+a+Table#AddandExtractaTable-GetTableWidth
[3]: https://docs.aspose.com/display/pdfnet/Add%2C+Delete+and+Get+Annotation#Add,DeleteandGetAnnotation-AddingRichMediaAnnotation
[4]: https://docs.aspose.com/display/pdfnet/Aspose.Pdf+for+.NET+17.3.0+Release+Notes
[5]: https://docs.aspose.com/display/pdfnet/Aspose.Pdf+for+.NET+17.3.0+Release+Notes
[6]: https://docs.aspose.com/display/pdfnet/Release+Notes
[7]: https://docs.aspose.com/display/pdfnet/Add%2C+Delete+and+Get+Annotation#Add,DeleteandGetAnnotation-AddingRichMediaAnnotation
[8]: https://docs.aspose.com/display/pdfnet/Add%2C+Delete+and+Get+Annotation#Add,DeleteandGetAnnotation-AddingInkAnnotation
[9]: http://www.aspose.com/products/pdf/net
[10]: https://downloads.aspose.com/pdf/net
[11]: http://forum.aspose.com
[12]: http://docs.aspose.com/display/pdfnet/Home
[13]: http://www.aspose.com/api/net/pdf
[14]: https://blog.aspose.com/
[15]: https://github.com/aspose-pdf/Aspose.Pdf-for-.NET





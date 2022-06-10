---
title: 'Enhanced Watermark Annotation and Footnote in Aspose.Pdf for .NET 17.2.0'
date: Fri, 10 Feb 2017 14:24:19 +0000
draft: false
url: /2017/02/10/enhanced-watermark-annotation-footnote-aspose.pdf-.net-17.2.0/
author: Tilal Ahmad
summary: ''
tags: []
categories: ['Aspose.PDF Product Family']
---

[![][1]](https://blog.aspose.com/wp-content/uploads/sites/2/2017/02/aspose_pdf-for-net.jpg)This month release of [Aspose.Pdf for .NET 17.2.0][2] has been published. It includes some important enhancements along with number of bug fixes those were reported in previous months' releases and making this release more reliable and stable. The enhancements include opacity feature in Watermark Annotation and hyperlink feature in Footnote. In this release, we have fixed PDF to PDFA, PDF to HTML conversion feature issues along with some other issues. In order to get an idea about the new features/enhancements and fixes made in this release, please check the detailed [release notes of this version][3].

Furthermore, If you are planning to upgrade the API from any previous version, we strongly recommend you to check the Public API Changes section of other intermediate releases from [release notes folder][4], to know what has been changed since your current revision of the API.

The following sections describe some details regarding these newly added enhancements.

## Adding Transparent Watermark Annotation

Some of our customers requested to control transparency of [Watermark Annotation][5], so we have implemented opacity property in new release for this purpose. Please check following sample code to add transparent Watermark Annotation:

```
//Load a Document
Aspose.Pdf.Document doc = new Aspose.Pdf.Document("source.pdf");
//Load Page object to add Annotation
Page page = doc.Pages[1];
//Create Annotation
WatermarkAnnotation wa = new WatermarkAnnotation(page, new Aspose.Pdf.Rectangle(100, 500, 400, 600));
//Add annotaiton into Annotation collection of Page
page.Annotations.Add(wa);
//Create TextState for Font settings
Aspose.Pdf.Text.TextState ts = new Aspose.Pdf.Text.TextState();
ts.ForegroundColor = Aspose.Pdf.Color.Blue;
ts.Font = FontRepository.FindFont("Times New Roman");
ts.FontSize = 32;
//Set opacity level of Annotation Text
wa.Opacity = 0.5;
//Add Text in Annotation
wa.SetTextAndState(new string[] { "HELLO", "Line 1", "Line 2" }, ts);
//Save the Docuemnt
doc.Save("Output.pdf"); 
```

## Hyperlink support in Footnote text

We already support Footnote feature in Aspose.Pdf for .NET. However recently, one of the customer asked for hyperlink enhancement in Footnote feature. To fulfill this requirement, we have enhanced Footnote feature in this release. Now, by default Footnote functionality will add a reference of Footnote text to related superscript text. For example, Footnote superscript text "1" will be linked to Footnote text in output PDF document of following code:

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
text.FootNote.Text = "1";
page.Paragraphs.Add(text);
doc.Save(myDir + "footnote.pdf"); 
```

## Aspose.Pdf for .NET Resources

The following resources will help you work with Aspose.Pdf for .NET:

*   [Home page for Aspose.Pdf for .NET][6]
*   [Download Aspose.Pdf for .NET][7]
*   [Pdf product family forum][8]– Post your technical questions and queries, or any other problem you faced while running Aspose.Pdf APIs.
*   Pdf for .NET online documentation– help documentation.
*   [Pdf for .NET online API reference][9] - API reference documents.
*   [Enable Blog Subscription][10]– Do not limit yourself, you can keep yourself updated with the latest news on Aspose.Pdf, APIs, new features, fixes and other API related topics by subscribing to Aspose.Pdf blog.
*   [Aspose.Pdf for .NET Examples][11]– We have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: https://blog.aspose.com/wp-content/uploads/sites/2/2017/02/aspose_pdf-for-net.jpg
[2]: https://downloads.aspose.com/pdf/net/new-releases/aspose.pdf-for-.net-17.2.0/
[3]: https://docs.aspose.com/display/pdfnet/Aspose.Pdf+for+.NET+17.2.0+Release+Notes
[4]: https://docs.aspose.com/display/pdfnet/Release+Notes
[5]: https://docs.aspose.com/display/pdfnet/Add%2C+Delete+and+Get+Annotation#Add,DeleteandGetAnnotation-AddingWatermarkAnnotation
[6]: http://www.aspose.com/products/pdf/net
[7]: http://www.aspose.com/downloads/pdf/net
[8]: http://www.aspose.com/community/forums/aspose.pdf-product-family/20/showforum.aspx
[9]: http://www.aspose.com/api/net/pdf
[10]: https://blog.aspose.com/
[11]: https://github.com/aspose-pdf/Aspose.Pdf-for-.NET





---
title: 'Add Hyperlink to TextSegment in PDF using C# .NET'
date: Sun, 25 Oct 2015 22:48:49 +0000
draft: false
url: /2015/10/25/add-hyperlink-to-textsegment-in-pdf-using-csharp-.net-pdf-library/
author: Codewarior
summary: ''
tags: ['Nayyer Shahbaz']
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/aspose-Pdf-for-net_100.png" alt="Aspose.Pdf for .NET logo">}}


Another release of [Aspose.PDF for .NET 10.9.0][1] has hit the download section with new enhancements and fixes for issues reported against previous release versions. Every new release we have created, we have created it on a single belief. The API should be more than a collection of features. It should be simple, workable, reliable and understandable. That's how you make an API which is ridiculously amazing. Each release should be backward compatible, so that whenever there is a new release with shiny new features, you should be able make most of the new version, without any hassle and aggravation related to code compatibility. Its that kind of thinking that also enabled us to create one of the best PDF file creation and manipulation API with proven track record spanning more than a decade. Get the best of our API with even couple of code lines and create stunningly impressive applications without worrying about complex implementation behind all those routines. What that means is, you don’t actually have to know what that means. All you have to do is use publically exposed methods to make impressive and amazing applications with fewer lines of code.

The fact is that there are numerous capable, beautiful, inspiring methods in our API and each and everyone has been reviewed and approved by a team of creative humans. With great taste. And great suggestions. And great ideas. We enable developers to make super safe and top-notch PDF's while providing encryption for PDF security using rock-solid encryption algorithms, which we have build in our API, as we believe data security is serious. All this high-end security encryption is built on the same simple rule, **things should always be easy** for our customers to use. And since we’re all using this API more than ever, we should be able to do more remarkable things than ever. In short, this new release brings refinements at every level. Furthermore, if you ever have any questions, and because we all have questions sometimes, you know exactly who to come to. Us. Contact our team of experts through Live chat or dedicated [Aspose.PDF product family forum][2] to get an instant reply to your query.

## Add Hyperlink to TextSegment in PDF ins C#

A PDF page may comprise of one or more TextFragment objects, where each TextFragment object can have one or more TextSegment instance. In order to set hyperlink for TextSegment, Hyperlink property of TextSegment class can be used while providing the object of Aspose.Pdf.WebHyperlink instance. Please try using the following code snippet to accomplish this requirement. For further details, please visit [add hyperlink in PDF][3].

```
// create document instance
Document doc = new Document();
// add page to pages collection of PDF file
Page page1 = doc.Pages.Add();
// create TextFragment instance
TextFragment tf = new TextFragment("Sample Text Fragment");
// set horizontal alignment for TextFragment
tf.HorizontalAlignment = Aspose.Pdf.HorizontalAlignment.Right;
// create a textsegment with sample text
TextSegment segment = new TextSegment(" ... Text Segment 1...");
// add segment to segments collection of TextFragment
tf.Segments.Add(segment);
// create a new TextSegment 
segment = new TextSegment("Link to Google");
// add segment to segments collection of TextFragment
tf.Segments.Add(segment);
// set hyperlink for TextSegment
segment.Hyperlink = new Aspose.Pdf.WebHyperlink("www.google.com");
// set forground color for text segment
segment.TextState.ForegroundColor = Aspose.Pdf.Color.Blue;
// set text formatting as italic
segment.TextState.FontStyle = FontStyles.Italic;
// create another TextSegment object
segment = new TextSegment("TextSegment without hyperlink");
// add segment to segments collection of TextFragment
tf.Segments.Add(segment);
// add TextFragment to paragraphs collection of page object
page1.Paragraphs.Add(tf);
// save output file
doc.Save("c:/pdftest/TextSegment_Hyperlink.pdf");
```

## Update

If your license subscription is valid (_license expiry date is after the release of this version_), you are eligible to update to this new release and our update policy ensures that you won’t miss out on all the amazing features and security enhancements in new versions. This new release is full of enhancements you’ll appreciate every day. Your applications become more essential. Under-the-hood refinements bring you more responsive performance, for everything you do with it. This blog post just gives you a sneak peek of enhancements offered in a particular release, and you are always encouraged to get the latest release and try exploring it in your environment. You may participate in API improvement by sharing your valuable feedback and let us know what you think, and the features you would like to see as part of this API.

## Miscellaneous fixes

As well as the enhancements and features discussed above, there has been a specific improvement for PDF to HTML and HTML to PDF conversion features with better support for HTML5. Among these fixes, the PCL to PDF, SVG to PDF, PDF to Excel, PDF to DOC, PDF to TIFF and TIFF to PDF conversion, PDF to XPS, ePUB to PDF, XML to PDF, conversion of PDF to PDF/A compliant documents, text replacement, Filling of the signature field with an image, flattening of PDF, FloatingBox rendering, Footnote, EndNote and rendering of non-English (specifically Arabic) contents are also improved. Please download and try the latest release of Aspose.PDF for .NET 10.9.0.




[1]: https://downloads.aspose.com/pdf/net
[2]: http://www.aspose.com/community/forums/aspose.pdf-product-family/20/showforum.aspx
[3]: https://docs.aspose.com/display/pdfnet/Add+and+Get+Hyperlink#AddandGetHyperlink-AddHyperlinkinaPDFFile





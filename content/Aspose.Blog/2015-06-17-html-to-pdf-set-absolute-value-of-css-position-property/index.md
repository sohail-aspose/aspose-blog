---
title: 'HTML to PDF using C# - Set Absolute Value of CSS Position Property'
date: Wed, 17 Jun 2015 15:02:17 +0000
draft: false
url: /2015/06/17/html-to-pdf-set-absolute-value-of-css-position-property/
author: Codewarior
summary: ''
tags: ['Nayyer Shahbaz']
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/aspose-Pdf-for-net_100.png" alt="Aspose.Pdf for .NET logo">}}


The new release of [Aspose.Pdf for .NET 10.5.0][1] has been published which provides some great enhancements specific for HTML to PDF conversion feature. There are indeed improvements at the foundation of the API to enhance performance and its enriched with lots enhancements, which you will appreciate every day. Your applications based on our API will become more essential and productive. The more you do with Aspose.Pdf for .NET 10.5.0, the more you’ll wonder how you ever did without it. At Aspose, we always strive to introduce brand-new features, which specifically change your experience with our API's.

## Enhancements

HTML to PDF conversion is one of the most widely used and liked feature by our customers and with every new release, we are trying our best to make it more stable and captivating, so that it caters all most all of the scenarios in which our customers use our API. One of the customers recently requested a feature to provide the support for absolute value of CSS position property and in this new release, we are excited to announce that our API now fully supports absolute positioning for CSS objects.

With this new release, we get the power to set the font for complete document and all this can be achieved using a single property **DefaultTextState**.

```
// instantiate TextState instance
TextState textState = new TextState();
// specify the bold variant of Arial font from Font Repository
textState.Font = FontRepository.FindFont("Arial", FontStyles.Bold);
// create a new document instance
Document doc = new Document();
// set the default text state for whole document
doc.PageInfo.DefaultTextState = textState;
// add blank page to pages collection of PDF file
Page page = doc.Pages.Add();
// add a textfragment to paragraphs collection of PDF file
page.Paragraphs.Add(new TextFragment("Some bold arial text"));
// save the PDF file
doc.Save(outFile);
```

When adding RadioButtonField to PDF document, we need to specify the page number on which it will be rendered. However when creating a PDF file dynamically where we are not entirely certain about the number of pages a PDF document will be comprised of, we cannot specify the exact page number to render the control. So in order to cater such scenarios, we have introduced a new overload of **RadioButtonField** constructor which takes Document object as an argument.

## Miscellaneous fixes

As well as the enhancements and features discussed above, there has been specific improvement for PDF to HTML and HTML to PDF conversion features. Among these fixes, the PCL to PDF, SVG to PDF, PDF to Excel, PDF to DOC, PDF to TIFF and TIFF to PDF conversion, conversion of PDF to PDF/A compliant documents, text replacement, Filling of the signature field with an image, flattening of PDF and rendering of PDF to XPS format are also improved. Please download and try the latest release of [Aspose.Pdf for .NET 10.5.0][2].




[1]: https://products.aspose.com/pdf/net
[2]: https://downloads.aspose.com/pdf/net





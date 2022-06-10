---
title: 'PDF Contents Redaction, Create Local Hyperlinks and Suppress Unsupported HTML Tags Exception using Aspose.PDF for .NET 10.2.0'
date: Sun, 29 Mar 2015 20:11:54 +0000
draft: false
url: /2015/03/29/pdf-contents-redaction-create-local-hyperlinks-suppress-unsupported-html-tags-exception-relative-path-support-during-html-to-pdf-conversion-with-aspose.pdf-for-.net-10.2.0/
author: Codewarior
summary: ''
tags: ['Nayyer Shahbaz', 'Apply text redaction in PDF', 'Redact PDF documents using Csharp']
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/aspose-Pdf-for-net_100.png" alt="Aspose.Pdf for .NET logo">}}


The new release of [Aspose.PDF for .NET 10.2.0][1] has hit the shelves with some great and new exciting features. We always strive to offer something new which can enable our users to create great PDF documents and we provide the capabilities which make our API prominent and viable enough to beat the competitors. Since the very beginning, we have been focusing on creating an API which is robust and stable enough that our customers can use a single API to accomplish all their industry requirements. Since our API is developed on PDF specifications from Adobe (which are standard specifications), we always have been working hard on providing almost all the features which are offered by Adobe Acrobat. The features ranging from PDF creation to PDF manipulation and the transformation to various output formats. Whenever we plan to introduce new features, we first listen to the requirements and features being demanded by our privileged customers and then try implementing the features which are demanded by most of the users. However the priority of fixing bugs; always stands first, so that we present a bug free, better and stable API to our customers, which can be used to create great applications.

## PDF Contents Redaction

We all are very well versed that data is very important and critical for individual as well as for organizations, and we prevent our data form unauthorized access through encryption and data encapsulation. Aspose.PDF for .NET is great when it comes to applying security restrictions and specifying access privileges over PDF documents. Recently we came across a requirement to redact certain page region so that information cannot be viewed/access/copied by customers receiving the documents. So in order to accomplish this requirement, we have enhanced our Annotations feature. We know that Aspose.PDF for .NET provides the feature to add as well as manipulate Annotations in existing PDF file, so in order to further enhance the powers of Annotations, a new class named **RedactionAnnotation** is provided, which can be used to redact certain page region or it can be used to manipulate existing RedactionAnnotations and redact them (i.e. flatten annotation and remove text under it). For further details, please visit Redact certain page region with RedactionAnnotation.

{{< gist aspose-pdf 7e1330795d76012fcb04248bb81d45b3 "Examples-CSharp-AsposePDF-Annotations-RedactPage-RedactPage.cs" >}}

## Create Hyperlinks to Sections in Same PDF

Aspose.PDF for .NET provides great feature to PDF creation as well as its manipulation. It also offers the feature to add links to PDF pages and a link can either direct to pages in another PDF file, a web URL, link to launch an Application or even link to pages in same PDF file. In order to add local hyperlinks (links to pages in same PDF file), a class named LocalHyperlink is added to Aspose.Pdf namespace and this class has a property named TargetPageNumber, which is used to specify the target/destination page for hyperlink. For further information, please visit [Create hyperlink to pages in same PDF][2].

{{< gist aspose-pdf 7e1330795d76012fcb04248bb81d45b3 "Examples-CSharp-AsposePDF-Links-Actions-CreateLocalHyperlink-CreateLocalHyperlink.cs" >}}

## Suppress Unsupported HTML Tags Exception

Aspose.PDF for .NET provides the capabilities to transform HTML file to PDF format and vice versa, it offers the feature to render PDF pages to HTML format. We know that due to open standards of HTML, the format is quite complex and due to custom implementation of these standards, errors may occur during HTML to PDF conversion. With every new release, we are trying our level best to make the feature to HTML to PDF conversion as stable and viable as we can. Even in this release, the HTML to PDF conversion has been one of the key improvement areas. Please note we have modified our API to cater the requirement of suppressing unsupported tags exception (_which may occur_) when new/custom HTML tags are parsed through our API, so that no exception / error should be displayed and HTML to PDF transformation process is completed without any intervention. Therefore we recommend using new Document Object Model (DOM) approach for [HTML to PDF conversion][3] which automatically handles such scenarios and produces output with great fidelity.

## Relative Path in HTML to PDF Conversion

An HTML file may reference external resources such as Image or CSS and during HTML to PDF conversion, we need to provide the path towards these resources, so that they are properly rendered inside resultant PDF. While providing the path information, we may provide relative path starting with slash.

```
string basePath = Path.GetDirectoryName(@"F:/ExternalTestsData/");
string outFile = @"F:/ExternalTestsData/37779.pdf";

// Instantiate Document object
Document doc = new Document();
Aspose.Pdf.HeaderFooter header = new Aspose.Pdf.HeaderFooter();

// Add a page to pages collection of PDF file
Page page = doc.Pages.Add();

// Instantiate HtmlFragment with HTML contnets
HtmlFragment htmlTitle = new HtmlFragment("");
htmlTitle.HorizontalAlignment = Aspose.Pdf.HorizontalAlignment.Left;
htmlTitle.Margin.Left = 0;
htmlTitle.Margin.Bottom = 10;

htmlTitle.HtmlLoadOptionsOfInstance = new HtmlLoadOptions(basePath);
// Add HTML Fragment to paragraphs collection of page
page.Paragraphs.Add(htmlTitle);
doc.Save(outFile);
```

## Miscellaneous Fixes

As well as the enhancements and features discussed above, there have been specific improvement for PDF to HTML and HTML to PDF conversion features. Among these fixes, the PCL to PDF, SVG to PDF, PDF to Excel, PDF to DOC, PDF to TIFF and TIFF to PDF conversion, conversion of PDF to PDF/A compliant documents, text replacement, rendering PDF files to XPS format are also improved. Please download and try the latest release of [Aspose.PDF for .NET 10.2.0][4].




[1]: https://downloads.aspose.com/pdf/net
[2]: https://docs.aspose.com/display/pdfnet/Add+and+Get+Hyperlink#AddandGetHyperlink-CreatehyperlinktopagesinsamePDF
[3]: https://docs.aspose.com/display/pdfnet/Convert+HTML+to+PDF
[4]: https://downloads.aspose.com/pdf/net





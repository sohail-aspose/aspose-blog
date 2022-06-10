---
title: 'Convert PDF Documents to HTML using C#'
date: Sun, 06 Apr 2014 21:04:36 +0000
draft: false
url: /2014/04/06/convert-pdf-documents-to-html-using-csharp-.net-pdf-library/
author: Codewarior
summary: ''
tags: ['Nayyer Shahbaz', 'Convert PDF Documents to HTML using Csharp']
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/aspose-Pdf-for-net_100.png" alt="Aspose.Pdf for .NET logo">}}


For the last few releases, we have been specifically working on improving our PDF to HTML conversion feature and in this release, [Aspose.PDF for .NET 9.1.0][1], we have made few more great improvements to this feature. When converting large PDF files to HTML format, you sometimes want to determine the progress of the conversion. For example, it might be important to show the progress of conversion (number of pages converted). To accomplish this requirement, we have introduced a property CustomProgressHandler in HtmlSaveOptions. Please visit the following topic of detailed information on [determining PDF to HTML conversion progress.][2]

## PDF to HTML - Place Text Position Information as Inline Style

With this latest release, now the HTML-results contain inline-styles with attributes "position:absolute", similar to:

```
<div style="position:absolute; top:3.2953em; left:12em;">
<span class="pages\_12345\_06 pages\_12345\_07 pages\_12345\_08" style="word-spacing:-0.27em;">
```

## PDF to HTML - Avoid Saving Images in SVG Format

Recently we received a requirement to completely remove SVG images from the PDF to HTML conversion process. In order to accomplish this requirement, a new member of the enumeration HtmlSaveOptions.RasterImagesSavingModes has been introduced. The complete instructions can be found in the [PDF to HTML - Avoid Saving Images in SVG Format][3] article.

## Control Image Quality when Adding Stamp

In this new release, we have also introduced a feature for controlling image quality when adding a stamp. In order to accomplish this requirement, we've added the Quality property to the ImageStamp class. It indicates the quality of image in percents (valid values are 0..100). For further information, please read [Adding Image Stamp to PDF file][4].

## Insert Metadata with Prefix

When adding metadata to PDF files, you can create/register a new metadata namespace with a prefix.

```
Document pdfDocument = new Document("input.pdf");
pdfDocument.Metadata.RegisterNamespaceUri("xmp", "http://ns.adobe.com/xap/1.0/"); // xmlns prefix was removed
pdfDocument.Metadata\["xmp:ModifyDate"\] = DateTime.Now;
pdfDocument.Save("updated.pdf");
```

For further information, please take a look at [Set XMP Metadata in PDF File][5].

## Render Table on New Page

We used to have a feature for rendering a table on a new page when using the Aspose.Pdf.Generator namespace. Starting with this release, we also have introduced a new property named IsInNewPage in the BaseParagraph class to provide an option to render a table in new page. For more information, please visit [Render Table in New Page][6].

## Improved Signing Feature

We have introduced a new class named **DocMDPSignature** and the enumeration DocMDPAccessPermissions to provide the feature to digitally sign PDF files. Also please note that we have added the IsCertified property to the PdfFileSignature class. For more information about this topic, please take a look at [Digitally Sign PDF Files][7].

Along with the new features and enhancements listed above, we have made numerous improvements in PDF to HTML conversion, HTML to PDF conversion, image to PDF and PDF to image conversion, stamping PDF files, manipulating text inside PDF documents, PDF to XPS conversion, image and text extraction, and various other features.

Download and start exploring the exciting new features of [Aspose.PDF for .NET 9.1.0][8].




[1]: https://downloads.aspose.com/pdf/net
[2]: https://docs.aspose.com/display/pdfnet/PDF+to+HTML+-+Basics+of+Conversion
[3]: https://docs.aspose.com/display/pdfnet/PDF+to+HTML+-+Basics+of+Conversion#PDFtoHTML-BasicsofConversion-CompressingSVGImagesDuringConversion
[4]: https://docs.aspose.com/display/pdfnet/Adding+Stamp+in+a+PDF+file
[5]: https://docs.aspose.com/display/pdfnet/PDF+File+Metadata
[6]: https://docs.aspose.com/display/pdfnet/Add+and+Extract+a+Table#AddandExtractaTable-RenderTableonNewPage
[7]: https://docs.aspose.com/display/pdfnet/Digitally+sign+PDF+file
[8]: https://downloads.aspose.com/pdf/net





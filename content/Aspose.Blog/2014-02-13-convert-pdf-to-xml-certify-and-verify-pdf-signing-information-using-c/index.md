---
title: 'Convert PDF to XML, Certify and Verify PDF Signing Information using C#'
date: Thu, 13 Feb 2014 06:27:59 +0000
draft: false
url: /2014/02/13/convert-pdf-to-xml-certify-and-verify-pdf-signing-information-using-c/
author: Codewarior
summary: ''
tags: ['Nayyer Shahbaz']
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/aspose-Pdf-for-net_100.png" alt="Aspose.Pdf for .NET logo">}}


One of the features we implemented for Aspose.PDF for .NET early on was converting an XML file to PDF. The API also provides the facility to transform custom XML files to PDF with the help of XSLT. With the release of [Aspose.PDF for .NET 8.9.0][1], we have introduced a new feature which lets you convert PDF documents to XML (MobiXML). as usual, we try to keep things simple, so this feature can be accomplished with two simple lines of code.

```
// Load source PDF file document 
doc = new Document(@"d:\document.pdf"); 
// Save output to XML format 
doc.Save("d:\outFile.xml", SaveFormat.MobiXml); 
```

For further details regarding this feature, please visit Convert PDF to XML.

## Determine if Source PDF is Signed

Aspose.PDF for .NET also offers the feature to determine if source PDF file is signed. As shown below, you can verify if the source PDF file is signed without providing the signature name.

```
PdfFileSignature pdfSign = new PdfFileSignature();
pdfSign.BindPdf(@"c:\input.pdf");
pdfSign.IsContainSignature(); // Any signatures?
pdfSign.Close(); 
```

For further information, read Verify whether the PDF File is Signed Using a Signature (Facades).

## PDF to HTML Conversion

PDF to HTML conversion is one of our prominent features and with every new release we make it more powerful by adding new capabilities. In this release, we have added the following features.

*   PDF to HTML - set prefix for URLs of SVG files
*   PDF to HTML - specify prefix for images
*   PDF to HTML - set URL prefix for fonts in style.css

As well as new features, there are many enhancements and bug fixes related to PDF to DOC conversion, customization in saving and referencing images during PDF to HTML conversion, PDF to image conversion, PDF to PDF/A conversion, image to PDF conversion and much more.

Download and start exploring the features of [Aspose.PDF for .NET 8.9.0][2].




[1]: https://products.aspose.com/pdf/net
[2]: https://downloads.aspose.com/pdf/net





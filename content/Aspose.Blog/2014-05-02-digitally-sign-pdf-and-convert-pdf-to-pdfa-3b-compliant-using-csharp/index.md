---
title: 'Digitally Sign PDF and Create PDF/A-3B Compliant PDF in C#'
date: Fri, 02 May 2014 11:45:55 +0000
draft: false
url: /2014/05/02/digitally-sign-pdf-and-convert-pdf-to-pdfa-3b-compliant-using-csharp/
author: Codewarior
summary: ''
tags: ['Nayyer Shahbaz', 'Convert PDF to PDFA-3B Compliant Csharp', 'Digitally Sign PDF using CSharp']
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/aspose-Pdf-for-net_100.png" alt="Aspose.Pdf for .NET logo">}}


Like in the last few releases, the specific focus of Aspose.Pdf development has been towards the PDF to HTML conversion feature. In adding more value to this functionality we have added a new feature: creating subsequent files with body contents only when converting multi-page PDF to HTML format. In order to accomplish this requirement, a new property, HtmlSaveOptions.HtmlMarkupGenerationMode has been introduced. With the following simple code snippet, you can split an output HTML to pages and force the HTML objects on the output pages to go exactly where they are now (fonts processing and output, CSS creation and output, images creation and output), except that resultant HTML will contain contents currently placed inside tags (now "body" tags will be omitted). However when using this approach, linking to CSS will be the responsibility of your code, because things like '' will be stripped out. For this purpose, you may read the CSS via File.ReadAllText() and send it via AJAX to a web page where it will be applied by jQuery. Further details, can be found in the article on the [basics of PDF to HTML conversion.][1]

{{< gist aspose-pdf 7e1330795d76012fcb04248bb81d45b3 "Examples-CSharp-AsposePDF-DocumentConversion-PDFToHTML-CreateSubsequentFiles.cs" >}}

## Digitally Signing PDF with Timestamp Server

We have introduced a feature that lets you digitally sign PDF documents using time-stamp servers. A new class named TimestampSettings has been added. For further details, please visit the [Digitally Signing PDF with Timestamp Server][2] article.

## Convert PDF to PDF/A\_3b

Over the years, Aspose.Pdf for .NET has proved to be a great API for converting PDF files to PDF/A format. In this latest release, we have introduced the support for converting PDF files to PDF/A\_3b compliant format. In order to support this feature, the value PDF\_A\_3B has been added to the PdfFormat enumeration. Please take a look at the following code snippet for further details. [Convert PDF File to PDF-A][3].

{{< gist aspose-pdf 7e1330795d76012fcb04248bb81d45b3 "Examples-CSharp-AsposePDF-DocumentConversion-PDFToPDFA3b-PDFToPDFA3b.cs" >}}

## Printing PDFs with Windows Service

We received a request regarding the printing of PDFs via a Windows Service because of System.Drawing.Printing is not supported by Microsoft in a Service. In order to resolve this problem, you need to first convert the PDF file to XPS format using Aspose.Pdf for .NET while using the following code snippet.

```
// Load source PDF file
Aspose.Pdf.Document doc = new Aspose.Pdf.Document("1.pdf");
// Save output in XPS format
doc.Save("1.xps", new Aspose.Pdf.XpsSaveOptions());
```

Once the PDF file is converted to XPS format, you can use Aspose.Words for .NET to [print a document on a server via XPSPrint][4]. In this approach, the System.Drawing.Printing namespace is not used (XpsConverter uses the System.Drawing namespace as it's not as bad as using System.Drawing.Printing in web-services).

## HTML to PDF - Support Resource Loading Callback

HTML to PDF is an important Aspose.Pdf for .NET feature. In this release, we have introduced a new feature regarding resource loading callback when converting HTML files to PDF format. In order to accomplish this requirement, a new property - HtmlSaveOptions.CustomLoaderOfExternalResources - has been introduced. Please note that this feature works when options.UseNewConversionEngine has the value of true. This custom strategy replaces pictures that are referenced in HTML with one predefined picture Custom\_picture.PNG. Therefore in order to ensure this feature works :

1.  Please put all supplied files in the test folder, open HTML in the browser, and see the original page where DrWeb's logo referenced in HTML.
2.  Execute the code and take a look into the result. The DrWeb logo will be replaced with Custom\_picture.PNG because CustomLoaderOfExternalResources refers to custom code that substitutes pictures.

{{< gist aspose-pdf 7e1330795d76012fcb04248bb81d45b3 "Examples-CSharp-AsposePDF-DocumentConversion-HTMLToPDF-HTMLToPDF.cs" >}}

{{< gist aspose-pdf 7e1330795d76012fcb04248bb81d45b3 "Examples-CSharp-AsposePDF-DocumentConversion-HTMLToPDF-HTMLToPDFHelper.cs" >}}

For further details, please take a look at the article [HTML to PDF - Resource Loading Callback][5].

## XML to FDF conversion

FDF stands for Forms Data Format, and an FDF file contains form values in a key/value pair. We also know that an XML file contains the values as tags, where, mostly the key is represented as the tag name, and value is represented as the value within that tag. Now, Aspose.Pdf.Facades provides the flexibility to convert any FDF file into XML. So with this release, you get the option to either

*   [convert XML to FDF format][6], or
*   [convert FDF to XML format][7].

## XSL-FO to PDF with New DOM

Conversion of XSL-FO files to PDF format using legacy Aspose.Pdf for .NET (the current Aspose.Pdf.Generator namespace) is one of the salient features of our API and many customers are already using this feature. Now we have also introduced this feature to the Aspose.Pdf namespace and, as shown in the following code snippet, the XslFoLoadOptions class can be used to accomplish this feature.

```
string inFo = @"F:\ExternalTestsData\33897.fo";
string outPdf = @"F:\ExternalTestsData\33897.pdf";

XslFoLoadOptions options = new XslFoLoadOptions();
// Indicate to use the new conversion engine
options.UseOldXslFoEngine = false;

Document pdfDocument = new Document(inFo, options);
pdfDocument.Save(outPdf); 
```

Also please note that the current implementations of encryption/decryption and hashing functions are FIPS compliant. Along with the above-listed features, we have made numerous enhancements to PDF to TIFF conversion, working with annotations, bookmark manipulation, filling forms, PDF to HTML conversion, HTML to PDF conversion, PDF to Microsoft Excel worksheet conversion, adding an image to PDF file and much more.

Please download and start exploring the new features in [Aspose.Pdf for .NET 9.2.0][8].




[1]: https://docs.aspose.com/display/pdfnet/PDF+to+HTML+-+Basics+of+Conversion
[2]: https://docs.aspose.com/display/pdfnet/Digitally+sign+PDF+file#DigitallysignPDFfile-DigitallySigningPDFwithTimestampServer
[3]: https://docs.aspose.com/display/pdfnet/Convert+PDF+file+to+other+Formats
[4]: https://docs.aspose.com/display/wordsnet/Print+a+Document+Programmatically+or+Using+Dialogs
[5]: https://docs.aspose.com/display/pdfnet/Convert+HTML+to+PDF
[6]: https://docs.aspose.com/display/pdfnet/Converting+an+XML+to+FDF+format
[7]: https://docs.aspose.com/display/pdfnet/Converting+an+FDF+to+XML+format
[8]: https://downloads.aspose.com/pdf/net





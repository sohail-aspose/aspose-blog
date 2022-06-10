---
title: 'Optimize PDF Documents using C# or VB.NET'
date: Thu, 22 Dec 2016 06:38:36 +0000
draft: false
url: /2016/12/22/support-of-pdfa_2u-standard-and-improved-pdf-optimization-in-aspose.pdf-for-.net-16.12.0/
author: Tilal Ahmad
summary: ''
tags: []
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/aspose_pdf-for-net1.jpg" alt="">}}


We are pleased to announce the release of [Aspose.PDF for .NET 16.12.0][1]. A new feature, the support of PDF/A\_2U standard along with number of enhancements and improvements are included in this release. Some of the enhancements are improved PDF Optimization and support of XML stream conversion to PDF. It also contains number of fixes of bugs reported in previous versions by our valued customers, which makes it more stable release as compared to previous releases. Some of them are PDF to PPTX conversion issues, PDF to PDFA standard conversion issues along with many other bug fixes. Please check the detailed [release notes of Aspose.PDF for .NET 16.12.0][2], in order to get an idea about the new features/enhancements and fixed bugs in this release of Aspose.Pdf for .NET.

Furthermore, If you are planning to upgrade the API from any previous version, we strongly recommend you to check the [Public API Changes section of current release][3] and other intermediate releases from release notes pages, to know what has been changed since your current revision of the API.

The following sections describe some details regarding these newly added features/enhancements.

## PDF Optimization - Improved

In this release, we have improved the PDF optimization feature with the introduction of some new properties in OptimizationOption class. Mainly resizing of the embedded images reduces the PDF file size, ResizeImages and MaxResolution properties for the purpose along with RemovePrivateInfo:

```
 Aspose.Pdf.Document document = new Aspose.Pdf.Document(inFile);
document.OptimizeResources(new Aspose.Pdf.Document.OptimizationOptions()
{
LinkDuplcateStreams = true,
RemoveUnusedObjects = true,
RemoveUnusedStreams = true,
CompressImages = true,
ResizeImages = true,
RemovePrivateInfo = true,
ImageQuality = 50,
MaxResoultion = 75
});

.... 
```

## Support of PDF/A\_2U Standard

We have introduced new PDFA standard, PDF/A\_2U, in Aspose.Pdf for .NET 16.12.0. We have included a new value PDF\_A\_2U in PdfFormt enum. Please check following code snippet for new feature.

```
string inFile = "Input.pdf";
string outFile = "Output.pdf";
string outLog = "log.xml";
Aspose.Pdf.Document doc = new Aspose.Pdf.Document(inFile);
PdfFormatConversionOptions opts = new PdfFormatConversionOptions(outLog, PdfFormat.PDF_A_2U, ConvertErrorAction.Delete);
doc.Convert(opts);
doc.Save(outFile);
```

## Convert XML Stream using C#

Some of customers have requirements to render XML stream to PDF instead of file. So we have introduced a new constructor of BindXml() that support the Stream parameter.

```
string inXml = "sample.xml";
string inXslt = "sample.xslt";
string outFile = "output.pdf";
Aspose.Pdf.Document doc = new Aspose.Pdf.Document();
doc.BindXml(new FileStream(inXml, FileMode.OpenOrCreate), new FileStream(inXslt, FileMode.OpenOrCreate));
doc.Save(outFile);
```

## Support of HTML Text Conversion in XML to PDF

Recently, we have introduced a new XML schema of Aspose.Pdf(new generator). XSD includes in MSI installer. We have introduced HTML text support in new XML schema with this release. Here is sample XML and code for the conversion:

**Sample XML**

```
<?xml version='1.0' encoding='utf-8'?>
<Document xmlns="Aspose.Pdf">
<Page>
<HtmlFragment>some text<Hyperlink URL="www.google.com" /></HtmlFragment>
</Page>
</Document>
```

**Sample Code**

```
string inXml = "sample.xml";
string outFile = "output.pdf";
Aspose.Pdf.Document doc = new Aspose.Pdf.Document();
doc.BindXml(inXml);
doc.Save(outFile);
```

## Aspose.PDF for .NET Resources

The following resources will help you work with Aspose.Pdf for .NET:

*   [Home page for Aspose.PDF for .NET][4]
*   [Download Aspose.PDF for .NET][5]
*   [Aspose.PDF product family forum][6] – Post your technical questions and queries, or any other problem you faced while running Aspose.PDF APIs.
*   [Aspose.PDF for .NET online documentation][7] – help documentation.
*   [Aspose.PDF for .NET online API reference][8] - API reference documents.
*   [Enable Blog Subscription][9] – Do not limit yourself, you can keep yourself updated with the latest news on Aspose.PDF, APIs, new features, fixes and other API related topics by subscribing to Aspose.PDF blog.
*   [Aspose.PDF for .NET Examples][10] – We have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: http://downloads.aspose.com/pdf/net/new-releases/aspose.pdf-for-.net-16.12.0/
[2]: https://docs.aspose.com/pdf/net/aspose-pdf-for-net-16-12-0-release-notes/
[3]: https://docs.aspose.com/pdf/net/aspose-pdf-for-net-16-12-0-release-notes/
[4]: http://www.aspose.com/products/pdf/net
[5]: http://www.aspose.com/downloads/pdf/net
[6]: http://www.aspose.com/community/forums/aspose.pdf-product-family/20/showforum.aspx
[7]: https://docs.aspose.com/pdf/net/
[8]: http://www.aspose.com/api/net/pdf
[9]: https://blog.aspose.com/
[10]: https://github.com/aspose-pdf/Aspose.Pdf-for-.NET





---
title: 'Replace Fonts in PDF to PDFA Conversion in C# using Aspose.PDF for .NET'
date: Thu, 21 Jul 2016 03:16:10 +0000
draft: false
url: /2016/07/21/support-of-font-replacement-introduced-in-pdf-to-pdfa-conversion-in-aspose.pdf-for-.net-11.8.0/
author: Tilal Ahmad
summary: ''
tags: []
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/aspose_pdf-for-net.jpg" alt="">}}


We are pleased to announce a new version of Aspose.PDF for .NET, [Aspose.PDF for .NET 11.8.0][1] . This month's release is mainly a maintenance release with a couple of enhancements. It includes the replacement of fonts in PDF to PDFA conversion as the main enhancement. This release includes fixes of bugs reported by our valued customers in previous releases, that makes it more stable and better release as compared to previous versions. Some of these bug fixes related to PDF to PDFA, PDF to XPS, PDF to HTML, HTML to PDF, rendering XFA form to Static form, PDF to image. Please check [release notes of Aspose.PDF for .NET 11.8.0][2] for the complete list.

## Replacing Missing Fonts in PDF to PDFA Conversion

In PDF to PDFA conversion, sometimes fonts are neither embedded in the source PDF document and nor available on the machine, so it is required to replace missing fonts with some alternative fonts. We can substitute missing fonts as following.

```
Aspose.Pdf.Text.Font originalFont = null;
try
{
originalFont = FontRepository.FindFont("AgencyFB");
}
catch (Exception)
{
//Font is missing on destination machine
FontRepository.Substitutions.Add(new SimpleFontSubstitution("AgencyFB", "Arial"));
}
var fiNew = new FileInfo("newfile.pdf");
var pdf = new Document("myfile.pdf");
pdf.Convert("convertlog.xml", PdfFormat.PDF_A_1B, ConvertErrorAction.Delete);
pdf.Save(fiNew.FullName);
```

## Aspose.PDF for .NET Resources

The following resources will help you work with Aspose.PDF for .NET:

*   [Home page for Aspose.PDF for .NET][3]
*   [Download Aspose.PDF for .NET][4]
*   [Aspose.PDF product family forum][5] – Post your technical questions and queries, or any other problem you faced while running Aspose.PDF APIs.
*   [Aspose.PDF for .NET online documentation][6] – help documentation.
*   [Aspose.PDF for .NET online API reference][7] - API reference documents.
*   [Enable Blog Subscription][8] – Do not limit yourself, you can keep yourself updated with the latest news on Aspose.PDF APIs, new features, fixes and other API related topics by subscribing to Aspose.PDF blog.
*   [Aspose.PDF for .NET Examples][9] – We have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: https://downloads.aspose.com/pdf/net
[2]: http://docs.aspose.com/display/pdfnet/Aspose.Pdf+for+.NET+11.8.0+Release+Notes
[3]: https://products.aspose.com/pdf/net
[4]: https://downloads.aspose.com/pdf/net
[5]: http://forum.aspose.com
[6]: http://docs.aspose.com/display/pdfnet/Home
[7]: https://apireference.aspose.com/net/pdf
[8]: https://blog.aspose.com/
[9]: https://github.com/aspose-pdf/Aspose.Pdf-for-.NET





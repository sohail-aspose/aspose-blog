---
title: 'Save Webpage as PDF in C#'
seoTitle: "Print or Save Webpage as PDF Programmatically in C#"
description: "Print or save webpage as PDF programmatically in C#. Save web page from URL to PDF file in .NET or .NET Core framework applications."
date: Thu, 09 Jun 2022 23:31:00 +0000
draft: false
url: /2022/06/09/print-save-webpage-pdf-csharp/
author: Farhan Raza
summary: 'Webpages can contain text, images, drawings, animations, etc. Sometimes you might need to convert a webpage to PDF for archival or several other purposes. Accordingly, this article covers **how to save or print a webpage to PDF format in C#** by specifying the URL of the webpage. It discusses the simple and basic conversion as well as the advanced conversion where you can encrypt the output file.'
tags: ['Print web page to PDF', 'Print web page to PDF in csharp', 'Save web page as PDF in csharp', 'Save webpage as PDF']
categories: ['Aspose.HTML Product Family']
---



{{< figure align=center src="images/Save-Webpage-PDF-1024x334.jpg" alt="Save webpage as PDF C#">}}


Webpages can contain text, images, drawings, animations, etc. Sometimes you might need to convert a webpage to PDF for archival or several other purposes. Accordingly, this article covers how to save or print a webpage to [PDF][1] format in C# by specifying the URL of the webpage. It discusses the simple and basic conversion as well as the advanced conversion where you can encrypt the output file.

*   [Save Webpage as PDF File – C# API Installation][2]
*   [Save Webpage as PDF in C#][3]
*   [Print Web Page to PDF with Encryption in C#][4]

## Save Webpage as PDF File – C# API Installation {#section1}

[Aspose.HTML for .NET][5] API can be used to process different web-related [file formats][6] like HTML, SVG,  EPUB, etc. You can easily configure the API by downloading its DLL files from the [Downloads][7] section or using the following [NuGet][8] installation command:

```
PM> Install-Package Aspose.Html
```

## Save Webpage as PDF File in C# {#section2}

You can quickly save a webpage to PDF format with the following steps:

1.  Load the input webpage by specifying its URL.
2.  Create an object of the [PdfSaveOptions][9] class.
3.  Save the webpage as a PDF file with [ConvertHTML][10] method.

The code snippet below elaborates how to save a webpage as PDF programmatically in C#:

\[gist id="7588fbdd00f173796beaeb57e69cbb58" file="Webpage to PDF.cs"\]

## Print Web Page to PDF with Encryption in C# {#section3}

You can print a web page to PDF while securing the PDF by following the steps below:

1.  Load the input web page by using its URL.
2.  Specify the document permissions using [PdfPermissions][11].
3.  Create [PdfSaveOptions][12] class object to encrypt the output PDF file.
4.  Write the output PDF document.

The following code sample demonstrates how to print a web page to PDF with encryption programmatically in C#:

\[gist id="7588fbdd00f173796beaeb57e69cbb58" file="Web page to PDF Encryption.cs"\]

## Explore Aspose.HTML for .NET API

You can learn many other features offered by the API by visiting the [documentation][13] section.

## Get Free License

You can evaluate the API in its full capacity by requesting a [free temporary license][14].

## Conclusion

In this article, you have learned how to save a webpage to PDF format by specifying its URL programmatically in C#. It explains a basic conversion use case in addition to the advanced conversion scenario. Moreover, please feel free to contact us at the [forum][15] if you need to discuss your concerns or requirements with us.

## See Also

[Download Image from URL in C#][16]


[1]: https://docs.fileformat.com/pdf/
[2]: #section1
[3]: #section2
[4]: #section3
[5]: https://products.aspose.com/html/net/
[6]: https://docs.aspose.com/html/net/getting-started/supported-file-formats/
[7]: https://downloads.aspose.com/html/net
[8]: https://www.nuget.org/packages/Aspose.Html/
[9]: https://apireference.aspose.com/html/net/aspose.html.saving/pdfsaveoptions
[10]: https://apireference.aspose.com/html/net/aspose.html.converters/converter/methods/converthtml/index
[11]: https://reference.aspose.com/html/net/aspose.html.rendering.pdf.encryption/pdfpermissions/
[12]: https://apireference.aspose.com/html/net/aspose.html.saving/pdfsaveoptions
[13]: https://docs.aspose.com/html/net/
[14]: https://purchase.aspose.com/temporary-license
[15]: https://forum.aspose.com/c/html
[16]: https://blog.aspose.com/2022/06/04/download-image-from-url-csharp/






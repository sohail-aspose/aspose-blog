---
title: 'Convert PUB to HTML webpage Programmatically using C#'
seoTitle: "Convert PUB to HTML webpage in C# | Publisher to HTML5 XHTML"
description: "Convert Microsoft Publisher (PUB) files to HTML webpage as HTML5 or XHTML file programmatically using C#. Change or Export Publisher files."
date: Fri, 25 Jun 2021 22:10:00 +0000
draft: false
url: /2021/06/25/pub-to-html-xhtml/
author: Farhan Raza
summary: 'In different scenarios, you can need to convert Microsoft Publisher (PUB) files to an HTML webpage. You may customize the output HTML file with different properties as per your requirements. In this article, you will learn how to **convert a PUB file to an HTML webpage in HTML5 or XHTML format programmatically using C#**.'
tags: ['Convert PUB to HTML5', 'PUB to HTML', 'PUB to HTML in csharp', 'PUB to Webpage', 'Publisher to HTML']
categories: ['Aspose.PUB Product Family']
---



{{< figure align=center src="images/PUB-to-HTML.png" alt="Convert PUB to HTML">}}


In different scenarios, you can need to convert Microsoft Publisher (PUB) files to an [HTML][1] webpage. You may customize the output HTML file with different properties as per your requirements. In this article, you will learn how to convert a PUB file to an HTML webpage in HTML5 or XHTML format programmatically using C#:

*   [PUB to HTML Webpage Converter – C# APIs Installation][2]
*   [Convert PUB to HTML file Programmatically using C#][3]
*   [Convert PUB to HTML in Xhtml Format Programmatically using C#][4]

## PUB to HTML Webpage Converter – C# APIs Installation {#section1}

[Aspose.PUB for .NET][5] API can convert a Microsoft Publisher file to PDF and that PDF file can be exported as an HTML webpage. It is helpful when you manage Microsoft Publisher files in a web application because these files are usually not supported in internet browsers. You can configure the APIs by downloading the DLL files from the [Downloads][6] section, or with the following NuGet installation commands:

```
PM> Install-Package Aspose.PUB
PM> Install-Package Aspose.PDF
```

## Convert PUB to HTML file Programmatically using C# {#section2}

You can convert a PUB file to an HTML file with the following steps:

1.  Load and parse the input PUB file with the [CreateParser][7] method.
2.  Convert the PUB file to PDF and save the result in a [MemoryStream][8].
3.  Load data from MemoryStream and initialize the [HtmlSaveOptions][9] class object.
4.  Save output HTML webpage.

The following code shows how to convert a PUB file to an HTML webpage with C#:

{{< gist aspose-com-gists ee7d21b2b6c232a60bb673d9aca3bdac "PUB-to-HTML.cs" >}}

## Convert PUB to HTML in XHTML Format Programmatically using C# {#section3}

You can convert a Publisher document to an HTML file in Xhtml format programmatically using C#. [HtmlSaveOptions][10] class exposes different properties which can be set to create different types of HTML files. The following steps explain PUB to HTML conversion in Xhtml format:

1.  Load input PUB file and parse it with the [Parse][11] method.
2.  Convert PUB to PDF document and store result in a MemoryStream instance.
3.  Initialize [HtmlSaveOptions][12] class object and set the [DocumenType][13] property.
4.  Save output HTML webpage in XHTML format.

The code below explains how to convert a PUB file to HTML webpage in XHTML format programmatically with C#:

{{< gist aspose-com-gists ee7d21b2b6c232a60bb673d9aca3bdac "PUB-to-HTML5-Xhtml.cs" >}}

## Get Free Temporary License

You can evaluate Aspose APIs in full capacity by requesting a [Free Temporary License][14].

## Conclusion

In this article, you have learned how to convert a Microsoft Publisher file to an HTML webpage in HTML5 or XHTML format programmatically using C#. You can render the PUB files while setting different other options as per your requirements. Moreover, you can refer to the [Documentation][15] of Aspose.PUB for .NET API or contact us at the [Free Support Forum][16] for any queries.

## See Also

[Convert PUB to Word Document (DOC/DOCX) in C#][17]




[1]: https://docs.fileformat.com/web/html/
[2]: #section1
[3]: #section2
[4]: #section3
[5]: https://products.aspose.com/pub/net
[6]: https://downloads.aspose.com/
[7]: https://apireference.aspose.com/pub/net/aspose.pub/pubfactory/methods/createparser/index
[8]: https://docs.microsoft.com/en-us/dotnet/api/system.io.memorystream?view=net-5.0
[9]: https://apireference.aspose.com/pdf/net/aspose.pdf/htmlsaveoptions
[10]: https://apireference.aspose.com/pdf/net/aspose.pdf/htmlsaveoptions
[11]: https://apireference.aspose.com/pub/net/aspose.pub/ipubparser/methods/parse
[12]: https://apireference.aspose.com/pdf/net/aspose.pdf/htmlsaveoptions
[13]: https://apireference.aspose.com/pdf/net/aspose.pdf/htmlsaveoptions/properties/documenttype
[14]: https://purchase.aspose.com/temporary-license
[15]: https://docs.aspose.com/pub/net/
[16]: https://forum.aspose.com/c/pub
[17]: https://blog.aspose.com/2021/06/16/convert-pub-to-word-doc-docx-csharp/






---
title: 'HTML to PDF C# Conversion using .NET API'
seoTitle: ""
description: ""
date: Fri, 28 Feb 2020 02:36:00 +0000
draft: false
url: /2020/02/28/convert-html-to-pdf-programmatically-in-csharp-net/
author: Usman Aziz
summary: 'There are various scenarios when you need to perform HTML to PDF conversion. For example, you may want to convert a web page to PDF from within your application or you may need to generate PDF from the content of a WYSIWYG HTML editor. Another scenario could be converting the HTML page from a specific URL to PDF. In order to deal with such cases, you will learn how to convert HTML to PDF in C#. The HTML content could be a .html file or a web page from a URL.'
tags: ['Convert HTML to PDF in Csharp', 'Convert web page to PDF', 'HTML to PDF', 'HTML to encrypted PDF']
categories: ['Aspose.PDF Product Family']
---

This article demonstrates some simple ways of **HTML to PDF** conversion using **C#**.



{{< figure align=center src="images/HTML-to-PDF-C.png" alt="HTML to PDF in C#">}}


There are various scenarios when you need to perform **HTML to PDF** conversion. For example, you may want to convert a web page to PDF from within your application or you may need to generate PDF from the content of a WYSIWYG HTML editor. Another scenario could be converting the HTML page from a specific URL to PDF. In order to deal with such cases, you will learn how to perform HTML to PDF conversion. The HTML content could be a _.html_ file or a web page from a URL.

*   [HTML to PDF Converter API][1]
*   [HTML to PDF C# Conversion][2]
*   [Convert HTML to password-protected PDF using C#][3]
*   [Generate PDF from a Web Page in C#][4]
*   [Get a Free API License][5]

**Info**: Aspose provides a free online web app that allows you to [view PDFs online][6], another one that allows you to [edit PDFs online][7], and one that demonstrates the [PDF to video conversion][8] process.

## HTML to PDF C# Converter API - Free Download {#CSharp-HTML-to-PDF-Converter-API}

[Aspose.PDF for .NET][9] is a PDF manipulation API that lets you convert HTML documents to PDF seamlessly. You can either [download][10] API's DLL or install its package from NuGet.

### NuGet Package Manager



{{< figure align=center src="images/Aspose.PDF-NPM.png" alt="HTML to PDF Converter Library">}}


### Package Manager Console```
PM> Install-Package Aspose.PDF
```

## Steps to Convert HTML to PDF

The following are the steps to generate PDF from HTML using Aspose.PDF for .NET.

*   Download and install the Aspose.PDF for .NET
*   Add required namespaces of the API
*   Load the HTML content from file or URL
*   Generate PDF from provided HTML content

## HTML to PDF C# Conversion {#Convert-HTML-to-PDF-in-CSharp}

The following are the simple steps to generate PDF from HTML using _Aspose.PDF for .NET_.

*   Create an instance of the [HtmlLoadOptions][11] class.
*   Create an instance of [Document][12] class and initialize it with the HTML file's path and _HtmlLoadOptions_ object.
*   Call [Document.Save(String)][13] method with the output PDF file's name.

The following code sample shows how to convert HTML to PDF using C#.

{{< gist aspose-com-gists ad68c928411bded41103ded76e6554c6 "convert-html-to-pdf.cs" >}}

### Input HTML File



{{< figure align=center src="images/HTML-Document.png" alt="C# HTML to PDF">}}


### Converted PDF Document



{{< figure align=center src="images/HTML-to-PDF.png" alt="Convert URL to PDF">}}


## C# HTML to PDF with Password-Protection {#HTML-to-password-protected-PDF-using-CSharp}

You can also convert HTML files to encrypted PDF documents using _Aspose.PDF for .NET_. The resultant PDF document can be protected with the user’s password, the owner’s password, access permissions, and cryptographic algorithm. You can encrypt the converted PDF using the Document.Encrypt() method. The following code sample shows how to convert an HTML file to an encrypted PDF.

{{< gist aspose-com-gists ad68c928411bded41103ded76e6554c6 "convert-html-to-pdf-with-encryption.cs" >}}

### Output



{{< figure align=center src="images/HTML-to-Password-Protected-PDF.png" alt="HTML to encrypted PDF">}}


## C# Generate PDF from HTML using URL {#Convert-HTML-page-from-a-particular-URL-to-PDF-CSharp}

_Aspose.PDF for .NET_ also supports conversion from the live URLs. The following are the steps to generate PDF from a webpage using C#.

*   Make a web request to the URL using [WebRequest][14].
*   Get the response of the web request into the _Stream_ object.
*   Create the _Document _object and initialize it with _InputStream _and _HtmlLoadOptions _objects.
*   Save HTML stream as PDF using _Document.Save()_ method.

The following code sample shows how to convert the web page to PDF in C#.

{{< gist aspose-com-gists ad68c928411bded41103ded76e6554c6 "convert-html-to-pdf-from-url.cs" >}}

## Get a Free API License {#Get-a-Free-API-License}

You can try the API without evaluation limitations by requesting a [temporary license][15].

## Conclusion

In this article, you have learned how to convert HTML content to PDF using programmatically using the .NET API. In addition to the simple conversion, this article also covered how to generate a password-protected PDF from HTML. You can easily port the provided code snippets to perform this conversion in VB.NET.

You may learn more about Aspose.PDF for .NET using the [documentation][16].

## Related Article

*   [Convert HTML to PDF in Java][17]




[1]: #CSharp-HTML-to-PDF-Converter-API
[2]: #Convert-HTML-to-PDF-in-CSharp
[3]: #HTML-to-password-protected-PDF-using-CSharp
[4]: #Convert-HTML-page-from-a-particular-URL-to-PDF-CSharp
[5]: #Get-a-Free-API-License
[6]: https://products.aspose.app/slides/viewer/pdf
[7]: https://products.aspose.app/slides/editor/pdf
[8]: https://products.aspose.app/slides/video/pdf
[9]: https://products.aspose.com/pdf/net
[10]: https://downloads.aspose.com/pdf/net
[11]: https://apireference.aspose.com/net/pdf/aspose.pdf/htmlloadoptions
[12]: https://apireference.aspose.com/net/pdf/aspose.pdf/document
[13]: https://apireference.aspose.com/net/pdf/aspose.pdf.document/save/methods/4
[14]: https://docs.microsoft.com/en-us/dotnet/api/system.net.webrequest?view=netframework-4.8
[15]: https://purchase.aspose.com/temporary-license
[16]: https://docs.aspose.com/display/pdfnet
[17]: https://blog.aspose.com/2020/01/30/convert-html-to-pdf-in-java/






---
title: 'Convert Markdown (MD) to PDF or PNG, JPG Image using C#'
seoTitle: "Convert Markdown (MD) to PDF, PNG, JPG Image Programmatically C#"
description: "You can convert the Markdown (MD) files to PDF, PNG, JPG image programmatically using C# in .NET. Import or Export Markdown files in .NET."
date: Sat, 12 Dec 2020 22:19:00 +0000
draft: false
url: /2020/12/12/convert-md-pdf-png-jpg-image-csharp/
author: Farhan Raza
summary: 'In this article, we will be learning Markdown file to PDF, PNG, JPG and other image formats conversion programmatically using C# language. MD files are quite common over the web and you might have noticed that readme files of different software as well as the documentations are often created in Markdown format.'
tags: ['Convert Markdown to Image', 'Convert Markdown to PDF', 'MD to Image', 'MD to JPG', 'MD to PDF', 'MD to PNG']
categories: ['Aspose.HTML Product Family']
---



{{< figure align=center src="images/Convert-Markdown-MD-PDF-Image-150x150.png" alt="Convert MD Markfown PDF Image">}}


In this article, we will be learning **[Markdown file][1] to [PDF][2], [PNG][3], [JPG][4], and other image formats conversion programmatically using C# language**. MD files are quite common over the web and you might have noticed that readme files of different software, as well as the documentation, are often created in Markdown format. Let us take a look over the following headings:

*   [Markdown (.md) to PDF and Images Converter – API Installation][5]
*   [Convert Markdown (MD) to PDF in C#][6]
*   [Convert Markdown (MD) to PNG or JPG Image in C#][7]

## Markdown (.md) to PDF and Images Converter – API Installation {#section1}

You need to install [Aspose.HTML for .NET][8] API for converting Markdown format files to PDF or image formats. You can configure the API by downloading it from the official [Downloads section][9] or via the [NuGet][10] gallery installation command, as under:

```
PM> Install-Package Aspose.Html
```

## Convert Markdown (MD) to PDF in C# {#section2}

You can easily convert Markdown Files (MD) to PDF using C# in your .NET applications. You need to follow the steps below for converting MD to PDF file:

1.  Prepare a simple Markdown example or load input MD file
2.  Call the [ConvertMarkdown][11] method
3.  Convert the input file to [HTMLDocument][12] instance
4.  Save the output PDF file using the [ConvertHTML][13] method

The following code shows how to convert markdown (MD) file to PDF using C#:

{{< gist aspose-com-gists 5a5b5924357fd23d465d48f34d6268b0 "MDtoPDF.cs" >}}

## Convert Markdown (MD) to PNG or JPG Image in C# {#section3}

Sometimes you might need to preview an MD file so rendering it to an image can be helpful. You can convert MD file to PNG or JPG image as per your requirements. This conversion is basically a two-step approach where, first of all, you will render it to HTML format and then to an image:

1.  Create or Load the input Markdown (MD) file
2.  Convert the Markdown to intermediary HTML format
3.  Render the results to PNG or JPG output Image

These simple steps help you create an image of the MD file as a preview. You may utilize the output image further as per your use case. Moreover, the code below shows how to convert Markdown (MD) file to PNG or JPG Image in C#:

{{< gist aspose-com-gists 5a5b5924357fd23d465d48f34d6268b0 "MDtoImage.cs" >}}

## Conclusion

To put it in a nutshell, we have considered the conversion of Markdown (MD) files to PNG, JPG, and PDF using C# in .NET applications. These features can make your applications second to none. Furthermore, there are many other features offered by the API which you can explore by taking a look at [Product Documentation][14]. In case of any ambiguities or concerns, please feel free to write to us at [Free Support Forum][15]. We would love to have your feedback!

## See Also

[Convert HTML to Markdown or Markdown to HTML in C#][16]




[1]: https://docs.fileformat.com/word-processing/md/
[2]: https://docs.fileformat.com/pdf/
[3]: https://docs.fileformat.com/image/png/
[4]: https://docs.fileformat.com/image/jpeg/
[5]: #section1
[6]: #section2
[7]: #section3
[8]: https://products.aspose.com/html/net
[9]: https://releases.aspose.com/
[10]: https://www.nuget.org/packages/Aspose.Html
[11]: https://apireference.aspose.com/html/net/aspose.html.converters/converter/methods/convertmarkdown/index
[12]: https://apireference.aspose.com/html/net/aspose.html/htmldocument/constructors/main
[13]: https://apireference.aspose.com/html/net/aspose.html.converters/converter/methods/converthtml/index
[14]: https://docs.aspose.com/html/net/
[15]: https://forum.aspose.com/c/html
[16]: https://blog.aspose.com/2020/12/08/convert-html-markdown-csharp/






---
title: 'Convert PUB to Word Document (DOC/DOCX) in C#'
seoTitle: "Convert Publisher (PUB) file to Word Document (DOC/DOCX) in C#"
description: "Convert Publisher File (PUB) to Microsoft Word file as DOC or DOCX format programmatically using C#. Export or change PUB files in .NET languages."
date: Wed, 16 Jun 2021 18:31:00 +0000
draft: false
url: /2021/06/16/convert-pub-to-word-doc-docx-csharp/
author: Farhan Raza
summary: 'Microsoft Publisher files are popularly used for professional designing and editing tasks. You can **convert a PUB file to a Word document in DOC and DOCX format**. This article covers how to convert the publisher files programmatically using C#.'
tags: ['Convert publisher to Word csharp', 'PUB to DOC', 'PUB to DOCX', 'PUB to Word', 'Publisher to DOC DOCX']
categories: ['Aspose.PUB Product Family']
---



{{< figure align=center src="images/PUB-to-Word.png" alt="PUB to Word DOCX DOC">}}


Microsoft Publisher files are popularly used for professional designing and editing tasks. You can convert a [PUB][1] file to a Word document in [DOC][2] and [DOCX][3] format. This article covers how to convert the publisher files programmatically using C#:

*   [PUB to Word DOC/DOCX Converter – C# APIs Installation][4]
*   [Convert PUB to Word DOC/DOCX Programmatically using C#][5]

## PUB to Word DOC/DOCX Converter – C# APIs Installation {#section1}

Aspose.PUB for .NET API supports PUB to PDF file conversion where you can further convert the output PDF file to a Word Document in DOC or DOCX format as per your requirements. Therefore, you need to download the DLL files of [Aspose.PUB for .NET][6] and [Aspose.PDF for .NET][7] API. You can also install these APIs with the following NuGet installation commands:

```
PM> Install-Package Aspose.PDF  
PM> Install-Package Aspose.PUB
```

## Convert PUB to Word DOC/DOCX Programmatically using C# {#section2}

You can convert Microsoft Publisher (.PUB) file to a Word document in DOC or DOCX format with the following steps:

1.  Initialize a [MemoryStream][8] to hold output document.
2.  Load and parse the input PUB file with [IPubParser.Parse()][9] method.
3.  Convert the PUB file to PDF and save the result in a MemoryStream.
4.  Load the PDF file and initialize the [DocSaveOptions][10] class object.
5.  Finally, specify the output format (DOC/DOCX) and save the Word file.

The below code shows how to convert a PUB file to a Word document in DOC or DOCX format programmatically using C#:

{{< gist aspose-com-gists 339959afdfacc1ab25a803fb66b8868f "PUB-to-Word-DOC-DOCX.cs" >}}

## Get Free API License

You can test the PUB to Word file conversion without any limitations by requesting a [Free Temporary License][11].

## Conclusion

In this article, you have learned how to convert Microsoft Publisher (PUB) files to Microsoft Word files in DOC or DOCX format programmatically using C#. You can check the high fidelity conversion by following the simple steps listed above. Moreover, you can further explore the API by visiting the [Documentation][12], or please feel free to write to us at the [Free Support Forum][13] in case of any queries. We look forward to getting in touch with you!

## See Also

[Convert PUB to PNG, JPEG, or TIF Image using C#][14]




[1]: https://en.wikipedia.org/wiki/PUB_(file_type)
[2]: https://docs.fileformat.com/word-processing/doc/
[3]: https://docs.fileformat.com/word-processing/docx/
[4]: #section1
[5]: #section2
[6]: https://products.aspose.com/pub/net
[7]: https://products.aspose.com/pdf/net/
[8]: https://docs.microsoft.com/en-us/dotnet/api/system.io.memorystream
[9]: https://apireference.aspose.com/pub/net/aspose.pub/ipubparser/methods/parse
[10]: https://apireference.aspose.com/pdf/net/aspose.pdf/docsaveoptions
[11]: https://purchase.aspose.com/temporary-license
[12]: https://docs.aspose.com/pub/net/
[13]: https://forum.aspose.com/c/pub
[14]: https://blog.aspose.com/2021/03/23/convert-pub-to-png-jpeg-or-tif-image-csharp/






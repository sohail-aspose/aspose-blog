---
title: 'Convert PUB to PPT/PPTX Presentation in C#'
date: Tue, 11 Jan 2022 09:42:00 +0000
draft: false
url: /2022/01/11/convert-pub-to-pptx-csharp/
author: ''Farhan Raza''
summary: 'Microsoft Publisher, PUB, files are often used for large scale printing of documents like brochures, booklets, posters, etc. In certain situations, you may need to convert a PUB file to a Presentation file as a PPT or PPTX file. This article covers how to **convert the publisher files programmatically in C#**.'
tags: ['Convert PUB to PPTX in csharp', 'PUB to PPT', 'PUB to PPTX', 'PUB to Presentation']
categories: ['Aspose.PUB Product Family']
---



{{< figure align=center src="images/PUB-to-PPTX.png" alt="PUB to PPT PPTX csharp">}}


Microsoft Publisher, PUB, files are often used for large scale printing of documents like brochures, booklets, posters, etc. In certain situations, you may need to convert a [PUB][1] file to a Presentation file as a [PPT][2] or [PPTX][3] file. This article covers how to convert the publisher files programmatically in C#.

*   [PUB to PPT/PPTX PowerPoint Presentation Converter – C# API Installation][4]
*   [Convert PUB to PPT/PPTX Programmatically in C#][5]

## PUB to PPT/PPTX PowerPoint Presentation Converter – C# API Installation {#section1}

PUB to PPT or PPTX PowerPoint conversion is a two-step process. In the first step, you need to convert a PUB file to a PDF file and then convert the PDF to a PPT or PPTX file. So you need to download the DLL files for [Aspose.PUB for .NET][6] and [Aspose.PDF for .NET][7] API. Or you can configure these APIs with the NuGet commands below:

```
PM> Install-Package Aspose.PDF  
PM> Install-Package Aspose.PUB
```

## Convert PUB to PPT/PPTX Programmatically in C# {#section2}

You can convert Microsoft Publisher, PUB, file to PPT or PPTX format PowerPoint Presentation by following the steps below:

1.  Create a [MemoryStream][8] object to save intermediate PDF file.
2.  Parse the source PUB file using [IPubParser.Parse()][9] method.
3.  Convert the PUB file to PDF and save the output in the MemoryStream.
4.  Load the PDF file and initialize the [PptxSaveOptions][10] class instance.
5.  Save the output PPT or PPTX file.

The following code snippet shows how to convert a PUB file to a PPT or PPTX PowerPoint Presentation programmatically in C#:



## Try Online Demo

Please try the [PUB to PPTX][11] web app developed using this API.

## Get Free API License

You can evaluate the API without any limitations by requesting a [free temporary license][12].

## Conclusion

In this article, you have learned how to convert Microsoft Publisher, PUB, file to PowerPoint Presentation as a PPT or PPTX file programmatically in C#. Furthermore, you can check other features of the API by visiting the [documentation][13], or get in touch with us via [forum][14].

## See Also

[Convert PUB to PNG, JPEG, or TIF Image using C#][15]




[1]: https://docs.fileformat.com/publisher/pub/
[2]: https://docs.fileformat.com/presentation/ppt/
[3]: https://docs.fileformat.com/presentation/pptx/
[4]: #section1
[5]: #section2
[6]: https://products.aspose.com/pub/net
[7]: https://products.aspose.com/pdf/net/
[8]: https://docs.microsoft.com/en-us/dotnet/api/system.io.memorystream
[9]: https://apireference.aspose.com/pub/net/aspose.pub/ipubparser/methods/parse
[10]: https://apireference.aspose.com/pdf/net/aspose.pdf/pptxsaveoptions
[11]: https://products.aspose.app/pub/conversion/pub-to-pptx
[12]: https://purchase.aspose.com/temporary-license
[13]: https://docs.aspose.com/pub/net/
[14]: https://forum.aspose.com/c/pub
[15]: https://blog.aspose.com/2021/03/23/convert-pub-to-png-jpeg-or-tif-image-csharp/





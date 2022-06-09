---
title: 'Convert EPS or PS to SVG in C#'
seoTitle: "Convert EPS to SVG | PS PostScript to SVG Programmatically in C#"
description: "Convert EPS to SVG or PS PostScript file to SVG image programmatically in C#. Export EPS file in .NET or .NET Core Framework based applications."
date: Tue, 08 Mar 2022 08:25:00 +0000
draft: false
url: /2022/03/08/convert-eps-ps-to-svg-csharp/
author: Farhan Raza
summary: 'EPS or PS files contain vector graphics and are commonly used by designers. They can contain high-resolution images including shapes or text and are often used for billboard printing or building wraps. In some scenarios, you might need to convert an EPS or PS file to an SVG image. This article covers how to **convert EPS or PS PostScript files to SVG in C#.**'
tags: ['Convert EPS PS to SVG in csharp', 'EPS to SVG using csharp', 'PS to SVG using csharp', 'PostScript to SVG Conversion']
categories: ['Aspose.Page Product Family']
---



{{< figure align=center src="images/Convert-EPS-PS-to-SVG.png" alt="EPS PS to SVG csharp">}}


[EPS][1] or [PS][2] files contain vector graphics and are commonly used by designers. They can contain high-resolution images including shapes or text and are often used for billboard printing or building wraps. In some scenarios, you might need to convert an EPS or PS file to an [SVG][3] image. This article covers how to convert EPS or PS PostScript files to SVG in C#.

*   [EPS or PS to SVG Converter – C# APIs Installation][4]
*   [Convert EPS or PS to SVG Programmatically using C#][5]

## EPS or PS to SVG Converter – C# APIs Installation {#section1}

You can convert an EPS or PS file to SVG image format in two steps. Firstly, you need to convert EPS to PDF documents with Aspose.Page for .NET. Then PDF to SVG conversion is performed using Aspose.PDF for .NET API. Please download the DLL files for [Aspose.Page for .NET][6] and [Aspose.PDF for .NET][7] API or install these APIs with the following NuGet commands:

```
PM> Install-Package Aspose.Page  
PM> Install-Package Aspose.PDF
```

## Convert EPS or PS to SVG Programmatically using C# {#section2}

You can convert EPS or PS PostScript files to SVG format by following the steps below:

1.  Create an instance of the [MemoryStream][8] class.
2.  Load the input EPS file with [PsDocument][9] class.
3.  Convert the EPS file to PDF with [PdfSaveOptions][10] class.
4.  Load the intermediary PDF file and initialize the [SvgSaveOptions][11] class instance.
5.  Save the output SVG file.

The code snippet below demonstrates how to convert an EPS or PS file to SVG image programmatically using C#:



## Get Free API License

You can get a [temporary license][12] to test all the features of the API without any evaluation limitations.

## Online Demo

Please try the [EPS to SVG Converter][13] web app to check the file conversion capabilities.

## Conclusion

In this article, you have explored how to convert an EPS or PS PostScript file to SVG image format programmatically in C#. Furthermore, you can check other features of the API by going through the [documentation][14] section. Please feel free to contact us at the [forum][15] to discuss any of your concerns.

## See Also

[Convert XPS or OXPS to Word DOCX/DOC in C#][16]




[1]: https://docs.fileformat.com/page-description-language/eps/
[2]: https://docs.fileformat.com/page-description-language/ps/
[3]: https://docs.fileformat.com/page-description-language/svg/
[4]: #section1
[5]: #section2
[6]: https://products.aspose.com/page/net
[7]: https://products.aspose.com/pdf/net/
[8]: https://docs.microsoft.com/en-us/dotnet/api/system.io.memorystream
[9]: https://apireference.aspose.com/page/net/aspose.page.eps/psdocument
[10]: https://apireference.aspose.com/page/net/aspose.page.eps.device/pdfsaveoptions
[11]: https://apireference.aspose.com/pdf/net/aspose.pdf/svgsaveoptions
[12]: https://purchase.aspose.com/temporary-license
[13]: https://products.aspose.com/pdf/net/conversion/eps-to-svg/
[14]: https://docs.aspose.com/page/net/
[15]: https://forum.aspose.com/c/page/39
[16]: https://blog.aspose.com/2022/02/07/convert-xps-oxps-word-csharp/





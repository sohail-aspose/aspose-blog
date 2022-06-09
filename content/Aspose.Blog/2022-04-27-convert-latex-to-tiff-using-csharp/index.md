---
title: 'Convert LaTeX to TIFF using C#'
seoTitle: "Convert LaTeX to TIFF using C# | TeX to TIFF in C# | LTX to TIFF in C#"
description: "Programmatically convert LaTeX to TIFF using C# with Aspose.TeX for .NET API. Convert TeX to TIFF programmatically in C#. Convert LTX to TIFF using C#."
date: Wed, 27 Apr 2022 09:33:31 +0000
draft: false
url: /2022/04/27/convert-latex-to-tiff-using-csharp/
author: Muzammil Khan
summary: 'As a C# developer, we can easily convert LaTeX source files (TeX or LTX) to TIFF images programmatically. In this article, you will learn **how to convert LaTeX to TIFF using C#**.'
tags: ['Convert LTX to TIFF using C#', 'Convert TeX to TIFF using C#', 'LTX to TIFF C#', 'LaTeX to TIFF', 'LaTeX to TIFF C#', 'TeX to TIFF C#']
categories: ['Aspose.TeX Product Family']
---



{{< figure align=center src="images/convert-latex-to-tiff-using-csharp.jpg" alt="Convert LaTeX to TIFF using C#">}}


We create technical and scientific documentation using LaTeX in the [TEX ][1]or [LTX][2] formats. A LaTeX file contains various commands to specify the format of the document, including text, symbols, mathematical expressions, and graphics. In certain cases, we may need to render or convert TeX or LTX files into [TIFF][3] images programmatically. In this article, we will learn **how to convert LaTeX to TIFF using C#**.

The following topics shall be covered in this article:

*   [LaTeX to TIFF Converter – C# API][4]
*   [Convert LaTeX (TeX) to TIFF in C#][5]
*   [Convert LaTeX (LTX) to TIFF using C#][6]

## LaTeX to TIFF Converter – C# API {#LaTeX-to-TIFF-Converter-CSharp-API}

For converting LaTeX files into TIFF images, we will be using the [Aspose.TeX for .NET][7] API. It allows the typesetting of TeX files and presents TeX input in various graphic formats like [XPS][8], [PDF][9], [PNG][10], [JPEG][11], TIFF, and [BMP][12]. Please either [download][13] the DLL of the API or install it using [NuGet][14]. 

```
PM> Install-Package Aspose.TeX
```

## Convert LaTeX (TeX) to TIFF in C# {#Convert-LaTeX-TeX-to-TIFF-in-CSharp}

We can create a TIFF image from a LaTeX (TeX) source file by following the steps given below:

1.  Firstly, create an instance of the [_**TeXOptions**_][15] class using the **_[ConsoleAppOptions()][16]_** method.
2.  Next, set typesetting TeX configuration as **_[TeXConfig.ObjectLaTeX][17]_**.
3.  Then, set the file system working directory for the output.
4.  Optionally, specify console or memory stream as an output terminal.
5.  After that, Initialize **_[TiffSaveOptions][18]_** for saving in TIFF format.
6.  Finally, call the **_[Run()][19]_** method for the newly created **_[TexJob][20]_** class and save the output TIFF with the **_[ImageDevice][21]_** class object.

The following code example shows **how to convert a LaTeX source to a TIFF image output file using C#.**

{{< gist aspose-com-gists 3c0fb70ab3b184db010f0193b6e9756b "ConvertLaTeXtoTIFF_CSharp_TeXtoTIFF.cs" >}}



{{< figure align=center src="images/Convert-LaTeX-TeX-to-TIFF-in-CSharp-1024x596.jpg" alt="Convert LaTeX (TeX) to TIFF in C#" caption="Convert LaTeX (TeX) to TIFF in C#.">}}


## LaTeX (LTX) to TIFF using C# {#LaTeX-LTX-to-TIFF-using-CSharp}

LaTeX also uses an LTX file extension for typesetting markup tags and properties to define the document structure and content. We can convert LaTeX (LTX) file output to a TIFF image as well by following the steps mentioned earlier. However, we just need to input the source file with the .ltx extension in the last step.

The following code example shows ****how to convert an LTX source file to a TIFF image using C#****

{{< gist aspose-com-gists 3c0fb70ab3b184db010f0193b6e9756b "ConvertLaTeXtoTIFF_CSharp_LTXtoTIFF.cs" >}}

## Get a Free License {#Get-a-Free-API-License}

You can evaluate Aspose.TeX for .NET without any limitations by getting a [temporary license][22].

## Conclusion

In this article, we have learned how to generate a TIFF image from the LaTeX source files (TeX or LTX) in C#. Besides, you can learn more about Aspose.TeX for .NET API using the [documentation][23]. In case of any ambiguity, please feel free to contact us on the [forum][24].

## See Also

*   [Convert LaTeX TeX LTX to PNG JPG Image Programmatically in C#][25]
*   [Convert TeX (LaTeX) to PDF or XPS File Programmatically using C#][26]




[1]: https://docs.fileformat.com/page-description-language/tex/
[2]: https://docs.fileformat.com/word-processing/ltx/
[3]: https://docs.fileformat.com/image/tiff/
[4]: #LaTeX-to-TIFF-Converter-CSharp-API
[5]: #Convert-LaTeX-TeX-to-TIFF-in-CSharp
[6]: #LaTeX-LTX-to-TIFF-using-CSharp
[7]: https://products.aspose.com/tex/net
[8]: https://docs.fileformat.com/page-description-language/xps/
[9]: https://docs.fileformat.com/pdf/
[10]: https://docs.fileformat.com/image/png/
[11]: https://docs.fileformat.com/image/jpeg/
[12]: https://docs.fileformat.com/image/bmp/
[13]: https://downloads.aspose.com/tex/net
[14]: https://www.nuget.org/packages/aspose.tex
[15]: https://apireference.aspose.com/tex/net/aspose.tex/TeXOptions
[16]: https://apireference.aspose.com/tex/net/aspose.tex/texoptions/methods/consoleappoptions
[17]: https://apireference.aspose.com/tex/net/aspose.tex/texconfig/properties/objectlatex
[18]: https://apireference.aspose.com/tex/net/aspose.tex.presentation.image/tiffsaveoptions
[19]: https://apireference.aspose.com/tex/net/aspose.tex/texjob/methods/run
[20]: https://apireference.aspose.com/tex/net/aspose.tex/TeXJob
[21]: https://apireference.aspose.com/tex/net/aspose.tex.presentation.image/imagedevice
[22]: https://purchase.aspose.com/temporary-license
[23]: https://docs.aspose.com/tex/net/
[24]: https://forum.aspose.com/c/tex/47
[25]: https://blog.aspose.com/2021/12/28/convert-latex-to-png-jpg-csharp/
[26]: https://blog.aspose.com/2021/04/13/convert-tex-latex-to-pdf-xps-csharp/





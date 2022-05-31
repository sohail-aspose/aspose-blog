---
title: 'Convert WOFF to TTF using C#'
date: Fri, 08 Apr 2022 19:50:19 +0000
draft: false
url: /2022/04/08/convert-woff-to-ttf-using-csharp/
author: ''Muzammil Khan''
summary: 'As a C# developer, you can easily convert Web fonts (WOFF or WOFF2) to True Type Fonts (TTF) programmatically. In this article, you will learn **how to convert WOFF to TTF using C#.**'
tags: ['C# Font Converter', 'Convert WOFF to TTF', 'Convert WOFF2 to TTF in C#', 'Font Converter API', 'WOFF to TTF C#', 'WOFF to TTF Converter API', 'WOFF2 to TTF C#', 'WOFF2TTF']
categories: ['Aspose.Font Product Family']
---



{{< figure align=center src="images/convert-woff-to-ttf-using-csharp.jpg" alt="Convert WOFF to TTF using C#.">}}


The _True Type Font_ or [TTF][1] is used in operating systems for all digital platforms. In the [previous post][2], we have seen how to convert TTF to web fonts. The _Web Open Font Format_ or simply [WOFF][3] is a web font mostly used on web pages. In certain cases, we may also need to convert Web fonts to true-type fonts. In this article, we will learn **how to convert WOFF to TTF using C#**.

The following topics shall be covered in this article:

*   [WOFF to TTF Converter C# API][4]
*   [Convert WOFF to TTF using C#][5]
*   [Convert WOFF2 to TTF in C#][6]

## WOFF to TTF Converter C# API {#WOFF-to-TTF-Converter-CSharp-API}

For converting WOFF to TTF, we will be using the [Aspose.Font for .NET][7] API. It allows loading, saving, and extracting information from [supported font types][8]. Please either [download][9] the DLL of the API or install it using [NuGet][10].

```
PM> Install-Package Aspose.Font
```

## Convert WOFF to TTF using C# {#Convert-WOFF-to-TTF-using-CSharp}

We can easily convert Web Open Fonts (WOFF) to True Type Fonts (TTF) by following the steps given below:

1.  Firstly, load the font file using the **_[FileSystemStreamSource][11] _**class.
2.  Next, create an instance of the **_[FontFileDefinition][12] _**class with file extension as "woff" and the source file object as arguments.
3.  Then, initialize the **_[FontDefinition][13] _**class object with Font type as TTF and FontFileDefinition object.
4.  After that, open the font using the **_[Font.Open()][14]_** method with FontDefinition object as argument.
5.  Finally, call the **_[SaveToFormat()][15]_** method to save it. It takes the output file path and **_[FontSavingFormats][16] _**to _TTF_ as arguments.

The following code sample demonstrates **how to convert WOFF to TTF using C#**.

{{< gist aspose-com-gists e0ec151a44de63a9448a6f030a39ca3a "ConvertWOFFtoTTF_CSharp_WOFFtoTTF.cs" >}}

## Convert WOFF2 to TTF in C# {#Convert-WOFF2-to-TTF-in-CSharp}

We can also convert WOFF2 to TTF by following the steps mentioned earlier. However, we just need to set the file extension as “woff2” in the second step.

The following code sample demonstrates **how to convert WOFF2 to TTF using C#**.

{{< gist aspose-com-gists e0ec151a44de63a9448a6f030a39ca3a "ConvertWOFFtoTTF_CSharp_WOFF2toTTF.cs" >}}

## Get a Free License {#Get-a-Free-API-License}

You can [get a free temporary license][17] to try the library without evaluation limitations.

## Conclusion

In this article, we have learned how to convert Web Open Fonts to True Type Fonts in C#. We have also seen how to save WOFF2 as TTF programmatically. Besides, you can learn more about Aspose.Font for .NET API using the [documentation][18]. In case of any ambiguity, please feel free to contact us on the [forum][19].

## See Also

*   [Convert TTF to WOFF using C#][20]
*   [Load, Save, and Extract Information from Fonts using C#][21]




[1]: https://docs.fileformat.com/font/ttf/
[2]: https://blog.aspose.com/2022/03/15/convert-ttf-to-woff-using-csharp/
[3]: https://docs.fileformat.com/font/woff/
[4]: #WOFF-to-TTF-Converter-CSharp-API
[5]: #Convert-WOFF-to-TTF-using-CSharp
[6]: #Convert-WOFF2-to-TTF-in-CSharp
[7]: https://products.aspose.com/font/net
[8]: https://docs.aspose.com/font/net/supported-file-formats/
[9]: https://downloads.aspose.com/font/net
[10]: https://www.nuget.org/packages/Aspose.Font/
[11]: https://apireference.aspose.com/font/net/aspose.font.sources/filesystemstreamsource
[12]: https://apireference.aspose.com/font/net/aspose.font.sources/fontfiledefinition
[13]: https://apireference.aspose.com/font/net/aspose.font.sources/fontdefinition
[14]: https://apireference.aspose.com/font/net/aspose.font.font/open/methods/2
[15]: https://apireference.aspose.com/font/net/aspose.font/font/methods/savetoformat
[16]: https://apireference.aspose.com/font/net/aspose.font/fontsavingformats
[17]: https://purchase.aspose.com/temporary-license
[18]: https://docs.aspose.com/font/net/
[19]: https://forum.aspose.com/c/font/41
[20]: https://blog.aspose.com/2022/03/15/convert-ttf-to-woff-using-csharp/
[21]: https://blog.aspose.com/2020/09/14/load-save-extract-information-from-fonts-using-csharp/





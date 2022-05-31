---
title: 'Convert TTF to WOFF using C#'
date: Tue, 15 Mar 2022 06:28:25 +0000
draft: false
url: /2022/03/15/convert-ttf-to-woff-using-csharp/
author: 'Muzammil Khan'
summary: ''
tags: ['C# API to Convert TTF', 'Convert TTF to WOFF', 'TTF to WOFF .NET Converter', 'TTF to WOFF Converter API', 'TTF to WOFF Converter C#', 'TTF to WOFF in C#']
categories: ['Aspose.Font Product Family']
---



{{< figure align=center src="images/convert-ttf-to-woff-using-csharp.jpg" alt="Convert TTF to WOFF using C#">}}


Fonts define the graphical representation of an individual character in the text, such as its size, display style, weight, color, etc. [TTF (_True Type Font_)][1] works fine on all digital platforms and gives excellent quality on-screen and in printed documents. On the other hand, the [WOFF (_Web Open Font Format_)][2] is mostly used in web pages. It contains format-specific compression and additional XML metadata. In certain cases, we may need to convert true-type fonts into Web fonts. In this article, we will learn **how to convert TTF to WOFF using C#**.

The following topics shall be covered in this article:

*   [C# TTF to WOFF Converter API][3]
*   [Convert TTF to WOFF using C#][4]
*   [Convert TTF to WOFF2 in C#][5]

## C# TTF to WOFF Converter API {#CSharp-TTF-to-WOFF-Converter-API}

For converting TTF to WOFF, we will be using the [Aspose.Font for .NET][6] API. It allows loading, saving, and extracting information from [supported font types][7]. Please either [download][8] the DLL of the API or install it using [NuGet][9].

```
PM> Install-Package Aspose.Font
```

## Convert TTF to WOFF using C# {#Convert-TTF-to-WOFF-using-CSharp}

We can easily convert True Type Fonts (TTF) to Web Open Fonts (WOFF) by following the steps given below:

*   Firstly, load the font file using the **_[FileSystemStreamSource][10]_** class.
*   Next, create an instance of the **_[FontFileDefinition][11]_** class with source file object as an argument.
*   Then, initialize the **_[FontDefinition][12]_** class object with Font type as TTF and _FontFileDefinition_ object.
*   After that, open the font using the **_[Font][13].[Open()][14]_** method with _FontDefinition_ object as argument.
*   Finally, call the **_[SaveToFormat()][15]_** method to save it. It takes output file path and **_[FontSavingFormats][16]_** to _WOFF_ as arguments.

The following code sample demonstrates **how to convert TTF to WOFF using C#**.

{{< gist aspose-com-gists 6e2885e59eeebe9c0d0a5f6d88403e8e "ConvertTTFtoWOFF_CSharp_TTFtoWOFF.cs" >}}

## Convert TTF to WOFF2 in C# {#Convert-TTF-to-WOFF2-in-CSharp}

WOFF2 is an updated version of WOFF. It offers more compression due to which it is smaller in file size and provides better performance for modern browsers. We can also convert TTF to WOFF2 by following the steps mentioned earlier. However, we just need to set the **_FontSavingFormats_** as _WOFF_2 in the last step.

The following code sample demonstrates **how to convert TTF to WOFF2 using C#**.

{{< gist aspose-com-gists 6e2885e59eeebe9c0d0a5f6d88403e8e "ConvertTTFtoWOFF_CSharp_TTFtoWOFF2.cs" >}}

## Get a Free License {#Get-a-Free-API-License}

You can [get a free temporary license][17] to try the library without evaluation limitations.

## Conclusion

In this article, we have learned how to convert True Type Fonts to Web Open Fonts in C#. We have also seen how to save TTF as WOFF2 programmatically. Besides, you can learn more about Aspose.Font for .NET API using the [documentation][18]. In case of any ambiguity, please feel free to contact us on the [forum][19].

## See Also

*   [Load, Save, and Extract Information from Fonts using C#][20]




[1]: https://docs.fileformat.com/font/ttf/
[2]: https://docs.fileformat.com/font/woff/
[3]: #CSharp-TTF-to-WOFF-Converter-API
[4]: #Convert-TTF-to-WOFF-using-CSharp
[5]: #Convert-TTF-to-WOFF2-in-CSharp
[6]: https://products.aspose.com/font/net
[7]: https://docs.aspose.com/font/net/supported-file-formats/
[8]: https://downloads.aspose.com/font/net
[9]: https://www.nuget.org/packages/Aspose.Font/
[10]: https://apireference.aspose.com/font/net/aspose.font.sources/filesystemstreamsource
[11]: https://apireference.aspose.com/font/net/aspose.font.sources/fontfiledefinition
[12]: https://apireference.aspose.com/font/net/aspose.font.sources/fontdefinition
[13]: https://apireference.aspose.com/font/net/aspose.font/font
[14]: https://apireference.aspose.com/font/net/aspose.font.font/open/methods/3
[15]: https://apireference.aspose.com/font/net/aspose.font/font/methods/savetoformat
[16]: https://apireference.aspose.com/font/net/aspose.font/fontsavingformats
[17]: https://purchase.aspose.com/temporary-license
[18]: https://docs.aspose.com/font/net/
[19]: https://forum.aspose.com/c/font/41
[20]: https://blog.aspose.com/2020/09/14/load-save-extract-information-from-fonts-using-csharp/





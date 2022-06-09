---
title: 'Detect Latin Symbols in TrueType and Type1 Fonts using C++'
seoTitle: ""
description: ""
date: Thu, 01 Oct 2020 16:18:43 +0000
draft: false
url: /2020/10/01/detect-latin-symbols-in-truetype-type1-fonts-cpp/
author: Usman Aziz
summary: 'In the previous post, you have seen how to load and work with CFF, TrueType, OpenType, and Type1 fonts from within your C++ applications. This article takes you one step further by demonstrating how to detect the Latin symbols in a font programmatically using C++. After detection, you can decide whether a font supports the Latin symbols or not.'
tags: ['Detect Latin Symbols fonts using CPP', 'Detect Latin Symbols in TrueType', 'Detect Latin Symbols in Type1']
categories: ['Aspose.Font Product Family']
---



{{< figure align=center src="images/aspose_font-for-cpp.png" alt="">}}


In the [previous post][1], you have seen how to load and work with [CFF][2], [TrueType][3], [OpenType][4], and [Type1][5] fonts from within your C++ applications. This article takes you one step further by demonstrating **how to detect the Latin symbols in a font programmatically using C++**. After detection, you can decide whether a font supports the Latin symbols or not.

*   [C++ API to Detect Latin Symbols in Fonts][6]
*   [Detect Latin Symbols in TrueType Fonts using C++][7]
*   [Detect Latin Symbols in Type1 Fonts using C++][8]

## C++ API to Detect Latin Symbols in Fonts {#C++-API-to-Detect-Latin-Symbols-in-Fonts}

[Aspose.Font for C++][9] is a font manipulation and management API that lets you detect the support of Latin symbols in the fonts quite easily. You can either [download][10] the API or install it via [NuGet][11].

```
PM> Install-Package Aspose.Font.Cpp
```

## Detect Latin Symbols in TrueType Fonts in C++ {#Detect-Latin-Symbols-in-TrueType-Fonts-in-C++}

Detecting the support of Latin symbols using Aspose.Font for C++ is as simple as a pie. The following are the steps to check if a particular TrueType font supports Latin symbols or not.

*   Create an object of [FontDefinition][12] class to load the font by specifying its type as TrueType.
*   Create an object of [TtfFont][13] class to access the font's information.
*   Loop through the possible codes and decode them into glyph IDs.
*   Match the glyph IDs to check if Latin symbols are supported in the source TrueType font or not.

The following code sample shows how to detect Latin symbols in TrueType fonts using C++.

{{< gist aspose-com-gists bf610decea4168f9c64482594164892b "Examples-example-source-WorkingWithTrueTypeAndOpenTypeFonts-DetectLatinSymbolsSupport-1.cpp" >}}

## Detect Latin Symbols in Type1 Fonts in C++ {#Detect-Latin-Symbols-in-Type1-Fonts-in-C++}

The process of detecting Latin symbols in Type1 fonts is as same as you have done for TrueType fonts. The only difference is the use of the [Type1Font][14] class. The following steps demonstrate the complete process of Latin symbol detection in Type1 fonts.

*   Use the [FontDefinition][15] class to load the font by specifying its type as Type1.
*   Use [](https://apireference.aspose.com/font/cpp/class/aspose.font.ttf.ttf_font)[Type1Font][16] class to access the information of the font.
*   Loop through the possible codes and decode them into glyph IDs.
*   Match the glyph IDs to check the support of Latin symbols in the provided Type1 font.

The following code sample shows how to detect Latin symbols in Type1 font using C++.

{{< gist aspose-com-gists bf610decea4168f9c64482594164892b "Examples-example-source-WorkingWithType1Fonts-DetectLatinSymbolsSupport_-1.cpp" >}}

## Conclusion

In this article, you have learned how to detect Latin symbols in TrueType and Type1 fonts using C++. The code samples in this article let you determine if the Latin symbols are supported by a particular font or not. You can learn more about the C++ font manipulation API using [documentation][17].

## See Also

*   [Work with CFF, TrueType, and Type1 Fonts using C++][18]




[1]: https://blog.aspose.com/2020/09/30/work-with-truetype-cff-opentype-type1-fonts-cpp/
[2]: https://docs.fileformat.com/font/cff/
[3]: https://docs.fileformat.com/font/ttf/
[4]: https://docs.fileformat.com/font/otf/
[5]: https://docs.fileformat.com/font/type1/
[6]: #C++-API-to-Detect-Latin-Symbols-in-Fonts
[7]: #Detect-Latin-Symbols-in-TrueType-Fonts-in-C++
[8]: #Detect-Latin-Symbols-in-Type1-Fonts-in-C++
[9]: https://products.aspose.com/font/cpp
[10]: https://downloads.aspose.com/font/cpp
[11]: https://www.nuget.org/packages/Aspose.Font.Cpp/
[12]: https://apireference.aspose.com/font/cpp/class/aspose.font.sources.font_definition
[13]: https://apireference.aspose.com/font/cpp/class/aspose.font.ttf.ttf_font
[14]: https://apireference.aspose.com/font/cpp/class/aspose.font.type1.type1_font
[15]: https://apireference.aspose.com/font/cpp/class/aspose.font.sources.font_definition
[16]: https://apireference.aspose.com/font/cpp/class/aspose.font.type1.type1_font
[17]: https://docs.aspose.com/font/cpp/getting-started/
[18]: https://blog.aspose.com/2020/09/30/work-with-truetype-cff-opentype-type1-fonts-cpp/






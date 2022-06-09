---
title: 'Work with CFF, TrueType, and Type1 Fonts using C++'
seoTitle: ""
description: ""
date: Wed, 30 Sep 2020 16:08:44 +0000
draft: false
url: /2020/09/30/work-with-truetype-cff-opentype-type1-fonts-cpp/
author: Usman Aziz
summary: 'Fonts are an integral part of the digital documents and web pages that are used to define the appearance of the text. The font files are used to store information about the fonts such as styles, weight, size and etc. There could be the case when you would need to manipulate fonts in order to extract their information. For such scenarios, in this article, you will learn how to load and read information from TrueType, CFF, and Type1 fonts using C++.'
tags: ['extract font information cpp', 'font manipulation api cpp', 'load cff font cpp', 'load ttf font cpp', 'load type1 font cpp']
categories: ['Aspose.Font Product Family']
---



{{< figure align=center src="images/aspose_font-for-cpp.png" alt="">}}


[Fonts][1] are an integral part of digital documents and web pages that are used to define the appearance of the text. The font files are used to store information about the fonts such as styles, weight, size and etc. There could be the case when you would need to manipulate fonts in order to extract their information. For such scenarios, in this article, you will learn **how to load and read information from TrueType, CFF, and Type1 fonts using C++**.

*   [C++ Font Manipulation API][2]
*   [Load CFF, TrueType, and Type1 Fonts using C++][3]
*   [Extract Font Metrics from TrueType or Type1 Fonts using C++][4]

## C++ Font Manipulation Library {#C++-Font-Manipulation-API}

[Aspose.Font for C++][5] is a powerful font manipulation API that allows you to work with [TrueType][6], [CFF][7], [OpenType][8], and [Type1][9], [EOT][10], and many [other fonts][11] from within your C++ applications. You can load, save, and extract encoding information from the fonts as well as work with glyphs. The API can be downloaded from the [downloads][12] section or installed via [NuGet][13].

## Load CFF, TrueType, and Type1 Fonts using C++ {#Load-CFF-TrueType-and-Type1-Fonts-using-C++}

Aspose.Font for C++ lets you load the CFF, TrueType, and Type1 fonts from the files located on your storage media. The following are the steps to load a font.

*   Create an object of [FontDefinition][14] class to load the font by specifying its type i.e. TrueType, Type1, etc.
*   Use [CffFont][15], [TtfFont][16], or [Type1Font][17] class to open CFF, TrueType, and Type1 fonts respectively from _FontDefinition_ object.

### Load CFF Fonts using C++

The following code sample shows how to load CFF fonts using C++.

{{< gist aspose-com-gists bf610decea4168f9c64482594164892b "Examples-example-source-WorkingWithCFFFonts-LoadCFFFont-LoadCFFFromDisc.cpp" >}}

### Load TrueType Fonts using C++

The following code sample shows how to load TrueType fonts using C++.

{{< gist aspose-com-gists bf610decea4168f9c64482594164892b "Examples-example-source-WorkingWithTrueTypeAndOpenTypeFonts-LoadTrueTypeFonts-1.cpp" >}}

### Load Type1 Fonts using C++

The following code sample shows how to load Type1 fonts using C++.

{{< gist aspose-com-gists bf610decea4168f9c64482594164892b "Examples-example-source-WorkingWithType1Fonts-LoadType1Fonts-1.cpp" >}}

## Extract Font Metrics from TrueType or Type1 using C++ {#Extract-Font-Metrics-from-TrueType-or-Type1-using-C++}

Aspose.Font for C++ also allows you to extract the font metrics which contain information such as _Ascender_, _Descender_, _TypoAscender_, _TypoDescender_, and _UnitsPerEm_. The following are the steps to retrieve font metrics from a TrueType or Type1 font.

*   Create an object of [FontDefinition][18] class to load TrueType or Type1 font.
*   Open font using [TtfFont][19] or [Type1Font][20] class according to the font's type.
*   Extract the font’s metrics information.

### Get Font Metrics from TrueType Font using C++

{{< gist aspose-com-gists bf610decea4168f9c64482594164892b "Examples-example-source-WorkingWithTrueTypeAndOpenTypeFonts-GetFontMetrics-1.cpp" >}}

### Extract Font Metrics from Type1 Font using C++

{{< gist aspose-com-gists bf610decea4168f9c64482594164892b "Examples-example-source-WorkingWithType1Fonts-GetFontMetrics_-1.cpp" >}}

## Conclusion

In this article, you have learned how to load CFF, TrueType, and Type1 fonts and extract their information using C++. You can explore more about the C++ Font Manipulation API using the [documentation][21].




[1]: https://en.wikipedia.org/wiki/Font
[2]: #C++-Font-Manipulation-API
[3]: #Load-CFF-TrueType-and-Type1-Fonts-using-C++
[4]: #Extract-Font-Metrics-from-TrueType-or-Type1-using-C++
[5]: https://products.aspose.com/font/cpp
[6]: https://docs.fileformat.com/font/ttf/
[7]: https://docs.fileformat.com/font/cff/
[8]: https://docs.fileformat.com/font/otf/
[9]: https://docs.fileformat.com/font/type1/
[10]: https://docs.fileformat.com/font/eot/
[11]: https://docs.fileformat.com/font/
[12]: https://downloads.aspose.com/font/cpp
[13]: http://nuget.org/packages/Aspose.Font.Cpp
[14]: https://apireference.aspose.com/font/cpp/class/aspose.font.sources.font_definition
[15]: https://apireference.aspose.com/font/cpp/class/aspose.font.cff.cff_font
[16]: https://apireference.aspose.com/font/cpp/class/aspose.font.ttf.ttf_font
[17]: https://apireference.aspose.com/font/cpp/class/aspose.font.type1.type1_font
[18]: https://apireference.aspose.com/font/cpp/class/aspose.font.sources.font_definition
[19]: https://apireference.aspose.com/font/cpp/class/aspose.font.ttf.ttf_font
[20]: https://apireference.aspose.com/font/cpp/class/aspose.font.type1.type1_font
[21]: https://docs.aspose.com/font/cpp/getting-started/






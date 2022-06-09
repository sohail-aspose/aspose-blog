---
title: 'Load, Save and Extract Information from Fonts using C#'
seoTitle: ""
description: ""
date: Mon, 14 Sep 2020 17:24:48 +0000
draft: false
url: /2020/09/14/load-save-extract-information-from-fonts-using-csharp/
author: Usman Aziz
summary: "In digital typography, fonts define particular styles to be used for the characters' appearance. Most often, the fonts are utilized in the documents and the web pages to stylize the text. Each font is described in a file which contains information about characters' size, weight, styles, as well as the encoding. Since fonts are an important part of the various file formats, Aspose offers a dedicated API for dealing with the manipulation and rendering of popular font types including TrueType, CFF, OpenType, and Type1. In this article, you will learn how to load, save, and extract information from fonts using C# with Aspose.Font for .NET."
tags: ['.net font management api', 'get font metrics using csharp', 'load CFF font using csharp', 'load truetype ttf fonts using csharp', 'load type1 font using csharp']
categories: ['Aspose.Font Product Family']
---



{{< figure align=center src="images/aspose_font-for-net.png" alt=".NET Font Management API">}}


In digital [typography][1], fonts define particular styles to be used for the characters' appearance. Most often, the fonts are utilized in the documents and the web pages to stylize the text. Each font is described in a file that contains information about characters' size, weight, styles, as well as encoding. Since fonts are an important part of the various file formats, Aspose offers a dedicated API for dealing with the manipulation and rendering of popular font types including [TrueType][2], [CFF][3], [OpenType][4], and [Type1][5]. In this article, you will learn **how to load, save, and extract information from fonts using C#** with [Aspose.Font for .NET][6].

*   [.NET Font Manipulation and Management API][7]
*   [Load and Save CFF, TrueType, and Type1 Fonts using C#][8]
*   [Extract Font Metrics Information using C#][9]
*   [Detect Latin Symbols in Fonts using C#][10]

## .NET Font Manipulation API - Free Download {#NET-Font-Manipulation-and-Management-API}

[Aspose.Font for .NET][11] is an on-premise API that lets you implement the font management features using C# within your .NET applications. Along with loading, saving, and information extraction from the font, the API also allows you to render the glyph or text if required. You can either [download][12] the API or install it within your .NET applications using [NuGet][13].

```
PM> Install-Package Aspose.Font
```

## Load or Save Fonts From File using C# {#Load-and-Save-CFF-TrueType-and-Type1-Fonts-using-CSharp}

You can load a font from the file stored on your digital storage for retrieving the font's information. Aspose.Font for .NET exposes separate classes to deal with the particular types of fonts i.e. CFF, TrueType, etc. The following are the steps to load and save a font.

*   Load the font from the file (using file's path or byte array) using [FontDefinition][14] class.
*   Access font's information using [CffFont][15], [TtfFont][16], or [Type1Font][17] class.
*   Save the file (if required).

### Load and Save CFF Font

The following code sample shows how to load and save CFF fonts using C#.

{{< gist aspose-com-gists 10f0e5f274b436379dbc8fd4fb183fc5 "Examples-CSharp-WorkingWithCFFFonts-SaveCFFToDisc-1.cs" >}}

### Load and Save TrueType Font

The following code sample shows how to load and save TrueType fonts using C#.

{{< gist aspose-com-gists 10f0e5f274b436379dbc8fd4fb183fc5 "Examples-CSharp-WorkingWithTrueTypeAndOpenTypeFonts-SaveTTFToDisc-1.cs" >}}

### Load and Save Type1 Font

The following code sample shows how to load and save Type1 fonts using C#.

{{< gist aspose-com-gists 10f0e5f274b436379dbc8fd4fb183fc5 "Examples-CSharp-WorkingWithType1Fonts-LoadType1Fonts-1.cs" >}}

## Extract Font Metrics using C# {#Extract-Font-Metrics-Information-using-CSharp}

Aspose.Font for .NET also allows you to retrieve the font metrics information such as _Ascender_, _Descender_, _TypoAscender_, _TypoDescender,_ and _UnitsPerEm_. The following are the steps to do so.

*   Use [FontDefinition][18] class to load TrueType or Type1 font from file.
*   Open font using respective font type class i.e. Type1Font, TtfFont, etc.
*   Access the font's metrics information.

The following code samples show how to extract font metrics from TrueType and Type1 fonts using C#.

### Extract Metrics from TrueType Font

{{< gist aspose-com-gists 10f0e5f274b436379dbc8fd4fb183fc5 "Examples-CSharp-WorkingWithTrueTypeAndOpenTypeFonts-GetFontMetrics-1.cs" >}}

### Extract Metrics from Type1 Font

{{< gist aspose-com-gists 10f0e5f274b436379dbc8fd4fb183fc5 "Examples-CSharp-WorkingWithType1Fonts-GetFontMetrics-1.cs" >}}

## Detect Latin Symbols in Fonts using C# {#Detect-Latin-Symbols-in-Fonts-using-CSharp}

You can also detect Latin text in the fonts by decoding the glyph codes using Aspose.Font for .NET. The following are the steps to perform this operation.

*   Load the Font from the file using [FontDefinition][19] class.
*   Decode the GlyphId using the _DecodeToGid()_ method of the respective font class.

The following code samples show how to decode Latin symbols in TrueType and Type1 fonts using C#.

### Detect Latin Symbols in TrueType Font

{{< gist aspose-com-gists 10f0e5f274b436379dbc8fd4fb183fc5 "Examples-CSharp-WorkingWithTrueTypeAndOpenTypeFonts-DetectLatinSymbolsSupport-1.cs" >}}

### Detect Latin Symbols in Type1 Font

{{< gist aspose-com-gists 10f0e5f274b436379dbc8fd4fb183fc5 "Examples-CSharp-WorkingWithType1Fonts-DetectLatinSymbolsSupport-1.cs" >}}

## Conclusion

In this article, you have seen how to load and save CFF, TrueType and Type1 fonts programmatically using C#. Furthermore, you have learned how to extract font metrics information from TrueType and Type1 fonts within your .NET applications. You can explore more interesting features offered by Aspose.Font for .NET in the [documentation][20]. For more updates, keep visiting Aspose.Font [blog][21].




[1]: https://en.wikipedia.org/wiki/Typography
[2]: https://docs.fileformat.com/font/ttf/
[3]: https://docs.fileformat.com/font/cff/
[4]: https://docs.fileformat.com/font/otf/
[5]: https://docs.fileformat.com/font/type1/
[6]: https://products.aspose.com/font/net
[7]: #NET-Font-Manipulation-and-Management-API
[8]: #Load-and-Save-CFF-TrueType-and-Type1-Fonts-using-CSharp
[9]: #Extract-Font-Metrics-Information-using-CSharp
[10]: #Detect-Latin-Symbols-in-Fonts-using-CSharp
[11]: https://products.aspose.com/font/net
[12]: https://downloads.aspose.com/font/net
[13]: https://www.nuget.org/packages/Aspose.Font
[14]: https://apireference.aspose.com/font/net/aspose.font.sources/fontdefinition
[15]: https://apireference.aspose.com/font/net/aspose.font.cff/cfffont
[16]: https://apireference.aspose.com/font/net/aspose.font.ttf/ttffont
[17]: https://apireference.aspose.com/font/net/aspose.font.type1/type1font
[18]: https://apireference.aspose.com/font/net/aspose.font.sources/fontdefinition
[19]: https://apireference.aspose.com/font/net/aspose.font.sources/fontdefinition
[20]: https://docs.aspose.com/font/net/getting-started/
[21]: https://blog.aspose.com/category/font/






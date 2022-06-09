---
title: 'Detect Latin Symbols in TrueType and Type1 Fonts using Java'
seoTitle: "Detect Latin Symbols in TrueType and Type1 Fonts using Java"
description: "Detect whether a particular TrueType or Type1 font supports Latin symbols or not with the simple and easy to use Aspose.Font for Java API."
date: Tue, 17 Aug 2021 14:49:51 +0000
draft: false
url: /2021/08/17/detect-latin-symbols-in-truetype-and-type1-fonts-using-java/
author: Muhammad Ahmad
summary: 'Fonts are a set of printable or displayable characters with different styles, weights, etc. They are used to add a different look and feel to documents or web pages based on different requirements. Font files contain the design and other information regarding the font. In this article, we will use the font files to detect whether a font supports Latin symbols or not programmatically with Java.'
tags: ['Detect Latin Symbols in Fonts using Java', 'Detect Latin Symbols in TrueType Fonts using Java', 'Detect Latin Symbols in Type1 Fonts using Java']
categories: ['Aspose.Font Product Family']
---

Fonts are a set of printable or displayable characters with different styles, weights, etc. They are used to add a different look and feel to documents or web pages based on different requirements. Font files contain the design and other information regarding the font. In this article, we will use the font files to detect whether a font supports Latin symbols or not programmatically with Java.

*   [Java API for Detecting Latin Symbols in TrueType and Type1 Fonts][1]
*   [Detect Latin Symbols in TrueType Fonts using Java][2]
*   [Detect Latin Symbols in Type1 Fonts using Java][3]

## Java API for Detecting Latin Symbols in TrueType and Type1 Fonts {#Java-API-for-Detecting-Latin-Symbols-in-TrueType-and-Type1-Fonts}

[Aspose.Font for Java][4] is a library for working with fonts such as [TrueType][5], [CFF][6], [Type1][7], etc. The API supports loading, saving, and extracting information regarding fonts. The API also lets you detect the support for Latin symbols in fonts. You can either download the API using Maven or download the JAR from the [downloads][8] section.

```
<repository>
    <id>AsposeJavaAPI</id>
    <name>Aspose Java API</name>
    <url>https://repository.aspose.com/repo/</url>
</repository>
```
```
<dependency>
    <groupId>com.aspose</groupId>
    <artifactId>aspose-font</artifactId>
    <version>21.4</version>
</dependency>
```

## Detect Latin Symbols in TrueType Fonts using Java {#Detect-Latin-Symbols-in-TrueType-Fonts-using-Java}

The following are the steps to detect if a particular TrueType font supports Latin symbols or not.

*   Create an instance of the [FontDefinition][9] class using the font file.
*   Create an instance of the [TtfFont][10] class using the object of [FontDefinition][11] created in the previous step.
*   Loop through the different codes and decode them into glyph IDs.
*   Check the glyph IDs for the support of Latin symbols.

The following sample code shows how to detect if a particular TrueType font supports Latin symbols or not.

{{< gist aspose-com-gists 1947a7e974012064eb40f96e6ac8c543 "Detect_Latin_Symbols_In_TrueType_Fonts.java" >}}

## Detect Latin Symbols in Type1 Fonts using Java {#Detect-Latin-Symbols-in-Type1-Fonts-using-Java}

The process for detecting support for Latin symbols in Type1 fonts is similar to TrueType fonts. The only difference is that we will use the [Type1Font][12] class to access the font information. The following are the steps to detect the support for Latin symbols in Type1 fonts.

*   Create an instance of the [FontDefinition][13] class using the font file.
*   Create an instance of the [Type1Font][14] class using the object of [FontDefinition][15] created in the previous step.
*   Loop through the different codes and decode them into glyph IDs.
*   Check the glyph IDs for the support of Latin symbols.

The following sample code shows how to detect if a particular Type1 font supports Latin symbols or not.

{{< gist aspose-com-gists 1947a7e974012064eb40f96e6ac8c543 "Detect_Latin_Symbols_In_Type1_Fonts.java" >}}

## Get a Free License

In order to try the API without evaluation limitations, you can request [a free temporary license][16].

## Conclusion

In this article, you have learned how to detect the support for Latin symbols in fonts using Java. The shared code samples enable you to detect whether a particular font supports Latin symbols or not. Aspose.Font for Java provides many additional features for working with fonts that you can explore in detail by visiting the [official documentation][17]. In case of any questions, please feel free to reach us at our [free support forum][18].

## See Also

*   [Render Text with TrueType and Type1 Fonts using Java][19]




[1]: #Java-API-for-Detecting-Latin-Symbols-in-TrueType-and-Type1-Fonts
[2]: #Detect-Latin-Symbols-in-TrueType-Fonts-using-Java
[3]: #Detect-Latin-Symbols-in-Type1-Fonts-using-Java
[4]: https://products.aspose.com/font/java/
[5]: https://docs.fileformat.com/font/ttf/
[6]: https://docs.fileformat.com/font/cff/
[7]: https://docs.fileformat.com/font/type1/
[8]: https://downloads.aspose.com/font/java
[9]: https://apireference.aspose.com/font/java/com.aspose.font/FontDefinition
[10]: https://apireference.aspose.com/font/java/com.aspose.font/TtfFont
[11]: https://apireference.aspose.com/font/java/com.aspose.font/FontDefinition
[12]: https://apireference.aspose.com/font/java/com.aspose.font/Type1Font
[13]: https://apireference.aspose.com/font/java/com.aspose.font/FontDefinition
[14]: https://apireference.aspose.com/font/java/com.aspose.font/Type1Font
[15]: https://apireference.aspose.com/font/java/com.aspose.font/FontDefinition
[16]: https://purchase.aspose.com/temporary-license
[17]: https://docs.aspose.com/font/java/
[18]: https://forum.aspose.com/c/font/41
[19]: https://blog.aspose.com/2020/10/28/render-text-with-truetype-and-type1-fonts-using-java/






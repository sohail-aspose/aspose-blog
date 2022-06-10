---
title: 'Manipulate CFF, TrueType, and Type1 Fonts using Java'
seoTitle: "Work with CFF, TrueType, Type1 Fonts in Java | Get Font Metrics Info"
description: "Use Java Font Management API to load or save CFF, TrueType, Type1, and OpenType fonts using Java. Get font metrics information within Java applications."
date: Tue, 27 Oct 2020 23:28:34 +0000
draft: false
url: /2020/10/27/work-with-cff-truetype-and-type1-fonts-using-java/
author: Usman Aziz
summary: '[Fonts][1] play an important role in the presentation of the text within the documents and web pages. Various font families are available that allow you to use fancy characters in order to make your text appealing. Since Aspose deals with file format automation, we have launched a dedicated font manipulation API to work with font file formats. In this article, you will get familiar with our **Java Font API** and learn **how to work with CFF, TrueType, OpenType, and Type1 fonts** from within your Java applications.'
tags: ['Java Font API', 'get font metrics in Java', 'work with CFF Fonts in Java', 'work with TrueType Fonts in Java', 'work with Type1 Fonts in Java']
categories: ['Aspose.Font Product Family']
---



{{< figure align=center src="images/manipulate-cff-truetype-type1-fonts-in-java.png" alt="manipulate fonts in java">}}


[Fonts][2] play an important role in the presentation of the text within the documents and web pages. Various font families are available that allow you to use fancy characters in order to make your text appealing. Since Aspose deals with file format automation, we have launched a dedicated font manipulation API to work with font file formats. In this article, you will get familiar with our **Java Font API** and learn **how to work with CFF, TrueType, OpenType, and Type1 fonts** from within your Java applications.

*   [Java Font Manipulation API][3]
*   [Load CFF, TrueType, and Type1 Fonts using Java][4]
*   [Extract Font Metrics from TrueType or Type1 Fonts using Java][5]

## Java Font Manipulation API {#Java-Font-Manipulation-API}

[Aspose.Font for Java][6] is the font manipulation API that allows you to load, save, and manipulate popular fonts including [CFF][7], [TrueType][8], [Type1][9], [EOT][10], and [OpenType][11]. In addition, the API supports retrieving font metrics as well as rendering the text using the supported font types. You can [download][12] the API or install it within your Maven-based applications using the following configurations.

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
    <version>20.10</version>
</dependency>
```

## Load CFF, TrueType, and Type1 Fonts using Java {#Load-CFF-TrueType-and-Type1-Fonts-using-Java}

You can easily load the font from a file located on your storage from within your Java program. Once you have loaded the font, you can perform further operations as required. The following are the steps to load a font using Aspose.Font for Java.

*   Use the [FontDefinition][13] class to load the font by specifying its type such as _TrueType_, _Type1_, etc.
*   Use [CffFont][14], [TtfFont][15], or [Type1Font][16] class to access the CFF, TrueType, and Type1 fonts respectively from _FontDefinition_ object.

### Load CFF Fonts using Java

This is how you can load a CFF font from file using Java.

{{< gist aspose-com-gists a018220e20bd5728294c39d632ebf22b "Examples-src-main-java-com-aspose-font-WorkingWithCFFFonts-LoadCffFont-1.java" >}}

### Load TrueType Fonts using Java

The following Java code sample loads a TrueType font.

{{< gist aspose-com-gists a018220e20bd5728294c39d632ebf22b "Examples-src-main-java-com-aspose-font-WorkingWithTrueTypeFonts-LoadTrueTypeFonts-1.java" >}}

### Load Type1 Fonts using Java

The following code sample shows how to load a Type1 font using Java.

{{< gist aspose-com-gists a018220e20bd5728294c39d632ebf22b "Examples-src-main-java-com-aspose-font-WorkingWithType1Fonts-LoadType1Fonts-1.java" >}}

## Extract Font Metrics from TrueType or Type1 Fonts using Java {#Extract-Font-Metrics-from-TrueType-or-Type1-Fonts-using-Java}

The font files also contain the font's information that is used to specify the line spacing, placement of subscript and superscript, alignment, and etc. Aspose.Font for Java also allows you to extract the font metric information including _Ascender_, _Descender_, _TypoAscender_, _TypoDescender_, and _UnitsPerEm_. The following are the steps to perform this operation.

*   Use [FontDefinition][17] class to load _TrueType_ or _Type1_ font.
*   Access the font using [TtfFont][18] or [Type1Font][19] class according to the font’s type.
*   Extract the font’s metrics information.

### Get Font Metrics from TrueType Font using Java

{{< gist aspose-com-gists a018220e20bd5728294c39d632ebf22b "Examples-src-main-java-com-aspose-font-WorkingWithTrueTypeFonts-GetFontMetrics-1.java" >}}

### Extract Font Metrics from Type1 Font using Java

{{< gist aspose-com-gists a018220e20bd5728294c39d632ebf22b "Examples-src-main-java-com-aspose-font-WorkingWithType1Fonts-GetFontMetrics-1.java" >}}

## Conclusion

In this article, you have learned how to work with CFF, TrueType, and Type1 fonts programmatically using Java. Furthermore, you have seen how to access the font metrics information of a specific font. You can explore more about the Java font manipulation API using [documentation][20] and [source code samples][21].




[1]: https://en.wikipedia.org/wiki/Font
[2]: https://en.wikipedia.org/wiki/Font
[3]: #Java-Font-Manipulation-API
[4]: #Load-CFF-TrueType-and-Type1-Fonts-using-Java
[5]: #Extract-Font-Metrics-from-TrueType-or-Type1-Fonts-using-Java
[6]: https://products.aspose.com/font/java
[7]: https://docs.fileformat.com/font/cff/
[8]: https://docs.fileformat.com/font/ttf/
[9]: https://docs.fileformat.com/font/type1/
[10]: https://docs.fileformat.com/font/eot/
[11]: https://docs.fileformat.com/font/otf/
[12]: https://downloads.aspose.com/font/java
[13]: https://apireference.aspose.com/font/java/com.aspose.font/FontDefinition
[14]: https://apireference.aspose.com/font/java/com.aspose.font/CffFont
[15]: https://apireference.aspose.com/font/java/com.aspose.font/TtfFont
[16]: https://apireference.aspose.com/font/java/com.aspose.font/Type1Font
[17]: https://apireference.aspose.com/font/java/com.aspose.font/FontDefinition
[18]: https://apireference.aspose.com/font/java/com.aspose.font/TtfFont
[19]: https://apireference.aspose.com/font/java/com.aspose.font/Type1Font
[20]: https://docs.aspose.com/font/java/getting-started/
[21]: https://github.com/aspose-font/Aspose.Font-for-Java






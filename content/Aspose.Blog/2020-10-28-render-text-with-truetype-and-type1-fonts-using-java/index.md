---
title: 'Render Text with TrueType and Type1 Fonts using Java'
seoTitle: "Java: Render Text with TrueType and Type1 Fonts using Java Font API"
description: "Use Java font manipulation API to render text with TrueType and Type1 fonts using Java. Render provided text as JPEG image using glyphs in Ttf and Type1."
date: Wed, 28 Oct 2020 23:41:55 +0000
draft: false
url: /2020/10/28/render-text-with-truetype-and-type1-fonts-using-java/
author: Usman Aziz
summary: ''
tags: ['Java Font API', 'render text using Type1 font in java', 'render text using fonts in java', 'render text using truetype font in java']
categories: ['Aspose.Font Product Family']
---



{{< figure align=center src="images/render-text-with-truetype-type1-fonts-in-java-featuredimage.png" alt="render text using font in Java">}}


In the [previous article][1], you have seen how to load [CFF][2], [TrueType][3] and [Type1][4] fonts programmatically using Java. Today, we will discuss another interesting feature of our Java font manipulation API - rendering text using fonts. By the end of this article, you will be able to **render text using TrueType and Type1 fonts from within your Java applications**. So let's start.

*   [About Java Font Manipulation API][5]
*   [Implement Text Rendering Method][6]
*   [Render Text using TrueType Fonts in Java][7]
*   [Render Text using Type1 Fonts in Java][8]

## Java Font Manipulation API {#About-Java-Font-Manipulation-API}

[Aspose.Font for Java][9] provides you with the features of loading and saving the fonts as well as getting the metrics of the popular font types including CFF, TrueType, [OpenType][10], and Type1. In addition, the API lets you render the text using the provided TrueType or Type1 fonts. You can either install the API using Maven configurations or [download][11] the API's JAR.

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

## Implement Text Rendering Method {#Implement-Text-Rendering-Interface}

In order to render the text, Aspose.Font for Java requires you to implement the _drawText()_ method which will draw the provided text. The following is the complete definition of the _drawText()_ method.

{{< gist aspose-com-gists a018220e20bd5728294c39d632ebf22b "Examples-src-main-java-com-aspose-font-WorkingWithTrueTypeFonts-RenderingText-2.java" >}}

The following is a utility method that is used to calculate the glyph width for bitmap coordinate system.

{{< gist aspose-com-gists a018220e20bd5728294c39d632ebf22b "Examples-src-main-java-com-aspose-font-WorkingWithTrueTypeFonts-RenderingText-3.java" >}}

## Steps to Render Text with Font in Java

The following are the steps of how to render a specified text as an image file using the above-mentioned _darwText()_ method.

*   Load the font using the [FontDefinition][12] class.
*   Access the font using the class such as [Type1Font][13] or [TtfFont][14].
*   Call the _drawText()_ method by providing the details in the form of its parameters.

### Render Text with TrueType Font using Java {#Render-Text-with-TrueType-Font-using-Java}

The following code sample shows how to use the _drawText()_ method to render text using a TrueType font. The rendering results will be generated as a JPEG image.

{{< gist aspose-com-gists a018220e20bd5728294c39d632ebf22b "Examples-src-main-java-com-aspose-font-WorkingWithTrueTypeFonts-RenderingText-1.java" >}}

### Render Text using Type1 Fonts in Java {#Render-Text-using-Type1-Fonts-in-Java}

The following code sample shows how to render text to a JPEG image with a Type1 font using Java.

{{< gist aspose-com-gists a018220e20bd5728294c39d632ebf22b "Examples-src-main-java-com-aspose-font-WorkingWithType1Fonts-RenderingText-1.java" >}}

## Conclusion

In this article, you have seen how to render the text as [JPEG][15] images using the TrueType or Type1 font from within the Java applications. In order to learn more about the Java font manipulation API, you can visit the [documentation][16] and evaluate the API's features using [source code samples][17].




[1]: https://blog.aspose.com/2020/10/27/work-with-cff-truetype-and-type1-fonts-using-java/
[2]: https://docs.fileformat.com/font/cff/
[3]: https://docs.fileformat.com/font/ttf/
[4]: https://docs.fileformat.com/font/type1/
[5]: #About-Java-Font-Manipulation-API
[6]: #Implement-Text-Rendering-Interface
[7]: #Render-Text-with-TrueType-Font-using-Java
[8]: #Render-Text-using-Type1-Fonts-in-Java
[9]: https://products.aspose.com/font/java
[10]: https://docs.fileformat.com/font/otf/
[11]: https://downloads.aspose.com/font/java
[12]: https://apireference.aspose.com/font/java/com.aspose.font/FontDefinition
[13]: https://apireference.aspose.com/font/java/com.aspose.font/Type1Font
[14]: https://apireference.aspose.com/font/java/com.aspose.font/TtfFont
[15]: https://docs.fileformat.com/image/jpeg/
[16]: https://docs.aspose.com/font/java/getting-started/
[17]: https://github.com/aspose-font/Aspose.Font-for-Java






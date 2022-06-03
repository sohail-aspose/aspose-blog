---
title: 'Convert TTF to WOFF and WOFF2 using Java'
date: Thu, 19 May 2022 17:20:00 +0000
draft: false
url: /2022/05/19/convert-ttf-to-woff-and-woff2-using-java/
author: 'Muzammil Khan'
summary: 'As a Java developer, you can easily convert true-type fonts into Web fonts programmatically in Java applications. In this article, you will learn **how to convert TTF to WOFF and WOFF2 using Java.**'
tags: ['Convert TTF to WOFF', 'Convert TTF to WOFF2', 'Font Converter API', 'Java Font Converter', 'TTF to WOFF Converter API', 'TTF to WOFF in Java', 'TTF to WOFF2 in Java', 'TTF2WOFF']
categories: ['Aspose.Font Product Family']
---



{{< figure align=center src="images/convert-ttf-to-woff-and-woff2-using-java.jpg" alt="Convert TTF to WOFF and WOFF2 using Java.">}}


[WOFF (_Web Open Font Format_)][1] is basically a [TTF (_True Type Font_)][2] but it contains format-specific compression and additional XML metadata. WOFF2 is an extended version of WOFF. It offers more compression as compared to WOFF. Both WOFF and WOFF2 are used on webpages. On the other hand, [TTF (_True Type Font_)][3] works fine on all digital platforms and gives excellent quality on-screen and in printed documents. In certain cases, we may need to convert true-type fonts into Web fonts programmatically in Java applications. In this article, we will learn **how to convert TTF to WOFF and WOFF2 using Java**.

The following topics shall be covered in this article:

*   [Java API to Convert TTF to WOFF & WOFF2][4]
*   [Convert TTF to WOFF using Java][5]
*   [Convert TTF to WOFF2 in using Java][6]

## Java API to Convert TTF to WOFF & WOFF2 {#Java-API-to-Convert-TTF-to-WOFF-and-WOFF2}

For converting TTF to WOFF, we will be using the [Aspose.Font for Java][7] API. It provides the **_FontFileDefinition_** class that represents Font file definition. It also provides **_FontDefinition_** class that represents Font file set definition and provides basic details of the Font, such as name, type, etc. The **_Open()_** method of this class returns the _**FontDefinition**_ for font file and font type. We can convert the loaded font to other formats using the **_SaveToFormat()_** method of the **_Font_** class. Moreover, the API allows loading, saving, and extracting information from [supported font types][8].

Please either [download][9] the JAR of the API or add the following _**pom.xml**_ configuration in a Maven-based Java application.

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
    <version>21.12</version>
    <type>pom</type>
</dependency>
```

## Convert TTF to WOFF using Java {#Convert-TTF-to-WOFF-using-Java}

We can easily convert True Type Fonts (TTF) to Web Open Font Format (WOFF) by following the steps given below:

*   Firstly, load the font file using the **_[FileSystemStreamSource][10] _**class.
*   Next, create an instance of the **_[FontFileDefinition][11] _**class with the source file object as an argument.
*   Then, initialize the **_[FontDefinition][12] _**class object with Font type as TTF and _FontFileDefinition _object.
*   After that, open the font using the **_[Font][13].[Open()][14]_** method with _FontDefinition _object as an argument.
*   Finally, call the **_[SaveToFormat()][15]_** method to save it. It takes output file path and **_[FontSavingFormats][16]_** to _WOFF _as arguments.

The following code sample demonstrates **how to convert TTF to WOFF using Java.**

{{< gist aspose-font-gists 887e3073d438b2bb244e8e6dd5cc7ea2 "Convert-TTF-to-WOFF-Java_TTF2WOFF.java" >}}

## Convert TTF to WOFF2 using Java {#Convert-TTF-to-WOFF2-using-Java}

WOFF2 is an updated version of WOFF. It offers more compression due to which it is smaller in file size and provides better performance for modern browsers. We can also convert TTF to WOFF2 by following the steps mentioned earlier. However, we just need to set the **_FontSavingFormats _**as _WOFF_2 in the last step.

The following code sample demonstrates **how to convert TTF to WOFF2 using Java.**

{{< gist aspose-font-gists 887e3073d438b2bb244e8e6dd5cc7ea2 "Convert-TTF-to-WOFF-Java_TTF2WOFF2.java" >}}

## Get a Free License {#Get-a-Free-API-License}

You can [get a free temporary license][17] to try the library without evaluation limitations.

## Conclusion

In this article, we have learned how to convert True Type Fonts to Web Open Fonts in Java. We have also seen how to save TTF as WOFF2 programmatically. Besides, you can learn more about Aspose.Font for Java API using the [documentation][18]. In case of any ambiguity, please feel free to contact us on the [forum][19].

## See Also

*   [Detect Latin Symbols in TrueType and Type1 Fonts using Java][20]
*   [Render Text with TrueType and Type1 Fonts using Java Font API][21]
*   [Work with CFF, TrueType, Type1 Fonts in Java][22]




[1]: https://docs.fileformat.com/font/woff/
[2]: https://docs.fileformat.com/font/ttf/
[3]: https://docs.fileformat.com/font/ttf/
[4]: #Java-API-to-Convert-TTF-to-WOFF-and-WOFF2
[5]: #Convert-TTF-to-WOFF-using-Java
[6]: #Convert-TTF-to-WOFF2-using-Java
[7]: https://products.aspose.com/font/java
[8]: https://docs.aspose.com/font/java/supported-file-formats/
[9]: https://downloads.aspose.com/font/java
[10]: https://apireference.aspose.com/font/java/com.aspose.font/FileSystemStreamSource
[11]: https://apireference.aspose.com/font/java/com.aspose.font/FontFileDefinition
[12]: https://apireference.aspose.com/font/java/com.aspose.font/FontDefinition
[13]: https://apireference.aspose.com/font/java/com.aspose.font/Font
[14]: https://apireference.aspose.com/font/java/com.aspose.font/Font#open-com.aspose.font.FontDefinition-
[15]: https://apireference.aspose.com/font/java/com.aspose.font/Font#saveToFormat-java.io.OutputStream-com.aspose.font.FontSavingFormats-
[16]: https://apireference.aspose.com/font/java/com.aspose.font/fontsavingformats
[17]: https://purchase.aspose.com/temporary-license
[18]: https://docs.aspose.com/font/java/
[19]: https://forum.aspose.com/c/font/41
[20]: https://blog.aspose.com/2021/08/17/detect-latin-symbols-in-truetype-and-type1-fonts-using-java/
[21]: https://blog.aspose.com/2020/10/28/render-text-with-truetype-and-type1-fonts-using-java/
[22]: https://blog.aspose.com/2020/10/27/work-with-cff-truetype-and-type1-fonts-using-java/





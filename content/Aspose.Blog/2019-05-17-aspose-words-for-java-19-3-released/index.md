---
title: 'Support of JDK 7 and Bi-Directional Marks in TXT using Aspose.Words for Java 19.3'
date: Fri, 17 May 2019 05:58:39 +0000
draft: false
url: /2019/05/17/aspose-words-for-java-19-3-released/
author: Awais Hafeez
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---

Guys, lets check out what's new for you in [Aspose.Words for Java 19.3][1] release.

## Release JAR Upgraded to JDK 7

We have upgraded the release JAR of Aspose.Words for Java from JDK 6 to JDK 7. This means that if you are referencing [Aspose.Words for Java from Maven][2] then you will have to update the classifier value to jdk17 as follows:

```
<dependency>
    <groupId>com.aspose</groupId>
    <artifactId>aspose-words</artifactId>
    <version>19.3</version>
    <classifier>jdk17</classifier>
</dependency>
```

## Preserve Representation of Legacy Control Characters While Exporting Document to OOXML

Some document formats support legacy control characters. MS Word does not save these symbols to DOCX format (_more accurately in OOXML formats_). However, we added new property [KeepLegacyControlChars in OoxmlSaveOptions][3] class to preserve such control characters. So far only one legacy character (ShortDateTime) is supported which declared in the “DOC” format. Here’s how you can use this property:

{{< gist aspose-com-gists aa75ee5112aca57022c741270ff8cbc4 "Examples-src-main-java-com-aspose-words-examples-loading_saving-WorkingWithOoXML-keepLegacyControlChars.java" >}}

## How to Add Bi-Directional Marks

You can use [TxtSaveOptions.AddBidiMarks property][4] to specify whether to add bi-directional marks before each BiDi run when exporting in plain text format. Aspose.Words inserts Unicode Character 'RIGHT-TO-LEFT MARK' (U+200F) before each bi-directional Run in text. This option corresponds to "Add bi-directional marks" option in MS Word File Conversion dialog when you export to a Plain Text format. Note that it appears in dialog only if any of Arabic or Hebrew editing languages are added in MS Word. Below code example shows how to use TxtSaveOptions.AddBidiMarks property. The default value of this property is false.

{{< gist aspose-com-gists aa75ee5112aca57022c741270ff8cbc4 "Examples-src-main-java-com-aspose-words-examples-loading_saving-WorkingWithTxt-AddBidiMarks.java" >}}

## Predefined Font Fallback Settings for Google Noto Fonts

You may know about [Noto][5]. It is a font family comprising over a hundred individual fonts. We have added predefined font fallback settings for Google Noto fonts. These are free fonts licensed under SIL OFL. Here are two important points:

*   The predefined settings uses only Sans style Noto fonts with regular weight.
*   Aspose.Words does not support advanced typography. So, the Noto fonts that use advanced typography may be rendered inaccurately

Following code example shows how to use predefined font fallback settings  

{{< gist aspose-com-gists aa75ee5112aca57022c741270ff8cbc4 "Examples-src-main-java-com-aspose-words-examples-rendering_printing-SetFontSettings-setPredefinedFontFallbackSettings.java" >}}

## Text Alignment of Axis Tick Labels

If you want to set text alignment for multi-line labels, you can simply achieve this by setting the value of [ChartAxis.setTickLabelAlignment()][6] property. Following code example shows how to tick label alignment.

{{< gist aspose-com-gists aa75ee5112aca57022c741270ff8cbc4 "Examples-src-main-java-com-aspose-words-examples-programming_documents-charts-WorkingWithChartAxis-TickMultiLineLabelAlignment.java" >}}

## Specify How List Levels are Indented When Exporting Document to Plain Text Format

Aspose.Words introduced [TxtListIndentation class][7] that allows specifying how list levels are indented while exporting to a plain text format. While working with TxtSaveOption, the ListIndentation property is provided to specify the character to be used for indenting list levels and count specifying how many characters to use as indentation per one list level. The default value for character property is '\\0' indicating that there is no indentation. For count property, the default value is 0 which means no indentation.

### Using Tab Character{{< gist aspose-com-gists aa75ee5112aca57022c741270ff8cbc4 "Examples-src-main-java-com-aspose-words-examples-loading_saving-WorkingWithTxt-useTabCharacterPerLevelForListIndentation.java" >}}

### Using Space Character{{< gist aspose-com-gists aa75ee5112aca57022c741270ff8cbc4 "Examples-src-main-java-com-aspose-words-examples-loading_saving-WorkingWithTxt-useSpaceCharacterPerLevelForListIndentation.java" >}}

### Using Default Indentation{{< gist aspose-com-gists aa75ee5112aca57022c741270ff8cbc4 "Examples-src-main-java-com-aspose-words-examples-loading_saving-WorkingWithTxt-defaultLevelForListIndentation.java" >}}

## See also Useful Links

*   [Aspose.Words for Java Online Documentation][8] - up-to-date documentation containing Programmer's Guide, Knowledge Base and much more.
*   [Aspose.Words for Java Product Page][9]
*   [Install Aspose.Words for Java from Maven][10]
*   [Aspose.Words for Java API Reference Guide][11] - detailing the publicly exposed classes, methods, properties, constants & interfaces.
*   [Download Examples at GitHub Repository][12] - we have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.

Keeping the Aspose tradition, you are welcome to shape the upcoming releases of Aspose.Words for Java API by posting your suggestions and concerns in the [Aspose.Words for Java Support Forum][13].




[1]: https://downloads.aspose.com/words/java/new-releases/aspose.words-for-java-19.3/
[2]: https://repository.aspose.com/repo/com/aspose/aspose-words/19.3/
[3]: https://apireference.aspose.com/java/words/com.aspose.words/ooxmlsaveoptions#KeepLegacyControlChars
[4]: https://apireference.aspose.com/java/words/com.aspose.words/txtsaveoptions#AddBidiMarks
[5]: https://www.google.com/get/noto/
[6]: https://apireference.aspose.com/java/words/com.aspose.words/chartaxis#TickLabelAlignment
[7]: https://apireference.aspose.com/java/words/com.aspose.words/TxtListIndentation
[8]: https://docs.aspose.com/display/wordsjava/Home
[9]: https://products.aspose.com/words/java
[10]: https://repository.aspose.com/webapp/#/artifacts/browse/tree/General/repo/com/aspose/aspose-words
[11]: https://apireference.aspose.com/java/words
[12]: https://github.com/aspose-words/Aspose.Words-for-Java
[13]: https://forum.aspose.com/c/words





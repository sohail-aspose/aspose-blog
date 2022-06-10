---
title: 'Use Additional Text Positioning Operators in Word Documents using Java'
date: Sat, 25 May 2019 11:03:28 +0000
draft: false
url: /2019/05/25/aspose-words-for-java-19-4-released/
author: Awais Hafeez
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---

Guys, lets check out what's new for you in [Aspose.Words for Java 19.4][1] release.

## Cold Startup Time Improved

Starting from this version, we have improved cold startup time by 10% and also reduced the parsing time of Fields during a MailMerge operation.

## Additional Text Positioning Operators

To overcome the issues with inaccurate text positioning with some printers, the [AdditionalTextPositioning][2] flag can be used which specifies whether to write additional text positioning operators or not. The downside is the increased PDF document size and the default value for this flag is false.

{{< gist aspose-com-gists aa75ee5112aca57022c741270ff8cbc4 "Examples-src-main-java-com-aspose-words-examples-rendering_printing-WorkingWithPdfSaveOptions-AdditionalTextPositioning.java" >}}

## Resolve Font While Loading HTML or SVG

Previously, while loading HTML or SVG documents, font families were resolved against fonts installed in the local system. If a font family couldn't be resolved to an installed font, it was stored in the model as is. This led to situations where resolved font names depended on the local system and were not affected by FontSettings specified by users.

Please check the following HTML. If ‘UnknownFont1’ is not installed on the system, the following font family declaration resolved to “Arial” (“Arial” is the font name we use for “san-serif” generic font name.)

```
<p style='font-family:UnknownFont1, sans-serif;'>This is a paragraph.
```

Starting from Aspose.Words 19.4, FontSettings are taken into account while importing HTML and SVG documents and you can set up FontSettings before loading a document (_add substitution rule, specify fonts folder, etc._) in order to change fonts available for font resolution.

Here is sample code example that shows how to add a font substitution rule while loading a document.

{{< gist aspose-com-gists aa75ee5112aca57022c741270ff8cbc4 "Examples-src-main-java-com-aspose-words-examples-rendering_printing-WorkingWithFontResolution-FontSettingsWithLoadOptions.java" >}}

## Added More Flexible Control Over Document Import

We added ImportFormatOptions class with public property [SmartStyleBehavior][3] in Aspose.Words 19.4. This property is used to specify how styles will be imported when they have equal names in source and destination documents. You can enable or disable this feature while importing one document into another.

When this option is enabled, a source style will be expanded into a direct attribute inside a destination document, if KeepSourceFormatting importing mode is used. And when this option is disabled, a source style will be expanded only if it is numbered. Existing destination attributes will not be overridden, including lists.

For a moment, this option can be used only with a new public method of a DocumentBuilder class as shown in the example given below:

{{< gist aspose-com-gists aa75ee5112aca57022c741270ff8cbc4 "Examples-src-main-java-com-aspose-words-examples-programming_documents-document-WorkingWithImportFormatOptions-SmartStyleBehavior.java" >}}

## Control Import of Numbering when it Clashes in Source and Destination Documents

When import nodes between different documents there can be a situation when source document has lists with the same identifiers that were already used in a destination document. Word in such case always uses the formatting from the destination lists. To allow users to choose an appropriate behavior, the [KeepSourceNumbering][4] property was introduced in ImportFormatOptions class which specifies how the numbering will be imported when it clashes in source and destination documents. The default value is false.

For using this property, a new public method that accepts the new KeepSourceNumbering option was introduced as shown in the following example:  

{{< gist aspose-com-gists aa75ee5112aca57022c741270ff8cbc4 "Examples-src-main-java-com-aspose-words-examples-programming_documents-document-WorkingWithImportFormatOptions-KeepSourceNumbering.java" >}}

## Improved Importing Behavior for TextBox

When importing a text box between different documents, the formatting of the destination document is applied to it. This corresponds to the behavior of MS Word. To allow users to choose an appropriate behavior, the [IgnoreTextBoxes][5] option was introduced in ImportFormatOptions class. This property indicates whether to ignore formatting in the text boxes of the source destination during the import and the default value is true.

{{< gist aspose-com-gists aa75ee5112aca57022c741270ff8cbc4 "Examples-src-main-java-com-aspose-words-examples-programming_documents-document-WorkingWithImportFormatOptions-IgnoreTextBoxes.java" >}}

## Set Vertically Aligned Text Within Text Box

If you want to set the text alignment of textbox vertically, the solution is simple. You can use [TextBox.VerticalAnchor][6] property. We added this property in Aspose.Words 19.4.

Following code example shows how to use this property.

{{< gist aspose-com-gists aa75ee5112aca57022c741270ff8cbc4 "Examples-src-main-java-com-aspose-words-examples-programming_documents-Shapes-WorkingWithShapes-SpecifyVerticalAnchor.java" >}}

## See also Useful Links

*   [Aspose.Words for Java Online Documentation][7] - up-to-date documentation containing Programmer's Guide, Knowledge Base and much more.
*   [Aspose.Words for Java Product Page][8]
*   [Install Aspose.Words for Java from Maven][9]
*   [Aspose.Words for Java API Reference Guide][10] - detailing the publicly exposed classes, methods, properties, constants & interfaces.
*   [Download Examples at GitHub Repository][11] - we have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.

Keeping the Aspose tradition, you are welcome to shape the upcoming releases of Aspose.Words for Java API by posting your suggestions and concerns in the [Aspose.Words for Java Support Forum][12].




[1]: https://downloads.aspose.com/words/java/new-releases/aspose.words-for-java-19.4/
[2]: https://apireference.aspose.com/java/words/com.aspose.words/pdfsaveoptions#AdditionalTextPositioning
[3]: https://apireference.aspose.com/java/words/com.aspose.words/importformatoptions#SmartStyleBehavior
[4]: https://apireference.aspose.com/java/words/com.aspose.words/importformatoptions#KeepSourceNumbering
[5]: https://apireference.aspose.com/java/words/com.aspose.words/importformatoptions#IgnoreTextBoxes
[6]: https://apireference.aspose.com/java/words/com.aspose.words/textbox#VerticalAnchor
[7]: https://docs.aspose.com/display/wordsjava/Home
[8]: https://products.aspose.com/words/java
[9]: https://repository.aspose.com/webapp/#/artifacts/browse/tree/General/repo/com/aspose/aspose-words
[10]: https://apireference.aspose.com/java/words
[11]: https://github.com/aspose-words/Aspose.Words-for-Java
[12]: https://forum.aspose.com/c/words





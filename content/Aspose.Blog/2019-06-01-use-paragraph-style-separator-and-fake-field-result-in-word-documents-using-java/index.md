---
title: 'Use Paragraph Style Separator and Fake Field Result in Word Documents using Java'
date: Sat, 01 Jun 2019 12:09:59 +0000
draft: false
url: /2019/06/01/use-paragraph-style-separator-and-fake-field-result-in-word-documents-using-java/
author: Awais Hafeez
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---

Guys, let's check out what's new for you in [Aspose.Words for Java 19.5][1] release.

## Paragraph Style Separator in Word Documents

A style separator can be added to the end of a paragraph using the Ctrl + Alt + Enter Keyboard Shortcut into MS Word. This feature allows for two different paragraph styles used in one logical printed paragraph. Starting from Aspose.Words 19.5, you will be able to identify either a paragraph break is a Style Separator or not. The Paragraph.BreakIsStyleSeparator property has been added to this release. The below code example shows how to use it.

{{< gist aspose-com-gists aa75ee5112aca57022c741270ff8cbc4 "Examples-src-main-java-com-aspose-words-examples-programming_documents-document-ParagraphStyleSeparator-ParagraphStyleSeparator.java" >}}

## Get Font Line Spacing in Word Documents

The line spacing of a font is the vertical distance between the baselines of two consecutive lines of text. Thus, the line spacing includes the blank space between lines along with the height of the character itself.

The LineSpacing property was introduced in the Font class to obtain this value as shown in the example given below:

{{< gist aspose-com-gists aa75ee5112aca57022c741270ff8cbc4 "Examples-src-main-java-com-aspose-words-examples-programming_documents-document-GetFontLineSpacing-GetFontLineSpacing.java" >}}

## AppendDocument Overload Added with Additional ImportFormatOptions Parameter

Aspose.Words now provides a new overloaded AppendDocument() method into a Document class. It allows specifying additional options that affect the formatting of a result document. The following code example shows the usage of this method.

{{< gist aspose-com-gists aa75ee5112aca57022c741270ff8cbc4 "Examples-src-main-java-com-aspose-words-examples-programming_documents-joining_appending-AppendwithImportFormatOptions-AppendwithImportFormatOptions.java" >}}

## Check if Particular DML Text Effect is Applied

Aspose.Words now provides Font.HasDmlEffect() method to check if particular DML text effect is applied to the Run. This is a boolean type property and returns true if particular DML text effect is applied. The given below code example shows how to use this property.

{{< gist aspose-com-gists aa75ee5112aca57022c741270ff8cbc4 "Examples-src-main-java-com-aspose-words-examples-programming_documents-document-CheckDMLTextEffect-CheckDMLTextEffect.java" >}}

## Get Fake Result of Field

Aspose.Words now provides a property to obtain the field's result for fields that do not have a field separator node. We call this "fake result" or display result; MS Word displays it in the document by calculating the field's value on the fly, but there is no such value in the document model. The following code example shows the usage of Filed.DisplayResult property.

{{< gist aspose-com-gists aa75ee5112aca57022c741270ff8cbc4 "Examples-src-main-java-com-aspose-words-examples-programming_documents-fields-FieldDisplayResult-FieldDisplayResult.java" >}}

## See also Useful Links

*   [Aspose.Words for Java Online Documentation][2] - up-to-date documentation containing Programmer's Guide, Knowledge Base and much more.
*   [Aspose.Words for Java Product Page][3]
*   [Install Aspose.Words for Java from Maven][4]
*   [Aspose.Words for Java API Reference Guide][5] - detailing the publicly exposed classes, methods, properties, constants & interfaces.
*   [Download Examples at GitHub Repository][6] - we have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.

Keeping the Aspose tradition, you are welcome to shape the upcoming releases of Aspose.Words for Java API by posting your suggestions and concerns in the [Aspose.Words for Java Support Forum][7].




[1]: https://downloads.aspose.com/words/java/new-releases/aspose.words-for-java-19.5/
[2]: https://docs.aspose.com/display/wordsjava/Home
[3]: https://products.aspose.com/words/java
[4]: https://repository.aspose.com/webapp/#/artifacts/browse/tree/General/repo/com/aspose/aspose-words
[5]: https://apireference.aspose.com/java/words
[6]: https://github.com/aspose-words/Aspose.Words-for-Java
[7]: https://forum.aspose.com/c/words





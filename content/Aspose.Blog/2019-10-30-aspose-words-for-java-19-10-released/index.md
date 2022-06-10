---
title: 'Insert Hyperlinks to Bookmarks in Word Documents using Java'
date: Wed, 30 Oct 2019 10:08:13 +0000
draft: false
url: /2019/10/30/aspose-words-for-java-19-10-released/
author: Awais Hafeez
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---

Today, I will highlight the major features introduced in [Aspose.Words for Java 19.10][1] release:

## Main Maven POM File Automation

We have now added automation code in the [Main Maven POM file][2]. When you run this POM file, it will automatically choose the correct JDK version and download the plugin (if needed) for advanced HarfBuzz Shaper based Typography (note that this only works for windows).

## Insert Hyperlink Dynamically using LINQ Reporting Engine

You can now insert hyperlinks to your reports dynamically by using the _link_ tags. Syntax of a _link_ tag is defined as follows.  
**<<link \[uri\_or\_bookmark\_expression\] \[display\_text\_expression\]>>**  

Here, _uri\_or\_bookmark\_expression_ defines URI or the name of a bookmark within the same document for a hyperlink to be inserted dynamically. This expression is mandatory and must return a non-empty value.

In turn, _display\_text\_expression_ defines text to be displayed for the hyperlink. This expression is optional. If it is omitted or returns an empty value, then during runtime, a value of _uri\_or\_bookmark\_expression_ is used as display text as well. For more details, refer to the following article:  
[Inserting Hyperlinks Dynamically][3]  

## Specify or Detect Document's Text Direction

Aspose.Words for Java now provides DocumentDirection property in TxtLoadOptions class to [detect the text direction (RTL / LTR) in the document][4]. This property sets or gets document text directions provided in DocumentDirection enumeration. The default value is left to right (LTR).

The following code example demonstrates how to detect text direction of the document while importing TXT file.

{{< gist aspose-com-gists aa75ee5112aca57022c741270ff8cbc4 "Examples-src-main-java-com-aspose-words-examples-loading_saving-WorkingWithTxt-DocumentTextDirection.java" >}}

## See also Useful Links

*   [Aspose.Words for Java Online Documentation][5] - up-to-date documentation containing Programmer's Guide, Knowledge Base and much more.
*   [Aspose.Words for Java Product Page][6]
*   [Install Aspose.Words for Java from Maven][7]
*   [Aspose.Words for Java API Reference Guide][8] - detailing the publicly exposed classes, methods, properties, constants & interfaces.
*   [Download Examples at GitHub Repository][9] - we have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.

Keeping the Aspose tradition, you are welcome to shape the upcoming releases of Aspose.Words for Java API by posting your suggestions and concerns in the [Aspose.Words for Java Support Forum][10].




[1]: https://downloads.aspose.com/words/java/new-releases/aspose.words-for-java-19.10/
[2]: https://repository.aspose.com/webapp/#/artifacts/browse/tree/PomView/repo/com/aspose/aspose-words/19.10/aspose-words-19.10.pom
[3]: https://docs.aspose.com/words/java/inserting-hyperlinks-dynamically/
[4]: https://docs.aspose.com/words/java/working-with-text-document/#WorkingwithTextDocument-DetectDocumentTextDirection
[5]: https://docs.aspose.com/words/java/
[6]: https://products.aspose.com/words/java
[7]: https://repository.aspose.com/webapp/#/artifacts/browse/tree/General/repo/com/aspose/aspose-words
[8]: https://apireference.aspose.com/java/words
[9]: https://github.com/aspose-words/Aspose.Words-for-Java
[10]: https://forum.aspose.com/c/words





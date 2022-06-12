---
title: 'Convert Text to PNG, JPEG, or GIF Image in Java'
seoTitle: "Convert Text to Image in Java | TXT to PNG, JPEG, or GIF images"
description: "Use Java word processing library to convert text to image in Java. Convert text in TXT files to PNG, JPEG, or GIF images programmatically."
date: Mon, 06 Jun 2022 11:31:45 +0000
draft: false
url: /2022/06/06/convert-text-to-image-in-java/
author: Usman Aziz
summary: 'Text-to-image conversion is often required in various cases, such as, to make the text read-only. In a [previous article][1], we wrote about how to convert the text in a [TXT][2] file to a PDF in Java. In this article, you will learn **how to convert a text to a [PNG][3], [JPEG][4], or [GIF][5] image programmatically in Java**.'
tags: ['Convert Text to GIF in Java', 'Convert Text to Image in Java', 'Convert Text to JPG in Java', 'Convert Text to PNG in Java', 'Java API to Convert Text to Images']
categories: ['Aspose.Words Product Family']
---



{{< figure align=center src="images/Convert-Text-to-Image.png" alt="Convert Text to PNG, JPEG, or GIF Image in Java">}}


Text-to-image conversion is often required in various cases, such as, to make the text read-only. In a [previous article][6], we wrote about how to convert the text in a [TXT][7] file to a PDF in Java. In this article, you will learn **how to convert a text to a [PNG][8], [JPEG][9], or [GIF][10] image programmatically in Java**.

*   [Java API to Convert Text to Images][11]
*   [Convert Text (TXT) to Image in Java][12]

## API to Convert Text to PNG, JPEG, or GIF Image in Java {#API-to-Convert-Text-to-Image}

[Aspose.Words for Java][13] is a feature-rich API to create, edit, or convert MS Word documents in Java-based applications. Furthermore, it supports high fidelity conversion of text documents to other document and image formats. In this article, we will use Aspose.Words for Java to convert text to PNG, JPEG, or GIF images. You can [download][14] the API’s JAR or install it using the following Maven configurations:

```
**Repository:**
<repository>
    <id>AsposeJavaAPI</id>
    <name>Aspose Java API</name>
    <url>https://repository.aspose.com/repo/</url>
</repository>

**Dependency:**
<dependency>
    <groupId>com.aspose</groupId>
    <artifactId>aspose-words</artifactId>
    <version>22.4</version>
    <classifier>jdk17</classifier>
</dependency>
```

## Convert Text (TXT) to Image in Java {#Convert-Text-TXT-to-Image}

TXT files provide the simplest and easiest way to store plain text without any formatting. Therefore, we will use a TXT file and convert its text into PNG, JPEG, or GIF images. The following are the steps to convert text to images in Java.

*   Load the text file using the ****[Document][15]**** class.
*   Loop through all the pages in the document.
*   Extract each page using **[Document.ExtractPages()][16]** method.
*   Save page as PNG (or another image format) using **[Document.save()][17]** method.

The following code sample shows how to convert text to images in Java.

\[gist id="3c0852b11533f8444cc7bdd3b579ff85" file="convert-text-to-image.java"\]

## Get a Free API License {#Get-a-Free-API-License}

You can [get a temporary license][18] in order to use Aspose.Words for Java without evaluation limitations.

## Conclusion

In this article, you have learned how to convert a text to image programmatically in Java. You can simply install the API and use the provided code sample to convert the text to PNG, JPEG, or GIF images. Besides, you can explore other features of Aspose.Words for Java using the [documentation][19]. Also, in case you would have any questions or queries, you can contact us via our [forum][20].

## See Also

*   [Create MS Word Document in C#][21]
*   [Create Rich Word Documents in Java][22]


[1]: https://blog.aspose.com/2021/11/01/convert-txt-to-pdf-in-java/
[2]: https://docs.fileformat.com/word-processing/txt/
[3]: https://docs.fileformat.com/image/png/
[4]: https://docs.fileformat.com/image/jpeg/
[5]: https://docs.fileformat.com/image/gif/
[6]: https://blog.aspose.com/2021/11/01/convert-txt-to-pdf-in-java/
[7]: https://docs.fileformat.com/word-processing/txt/
[8]: https://docs.fileformat.com/image/png/
[9]: https://docs.fileformat.com/image/jpeg/
[10]: https://docs.fileformat.com/image/gif/
[11]: #API-to-Convert-Text-to-Image
[12]: #Convert-Text-TXT-to-Image
[13]: https://products.aspose.com/words/java/
[14]: https://downloads.aspose.com/words/java
[15]: https://apireference.aspose.com/words/java/com.aspose.words/Document
[16]: https://reference.aspose.com/words/java/com.aspose.words/document#extractPages(int,int)
[17]: https://reference.aspose.com/words/java/com.aspose.words/document#save(java.lang.String)
[18]: https://purchase.aspose.com/temporary-license
[19]: https://docs.aspose.com/words/java/
[20]: https://forum.aspose.com/
[21]: https://blog.aspose.com/2020/01/08/csharp-word-automation-create-edit-process-word-documents/
[22]: https://blog.aspose.com/2020/03/11/create-rich-word-documents-programmatically-in-java-using-java-word-api/






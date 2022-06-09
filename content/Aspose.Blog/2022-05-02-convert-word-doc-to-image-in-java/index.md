---
title: 'Convert Word DOC to PNG, JPEG, BMP, GIF, or TIFF in Java'
seoTitle: "Java Convert Word DOC to PNG, JPEG, BMP, GIF, TIFF | Java Word API"
description: "Use Java Word processing API to convert Word DOC or DOCX to PNG, JPEG, BMP, GIF, or TIFF images programmatically. Customize Word to image in conversion."
date: Mon, 02 May 2022 06:17:00 +0000
draft: false
url: /2022/05/02/convert-word-doc-to-image-in-java/
author: Usman Aziz
summary: 'In various cases, we need to display MS Word documents into our applications programmatically. One of the most convenient ways in such scenarios is the conversion from DOCX/DOC to image formats. To accomplish that, in this article, you will learn **how to convert Word [DOC][1] or **[DOCX][2]** files to [PNG][3], [JPEG][4], [BMP][5], [GIF][6], or [TIFF][7] images in Java**. Furthermore, we will cover how to control the Word to image conversion using different options.'
tags: ['Convert Word DOC to BMP in Java', 'Convert Word DOC to GIF in Java', 'Convert Word DOC to JPG in Java', 'Convert Word DOC to PNG in Java', 'Convert Word DOC to TIFF in Java', 'Java API for Word to Image Conversion']
categories: ['Aspose.Words Product Family']
---



{{< figure align=center src="images/Word-to-Image.jpg" alt="Convert Word DOC to PNG, JPEG, BMP, GIF, or TIFF in Java">}}


In various cases, we need to display MS Word documents into our applications programmatically. One of the most convenient ways in such scenarios is the conversion from DOCX/DOC to image formats. To accomplish that, in this article, you will learn **how to convert Word [DOC][8] or **[DOCX][9]** files to [PNG][10], [JPEG][11], [BMP][12], [GIF][13], or [TIFF][14] images in Java**. Furthermore, we will cover how to customize the Word to image conversion using different options.

*   [Java API for Word to Image Conversion][15]
*   [Convert a Word Document to Image Format][16]
*   [Customize Word to Image Conversion][17]

## Java API for Word DOC to Image Conversion {#API-for-Word-to-Image-Conversion}

[Aspose.Words for Java][18] is a feature-rich API to create, edit, or convert MS Word documents in Java-based applications. We will use this API to convert Word documents to image formats. You can [download][19] the API’s JAR or install it using the following Maven configurations:

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

## Java Convert a Word DOC to PNG, JPEG, BMP, GIF, or TIFF {#Convert-a-Word-Document-to-PNG-JPEG-or-BMP}

You can convert a Word document into PNG, JPEG, BMP, GIF, or TIFF images depending upon your requirement. To set the output image format, **[SaveFormat][20]** enum is used. For demonstration, let's convert a Word DOCX file to PNG images in Java.

*   Load the Word document using the **[Document][21]**  class.
*   Create an instance of **[ImageSaveOptions][22]** class and specify the output image format.
*   Loop through the pages in the document.
*   Convert each page in Word document to an image using **[Document.save(string, ImageSaveOptions)][23]** method.

The following code sample shows how to convert a Word DOCX to PNG images in Java.

{{< gist aspose-com-gists 508219459d9ad52444ea2b99e45a7d0b "word-to-image.java" >}}

## Customize DOC/DOCX to Image Conversion in Java {#Control-Word-to-Image-Conversion}

You can also customize the Word to image conversion using different options. For example, you can set horizontal resolution, vertical resolution, overall resolution, scale, pixel format, brightness, color mode, contrast, etc. The following are the steps to customize Word to image conversion in Java.

*   Load the Word document using the ****[Document][24]**** class.
*   Create an instance of **[ImageSaveOptions][25]** class and specify the output image format.
*   Set desired options such as brightness, contrast, etc. using the **ImageSaveOptions** object.
*   Loop through the pages in the document.
*   Convert each page to image using **[Document.save(string, ImageSaveOptions)][26]** method.

The following code sample shows how to customize Word to JPEG image conversion using different options.

{{< gist aspose-com-gists 508219459d9ad52444ea2b99e45a7d0b "word-to-image-custom.java" >}}

## Get a Free API License {#Get-a-Free-API-License}

You can [get a temporary license][27] in order to use Aspose.Words for Java without evaluation limitations.

## Conclusion

In this article, you have learned how to convert Word documents to PNG, JPEG, BMP, GIF, or TIFF images in Java. Furthermore, you have seen how to customize Word to image conversion using different options. Apart from that, you can explore other features of Aspose.Words for Java using the [documentation][28]. Also, you can post your questions on our [forum][29].

## See Also

*   [Create MS Word Document in C#][30]
*   [Create Rich Word Documents in Java][31]




[1]: https://docs.fileformat.com/word-processing/doc/
[2]: https://docs.fileformat.com/word-processing/docx/
[3]: https://docs.fileformat.com/image/png/
[4]: https://docs.fileformat.com/image/jpeg/
[5]: https://docs.fileformat.com/image/bmp/
[6]: https://docs.fileformat.com/image/gif/
[7]: https://docs.fileformat.com/image/tiff/
[8]: https://docs.fileformat.com/word-processing/doc/
[9]: https://docs.fileformat.com/word-processing/docx/
[10]: https://docs.fileformat.com/image/png/
[11]: https://docs.fileformat.com/image/jpeg/
[12]: https://docs.fileformat.com/image/bmp/
[13]: https://docs.fileformat.com/image/gif/
[14]: https://docs.fileformat.com/image/tiff/
[15]: #API-for-Word-to-Image-Conversion
[16]: #Convert-a-Word-Document-to-PNG-JPEG-or-BMP
[17]: #Control-Word-to-Image-Conversion
[18]: https://products.aspose.com/words/java/
[19]: https://downloads.aspose.com/words/java
[20]: https://apireference.aspose.com/words/java/com.aspose.words/SaveFormat
[21]: https://apireference.aspose.com/words/java/com.aspose.words/Document
[22]: https://apireference.aspose.com/words/java/com.aspose.words/ImageSaveOptions
[23]: https://apireference.aspose.com/words/java/com.aspose.words/document#save(java.lang.String,com.aspose.words.SaveOptions)
[24]: https://apireference.aspose.com/words/java/com.aspose.words/Document
[25]: https://apireference.aspose.com/words/java/com.aspose.words/ImageSaveOptions
[26]: https://apireference.aspose.com/words/java/com.aspose.words/document#save(java.lang.String,com.aspose.words.SaveOptions)
[27]: https://purchase.aspose.com/temporary-license
[28]: https://docs.aspose.com/words/java/
[29]: https://forum.aspose.com/
[30]: https://blog.aspose.com/2020/01/08/csharp-word-automation-create-edit-process-word-documents/
[31]: https://blog.aspose.com/2020/03/11/create-rich-word-documents-programmatically-in-java-using-java-word-api/





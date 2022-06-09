---
title: 'Add Watermark to Word Documents using Java'
seoTitle: "Java: Add Watermark to Word Documents | Add Text or Image Watermark"
description: "Use Java Word Processing API to add watermark to MS Word documents in Java. Add text or image watermarks to the documents seamlessly."
date: Mon, 19 Jul 2021 10:47:22 +0000
draft: false
url: /2021/07/19/add-watermark-to-word-documents-using-java/
author: Usman Aziz
summary: "Watermarks are added to the Word documents for various purposes such as preventing illegal usage, defining the ownership, displaying the document's status, etc. In this article, you will learn **how to add a watermark to Word documents using Java**. The article will demonstrate the insertion of text and image watermarks into a Word document separately."
tags: ['Add Image Watermark to a Word Document Java', 'Add Text Watermark to a Word Document Java', 'Java API to Add Watermark in Word Documents']
categories: ['Aspose.Words Product Family']
---



{{< figure align=center src="images/Add-Watermark-to-Word-DOCX.jpg" alt="Add Watermark to Word DOCX Java">}}


[Watermarks][1] are added to the Word documents for various purposes such as preventing illegal usage, defining the ownership, displaying the document's status, etc. In this article, you will learn **how to add a watermark to Word documents using Java**. The article will demonstrate the insertion of text and image watermarks into a Word document separately.

*   [Java API to Add Watermark in Word Documents][2]
*   [Add Text Watermark to a Word Document][3]
*   [Add Image Watermark to a Word Document][4]

## Java API to Add Watermark in Word Documents {#Java-API-to-Add-Watermark-in-Word-Documents}

In order to add watermarks to the Word documents, we will use [Aspose.Words for Java][5]. It is a feature-rich API that lets you create word processing documents from scratch. Also, it allows you to manipulate the existing Word documents quite easily. You can either [download][6] the API or install it using the following Maven configurations.

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
    <artifactId>aspose-words</artifactId>
    <version>21.7</version>
    <type>pom</type>
</dependency>
```

## Add Text Watermark to a Word Document in Java {#Add-Text-Watermark-to-a-Word-Document-Java}

The following are the steps to insert a text watermark into a Word document using Java.

*   First, load the Word document using [Document][7] class.
*   Create an instance of [TextWatermarkOptions][8] class to set watermark options such as font family, font size, color, layout, etc.
*   Add text watermark to the document using [Document.getWatermark().setText(String, TextWatermarkOptions)][9] method.
*   Finally, save the updated Word document using [Document.save(String)][10] method.

The following code sample shows how to add a text watermark to a Word document.

{{< gist aspose-com-gists 9c2cf3f92d75b861f1d1c51de1d791c5 "add-text-watermark-to-Word.java" >}}

The following is the screenshot of a Word document after adding the text watermark.



{{< figure align=center src="images/Add-Text-Watermark-to-Word.jpg" alt="Add text watermark to Word in Java">}}


## Add Image Watermark to a Word Document {#Add-Image-Watermark-to-a-Word-Document}

The following are the steps to add an image watermark to a Word document using Java.

*   First, load the Word document using [Document][11] class.
*   Create an instance of [ImageWatermarkOptions][12] class to set watermark options.
*   Load the watermark image into a [BufferedImage][13] object.
*   Add image watermark to the document using [Document.getWatermark().setImage(BufferedImage, ImageWatermarkOptions)][14] method.
*   Finally, save the updated Word document using [Document.save(String)][15] method.

The following code sample shows how to add an image watermark to the Word document.

{{< gist aspose-com-gists 9c2cf3f92d75b861f1d1c51de1d791c5 "add-image-watermark-to-Word.java" >}}

The following is the screenshot of a Word document after adding the image watermark.



{{< figure align=center src="images/Add-Image-Watermark-to-Word.jpg" alt="Add image watermark to Word in Java">}}


## Get a Free API License {#Get-a-Free-API-License}

You can [get a temporary license][16] in order to use the API without evaluation limitations.

## Conclusion

In this article, you have learned how to add a watermark to Word documents using Java. The steps and code samples have demonstrated how to insert a text or image watermark into a Word document. You can learn more about the Java word processing API using the [documentation][17]. In case you would have any questions, feel free to let us know via our [forum][18].

## See Also

*   [Create MS Word Documents using Java without MS Office][19]
*   [Mail Merge in MS Word Documents using Java][20]




[1]: https://en.wikipedia.org/wiki/Watermark#:~:text=A%20watermark%20is%20an%20identifying,density%20variations%20in%20the%20paper.
[2]: #Java-API-to-Add-Watermark-in-Word-Documents
[3]: #Add-Text-Watermark-to-a-Word-Document-Java
[4]: #Add-Image-Watermark-to-a-Word-Document
[5]: https://products.aspose.com/words/java
[6]: https://downloads.aspose.com/words/java
[7]: https://apireference.aspose.com/words/java/com.aspose.words/Document
[8]: https://apireference.aspose.com/words/java/com.aspose.words/TextWatermarkOptions
[9]: https://apireference.aspose.com/words/java/com.aspose.words/watermark#setText(java.lang.String,com.aspose.words.TextWatermarkOptions)
[10]: https://apireference.aspose.com/words/java/com.aspose.words/document#save(java.lang.String)
[11]: https://apireference.aspose.com/words/java/com.aspose.words/Document
[12]: https://apireference.aspose.com/words/java/com.aspose.words/ImageWatermarkOptions
[13]: https://docs.oracle.com/javase/7/docs/api/java/awt/image/BufferedImage.html
[14]: https://apireference.aspose.com/words/java/com.aspose.words/watermark#setImage(java.awt.image.BufferedImage,com.aspose.words.ImageWatermarkOptions)
[15]: https://apireference.aspose.com/words/java/com.aspose.words/document#save(java.lang.String)
[16]: https://purchase.aspose.com/temporary-license
[17]: https://docs.aspose.com/words/java
[18]: https://forum.aspose.com/
[19]: https://blog.aspose.com/2020/03/11/create-rich-word-documents-programmatically-in-java-using-java-word-api/
[20]: https://blog.aspose.com/2020/12/11/mail-merge-in-word-documents-using-java/






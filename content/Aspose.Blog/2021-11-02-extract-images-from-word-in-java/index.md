---
title: 'Extract Images from Word Documents in Java'
seoTitle: "Extract Images in Word Documents in Java | Image Extractor for DOCX"
description: "Use Java Word API to extract images from Word documents using Java. Extract images from DOCX or DOC files and save them to the desired location."
date: Tue, 02 Nov 2021 14:12:00 +0000
draft: false
url: /2021/11/02/extract-images-from-word-in-java/
author: Usman Aziz
summary: 'Images are commonly used to represent important information in Word documents. The inclusion of images alongside text makes the content more appealing. In certain cases, you may need to extract the images embedded within the Word documents programmatically. To achieve that, this article covers **how to extract images from Word documents using Java**.'
tags: ['Java images extractor for Word', 'extract images from Word document in Java', 'extract images from doc in Java', 'extract images from docx in Java']
categories: ['Aspose.Words Product Family']
---



{{< figure align=center src="images/Extract-Images-from-Word-Document.jpg" alt="Extract images from word documents using Java">}}


Images are commonly used to represent important information in Word documents. The inclusion of images alongside text makes the content more appealing. In certain cases, you may need to extract the images embedded within the Word documents programmatically. To achieve that, this article covers **how to extract images from Word documents using Java**.

*   [API to Extract Images from Word Documents][1]
*   [Extract Images from a Word Document][2]

## Java API to Extract Images from Word Documents {#API-to-Extract-Images-from-Word-Documents}

[Aspose.Words for Java][3] is a powerful and feature-rich API for creating, manipulating, and converting MS Word documents. Therefore, we will use this API to extract images from MS Word DOCX/DOC documents. You can [download][4] the API's JAR or install it into your Java application using the following Maven configurations.

```
<repository>
    <id>AsposeJavaAPI</id>
    <name>Aspose Java API</name>
    <url>https://repository.aspose.com/repo/</url>
</repository>
<dependency>
    <groupId>com.aspose</groupId>
    <artifactId>aspose-words</artifactId>
    <version>21.11</version>
    <type>pom</type>
</dependency>
```

## How to Extract Images from a Word Document {#Extract-Images-from-a-Word-Document}

The images in a Word document are represented using shape objects. Therefore, to retrieve images, you will have to process every shape in the document. The following are the steps to extract images from a Word DOCX document in Java.

*   First, load the Word file using [Document][5] class.
*   Then, get all the shapes into an [NodeCollection<Shape>][6] object using [Document.getChildNodes(NodeType.SHAPE, Boolean)][7] method.
*   Loop through the retreieved shapes.
*   In each iteration, check if the shape has an image using [Shape.hasImage()][8] method.
*   Finaly, extract the image and save it using [Shape.getImageData().save(string)][9] method.

The following code sample shows how to extract images from a DOCX document in Java.

{{< gist aspose-com-gists 7af5b641d0ab658dbddce3292649c227 "extract-images-from-word.java" >}}

## Get a Free API License

[Get a free temporary license][10] to use Aspose.Words for Java without evaluation limitations.

**Info**: You may be interested in another Java API ([Aspose.Slides for Java][11] that allows you to convert presentations (into PDFs, [word documents][12], etc.) and [import images][13] or other documents into presentations.

## Conclusion

In this article, you have learned how to extract images from a Word document using Java. Moreover, the code sample has shown how to extract the images from a DOCX file and save them to the desired location. Besides, Aspose.Words for Java provides a wide range of features for document manipulation. To explore those features, you can visit the [documentation][14]. Also, you can ask your questions via our [forum][15].

## See Also

*   [Create Word Documents from Scratch in Java][16]
*   [Generate Word Documents from Templates in Java][17]
*   [Convert Word Files to PDF in Java][18]




[1]: #API-to-Extract-Images-from-Word-Documents
[2]: #Extract-Images-from-a-Word-Document
[3]: https://products.aspose.com/words/java/
[4]: https://downloads.aspose.com/words/java/
[5]: https://apireference.aspose.com/words/java/com.aspose.words/Document
[6]: https://apireference.aspose.com/words/java/com.aspose.words/NodeCollection
[7]: https://apireference.aspose.com/words/java/com.aspose.words/document#ChildNodes
[8]: https://apireference.aspose.com/words/java/com.aspose.words/shape#HasImage
[9]: https://apireference.aspose.com/words/java/com.aspose.words/imagedata#save(java.lang.String)
[10]: https://purchase.aspose.com/temporary-license
[11]: https://products.aspose.com/slides/java/)
[12]: https://products.aspose.app/slides/conversion/ppt-to-word
[13]: https://products.aspose.app/slides/import/jpg-to-ppt
[14]: https://docs.aspose.com/words/java/
[15]: https://forum.aspose.com/
[16]: https://blog.aspose.com/2020/03/11/create-rich-word-documents-programmatically-in-java-using-java-word-api/
[17]: https://blog.aspose.com/2020/01/14/generate-word-documents-from-templates-dynamically-using-java/
[18]: https://blog.aspose.com/2020/02/20/convert-word-doc-docx-to-pdf-in-java-programmatically/





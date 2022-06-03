---
title: 'Extract Text or Images from OneNote Documents using Java'
date: Fri, 25 Mar 2022 09:49:20 +0000
draft: false
url: /2022/03/25/extract-text-or-images-from-onenote-documents-using-java/
author: ''Muzammil Khan''
summary: 'As a Java developer, you can easily extract text or images from OneNote documents programmatically without using MS OneNote. In this article, you will learn **how to extract text and images from OneNote documents using Java**.'
tags: ['Extract Image', 'Extract Images from OneNote Java', 'Extract Text', 'Extract Text from OneNote Java', 'Text and Image Extractor Java API']
categories: ['Aspose.Note Product Family']
---



{{< figure align=center src="images/extract-text-or-images-from-onenote-documents-using-java.jpg" alt="Extract Text or Images from OneNote Documents using Java">}}


We can collect and organize notes in the form of text, drawings, screen clippings, and audio commentaries in the OneNote document. We may occasionally need to extract text or images from OneNote documents programmatically in Java applications. Such extraction allows us to reuse the extracted text or images separately. In this article, we will learn **how to extract text or images from OneNote documents using Java**.

The following topics shall be covered in this article:

*   [Java API to Extract Text or Images from OneNote][1]
*   [Extract All the Text from OneNote using Java][2]
*   [Get Text from Specific Pages of OneNote in Java][3]
*   [Extract Images from OneNote using Java][4]

## Java API to Extract Text or Images from OneNote {#Java-API-to-Extract-Text-and-Images-from-OneNote}

For extracting text and images from the [OneNote][5] document, we will be using the [Aspose.Note for Java][6] API. It allows creating, reading, and converting OneNote documents programmatically without using MS OneNote. Please either [download][7] the JAR of the API or add the following **_pom.xml_** configuration in a Maven-based Java application.

```
<repository>
    <id>AsposeJavaAPI</id>
    <name>Aspose Java API</name>
    <url>http://repository.aspose.com/repo/</url>
</repository>
```
```
<dependency>
    <groupId>com.aspose</groupId>
    <artifactId>aspose-note</artifactId>
    <version>22.1</version>
    <classifier>jdk17</classifier>
</dependency>
```

## Extract All the Text from OneNote Document using Java {#Extract-All-the-Text-from-OneNote-Document-using-Java}

We can easily extract all the text from the OneNote document by following the steps given below:

1.  Firstly, load a OneNote file using the **_[Document][8]_** class.
2.  After that, call the **_[GetChildNodes][9]_** method with **_[RichText.class][10]_** as an argument to extract text.
3.  Finally, show the extracted text.

The following code sample shows **how to extract all the text from a OneNote file using Java**.

{{< gist aspose-com-gists 7c46c61f771888e8969767564d380fe7 "ExtractTextOrImagesFromOneNote_Java_ExtractText.java" >}}



{{< figure align=center src="images/Extract-All-the-Text-from-OneNote-Document-using-Java-1024x512.jpg" alt="Extract All the Text from OneNote Document using Java" caption="Extract All the Text from OneNote Document using Java">}}


## Get Text from Specific Pages of OneNote Document in Java {#Get-Text-from-Specific-Pages-of-OneNote-Document-in-Java}

We can extract text from specific pages of the OneNote document by following the steps given below:

1.  Firstly, load a OneNote file using the **_[Document][11]_** class.
2.  Next, call the **_[GetChildNodes][12]_** method with **_[Page.class][13]_** as an argument to extract pages.
3.  Then, get a specific page by its index from list of pages.
4.  After that, get a list of text items for the page using the **_[GetChildNodes][14]_** method with **_[RichText.class][15]_** as an argument.
5.  Finally, show the extracted text.

The following code sample shows **how to extract text from a specific page of a OneNote file using Java**.

{{< gist aspose-com-gists 7c46c61f771888e8969767564d380fe7 "ExtractTextOrImagesFromOneNote_Java_ExtractSpecificPageText.java" >}}



{{< figure align=center src="images/Get-Text-from-a-Specific-Page-of-OneNote-Document-in-Java-1-1024x512.jpg" alt="" caption="Extract Text from a Specific Page of OneNote Document in Java">}}


We may iterate over all the pages one by one and extract the text for each page as shown in the code sample given below:

{{< gist aspose-com-gists 7c46c61f771888e8969767564d380fe7 "ExtractTextOrImagesFromOneNote_Java_ExtractPagesText.java" >}}



{{< figure align=center src="images/Get-Text-from-Specific-Pages-of-OneNote-Document-in-Java-1024x512.jpg" alt="Get Text from Specific Pages of OneNote Document in Java" caption="Get Text from all the Pages one by one in Java">}}


## Extract Images from OneNote Document using Java {#Extract-Images-from-OneNote-Document-using-Java}

We can also extract images from the OneNote document by following the steps given below:

1.  Firstly, load a OneNote file using the **_[Document][16]_** class.
2.  After that, get a list of images using the **_[GetChildNodes][17]_** method with the _**[Image.class][18]**_ as an argument.
3.  Finally, show the image properties and save to local disk.

The following code sample shows **how to extract images from a OneNote file using Java**.

{{< gist aspose-com-gists 7c46c61f771888e8969767564d380fe7 "ExtractTextOrImagesFromOneNote_Java_ExtractImages.java" >}}



{{< figure align=center src="images/Extract-Images-from-OneNote-Document-using-Java-1024x535.jpg" alt="Extract Images from OneNote Document using Java" caption="Extract Images from OneNote Document using Java">}}


## Get a Free License {#Get-a-Free-API-License}

You can [get a free temporary license][19] to try the library without evaluation limitations.

## Conclusion

In this article, we have learned **how to extract text from the whole OneNote document or from a specific page** of the document. We have also seen **how to extract images from OneNote documents** programmatically. Besides, you can learn more about Aspose.Note for Java API using the [documentation][20]. In case of any ambiguity, please feel free to contact us on the [forum][21].

## See Also

*   [Insert or Extract an Image from a OneNote file Programmatically in Java][22]




[1]: #Java-API-to-Extract-Text-and-Images-from-OneNote
[2]: #Extract-All-the-Text-from-OneNote-Document-using-Java
[3]: #Get-Text-from-Specific-Pages-of-OneNote-Document-in-Java
[4]: #Extract-Images-from-OneNote-Document-using-Java
[5]: https://docs.fileformat.com/note-taking/one/
[6]: https://products.aspose.com/note/java
[7]: https://downloads.aspose.com/note/java
[8]: https://apireference.aspose.com/note/java/com.aspose.note/Document
[9]: https://apireference.aspose.com/note/java/com.aspose.note/CompositeNode#getChildNodes-java.lang.Class-
[10]: https://apireference.aspose.com/note/java/com.aspose.note/RichText
[11]: https://apireference.aspose.com/note/java/com.aspose.note/Document
[12]: https://apireference.aspose.com/note/java/com.aspose.note/CompositeNode#getChildNodes-java.lang.Class-
[13]: https://apireference.aspose.com/note/java/com.aspose.note/Page
[14]: https://apireference.aspose.com/note/java/com.aspose.note/CompositeNode#getChildNodes-java.lang.Class-
[15]: https://apireference.aspose.com/note/java/com.aspose.note/RichText
[16]: https://apireference.aspose.com/note/java/com.aspose.note/Document
[17]: https://apireference.aspose.com/note/java/com.aspose.note/CompositeNode#getChildNodes-java.lang.Class-
[18]: https://apireference.aspose.com/note/java/com.aspose.note/Image
[19]: https://purchase.aspose.com/temporary-license
[20]: https://docs.aspose.com/note/java/
[21]: https://forum.aspose.com/c/note/28
[22]: https://blog.aspose.com/2021/11/07/insert-extract-image-onenote-java/





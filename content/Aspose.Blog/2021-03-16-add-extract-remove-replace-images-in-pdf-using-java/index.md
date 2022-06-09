---
title: 'Add, Extract, Remove or Replace Images in PDF Files using Java'
seoTitle: "Java: Add, Remove, and Replace Images in PDF | Extract Images in PDF"
description: "Use Aspose.PDF for Java to manipulate images in PDF. Extract, add, remove, and replace images in a PDF file programmatically using Java"
date: Tue, 16 Mar 2021 20:14:00 +0000
draft: false
url: /2021/03/16/add-extract-remove-replace-images-in-pdf-using-java/
author: Usman Aziz
summary: 'Images are widely used for different types of depictions and demonstrations in PDF files. In this article, you will learn how to manipulate images in PDF files programmatically. Particularly, the article will cover **how to add, extract, remove or replace images in PDF files using Java**.'
tags: ['Add an Image in a PDF using Java', 'Extract Images from a PDF using Java', 'Java API to Manipulate Images in PDF', 'Remove Images from a PDF using Java', 'Replace an Image in a PDF using Java']
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/Work-with-Images-in-PDF.png.jpg" alt="Work with PDF Images using Java">}}


Images are widely used for different types of depictions and demonstrations in [PDF][1] files. In this article, you will learn how to manipulate images in PDF files programmatically. Particularly, the article will cover **how to add, extract, remove or replace images in PDF files using [Java][2]**.

*   [Java API to Manipulate Images in PDF][3]
*   [Add an Image in a PDF using Java][4]
*   [Extract an Image from a PDF using Java][5]
*   [Remove Images from a PDF using Java][6]
*   [Replace an Image in a PDF using Java][7]
*   [Get a Free License][8]

## Java API to Manipulate Images in PDF Files {#Java-API-to-Manipulate-Images-in-PDF}

[Aspose.PDF for Java][9] is a powerful API that provides you with a wide range of PDF manipulation features. The API lets you work with text, annotations, or images in the PDF files seamlessly. You can either [download][10] the API's JAR or install it using the following Maven configurations.

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
    <artifactId>aspose-pdf</artifactId>
    <version>21.2</version>
</dependency>
```

## Add an Image in a PDF File using Java {#Java-API-to-Manipulate-Images-in-PDF}

The following are the steps to add an image in the PDF file using Java.

*   First, create an instance of the [Document][11] class to load the PDF document.
*   Get the [Page][12] you want to add an image to using [Document.getPages().get\_Item(int)][13] method.
*   Load the image file into a [FileInputStream][14] object.
*   Add the image into the page’s resources using [Page.getResources().getImages().add(FileInputStream)][15] method.
*   Use operators to place the image on the page:
    1.  [GSave][16] operator to save the current graphical state.
    2.  [ConcatenateMatrix][17] operator to specify where the image is to be placed.
    3.  [Do][18] operator to draw the image on the page.
    4.  [GRestore][19] operator to save the updated graphical state.
*   Finally, save the updated PDF file using [Document.save(string)][20] method.

The following code sample shows how to add image to a PDF file using Java.

{{< gist aspose-com-gists d2fe397171126d9c62830f5acdd342eb "add-image-to-pdf.java" >}}

## Extract Images from a PDF File using Java {#Extract-Images-from-a-PDF-using-Java}

The following are the steps to extract images from a PDF document using Java.

*   Create an instance of the [Document][21] class to load the PDF document.
*   Extract desired image into [XImage][22] object using [Document.getPages().get\_Item(int).getResources().getImages().get\_Item(int)][23] method.
*   You can also loop through the image collection to extract and save all the images.
*   Finally, save the extracted image as a file using [OutputStream][24].

The following code sample shows how to extract images from PDF files using Java.

{{< gist aspose-com-gists d2fe397171126d9c62830f5acdd342eb "extract-image-from-pdf.java" >}}

## Remove Images from a PDF File using Java {#Remove-Images-from-a-PDF-using-Java}

The following are the steps to remove an image from a PDF file using Java.

*   Load the PDF file into a [Document][25] object.
*   Delete the desired image(s) using one of the following methods.
    *   [delete()][26] to delete images from collection.
    *   [delete(int index)][27] to delete an image from the collection by index.
    *   [delete(String name)][28] to delete an image from the collection by name.
*   Finally, save the updated PDF file using the [Document.save(string)][29] method.

The following code sample shows how to delete an image in PDF using Java.

{{< gist aspose-com-gists d2fe397171126d9c62830f5acdd342eb "remove-image-from-pdf.java" >}}

## Replace an Image in a PDF File using Java {#Replace-an-Image-in-a-PDF-using-Java}

The following are the steps to replace an image in a PDF file using Java.

*   Load the PDF file into a [Document][30] object.
*   Load the new image into [FileInputStream][31] object.
*   Use [Document.getPages().get\_Item(int).getResources().getImages().replace(int, FileInputStream)][32] method to replace the image by specifying the index.
*   Finally, save the updated PDF file using the [Document.save(string)][33] method.

The following code sample shows how to replace an image in PDF using Java.

{{< gist aspose-com-gists d2fe397171126d9c62830f5acdd342eb "replace-image-in-pdf.java" >}}

## Get a Free API License {#Get-a-Free-License}

You can try Aspose.PDF for Java for free by [getting a temporary license][34].

## Conclusion

In this article, you have learned how to manipulate images in PDF files using Java. The step-by-step guide and code samples have shown how to extract, add, remove, and replace images in a PDF file. You can explore other features of Aspose.PDF for Java using [documentation][35]. In case of any queries, you can contact us via our [forum][36].

## See Also

*   [Generate PDF File from Images using Java][37]




[1]: https://docs.fileformat.com/pdf/
[2]: https://docs.fileformat.com/programming/java/
[3]: #Java-API-to-Manipulate-Images-in-PDF
[4]: #Java-API-to-Manipulate-Images-in-PDF
[5]: #Extract-Images-from-a-PDF-using-Java
[6]: #Remove-Images-from-a-PDF-using-Java
[7]: #Replace-an-Image-in-a-PDF-using-Java
[8]: #Get-a-Free-License
[9]: https://products.aspose.com/pdf/java
[10]: https://downloads.aspose.com/pdf/java
[11]: https://apireference.aspose.com/java/pdf/com.aspose.pdf/Document
[12]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/Page
[13]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/PageCollection#get_Item-int-
[14]: https://www.javatpoint.com/java-fileinputstream-class
[15]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/XImageCollection#add-java.io.InputStream-
[16]: https://apireference.aspose.com/pdf/java/com.aspose.pdf.operators/GSave
[17]: https://apireference.aspose.com/pdf/java/com.aspose.pdf.operators/ConcatenateMatrix
[18]: https://apireference.aspose.com/pdf/java/com.aspose.pdf.operators/Do
[19]: https://apireference.aspose.com/pdf/java/com.aspose.pdf.operators/GRestore
[20]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/Document#save-java.lang.String-
[21]: https://apireference.aspose.com/java/pdf/com.aspose.pdf/Document
[22]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/XImage
[23]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/XImageCollection#get_Item-int-
[24]: https://docs.oracle.com/javase/7/docs/api/java/io/OutputStream.html
[25]: https://apireference.aspose.com/java/pdf/com.aspose.pdf/Document
[26]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/XImageCollection#delete--
[27]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/XImageCollection#delete-int-
[28]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/XImageCollection#delete-java.lang.String-
[29]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/Document#save-java.lang.String-
[30]: https://apireference.aspose.com/java/pdf/com.aspose.pdf/Document
[31]: https://www.javatpoint.com/java-fileinputstream-class
[32]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/XImageCollection#replace-int-java.io.InputStream-
[33]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/Document#save-java.lang.String-
[34]: https://purchase.aspose.com/temporary-license
[35]: https://docs.aspose.com/pdf/java/getting-started/
[36]: https://forum.aspose.com/
[37]: https://blog.aspose.com/2021/03/01/generate-pdf-file-from-images-using-java/






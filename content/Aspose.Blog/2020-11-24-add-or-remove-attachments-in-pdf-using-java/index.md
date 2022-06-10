---
title: 'Add or Remove Attachments in PDF using Java'
seoTitle: "Add or Remove Attachments in PDF in Java | Get PDF Attachment Info"
description: "Use Java PDF API to add or remove attachments from PDF in Java. Get attachment information and remove one or all attachments in PDF using Java PDF API."
date: Tue, 24 Nov 2020 01:49:51 +0000
draft: false
url: /2020/11/24/add-or-remove-attachments-in-pdf-using-java/
author: Usman Aziz
summary: '[PDF][1] is one of the ruling file formats in the world of digital documents. Along with other popular features, PDF format also allows you to embed files as attachments within a PDF file. These attachments are similar to ones you add to an email message. In order to automate PDF attachment manipulation, this article provides you some simple ways of **adding and removing attachments in PDF files using Java**.'
tags: ['add attachment in pdf java', 'get pdf attachment info in java', 'remove attachment from pdf java']
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/add-remove-attachments-in-pdf-using-java.jpg" alt="add or remove pdf attachments in java">}}


[PDF][2] is one of the ruling file formats in the world of digital documents. Along with other popular features, PDF format also allows you to embed files as attachments within a PDF file. These attachments are similar to ones you add to an email message. In order to automate PDF attachment manipulation, this article provides you some simple ways to **add and remove attachments in PDF files using Java**.

*   [Java API for PDF Attachments – Free Download][3]
*   [Extract PDF Attachment Information using Java][4]
*   [Add an Attachment to PDF in Java][5]
*   [Remove Attachments from PDF in Java][6]

## Java API for PDF Attachments – Free Download {#Java-API-for-PDF-Attachments-Free-Download}

[Aspose.PDF for Java][7] is PDF file manipulation API that lets you create, edit, and manipulate PDF documents from within your Java applications. In addition, it provides easy to use methods to add and remove attachments in the PDF files. You can either [download][8] API's JAR or install it within your Maven-based applications using the following configurations.

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
    <version>20.10</version>
    <classifier>jdk17</classifier>
</dependency>
```

## Extract PDF Attachment Information using Java {#Get-PDF-Attachment-Information-using-Java}

First of all, let's check out how to retrieve information about the attachments in a PDF file. The information contains the attachment's name, description, MIME type, and other parameters such as the checksum, modified date, etc. The following are the steps to get information about an attachment in a PDF file.

*   Load the PDF file using [Document][9] class.
*   Use [FileSpecification][10] class to retrieve the PDF attachment using [Document.getEmbeddedFiles().get\_Item(int)][11] method.
*   Retrieve the attachment's information using the _FileSpecification_ object.

The following code sample shows how to get information of a PDF attachment using Java.

{{< gist aspose-pdf 474c352a71ac9477aa0d604fd32e1c6a "Examples-src-main-java-com-aspose-pdf-examples-NewDocumentObject-attachments-GetAttachmentInformation-.java" >}}

## Add an Attachment to PDF in Java {#Add-an-Attachment-to-PDF-in-Java}

The following are the steps to add an attachment to a PDF document.

*   Load the PDF file using [Document][12] class.
*   Create an object of [FileSpecification][13] class to load the attachment file.
*   Add attachment using [Document.getEmbeddedFiles().add(FileSpecificatio)][14] method.
*   Save the PDF file using the [Document.save(String)][15] method.

The following code sample shows how to add an attachment to a PDF using Java.

{{< gist aspose-pdf 474c352a71ac9477aa0d604fd32e1c6a "Examples-src-main-java-com-aspose-pdf-examples-NewDocumentObject-attachments-AddAttachmentToPDF-.java" >}}

## Remove Attachments from PDF in Java {#Remove-an-Attachment-from-PDF-in-Java}

You can either delete a particular attachment using its name or delete all attachments at once. The following are the steps to remove attachments from the PDF document.

*   Load the PDF file using [Document][16] class.
*   Use [Document.getEmbeddedFiles().delete()][17] and [Document.getEmbeddedFiles().delete(String)][18] to delete all or specific attachment respectively.
*   Save the PDF file using the [Document.save(String)][19] method.

The following code sample shows how to remove PDF attachments using Java.

{{< gist aspose-pdf 474c352a71ac9477aa0d604fd32e1c6a "Examples-src-main-java-com-aspose-pdf-examples-NewDocumentObject-attachments-DeleteAllAttachmentsFromPDF-.java" >}}

## Conclusion

In this article, you have learned how to work with attachments in PDF files using Java. The step-by-step guide and code samples have shown how to add and remove attachments from PDF programmatically using Java. You can explore more about Aspose.PDF for Java using [documentation][20].

## See Also

*   [Convert PDF to SVG Format using Java][21]




[1]: https://docs.fileformat.com/pdf/
[2]: https://docs.fileformat.com/pdf/
[3]: #Java-API-for-PDF-Attachments-Free-Download
[4]: #Get-PDF-Attachment-Information-using-Java
[5]: #Add-an-Attachment-to-PDF-in-Java
[6]: #Remove-an-Attachment-from-PDF-in-Java
[7]: https://products.aspose.com/pdf/java
[8]: https://downloads.aspose.com/pdf/java
[9]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/Document
[10]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/FileSpecification
[11]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/EmbeddedFileCollection#get_Item-int-
[12]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/Document
[13]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/FileSpecification
[14]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/EmbeddedFileCollection#add-com.aspose.pdf.FileSpecification-
[15]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/Document#save-java.lang.String-
[16]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/Document
[17]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/EmbeddedFileCollection#delete--
[18]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/EmbeddedFileCollection#delete-java.lang.String-
[19]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/Document#save-java.lang.String-
[20]: https://docs.aspose.com/pdf/java/getting-started/
[21]: https://blog.aspose.com/2020/11/04/convert-pdf-to-svg-using-java/






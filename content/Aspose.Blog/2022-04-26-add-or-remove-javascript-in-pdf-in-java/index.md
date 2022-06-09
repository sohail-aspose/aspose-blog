---
title: 'Add or Remove JavaScript in PDF Files in Java'
seoTitle: "Add JavaScript to PDF in Java | Java PDF Generator Library"
description: "Use Java PDF API to add JavaScript to PDF files in Java. Add page level or document level JavaScript in PDF. Remove JavaScript from PDF programmatically."
date: Tue, 26 Apr 2022 23:07:00 +0000
draft: false
url: /2022/04/26/add-or-remove-javascript-in-pdf-in-java/
author: Usman Aziz
summary: '[PDF][1] is one of the widely used document formats because of its consistent layout across heterogeneous platforms. Furthermore, it can be displayed in desktop-based software applications as well as the web browsers at the same time. The support of web browsers make PDF files capable of running JavaScript. In this article, you will learn **how to add or remove JavaScript in PDF files programmatically in Java**.'
tags: ['Add Document Level JavaScript in PDF in Java', 'Add JavaScript to PDF Files in Java', 'Java API to Add or Remove JavaScript in PDF', 'Java PDF Generator API', 'Remove JavaScript from PDF in Java']
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/Add-JavaScript-to-PDF.png" alt="Add JavaScript to PDF Files in Java">}}


[PDF][2] is one of the widely used document formats because of its consistent layout across heterogeneous platforms. Furthermore, it can be displayed in desktop-based software applications as well as the web browsers at the same time. The support of web browsers make PDF files capable of running JavaScript. In this article, you will learn **how to add or remove JavaScript in PDF files programmatically in Java**.

*   [Java API to Add or Remove JavaScript in PDF][3]
*   [Add JavaScript to PDF Files][4]
*   [Add Document Level JavaScript in a PDF File][5]
*   [Remove JavaScript from a PDF File][6]

## Java API to Add or Remove JavaScript in PDF Files {#API-to-Work-with-JavaScript-in-PDF}

[Aspose.PDF for Java][7] is an amazing API that provides a range of features for PDF generation and manipulation. With this API, you can seamlessly create new and manipulate the existing PDF files. We will use this API to add and remove JavaScript in PDF files. You can [download][8] the API or install it using the following Maven configurations.

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
    <artifactId>aspose-pdf</artifactId>
    <version>22.4</version>
</dependency>
```

## Add JavaScript to PDF Files in Java {#Add-JavaScript-to-PDF-Files}

PDF files support Acrobat JavaScript, which is based on the core of JavaScript version 1.5 of ISO-16262, formerly known as ECMAScript. It is an object-oriented scripting language developed by Netscape Communications. Before proceeding to add JavaScript to PDF files, let's have a look at the differences between Acrobat JavaScript and HTML JavaScript which is used in web browsers.

*   Acrobat JavaScript does not have access to objects within an HTML page. Similarly, HTML JavaScript cannot access objects within a PDF file.
*   HTML JavaScript is able to manipulate objects such as Window. However, Acrobat JavaScript cannot access these particular objects but it can manipulate PDF-specific objects.

The following are the steps to add JavaScript to a PDF file.

*   Load the PDF file using the **[Document][9]** class.
*   Create an instance of **[JavascriptAction][10]** class and initialize it with the desired script.
*   Assign **JavascriptAction** object to **[Document.setOpenAction()][11]** method for document level JavaScript.
*   To add page level JavaScript, use **[setOnClose()][12]** and **[setOnOpen()][13]** methods.
*   Save PDF using ****[**Document.save(String)**][14]**** method.

The following code sample shows how to add JavaScript to a PDF file.

{{< gist aspose-com-gists e330cd590b8f10f7f95faaa9eb108c98 "add-javascript-to-pdf.java" >}}

## Add Document Level JavaScript in a PDF in Java {#Add-Document-Level-JavaScript-in-PDF}

You can also add JavaScript to the document level using **[**Document.getJavaScript().set\_Item**()][15]** method. The following are the steps to add JavaScript to the document level in Java.

*   Load the PDF file using **[Document][16]** class.
*   Use ****[**Document.getJavaScript().set\_Item**()][17]**** method to add JavaScript functions.
*   Save PDF using **[**Document.save(String)**][18]** method.

The following code sample shows how to add JS script to a PDF file in Java.

{{< gist aspose-com-gists e330cd590b8f10f7f95faaa9eb108c98 "add-document-level-javascript-to-pdf.java" >}}

## Remove JavaScript from a PDF File in Java {#Remove-JavaScript-from-PDF}

The following are the steps to remove JavaScript from a PDF file in Java.

*   Load the PDF file using **[Document][19]** class.
*   Remove desired JavaScript by its key using **[Document.getJavaScript().remove(String)][20]** method.
*   Save PDF using **[**Document.save(String)**][21]** method.

The following code sample shows how to remove JavaScript from a PDF file in Java.

{{< gist aspose-com-gists e330cd590b8f10f7f95faaa9eb108c98 "remove-javascript-from-pdf.java" >}}

## Get a Free License {#Get-a-Free-License}

You can [get a free temporary license][22] in order to use Aspose.PDF for Java without evaluation limitations.

## Conclusion

In this article, you have learned how to add JavaScript to PDF files in Java. Furthermore, you have seen how to remove JavaScript from a PDF file programmatically. Besides, you can explore more about Java PDF API using the [documentation][23]. In case you would have any questions or queries, you can contact us via our [forum][24].

## See Also

*   [Creating PDF Files from Scratch using Java][25]




[1]: https://docs.fileformat.com/pdf/
[2]: https://docs.fileformat.com/pdf/
[3]: #API-to-Work-with-JavaScript-in-PDF
[4]: #Add-JavaScript-to-PDF-Files
[5]: #Add-Document-Level-JavaScript-in-PDF
[6]: #Remove-JavaScript-from-PDF
[7]: https://products.aspose.com/pdf/java/
[8]: https://downloads.aspose.com/pdf/java
[9]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/Document
[10]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/JavascriptAction
[11]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/Document#setOpenAction-com.aspose.pdf.IAppointment-
[12]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/PageActionCollection#setOnClose-com.aspose.pdf.PdfAction-
[13]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/PageActionCollection#setOnOpen-com.aspose.pdf.PdfAction-
[14]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/Document#save-java.lang.String-
[15]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/JavaScriptCollection#set_Item-java.lang.String-java.lang.String-
[16]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/Document
[17]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/JavaScriptCollection#set_Item-java.lang.String-java.lang.String-
[18]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/Document#save-java.lang.String-
[19]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/Document
[20]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/JavaScriptCollection#remove-java.lang.String-
[21]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/Document#save-java.lang.String-
[22]: https://purchase.aspose.com/temporary-license
[23]: https://docs.aspose.com/pdf/java/
[24]: https://forum.aspose.com/
[25]: https://blog.aspose.com/2020/12/31/create-pdf-files-in-java/





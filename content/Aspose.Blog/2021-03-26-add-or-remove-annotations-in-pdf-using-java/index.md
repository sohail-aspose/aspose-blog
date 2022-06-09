---
title: 'Add or Remove Annotations in PDF Files using Java'
seoTitle: "Add or Remove Annotations in PDF in Java | Java PDF Annotation"
description: "Use Java PDF API to add or remove annotations in PDF documents using Java. Add line, text, watermark, circles, popup and multimedia PDF annotations."
date: Fri, 26 Mar 2021 16:51:00 +0000
draft: false
url: /2021/03/26/add-or-remove-annotations-in-pdf-using-java/
author: Usman Aziz
summary: 'Annotations in PDF files are used to elaborate the content. An annotation could be a note, popup, or a graphical object such as an arrow, line, etc. Since PDF files are not editable, annotations let you provide additional information. In this article, you will learn how to work with annotations in PDF files programmatically. Particularly, you will learn **how to add or remove annotations in PDF files using Java**.'
tags: ['Add Annotations to PDF using Java', 'Delete a Particular PDF Annotation in Java', 'Remove Annotations from PDF using Java']
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/Add-or-Remove-Annotation-in-PDF-2.jpg" alt="Add or Remove Annotation in PDF">}}


Annotations in [PDF][1] files are used to elaborate the content. An annotation could be a note, popup, or a graphical object such as an arrow, line, etc. Since PDF files are not editable, annotations let you provide additional information. In this article, you will learn how to work with annotations in PDF files programmatically. Particularly, you will learn **how to add or remove annotations in PDF files using [Java][2]**.

*   [Java API to Work with PDF Annotations][3]
*   [Add Annotations to PDF using Java][4]
*   [Remove Annotations from PDF using Java][5]
    *   [Delete a Particular Annotation][6]
    *   [Delete all Annotations][7]
*   [Get a Free API License][8]

## Java API to Add or Remove PDF Annotations {#Java-API-to-Work-with-PDF-Annotations}

In order to add or remove PDF annotations, we will use [Aspose.PDF for Java][9]. It is a feature-rich API that lets you generate, edit and convert PDF files using Java. In addition, the API allows you to work with a wide range of PDF annotations seamlessly. You can either [download][10] the API or install it using the following Maven configurations.

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
    <version>21.3</version>
</dependency>
```

## Add Annotation to PDF using Java {#Add-Annotations-to-PDF-using-Java}

Aspose.PDF for Java supports a number of annotations including but not limited to text, line, circle, square, highlight, etc. To add each annotation type, Aspose.PDF for Java provides a separate class. For example, [LineAnnotation][11] class is used to add a line whereas [HighlightAnnotation][12] class is used to add a highlight annotation.

### Steps to Add an Annotation to PDF using Java

For demonstration, let's add a text annotation to a PDF file. The following are the steps along with API references to add a text annotation to PDF using Java.

*   First, load the PDF document using [Document][13] class.
*   Create an object of [TextAnnotation][14] class to add text annotation.
*   Set properties of the annotation such as title, subject, etc.
*   Set border of the annotation using [Border][15] class.
*   Add annotation to the document using [Document.getPages().get\_Item(int).getAnnotations().add(Annotation)][16] method.
*   Finally, save the updated PDF using [Document.save(string)][17] method.

The following code sample shows how to add a text annotation to PDF using Java.

{{< gist aspose-com-gists 7cb73e8f2df1d8ad4a4cc6f98959bba2 "add-annotation.java" >}}

## Remove Annotations from PDF using Java {#Remove-Annotations-from-PDF-using-Java}

For removing the annotations from a page in PDF, Aspose.PDF for Java provides the following options:

*   Delete a particular annotation on a page
*   Delete all annotations on a page

### Remove a Particular PDF Annotation {#Remove-a-Particular-Annotation}

The following are the steps to remove an annotation from a PDF file using Java.

*   First, load the PDF document using [Document][18] class.
*   Remove desired annotation by index using [Document.getPages().get\_Item(int).getAnnotations().delete(int)][19] method.
*   Finally, save the updated PDF using [Document.save(string)][20] method.

The following code sample shows how to remove a particular annotation from a page in PDF using Java.

{{< gist aspose-com-gists 7cb73e8f2df1d8ad4a4cc6f98959bba2 "remove-annotation.java" >}}

### Remove all PDF Annotations {#Remove-all-PDF-Annotations}

The following are the steps to remove all the annotations on a page in PDF using Java.

*   First, load the PDF document using [Document][21] class.
*   Remove all annotations using [Document.getPages().get\_Item(int).getAnnotations().delete()][22] method.
*   Finally, save the updated PDF using [Document.save(string)][23] method.

The following code sample shows how to remove all annotations on a page in PDF using Java.

{{< gist aspose-com-gists 7cb73e8f2df1d8ad4a4cc6f98959bba2 "remove-all-annotations.java" >}}

## Get a Free API License {#Get-a-Free-API-License}

You can try Aspose.PDF for Java for free without evaluation limitations using a [temporary license][24].

## Conclusion

In this article, you have learned how to work with annotations in PDF files. Particularly, you have seen how to add or remove annotations in PDF files using Java. You can explore more about Aspose.PDF for Java using [documentation][25]. In case you would have any questions or queries, please let us know via our [forum][26].

## See Also

*   [Split a PDF File Programmatically using Java][27]




[1]: https://docs.fileformat.com/pdf/
[2]: https://docs.fileformat.com/programming/java/
[3]: #Java-API-to-Work-with-PDF-Annotations
[4]: #Add-Annotations-to-PDF-using-Java
[5]: #Remove-Annotations-from-PDF-using-Java
[6]: #Remove-a-Particular-Annotation
[7]: #Remove-all-PDF-Annotations
[8]: #Get-a-Free-API-License
[9]: https://products.aspose.com/pdf/java
[10]: https://downloads.aspose.com/pdf/java
[11]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/LineAnnotation
[12]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/HighlightAnnotation
[13]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/Document
[14]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/TextAnnotation
[15]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/Border
[16]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/AnnotationCollection#add-com.aspose.pdf.Annotation-
[17]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/Document#save-java.lang.String-
[18]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/Document
[19]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/AnnotationCollection#delete-int-
[20]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/Document#save-java.lang.String-
[21]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/Document
[22]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/AnnotationCollection#delete--
[23]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/Document#save-java.lang.String-
[24]: https://purchase.aspose.com/temporary-license
[25]: https://docs.aspose.com/pdf/java/
[26]: https://forum.aspose.com/
[27]: https://blog.aspose.com/2021/01/15/Split-PDF-Files-using-Java/






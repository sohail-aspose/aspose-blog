---
title: 'Merge Multiple PDF Files  into a Single PDF using Java'
seoTitle: "Merge PDF Files in Java | Combine Two or Multiple PDF Files in Java"
description: "Merge PDF files in Java. Combine or merge two or multiple PDF files programmatically in Java. Merge PDFs in single PDF in Spring or any Java application."
date: Thu, 18 Jun 2020 01:32:16 +0000
draft: false
url: /2020/06/18/merge-two-or-multiple-pdf-files-using-java/
author: Usman Aziz
summary: ''
tags: ['Merge Multiple PDF Files into Single PDF', 'Merge PDF Files using Java']
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/Merge-PDF-Files-into-Single-PDF.jpg" alt="Merge PDF Files into Single PDF">}}


In various scenarios, you come across the need of **merging two or more PDF documents into a single file**. For example, PDF merging allows you to combine similar kinds of documents. Furthermore, you can merge multiple PDFs into a single PDF before sharing it online or sending it to someone. In this article, I'll demonstrate how to automate this feature and **merge multiple PDF files programmatically using Java**.

*   [Merge Two PDF Files into a Single PDF using Java][1]
*   [Merge Multiple PDF Files using Java][2]
*   [Use InputStream Objects to Merge PDF Files using Java][3]

## Java API to Merge PDF Files

[Aspose.PDF for Java][4] is a feature-rich PDF API that lets you merge multiple PDF documents quite easily within a few lines of code. You can either [download][5] the API's JAR or install it in your Maven-based application using the following configuration.

### Repository```
<repository>
    <id>AsposeJavaAPI</id>
    <name>Aspose Java API</name>
    <url>https://repository.aspose.com/repo/</url>
</repository>
```

### Dependency```
<dependency>
    <groupId>com.aspose</groupId>
    <artifactId>aspose-pdf</artifactId>
    <version>20.5</version>
    <classifier>jdk17</classifier>
</dependency>'
```

## Merge Two PDF Files into One PDF in Java {#Merge-Two-PDF-Files-using-Java}

Lets first check out the simple scenario of merging only two PDF files and this can be achieved within a couple of steps.

*   Create an instance of the [PdfFileEditor][6] class.
*   Merge PDF files using [PdfFileEditor.concatenate(String firstInputFile, String secInputFile, String outputFile)][7] method.

The following code sample shows how to merge two PDF files into a single PDF using Java.

{{< gist aspose-com-gists 71e67641b18c8933a417a30f000ee63f "merge-two-pdf.java" >}}

## Merge Multiple PDF Files using Java {#Merge-Multiple-PDF-Files-using-Java}

In the previous example, we have merged only two PDF files into a single PDF. However, there could be a case when you need to merge more than two PDF files. In such cases, you can pass an array to the PDF files' paths to the _concatenate_ method. The following are the steps to perform this operation.

*   Create an instance of the [PdfFileEditor][8] class.
*   Put the PDF files' paths into a string array.
*   Merge PDF files using [PdfFileEditor.concatenate(String\[\] inputFiles, String outputFile)][9] method.

The following code sample shows how to merge multiple PDF files into a single PDF using Java.

{{< gist aspose-com-gists 71e67641b18c8933a417a30f000ee63f "merge-multiple-pdf.java" >}}

## Merge PDF Files using InputStream in Java {#Merge-Files-using-InputStream-objects-in-Java}

In case you are dealing with the PDF files in the form of InputStream, you can directly pass the _InputStream_ objects and get the merged PDF as an _OutputStream_ object. The following are the steps to merge PDF files loaded into InputStream objects.

*   Create an instance of the [PdfFileEditor][10] class.
*   Load the PDF files into the _InputStream_ objects.
*   Merge PDFs using [PdfFileEditor.concatenate(InputStream firstInputStream, InputStream secInputStream, OutputStream outputStream)][11] method.

The following code sample shows how to merge PDF files using _InputStream_ objects in Java.

{{< gist aspose-com-gists 71e67641b18c8933a417a30f000ee63f "merge-multiple-pdf-stream.java" >}}

## Conclusion

In this article, you have learned how to merge PDF files programmatically using Java. The code samples and step by step guide shows how to merge two or more than two PDF files using physical paths or InputStream objects. You can learn more about the Java PDF Merger library using the [documentation][12].

## See Also

*   [Merge Multiple PDF Files into One PDF using C# .NET][13]




[1]: #Merge-Two-PDF-Files-using-Java
[2]: #Merge-Multiple-PDF-Files-using-Java
[3]: #Merge-Files-using-InputStream-objects-in-Java
[4]: https://products.aspose.com/pdf/java
[5]: https://downloads.aspose.com/pdf/java
[6]: https://apireference.aspose.com/pdf/java/com.aspose.pdf.facades/PdfFileEditor
[7]: https://apireference.aspose.com/pdf/java/com.aspose.pdf.facades/PdfFileEditor#concatenate-java.lang.String-java.lang.String-java.lang.String-
[8]: https://apireference.aspose.com/pdf/java/com.aspose.pdf.facades/PdfFileEditor
[9]: https://apireference.aspose.com/pdf/java/com.aspose.pdf.facades/PdfFileEditor#concatenate-java.lang.String:A-java.lang.String-
[10]: https://apireference.aspose.com/pdf/java/com.aspose.pdf.facades/PdfFileEditor
[11]: https://apireference.aspose.com/pdf/java/com.aspose.pdf.facades/PdfFileEditor#concatenate-java.io.InputStream-java.io.InputStream-java.io.OutputStream-
[12]: https://docs.aspose.com/display/pdfjava/Getting+Started
[13]: https://blog.aspose.com/2020/01/16/merge-multiple-pdf-files-in-csharp-net/






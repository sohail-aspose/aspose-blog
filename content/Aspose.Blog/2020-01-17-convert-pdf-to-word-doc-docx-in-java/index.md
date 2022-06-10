---
title: 'Convert PDF Files to MS Word Documents (DOC/DOCX) in Java'
seoTitle: "Java PDF to Word | Convert PDF to DOC or PDF to DOCX in Java"
description: "Convert PDF to Word in Java. Convert PDF to DOC or PDF to DOCX programmatically using Java PDF to Word (DOC/DOCX) converter library. PDF Converter API."
date: Fri, 17 Jan 2020 13:33:18 +0000
draft: false
url: /2020/01/17/convert-pdf-to-word-doc-docx-in-java/
author: Usman Aziz
summary: "**PDF** is one of the most commonly used formats for sending the document out to third parties. The reason behind this popularity is PDF's compatibility across multiple platforms regardless of any hardware/software requirements. However, in some cases, you would want to convert the PDF document into an editable document format. **PDF to DOC or DOCX** format could be the priority conversion option in such cases. In order to automate the conversion process, this article showcases how to **convert PDF to Word programmatically in Java**."
tags: ['PDF to DOC', 'convert pdf to doc in java', 'convert pdf to docx in java', 'convert pdf to word in java', 'pdf to word']
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/PDF-to-Word.png" alt="PDF to Word">}}


[**PDF**][1] is one of the most commonly used formats for sending the document out to third parties. The reason behind this popularity is PDF's compatibility across multiple platforms regardless of any hardware/software requirements. However, in some cases, you would want to convert the PDF document into an editable document format. **PDF to DOC or DOCX** format could be the priority conversion option in such cases. In order to automate the conversion process, this article showcases how to **convert PDF to Word programmatically in Java**.

So in this article, you will get to know how to:

*   Convert PDF to DOC using Java.
*   Convert PDF to DOCX format using Java.
*   Customize PDF to Word (DOC/DOCX) conversion.

## Java PDF to Word Converter Library

Thanks to [Aspose.PDF for Java][2] - a PDF manipulation Java API that provides easy ways to convert PDF files to a variety of other formats including PDF to DOC and PDF to DOCX. You can [download][3] and add API's JAR file to your project or reference it using the following Maven configurations:

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
    <version>19.12</version>
</dependency>
```

## Convert PDF to DOC using Java

Once you have referenced _Aspose.PDF for Java_ in your application, you can convert any PDF document to DOC format in a couple of lines of code. The following are the steps required to perform this conversion.

*   Create an instance of the [Document][4] class and initialize it with the input PDF file's path.
*   Call [Document.save()][5] method with the output DOC file's name and [SaveFormat.Doc][6] arguments.

The following code sample shows how to convert PDF to DOC in Java.

{{< gist aspose-com-gists 6b3fd2f622633cffc7e000b4d33bb027 "convert-pdf-to-doc.java" >}}

### Input PDF Document



{{< figure align=center src="images/Convert-PDF-to-DOC.png" alt="How to Convert PDF to DOC in Java">}}


### Output Word Document



{{< figure align=center src="images/Convert-PDF-to-DOCX.png" alt="Convert PDF to DOCX in Java">}}


## Convert PDF to DOCX using Java

DOCX is a well-known format for Word documents and in contrast to the DOC format, the structure of DOCX was based on the binary as well as the XML files. In case you want to convert PDF to DOCX format, you can tell the API to do so using the [SaveFormat.DocX][7] argument in _Document.save()_ method.

The following code sample shows how to convert PDF to DOCX in Java.

{{< gist aspose-com-gists 6b3fd2f622633cffc7e000b4d33bb027 "convert-pdf-to-docx.java" >}}

## Convert PDF to Word with Additional Options

_Aspose.PDF for Java_ also provides some additional options that you can use in PDF to Word conversion, such as the output format, image resolution, distance between text lines and so on. [DocSaveOptions][8] class is used for this purpose and the following is the list of options you can use:

*   [setFormat(int value)][9] - To set the output format (Doc, Docx, etc.).
*   [setAddReturnToLineEnd(boolean value)][10] - To add the paragraph or line breaks.
*   [setImageResolutionX(int value)][11] - To set the X resolution for the images.
*   [setImageResolutionY(int value)][12] - To set the Y resolution for the images.
*   [setMaxDistanceBetweenTextLines(float value)][13] - To group text lines into paragraphs.
*   [setMode(int value)][14] - To set recognition mode.
*   [setRecognizeBullets(boolean value)][15] - To switch the recognition of bullets on.
*   [setRelativeHorizontalProximity(float value)][16] - To set the width of space between different text elements in the input PDF file.

The following code sample shows how to use [DocSaveOptions][17] class in PDF to DOCX conversion using Java.

{{< gist aspose-com-gists 6b3fd2f622633cffc7e000b4d33bb027 "convert-pdf-to-docx-additional-options.java" >}}

## Conclusion

In this article, you have learned how easy it is to convert PDF documents to Word formats using Java. You can either convert PDF to DOC or PDF to DOCX based on your requirements. Furthermore, additional features to customize the PDF to Word DOC/DOCX conversion have also been discussed. You can learn more about converting PDF to other formats from the [documentation][18].

## Related Article(s)

*   [Convert PDF to Word DOC/DOCX in C#][19]
*   [Convert PDF Files to Excel Spreadsheets][20]




[1]: https://wiki.fileformat.com/view/pdf/
[2]: https://products.aspose.com/pdf/java
[3]: https://downloads.aspose.com/pdf/java
[4]: https://apireference.aspose.com/java/pdf/com.aspose.pdf/Document
[5]: https://apireference.aspose.com/java/pdf/com.aspose.pdf/Document#save-java.lang.String-int-
[6]: https://apireference.aspose.com/java/pdf/com.aspose.pdf/SaveFormat#Doc
[7]: https://apireference.aspose.com/java/pdf/com.aspose.pdf/SaveFormat#DocX
[8]: https://apireference.aspose.com/java/pdf/com.aspose.pdf/DocSaveOptions
[9]: https://apireference.aspose.com/java/pdf/com.aspose.pdf/DocSaveOptions#setFormat-int-
[10]: https://apireference.aspose.com/java/pdf/com.aspose.pdf/DocSaveOptions#setAddReturnToLineEnd-boolean-
[11]: https://apireference.aspose.com/java/pdf/com.aspose.pdf/DocSaveOptions#setImageResolutionX-int-
[12]: https://apireference.aspose.com/java/pdf/com.aspose.pdf/DocSaveOptions#setImageResolutionY-int-
[13]: https://apireference.aspose.com/java/pdf/com.aspose.pdf/DocSaveOptions#setMaxDistanceBetweenTextLines-float-
[14]: https://apireference.aspose.com/java/pdf/com.aspose.pdf/DocSaveOptions#setMode-int-
[15]: https://apireference.aspose.com/java/pdf/com.aspose.pdf/DocSaveOptions#setRecognizeBullets-boolean-
[16]: https://apireference.aspose.com/java/pdf/com.aspose.pdf/DocSaveOptions#setRelativeHorizontalProximity-float-
[17]: https://apireference.aspose.com/java/pdf/com.aspose.pdf/DocSaveOptions
[18]: https://docs.aspose.com/display/pdfjava/Convert+PDF+to+other+Formats
[19]: https://blog.aspose.com/2019/11/24/convert-pdf-to-word-doc-docx-in-csharp-vb-net/
[20]: https://blog.aspose.com/2020/01/03/convert-pdf-to-excel-in-csharp-net-pdf-to-xls-pdf-to-xlsx/






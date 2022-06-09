---
title: 'Convert OneNote .one File to a Word DOCX or DOC Document in Java'
seoTitle: "Convert OneNote .one to Word DOCX or DOC Document with Java"
description: "You can convert OneNote .one file to a Word DOCX or DOC format document programmatically using Java. Export Microsoft OneNote to Word Document."
date: Thu, 14 Oct 2021 08:15:00 +0000
draft: false
url: /2021/10/14/convert-onenote-word-java/
author: Farhan Raza
summary: 'OneNote files contain digital notes that can include text, images, drawings, etc. In some scenarios, you might need to convert a OneNote .one file to a Word document. This article covers how to convert a Microsoft OneNote .one file to DOCX or DOC file format.'
tags: ['.one to DOCX', '.one to Word', 'Export OneNote to Word', 'OneNote to Word']
categories: ['Aspose.Note Product Family']
---



{{< figure align=center src="images/OneNote-to-Word.jpg" alt="OneNote to Word DOCX">}}


OneNote files contain digital notes that can include text, images, drawings, etc. In some scenarios, you might need to convert a OneNote [.one][1] file to a Word document. This article covers how to convert a Microsoft OneNote .one file to [DOCX][2] or [DOC][3] file format.

*   [OneNote .one File to Word DOCX DOC Converter – Java API Installation][4]
*   [Convert OneNote .one File to DOCX or DOC file in Java][5]

## OneNote .one File to Word DOCX DOC Converter – Java API Installation

You can convert a OneNote file to a Word DOCX or DOC document in two steps. Firstly, export the .one file to a PDF document using [Aspose.Note for Java][6] API. Secondly, convert the output PDF file to a Word document as DOCX or DOC file using [Aspose.PDF for Java][7] API. You can get the JAR files from the Downloads, or use the following Maven configurations in pom.xml file of your project:

### Repository```
 <repositories>
    <repository>
        <id>AsposeJavaAPI</id>
        <name>Aspose Java API</name>
        <url>https://repository.aspose.com/repo/</url>
    </repository>
</repositories>
```

### Dependency```
 <dependencies>
    <dependency>
        <groupId>com.aspose</groupId>
        <artifactId>aspose-note</artifactId>
        <version>21.9</version>
        <classifier>jdk17</classifier>        
    </dependency>

    <dependency>
        <groupId>com.aspose</groupId>
        <artifactId>aspose-pdf</artifactId>
        <version>21.9</version>
    </dependency>
</dependencies>
```

## Convert OneNote .one File to Word DOCX or DOC file in Java

You can convert a OneNote .one file to Word DOCX or DOC document by following the steps below:

1.  Initialize an instance of [ByteArrayOutputStream][8] class.
2.  Load the OneNote .one file using the [Document][9] class.
3.  Export the .one file as PDF with the [save][10] method.
4.  Load the file using [Document][11] class of Aspose.PDF for Java API.
5.  Convert the OneNote .one file as Word DOCX or DOC document.

The code snippet below explains how to convert a OneNote .one file to DOCX or DOC Word Document using Java:

{{< gist aspose-com-gists f39166a7085445fc5a1c5879b4fd3eba "OneNote-to-Word.java" >}}

## Get Free API License

You can test the APIs in full capacity by requesting a [Free Evaluation License][12].

## Conclusion

In conclusion, you have learned how to convert a Microsoft OneNote .one file to a Word document in DOCX or DOC format file programmatically using Java. You can easily integrate this feature into any Java application and start converting your notes. Moreover, please visit the [Documentation][13] section to learn many other features offered by the APIs. In case of any inquiries, please feel free to contact us at the [Free Support Forum][14].

## See Also

[Print OneNote .one Notebook Programmatically using Java][15]




[1]: https://docs.fileformat.com/note-taking/one/
[2]: https://docs.fileformat.com/word-processing/docx/
[3]: https://docs.fileformat.com/word-processing/doc/
[4]: #section1
[5]: #section2
[6]: https://products.aspose.com/note/java/
[7]: https://products.aspose.com/pdf/java/
[8]: https://docs.oracle.com/en/java/javase/11/docs/api/java.base/java/io/ByteArrayOutputStream.html
[9]: https://apireference.aspose.com/note/java/com.aspose.note/Document
[10]: https://apireference.aspose.com/note/java/com.aspose.note/Document#save-java.lang.String-
[11]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/Document
[12]: https://purchase.aspose.com/temporary-license
[13]: https://docs.aspose.com/
[14]: https://forum.aspose.com/
[15]: https://blog.aspose.com/2021/09/09/print-onenote-.one-notebook-programmatically-using-java/





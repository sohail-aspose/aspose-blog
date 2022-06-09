---
title: 'Convert PUB to Word Document DOC or DOCX Programmatically in Java'
seoTitle: "Convert or Export Publisher PUB file to Word DOCX DOC File"
description: "You can convert or export Microsoft Publisher PUB file to Microsoft Word file in DOCX or DOC format in your Java applications programmatically."
date: Tue, 31 Aug 2021 10:53:52 +0000
draft: false
url: /2021/08/31/convert-pub-to-word-docx-doc-java/
author: Farhan Raza
summary: 'In this article, you will learn how to convert or export an MS Publisher PUB file to an MS Word Document in DOCX or DOC format. The step-by-step guide will demonstrate all the details about the conversion.'
tags: ['Convert PUB to DOCX', 'Convert PUB to Word', 'Export PUB to DOCX', 'Export PUB to Word']
categories: ['Aspose.PUB Product Family']
---



{{< figure align=center src="images/PUB-to-Word.png" alt="Convert Export PUB to Word DOCX">}}


In this article, you will learn how to convert or export an MS Publisher [PUB][1] file to an MS Word Document in [DOCX][2] or [DOC][3] format. The step-by-step guide will demonstrate all the details about the conversion:

*   [Java APIs to Convert PUB file to Word Document as DOC/DOCX][4]
*   [Convert PUB File to Word Document DOCX DOC Programmatically in Java][5]

## Java APIs to Convert PUB file to Word Document as DOC/DOCX {#section1}

You will convert a PUB file to a Word document in two steps. First, you convert a PUB file to PDF using [Aspose.PUB for Java][6] API. Then you convert the PDF file to a Word document using [Aspose.PDF for Java][7] API. You can download the JAR files from the [New Releases][8] section, or specify the following configurations in the pom.xml file of your Maven-based projects:

### Repository```
 <repositories>
    <repository>
        <id>AsposeJavaAPI</id>
        <name>Aspose Java API</name>
        <url>http://repository.aspose.com/repo/</url>
    </repository>
</repositories>
```

### Dependency```
 <dependencies>

    <dependency>
        <groupId>com.aspose</groupId>
        <artifactId>aspose-pub</artifactId>
        <version>20.8</version>
    </dependency>

    <dependency>
        <groupId>com.aspose</groupId>
        <artifactId>aspose-pdf</artifactId>
        <version>21.8</version>
    </dependency>

</dependencies>
```

## Convert PUB File to Word Document DOCX DOC Programmatically in Java {#section2}

You can convert a Microsoft Publisher PUB file to a Word Document in DOCX or DOC format with the following steps:

1.  Firstly, initialize [ByteArrayOutputStream][9] to hold intermediary file.
2.  Initialize [Pub Parser][10] for the PUB file.
3.  [Parse][11] the input Publisher file.
4.  Convert PUB to PDF file and save output into the stream.
5.  Load the intermediary PDF document with [Document][12] class object.
6.  Finally, convert the file to MS Word DOCX or DOC format with the [Save][13] method.

The code below explains how to convert or export a PUB file to a Word document in DOCX DOC format programmatically using Java:

{{< gist aspose-com-gists 1e9e2f83bba549ef6e134c5cfd4c12c4 "Convert-PUB-to-Word-DOCX.java" >}}

## Get Free API License

You can evaluate the Aspose APIs without any limitations by requesting a [Free Temporary License][14].

## Conclusion

In conclusion, you have learned how to convert or export Microsoft Publisher PUB file to a Word document as DOC or DOCX file programmatically using Java. You can integrate this feature in any of your Java-based applications. Moreover, you can explore several other features offered by Aspose APIs by visiting the [Documentation][15]. In case of any concerns, please feel free to contact us at the [Free Support Forum][16]. Happy coding!

## See Also

[Convert PUB to Image Programmatically in Java][17]




[1]: https://fileinfo.com/extension/pub
[2]: https://docs.fileformat.com/word-processing/docx/
[3]: https://docs.fileformat.com/word-processing/doc/
[4]: #section1
[5]: #section2
[6]: https://products.aspose.com/pub/java/
[7]: https://products.aspose.com/pdf/java/
[8]: https://releases.aspose.com/
[9]: https://docs.oracle.com/en/java/javase/11/docs/api/java.base/java/io/ByteArrayOutputStream.html
[10]: https://apireference.aspose.com/pub/java/com.aspose.pub.class-use/IPubParser
[11]: https://apireference.aspose.com/pub/java/com.aspose.pub/IPubParser#parse--
[12]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/Document
[13]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/Document#save-java.lang.String-int-
[14]: https://purchase.aspose.com/temporary-license
[15]: https://docs.aspose.com/pub/java/
[16]: https://forum.aspose.com/c/pub
[17]: https://blog.aspose.com/2021/05/31/convert-pub-to-image-programmatically-in-java/






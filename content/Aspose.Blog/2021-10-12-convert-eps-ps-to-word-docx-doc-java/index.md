---
title: 'Convert PS or EPS to Word DOCX or DOC in Java'
seoTitle: "Convert PS or EPS to Word DOCX or DOC Document in Java"
description: "Convert EPS or PS PostScript file to Word DOCX DOC Document Programmatically in Java. Export Encapsulated PostScript file to DOCX."
date: Tue, 12 Oct 2021 07:49:00 +0000
draft: false
url: /2021/10/12/convert-eps-ps-to-word-docx-doc-java/
author: Farhan Raza
summary: 'EPS or PS are postscript files that can be used for placing different graphics. In some scenarios, you may need to convert an EPS or PS PostScript file to a Word Document as DOCX or DOC file. This article covers EPS to Word DOCX file format conversion programmatically using Java.'
tags: ['EPS or PS to Word in Java', 'EPS to DOCX', 'EPS to DOCX in Java', 'EPS to Word', 'PS to DOCX', 'PS to Word', 'PostScript to DOCX', 'PostScript to Word']
categories: ['Aspose.Page Product Family']
---



{{< figure align=center src="images/EPS-PostScript-to-Word-DOCX.jpg" alt="EPS PostScript to Word DOCX">}}


EPS or PS are postscript files that can be used for placing different graphics. In some scenarios, you may need to convert an [EPS][1] or [PS][2] PostScript file to a Word Document as [DOCX][3] or [DOC][4] file. This article covers EPS to Word DOCX file format conversion programmatically using Java:

*   [EPS or PS PostScript File to Word DOCX/DOC Converter – Java API Installation][5]
*   [Convert EPS or PS PostScript File to Word DOCX or DOC File in Java][6]

## EPS or PS PostScript File to Word DOCX/DOC Converter – Java API Installation {#section1}

EPS or PS to Word DOCX or DOC document conversion can be done in two steps. Firstly, convert an EPS or PS file to a PDF document using [Aspose.Page for Java][7]. Then convert the intermediary PDF file to a Word document as DOCX or DOC using [Aspose.PDF for Java][8] API. You can download the APIs from the [New Releases][9] section, or use the following Maven configurations to download the APIs from [Aspose Repository][10]:

### Repository```
 <repositories>
     <repository>
         <id>snapshots</id>
         <name>repo</name>
         <url>http://repository.aspose.com/repo/</url>
     </repository>

</repositories>
```

### Dependency```
 <dependencies>
    <dependency>
        <groupId>com.aspose</groupId>
        <artifactId>aspose-page</artifactId>
        <version>21.8</version>
    </dependency>

    <dependency>
        <groupId>com.aspose</groupId>
        <artifactId>aspose-pdf</artifactId>
        <version>21.9</version>
    </dependency>

</dependencies>
```

## Convert EPS or PS PostScript File to Word DOCX or DOC File in Java {#section2}

You can convert an EPS or PS PostScript file to a Word DOCX or DOC document with the following steps:

1.  Declare a [ByteArrayOutputStream][11] to save intermediary PDF document.
2.  Instantiate EPS or PS PostScript using the [FileInputSream][12].
3.  Initialize [PsDocument][13] class object.
4.  Initialize [PdfSaveOptions][14] object with necessary parameters.
5.  Convert EPS or PS Postscript file to PDF.
6.  Instantiate [DocSaveOptions][15] object and set the format as DOCX or DOC.
7.  Convert the EPS or PS file to a Word DOCX or DOC document with [save][16] method.

The following code snippet shows how to convert an EPS or PS PostScript file programmatically in Java:

{{< gist aspose-com-gists 75b9f1628cfdabc6c1dd1b0a2137fc82 "EPS-to-Word-DOCX-DOC.java" >}}

## Get Free Evaluation License

You can test the APIs without any limitations by requesting a [Free Temporary License][17].

## Conclusion

In this article, you have learned how to convert an EPS or PS PostScript file to a Word DOCX or DOC format file using Java. Moreover, you can take a look at the [Documentation][18] section for exploring more features. Please feel free to contact us at the [Free Support Forum][19],

## See Also

[Convert a Postscript PS or EPS file to PDF using Java][20]

[Convert OXPS or XPS to PDF Programmatically with Java][21]




[1]: https://docs.fileformat.com/page-description-language/eps/
[2]: https://docs.fileformat.com/page-description-language/ps/
[3]: https://docs.fileformat.com/word-processing/docx/
[4]: https://docs.fileformat.com/word-processing/doc/
[5]: #section1
[6]: #section2
[7]: https://products.aspose.com/page/java/
[8]: https://products.aspose.com/pdf/java/
[9]: https://releases.aspose.com/
[10]: https://repository.aspose.com/repo/com/aspose/
[11]: https://docs.oracle.com/javase/7/docs/api/java/io/ByteArrayOutputStream.html
[12]: https://docs.oracle.com/en/java/javase/11/docs/api/java.base/java/io/FileInputStream.html
[13]: https://apireference.aspose.com/page/java/com.aspose.eps/PsDocument
[14]: https://apireference.aspose.com/page/java/com.aspose.eps.device/PdfSaveOptions
[15]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/DocSaveOptions
[16]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/Document#save-java.lang.String-
[17]: https://purchase.aspose.com/temporary-license
[18]: https://docs.aspose.com/
[19]: https://forum.aspose.com/
[20]: https://blog.aspose.com/2021/06/08/convert-postscript-ps-eps-to-pdf-java/
[21]: https://blog.aspose.com/2021/02/09/convert-oxps-xps-pdf-java/





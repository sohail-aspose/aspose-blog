---
title: 'Convert XPS or OXPS to Word Document using Java'
date: Fri, 07 Jan 2022 08:08:00 +0000
draft: false
url: /2022/01/07/convert-xps-oxps-word-java/
author: ''Farhan Raza''
summary: 'XPS and OXPS files are often preferred owing to their resolution-independent nature to create high-quality printing output. In certain cases, you might need to convert an XPS or OXPS file to a Word document. This article discusses how to **convert XPS or OXPS documents to a word file with DOCX or DOC file extension programmatically in Java**.'
tags: ['Convert OXPS to Word Java', 'Java Convert XPS to Word', 'OXPS to DOCX', 'OXPS to Word', 'XPS to DOCX', 'XPS to Word']
categories: ['Aspose.Page Product Family']
---



{{< figure align=center src="images/Convert-XPS-OXPS-to-Word-1.png" alt="Convert XPS OXPS to Word Java">}}


[XPS][1] and [OXPS][2] files are often preferred owing to their resolution-independent nature to create high-quality printing output. In certain cases, you might need to convert an XPS or OXPS file to a Word document. This article discusses how to convert XPS or OXPS documents to a word file with [DOCX][3] or [DOC][4] file extension programmatically in Java.

*   [Create XPS to Word Converter in Java - API Installation][5]
*   [Convert XPS to Word DOCX/DOC File in Java][6]
*   [Convert OXPS to Word DOCX/DOC File Programmatically using Java][7]

**TIP:** You may want to check Aspose [PowerPoint to Word][8] Converter because it demonstrates the popular presentation to Word document conversion process.

## Create XPS to Word Converter in Java - API Installation {#section1}

XPS or OXPS files can be converted to Word documents in DOC or DOCX file format. This conversion is based on two steps where the input XPS or OXPS is first rendered as a PDF document, which is later converted to a Word document. So you need to configure [Aspose.Page for Java][9] and [Aspose.PDF for Java][10] API by downloading the JAR files from the [Downloads][11] section, or use the following Maven configurations:

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
        <version>21.12</version>
    </dependency>

    <dependency>
        <groupId>com.aspose</groupId>
        <artifactId>aspose-pdf</artifactId>
        <version>22.1</version>
    </dependency>
</dependencies>
```

## Convert XPS to Word DOCX/DOC File in Java {#section2}

You can convert an XPS file to a DOCX or DOC format Word document by following the steps below:

1.  Load the source XPS file for the conversion.
2.  Create an object of the [PdfSaveOptions][12] class and specify its properties.
3.  Render the XPS file to a PDF file.
4.  Export this intermediary PDF document to a Word file.

The following code snippet elaborates how to convert an XPS file to a Word document programmatically in Java:



## Convert OXPS to Word DOCX/DOC File Programmatically using Java {#section3}

You can convert an OXPS file to a Word document with DOCX or DOC file extension with the following steps:

1.  Firstly, load the source OXPS file.
2.  Instantiate an instance of the [PdfSaveOptions][13] class
3.  Write the intermediate PDF file to a stream.
4.  Save the intermediate PDF file as a Word document.

The code snippet below demonstrates how to convert OXPS to Word in Java:



## Get Free Temporary License

You can request a free trial to evaluate the API in full capacity by requesting a [free temporary license][14].

## Conclusion

In this article, you have gained an understanding of how to convert **XPS to Word** and **OXPS to Word** in DOCX or DOC format programmatically in Java. Moreover, please visit the [documentation][15] section to discover more features. Please feel free to reach out to us at the [forum][16], in case of any inquiries.

## See Also

[Convert XPS to JPG or PNG Image in Java][17]




[1]: https://docs.fileformat.com/page-description-language/xps/
[2]: https://docs.fileformat.com/page-description-language/oxps/
[3]: https://docs.fileformat.com/word-processing/docx/
[4]: https://docs.fileformat.com/word-processing/doc/
[5]: #section1
[6]: #section2
[7]: #section3
[8]: https://products.aspose.app/slides/conversion/ppt-to-wordhttps://products.aspose.app/slides/conversion/ppt-to-word
[9]: https://products.aspose.com/page/java
[10]: https://products.aspose.com/pdf/java
[11]: https://downloads.aspose.com/
[12]: https://apireference.aspose.com/page/java/com.aspose.xps.rendering/PdfSaveOptions
[13]: https://apireference.aspose.com/page/java/com.aspose.xps.rendering/PdfSaveOptions
[14]: https://purchase.aspose.com/temporary-license
[15]: https://docs.aspose.com/display/pagenet/Home
[16]: https://forum.aspose.com/c/page/39
[17]: https://blog.aspose.com/2022/01/24/convert-xps-to-jpg-png-image-in-java/





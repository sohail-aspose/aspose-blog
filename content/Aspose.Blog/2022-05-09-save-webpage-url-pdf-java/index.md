---
title: 'Save Webpage as PDF in Java'
seoTitle: "Print or Save Webpage from URL as PDF Programmatically in Java"
description: "Print or Save the webpage as a PDF. Save URL HTML page to PDF using Java. Save Webpage to PDF document programmatically in Java applications."
date: Mon, 09 May 2022 12:42:00 +0000
draft: false
url: /2022/05/09/save-webpage-url-pdf-java/
author: Farhan Raza
summary: 'Web pages are used to show all kinds of information on the websites. In certain scenarios, you may need to save a webpage as a PDF in Java. In accordance with such scenarios, this article covers **how to save a webpage as a PDF in Java.**'
tags: ['Webpage to PDF java', 'print web page to PDF in Java', 'web page to PDF java']
categories: ['Aspose.HTML Product Family']
---



{{< figure align=center src="images/Save-Webpage-PDF-1-1024x334.jpg" alt="Web page PDF Java">}}


Web pages are used to show all kinds of information on the websites. In certain scenarios, you may need to save a webpage as a PDF in Java. In accordance with such scenarios, this article covers how to save a webpage as a PDF in Java.

*   [Save Webpage to PDF – Java API Configuration][1]
*   [Save Webpage as PDF File Programmatically in Java][2]
*   [Print Web page to PDF with Password Protection in Java][3]

## Save Webpage to PDF – Java API Configuration {#section1}

[Aspose.HTML for Java][4] API can be used to work with HTML, PDF, and many other supported [file formats][5]. Simply configure the API by downloading its JAR file from [New Releases][6] page, or with the following configurations to access it from [Aspose Repository][7]:

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
        <artifactId>aspose-html</artifactId>
        <version>21.12</version>
        <classifier>jdk16</classifier>
    </dependency>
</dependencies>
```

## Save Webpage as PDF File Programmatically in Java {#section2}

You need to follow the steps below to save a webpage as a PDF file in Java:

1.  Load the input webpage using its URL.
2.  Create an object of [PdfSaveOptions][8] class.
3.  Save the webpage to a PDF file.

The following code shows how to save webpage as PDF programmatically using Java:

\[gist id="76a4abf0377956378246510c2ccb71b5" file="Webpage to PDF.java"\]

## Print web page to PDF with Password Protection in Java {#section3}

You can easily print a web page to PDF while protecting it with a password. The steps below explain the process to create an encrypted PDF document:

1.  Load the input HTML document with the URL.
2.  Create an object of [PdfEncryptionInfo][9] class.
3.  Print the web page to PDF with [PdfSaveOptions][10] class.

The following code snippet demonstrates how to print a web page to PDF with password protection in Java:

\[gist id="76a4abf0377956378246510c2ccb71b5" file="Web page to PDF Encryption.java"\]

## Conclusion

In conclusion, you have learned how to save web pages as PDF in Java. Moreover, you have also understood the protection and encryption of the PDF document. Furthermore, you may visit the [documentation][11] section to learn other features supported by the API. In case of any concerns, please write to us at the [forum][12].

## See Also

[Convert XHTML to PDF in Java][13]


[1]: #section1
[2]: #section2
[3]: #section3
[4]: https://products.aspose.com/html/java
[5]: https://docs.aspose.com/html/java/supported-file-formats/
[6]: https://downloads.aspose.com/html/java
[7]: https://repository.aspose.com/html/
[8]: https://apireference.aspose.com/html/java/com.aspose.html.saving/PdfSaveOptions
[9]: https://apireference.aspose.com/html/java/com.aspose.html.rendering.pdf.encryption/pdfencryptioninfo
[10]: https://apireference.aspose.com/html/java/com.aspose.html.saving/PdfSaveOptions
[11]: https://docs.aspose.com/html/java/
[12]: https://forum.aspose.com/c/html
[13]: https://blog.aspose.com/2022/05/17/convert-xhtml-pdf-java/






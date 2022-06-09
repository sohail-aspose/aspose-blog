---
title: 'Convert a Postscript PS or EPS file to PDF using Java'
seoTitle: "Convert a Postscript PS or EPS file to PDF Programmatically using Java"
description: "Convert PostScript EPS PS to PDF file Programmatically using Java. Export or change Postscript file in Page Description Language to PDF file."
date: Tue, 08 Jun 2021 09:34:00 +0000
draft: false
url: /2021/06/08/convert-postscript-ps-eps-to-pdf-java/
author: Farhan Raza
summary: 'Postscript is page description language and the PS/EPS files are can contain text, graphics and different glyphs. You can convert a PS/EPS file to PDF file programmatically using Java. Please refer to the following sections for further details.'
tags: ['Convert EPS to PDF', 'Convert PS to PDF', 'Convert PostScript to PDF in Java', 'EPS to PDF java', 'PS to PDF in Java']
categories: ['Aspose.Page Product Family']
---



{{< figure align=center src="images/Convert-PS-EPS-to-PDF.png" alt="PostScript EPS PS to PDF Java">}}


Postscript is page description language and the PS/EPS files are can contain text, graphics and different glyphs. You can convert a PS/EPS file to PDF file programmatically using Java. Please refer to the following sections for further details:

*   [Postscript PS/EPS file to PDF Converter – Java API Installation][1]
*   [Convert PS/EPS Postscript File to PDF Programmatically with Java][2]
*   [Convert PS/EPS Postscript File to PDF with Advanced Options in Java][3]

## Postscript PS/EPS file to PDF Converter – Java API Installation {#section1}

[Aspose.Page for Java][4] API supports working with the postscript files. You can render a [PS][5] or [EPS][6] file to a PDF document programmatically using Java. Simply download the JAR file from the [New Releases][7] section or use the below configurations in your pom.xml file:

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
        <version>21.4</version>
    </dependency>
</dependencies>
```

## Convert PS/EPS Postscript File to PDF Programmatically with Java {#section2}

You can convert a PS or EPS file to PDF with the following steps:

1.  Initialize PDF output stream and PostScript input stream.
2.  Initialize [PdfSaveOptions][8] object with necessary parameters.
3.  Convert PS/EPS Postscript file to PDF.

The code below shows how to convert a PS or EPS file to PDF programmatically with Java:

{{< gist aspose-com-gists 81ab11194ac76cc643fde5787a3f23e3 "EPS-to-PDF.java" >}}

## Convert PS/EPS Postscript File to PDF with Advanced Options in Java {#section3}

Here you will explore advanced options like setting the page size of output PDF document as well as the custom font folders and image quality. Please follow the following steps for converting a PS/EPS file to PDF Programmatically using Java:

1.  Initialize the input and output streams.
2.  Declare [PsDocument][9] class object.
3.  Set page size with [PdfDevice][10] class instance.
4.  Convert PS/EPS Postscript file to PDF.

The following code demonstrates how to convert a PS or EPS file to PDF Programmatically using Java:

{{< gist aspose-com-gists 81ab11194ac76cc643fde5787a3f23e3 "EPS-to-PDFsize.java" >}}

## Get Free API License

You can request [Free Evaluation License][11] to test the API in its full capacity.

## Conclusion

In this article, you have learned how to work with Aspose.Page for Java API for converting a Postscript file like a PS or EPS to PDF file programmatically using Java. You can explore several other features of the API by visiting the [Documentation][12]. Please feel free to contact us at the [Free Support Forum][13] in case of any queries.

## See Also

[Convert OXPS or XPS to PDF Programmatically with Java][14]




[1]: #section1
[2]: #section2
[3]: #section3
[4]: https://products.aspose.com/page/java
[5]: https://docs.fileformat.com/page-description-language/ps/
[6]: https://docs.fileformat.com/page-description-language/eps/
[7]: https://downloads.aspose.com/page/java
[8]: https://apireference.aspose.com/page/java/com.aspose.eps.device/PdfSaveOptions
[9]: https://apireference.aspose.com/page/java/com.aspose.eps/PsDocument
[10]: https://apireference.aspose.com/page/java/com.aspose.eps.device/PdfDevice
[11]: https://purchase.aspose.com/temporary-license
[12]: https://docs.aspose.com/page/java/
[13]: https://forum.aspose.com/c/page
[14]: https://blog.aspose.com/2021/02/09/convert-oxps-xps-pdf-java/






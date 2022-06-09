---
title: 'Convert VSD/VSDX Visio Diagram File to PDF using Java'
seoTitle: "Convert VSD/VSDX Visio Diagram File to PDF using Java"
description: "Convert Visio VSDX or VSD file to PDF Document Programmatically using Java. Export or Change Visio Diagram to PDF File easily."
date: Fri, 22 Oct 2021 08:46:00 +0000
draft: false
url: /2021/10/22/convert-vsdx-vsd-to-pdf-java/
author: Farhan Raza
summary: 'VSD or VSDX Visio files are commonly used to design processes, workflows, flow charts, etc. However, these file types are supported by a limited number of applications. In certain situations, you may need to convert a VSDX or VSD Visio file to a PDF document. This article covers how to convert a VSD/VSDX Diagram file to a PDF document using Java.'
tags: ['Convert VSDX to PDF', 'VSD to PDF', 'VSDX to PDF']
categories: ['Aspose.Diagram Product Family']
---



{{< figure align=center src="images/Visio-to-PDF-1024x361.jpg" alt="VSDX VSD Visio to PDF">}}


VSD or VSDX Visio files are commonly used to design processes, workflows, flow charts, etc. However, these file types are supported by a limited number of applications. In certain situations, you may need to convert a VSDX or VSD Visio file to a PDF document. This article covers how to convert a [VSD][1]/[VSDX][2] Diagram file to a [PDF][3] document using Java:

*   [Visio to PDF Converter – Java API Configuration][4]
*   [Convert VSD/VSDX Visio Diagram to PDF File using Java][5]
*   [Convert VSDX/VSD Diagram to PDF with Advanced Options in Java][6]

## Visio to PDF Converter - Java API Configuration {#section1}

[Aspose.Diagram for Java][7] is a class library designed to create, edit, or manipulate MS Visio diagrams from Java-based applications. You can download the JAR file from the [New Releases][8] section, or use the following Maven configurations in the pom.xml file of your project:

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
        <artifactId>aspose-diagram</artifactId>
        <version>21.10</version>
        <classifier>jdk16</classifier>
    </dependency>
</dependencies>
```

## Convert VSD/VSDX Visio Diagram to PDF in Java {#section2}

You can convert a VSD or VSDX file to PDF with the following steps:

1.  Create a [Diagram][9] class object to load a VSD/VSDX Visio file.
2.  Convert the Visio diagram to a PDF file with [Save][10] method.

The following code snippet shows how to convert a VSD/VSDX file to a PDF document using Java:

{{< gist aspose-com-gists eb08ed27910f46bffaceb1d11a6c8f8d "VSD-to-PDF.java" >}}

## Convert VSDX/VSD Diagram to PDF with Advanced Options in Java {#section3}

You can customize the Visio VSD/VSDX conversion to a PDF document using different properties like the page size, encryption, PDF/A compliance, etc. The following steps show how to convert a VSDX or VSD Diagram file to a PDF document programmatically using Java:

1.  Create a [Diagram][11] class object to load a VSD/VSDX diagram.
2.  Initialize [PdfSaveOptions][12] for saving a diagram.
3.  Set conformance level for generated PDF document.
4.  Set encryption details and page size.
5.  Convert the VSDX Visio file to a PDF file.

The code snippet below shows how to convert a VSD/VSDX Visio file to a PDF document with encryption and PDF/A compliance programmatically with Java:

{{< gist aspose-com-gists eb08ed27910f46bffaceb1d11a6c8f8d "VSDX-Visio-to-PDF-advance.java" >}}

## Get a Free License

You can request [Free Temporary License][13] for evaluating the API in its full capacity.

## Conclusion

Aspose.Diagram for Java API provides a lot of features for working with VSD/VSDX Visio diagrams. Moreover, it provides high-fidelity conversion of diagrams to PDF file format. In this article, you have explored how to convert a VSD or VSDX diagram to PDF format programmatically using Java. You can learn more about the API by taking a look at the [Documentation][14]. In case of any inquiry, please feel free to write to us at the [Free Support Forum][15].

## See Also

[Convert Visio VSDX VSD Diagram to HTML or SVG using Java][16]




[1]: https://docs.fileformat.com/image/vsd/
[2]: https://docs.fileformat.com/image/vsdx/
[3]: https://docs.fileformat.com/pdf/
[4]: #section1
[5]: #section2
[6]: #section3
[7]: https://products.aspose.com/diagram/net
[8]: https://downloads.aspose.com/diagram/java
[9]: https://apireference.aspose.com/diagram/java/com.aspose.diagram/Diagram
[10]: https://apireference.aspose.com/diagram/java/com.aspose.diagram/diagram#save(java.io.OutputStream,%20int)
[11]: https://apireference.aspose.com/diagram/java/com.aspose.diagram/Diagram
[12]: https://apireference.aspose.com/diagram/java/com.aspose.diagram/savefileformat#PDF
[13]: https://purchase.aspose.com/temporary-license
[14]: https://docs.aspose.com/diagram/java/
[15]: https://forum.aspose.com/c/diagram
[16]: https://blog.aspose.com/2021/09/30/convert-visio-vsdx-vsd-diagram-to-html-or-svg/





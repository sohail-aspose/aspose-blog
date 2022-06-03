---
title: 'Convert IFC to PDF in Java'
date: Mon, 14 Mar 2022 09:44:00 +0000
draft: false
url: /2022/03/14/convert-ifc-to-pdf-java/
author: ''Farhan Raza''
summary: 'In certain scenarios, you might need to convert an IFC file to PDF format. This article covers how to **convert IFC files to PDF with only a few lines of code in Java.**'
tags: ['Convert IFC to PDF using Java', 'IFC to PDF in Java', 'Java IFC to PDF']
categories: ['Aspose.CAD Product Family']
---



{{< figure align=center src="images/IFC-to-PDF-1.jpg" alt="IFC to PDF Java">}}


[IFC][1] files are Industry Foundation Classes files that are often used by Building Information Modelling programs. Such programs are helpful for model validation and fast clash detection and IFC files can include information about materials and spatial elements. In certain scenarios, you might need to convert an IFC file to [PDF][2] format. This article covers how to convert IFC files to PDF with only a few lines of code in Java.

*   [IFC to PDF Converter –  Java API Installation][3]
*   [Convert IFC to PDF Programmatically in Java][4]

## IFC to PDF Converter – Java API Installation {#section1}

[Aspose.CAD for Java][5] API can be used to work with different CAD file formats as mentioned in the [supported file formats][6] section. You can quickly access the API by downloading its JAR files from the [New Releases][7] page or with the following configurations in the pom.xml file to access the API from [Aspose Repository][8].

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
        <artifactId>aspose-cad</artifactId>
        <version>22.1</version>        
   </dependency>
</dependencies>
```

## Convert IFC to PDF Programmatically in Java {#section2}

You can convert an IFC file to a PDF document by following the steps below:

1.  Load the input IFC file.
2.  Instantiate an object of [CadRasterizationOptions][9] class.
3.  Initialize an instance of the [PdfOptions][10] class.
4.  Finally, write the output file in PDF format.

The following code sample demonstrates how to convert an IFC format file to a PDF file programmatically in Java:



## Explore More Features

You can take a look at many other features of the API by visiting the [documentation][11] space.

## Conclusion

In this article, you have understood how to convert an IFC file to PDF format programmatically in C#. It merely takes a few API calls to complete the requirements without needing to install any user interface-based application. However, the API supports the IFC2X3 dialect of IFC files at the moment. Please feel free to write to us at the [forum][12] in case of any queries.

## See Also

[Convert DWG to FBX in Java][13]




[1]: https://docs.fileformat.com/page-description-language/pcl/
[2]: https://docs.fileformat.com/pdf/
[3]: #section1
[4]: #section2
[5]: https://products.aspose.com/cad/java
[6]: https://docs.aspose.com/cad/java/supported-file-formats/
[7]: https://downloads.aspose.com/cad/java
[8]: https://repository.aspose.com/webapp/#/artifacts/browse/tree/General/repo/com/aspose/aspose-cad
[9]: https://apireference.aspose.com/cad/java/com.aspose.cad.imageoptions/CadRasterizationOptions
[10]: https://apireference.aspose.com/cad/java/com.aspose.cad.imageoptions/PdfOptions
[11]: https://docs.aspose.com/cad/net/
[12]: https://forum.aspose.com/c/cad
[13]: https://blog.aspose.com/2022/02/14/convert-dwg-to-fbx-java/





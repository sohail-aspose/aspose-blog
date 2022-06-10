---
title: 'Convert DWG and DXF Files to PDF using Java'
seoTitle: "DWG or DXF to PDF in Java | Convert CAD Files to PDF in Java"
description: "Use Java CAD API to convert CAD's DWG and DXF files to PDF format using Java. Convert all or selected layers in DWG to PDF. Java source code with examples."
date: Fri, 13 Nov 2020 07:27:15 +0000
draft: false
url: /2020/11/13/convert-dwg-and-dxf-to-pdf-in-java/
author: Usman Aziz
summary: '[CAD][1] file formats are used by the designers or architects to create drawings in various industries such as construction, automobile, hardware, and etc. [DWG][2] and [DXF][3] are the most widely used CAD formats, however, you need a dedicated software to view the content in DWG and DXF files. In order to tackle this limitation, you can convert the CAD drawings to PDF format. In this article, you will learn how to automate CAD to PDF conversion and convert DWG and DXF files to PDF using Java.'
tags: ['CAD to PDF Java', 'Convert CAD to PDF in Java', 'Convert DWG to PDF in Java', 'Convert DXF to PDF in Java']
categories: ['Aspose.CAD Product Family']
---

[CAD][4] file formats are used by designers or architects to create drawings in various industries such as construction, automobile, hardware, and etc. [DWG][5] and [DXF][6] are the most widely used CAD formats, however, you need dedicated software to view the content in DWG and DXF files. In order to tackle this limitation, you can convert the CAD drawings to PDF format. In this article, you will learn **how to automate CAD to PDF conversion** and **convert DWG and DXF files to PDF using Java**.

*   [Java CAD to PDF Converter API][7]
*   [Convert DWG/DXF to PDF using Java][8]
*   [Set Canvas Size in DWG/DXF to PDF using Java][9]
*   [Auto-Scaling in CAD to PDF in Java][10]
*   [Set Background and Drawing Color in CAD to PDF][11]
*   [Convert Specific Layers in CAD File to PDF using Java][12]

## Java CAD to PDF Converter API {#Java-CAD-to-PDF-Converter-API}

[Aspose.CAD for Java][13] is a powerful CAD file manipulation API that lets you convert DWG and DXF files to PDF with high fidelity. You can either [download][14] the API's JAR or install it within your Maven-based applications using the following configurations.

```
<repository>
    <id>AsposeJavaAPI</id>
    <name>Aspose Java API</name>
    <url>https://repository.aspose.com/repo/</url>
</repository>
```
```
<dependency>
    <groupId>com.aspose</groupId>
    <artifactId>aspose-cad</artifactId>
    <version>20.10</version>
    <classifier>jdk16</classifier>
</dependency>
```

## DWG or DXF to PDF Java Conversion {#Convert-DWG/DXF-to-PDF-using-Java}

The following are the steps to convert a DWG or DXF file to PDF using Aspose.CAD for Java.

*   Load the DWG or DXF file using the [Image][15] class.
*   Create an object of [PdfOptions][16] class.
*   Save CAD drawing as PDF using [Image.save(String, ImageOptionsBase)][17] method.

The following code sample shows how to convert DWG to PDF using Java.

{{< gist aspose-com-gists 8b30a88663eafaa11a640c18e5eed690 "convert-dwg-to-pdf.java" >}}

## Java DWG or DXF to PDF - Set Canvas Size {#Set-Canvas-Size-in-DWG/DXF-to-PDF-using-Java}

Aspose.CAD for Java also allows you to set the canvas size when converting CAD to PDF. Thus, you can specify the size of the pages in the converted PDF document. The following are the steps to perform this operation.

*   Load the CAD's DWG or DXF file using the [Image][18] class.
*   Create an instance of [CadRasterizationOptions][19] class.
*   Set page's width and height using [setPageWidth][20] and [setPageHeight][21] methods respectively.
*   Create an object of [PdfOptions][22] class.
*   Use [PdfOptions.setVectorRasterizationOptions()][23] method to set _CadRasterizationOptions_.
*   Convert DWG or DXF to PDF using [Image.save(String, ImageOptionsBase)][24] method.

The following code sample shows how to set canvas size in DWG or DXF to PDF conversion in Java.

{{< gist aspose-com-gists 8b30a88663eafaa11a640c18e5eed690 "convert-dwg-to-pdf-page-dimensions.java" >}}

## Auto-Scaling in CAD to PDF in Java {#Auto-Scaling-in-CAD-to-PDF-in-Java}

You can also perform auto-scaling of the pages in CAD to PDF conversion. This feature becomes useful when the layers in the CAD drawing have different dimensions. The auto-scaling feature scales the layers according to the unified page size in the PDF. The following are the steps to perform auto-scaling.

*   Load the CAD file using the [Image][25] class.
*   Create an instance of [CadRasterizationOptions][26] class.
*   Set [CadRasterizationOptions.setAutomaticLayoutsScaling][27] to _true_.
*   Create an instance of [PdfOptions][28] class and set [PdfOptions.setVectorRasterizationOptions][29].
*   Convert CAD drawing to PDF using [Image.save(String, ImageOptionsBase)][30] method.

The following code sample shows how to convert DWG to PDF with auto-scaling.

{{< gist aspose-com-gists 8b30a88663eafaa11a640c18e5eed690 "convert-dwg-to-pdf-auto-scaling.java" >}}

## Java CAD to PDF - Set Background and Drawing Color {#Set-Background-and-Drawing-Color-in-CAD-to-PDF}

By default, the CAD drawings are rendered in black and white colors in the PDF. However, you can override this feature and set your desired background and drawing colors. The following are the steps to achieve this.

*   Load the DWG or DXF file using the [Image][31] class.
*   Create an instance of [CadRasterizationOptions][32] class.
*   Set background color using [CadRasterizationOptions.setBackgroundColor][33] method.
*   Set drawing color using [CadRasterizationOptions.setDrawColor][34] method.
*   Create an object of [PdfOptions][35] class and set [PdfOptions.setVectorRasterizationOptions][36].
*   Convert DWG or DXF to PDF using [Image.save(String, ImageOptionsBase)][37] method.

The following code sample shows how to modify colors in DWG or DXF to PDF conversion using Java.

{{< gist aspose-com-gists 8b30a88663eafaa11a640c18e5eed690 "convert-dwg-to-pdf-modify-colors.java" >}}

## Convert Specific Layers of CAD to PDF using Java {#Convert-Specific-Layers-of-CAD-to-PDF-using-Java}

CAD drawings usually consist of multiple layers and in certain cases, you may need to convert only the selected layers of the drawing to PDF. For this, you can provide a list of layers to be converted using the [CadRasterizationOptions.setLayers()][38] method. The following code sample shows how to convert a specific layer in CAD to PDF conversion.

{{< gist aspose-com-gists 8b30a88663eafaa11a640c18e5eed690 "convert-layer-to-pdf.java" >}}

## Conclusion

In this article, you have learned how to convert CAD's DWG and DXF files to PDF using Java. Furthermore, you have seen various scenarios in which you can customize the CAD to PDF conversion as desired. You can explore more about Aspose's CAD API using [documentation][39].

## See Also

*   [Convert DWG/DXF to PNG, JPEG, BMP, TIFF, and GIF in C#][40]




[1]: https://docs.fileformat.com/cad/
[2]: https://docs.fileformat.com/cad/dwg/
[3]: https://docs.fileformat.com/cad/dxf/
[4]: https://docs.fileformat.com/cad/
[5]: https://docs.fileformat.com/cad/dwg/
[6]: https://docs.fileformat.com/cad/dxf/
[7]: #Java-CAD-to-PDF-Converter-API
[8]: #Convert-DWG/DXF-to-PDF-using-Java
[9]: #Set-Canvas-Size-in-DWG/DXF-to-PDF-using-Java
[10]: #Auto-Scaling-in-CAD-to-PDF-in-Java
[11]: #Set-Background-and-Drawing-Color-in-CAD-to-PDF
[12]: #Convert-Specific-Layers-of-CAD-to-PDF-using-Java
[13]: https://products.aspose.com/cad/java
[14]: https://downloads.aspose.com/cad/java
[15]: https://apireference.aspose.com/cad/java/com.aspose.cad/Image
[16]: https://apireference.aspose.com/cad/java/com.aspose.cad.imageoptions/PdfOptions
[17]: https://apireference.aspose.com/cad/java/com.aspose.cad/Image#save-java.lang.String-com.aspose.cad.ImageOptionsBase-
[18]: https://apireference.aspose.com/cad/java/com.aspose.cad/Image
[19]: https://apireference.aspose.com/cad/java/com.aspose.cad.imageoptions/CadRasterizationOptions
[20]: https://apireference.aspose.com/cad/java/com.aspose.cad.imageoptions/VectorRasterizationOptions#setPageWidth-float-
[21]: https://apireference.aspose.com/cad/java/com.aspose.cad.imageoptions/VectorRasterizationOptions#setPageHeight-float-
[22]: https://apireference.aspose.com/cad/java/com.aspose.cad.imageoptions/PdfOptions
[23]: https://apireference.aspose.com/cad/java/com.aspose.cad/ImageOptionsBase#setVectorRasterizationOptions-com.aspose.cad.imageoptions.VectorRasterizationOptions-
[24]: https://apireference.aspose.com/cad/java/com.aspose.cad/Image#save-java.lang.String-com.aspose.cad.ImageOptionsBase-
[25]: https://apireference.aspose.com/cad/java/com.aspose.cad/Image
[26]: https://apireference.aspose.com/cad/java/com.aspose.cad.imageoptions/CadRasterizationOptions
[27]: https://apireference.aspose.com/cad/java/com.aspose.cad.imageoptions/CadRasterizationOptions#setAutomaticLayoutsScaling-boolean-
[28]: https://apireference.aspose.com/cad/java/com.aspose.cad.imageoptions/PdfOptions
[29]: https://apireference.aspose.com/cad/java/com.aspose.cad/ImageOptionsBase#setVectorRasterizationOptions-com.aspose.cad.imageoptions.VectorRasterizationOptions-
[30]: https://apireference.aspose.com/cad/java/com.aspose.cad/Image#save-java.lang.String-com.aspose.cad.ImageOptionsBase-
[31]: https://apireference.aspose.com/cad/java/com.aspose.cad/Image
[32]: https://apireference.aspose.com/cad/java/com.aspose.cad.imageoptions/CadRasterizationOptions
[33]: https://apireference.aspose.com/cad/java/com.aspose.cad.imageoptions/VectorRasterizationOptions#setBackgroundColor-com.aspose.cad.Color-
[34]: https://apireference.aspose.com/cad/java/com.aspose.cad.imageoptions/VectorRasterizationOptions#setDrawColor-com.aspose.cad.Color-
[35]: https://apireference.aspose.com/cad/java/com.aspose.cad.imageoptions/PdfOptions
[36]: https://apireference.aspose.com/cad/java/com.aspose.cad/ImageOptionsBase#setVectorRasterizationOptions-com.aspose.cad.imageoptions.VectorRasterizationOptions-
[37]: https://apireference.aspose.com/cad/java/com.aspose.cad/Image#save-java.lang.String-com.aspose.cad.ImageOptionsBase-
[38]: https://apireference.aspose.com/cad/java/com.aspose.cad.imageoptions/CadRasterizationOptions#setLayers-java.util.List-
[39]: https://docs.aspose.com/cad/java/getting-started/
[40]: https://blog.aspose.com/2020/09/28/dwg-dxf-to-png-jpeg-bmp-tiff-gif-using-csharp/






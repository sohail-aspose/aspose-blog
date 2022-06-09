---
title: 'Convert DWF to PNG or JPG Image in Java'
seoTitle: "Convert DWF to PNG or JPG JPEG Image File in Java"
description: "Convert DWF to PNG or JPG file programmatically in Java. Export DWF to PNG JPEG Image within your Java based applications."
date: Thu, 30 Dec 2021 08:15:00 +0000
draft: false
url: /2021/12/30/convert-dwf-to-jpg-png-image-java/
author: Farhan Raza
summary: 'DWF files contain 2D or 3D drawings in compressed format. In certain situations, you might need to convert DWF to an image. Considering that perspective, the article covers how to convert a DWF file to a JPG or PNG image programmatically using Java.'
tags: ['DWF to JPG Image', 'DWF to JPG Java', 'DWF to PNG Image', 'DWF to PNG Java']
categories: ['Aspose.CAD Product Family']
---



{{< figure align=center src="images/DWF-to-JPG-PNG-1.jpg" alt="DWF to JPG PNG Java">}}


[DWF][1] files contain 2D or 3D drawings in compressed format. In certain situations, you might need to convert DWF to an image. Considering that perspective, the article covers how to convert a DWF file to a [JPG][2] or [PNG][3] image programmatically using Java.

*   [DWF to JPG or PNG Image Converter – Java API Installation][4]
*   [Convert DWF to JPG Image Programmatically in Java][5]
*   [Convert DWF to PNG Image Programmatically in Java][6]

## DWF to JPG or PNG Image Converter – Java API Installation {#section1}

[Aspose.CAD for Java][7] API can be used to create, edit, or manipulate CAD files without even needing to install CAD applications. Simply install the API by downloading its JAR file from the [Downloads][8] section or using the Maven configurations below:

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
        <version>21.11</version>        
   </dependency>
</dependencies>
```

## Convert DWF to JPG Image Programmatically in Java {#section2}

You can convert a DWF file to a JPG image with the following steps:

1.  Firstly, load source DWF file with the [Image][9] class constructor.
2.  Initialize [CadRasterizationOptions][10] class object.
3.  Create an instance of [JpegOptions][11] type.
4.  Save the output JPG image using [VectorRasterizationOptions][12].

The following code snippet elaborates how to convert a DWF file to a JPG image in Java:

{{< gist aspose-com-gists 3c3b7cc7aac450ec575551b623dd4172 "DWF-to-JPG.java" >}}

## Convert DWF to PNG Image Programmatically in Java {#section3}

You can convert a DWF file to a PNG image with the following steps:

1.  Load the input DWF file using the [Image][13] class.
2.  Initialize an object of [CadRasterizationOptions][14] class.
3.  Create [PngOptions][15] class object.
4.  Finally, save the output PNG image with [VectorRasterizationOptions][16].

The code snippet below shows how to convert a DWF to a PNG image in Java:

{{< gist aspose-com-gists 3c3b7cc7aac450ec575551b623dd4172 "DWF-to-PNG.java" >}}

## Get Free Temporary License

You can test the API in its full capacity by requesting a [free temporary license][17].

## Conclusion

In this article, you have learned how to convert a DWF file to an image as a JPG or PNG file programmatically in Java. You may take a look at the [documentation][18] section to explore other features supported by the API. Furthermore, feel free to reach out to us at the [forum][19] in case of any concerns.

## See Also

[Convert CFF to PDF Programmatically in Java][20]




[1]: https://docs.fileformat.com/cad/dwf/
[2]: https://docs.fileformat.com/image/jpeg/
[3]: https://docs.fileformat.com/image/png/
[4]: #section1
[5]: #section2
[6]: #section3
[7]: https://products.aspose.com/cad/java/
[8]: https://downloads.aspose.com/cad/java
[9]: https://apireference.aspose.com/cad/java/com.aspose.cad/Image
[10]: https://apireference.aspose.com/cad/java/com.aspose.cad.imageoptions/CadRasterizationOptions
[11]: https://apireference.aspose.com/cad/java/com.aspose.cad.imageoptions/JpegOptions
[12]: https://apireference.aspose.com/cad/java/com.aspose.cad.imageoptions.class-use/vectorrasterizationoptions
[13]: https://apireference.aspose.com/cad/java/com.aspose.cad/Image
[14]: https://apireference.aspose.com/cad/java/com.aspose.cad.imageoptions/CadRasterizationOptions
[15]: https://apireference.aspose.com/cad/java/com.aspose.cad.imageoptions/PngOptions
[16]: https://apireference.aspose.com/cad/java/com.aspose.cad.imageoptions.class-use/vectorrasterizationoptions
[17]: https://purchase.aspose.com/temporary-license
[18]: https://docs.aspose.com/cad/java/
[19]: https://forum.aspose.com/c/cad
[20]: https://blog.aspose.com/2021/12/06/convert-cff-to-pdf-java/





---
title: 'Convert IFC to JPG or PNG Image using Java'
seoTitle: "Convert IFC to JPG or PNG Image Programmatically using Java"
description: "Convert IFC file to a JPG or PNG raster image programmatically using Java. Export or change IFC file to different images for preview."
date: Sat, 02 Oct 2021 18:13:00 +0000
draft: false
url: /2021/10/02/convert-ifc-to-png-jpg-image-java/
author: Farhan Raza
summary: 'IFC files are used to model different buildings for construction purposes. In certain situations, you might want to convert an IFC file to a JPG or PNG image to display the model on different operating systems. This article explains **how to convert an IFC file to an image programmatically using Java.**'
tags: ['Convert IFC to Image in Java', 'IFC to JPG', 'IFC to JPG in Java', 'IFC to PNG', 'IFC to PNG in Java']
categories: ['Aspose.CAD Product Family']
---



{{< figure align=center src="images/IFC-to-Image-1.jpg" alt="IFC to JPG PNG">}}


[IFC][1] files are used to model different buildings for construction purposes. In certain situations, you might want to convert an IFC file to a [JPG][2] or [PNG][3] image to display the model on different operating systems. This article explains how to convert an IFC file to an image programmatically using Java.

*   [IFC to JPG or PNG Image Converter – Java API Installation][4]
*   [Convert IFC File to JPG Image Programmatically with Java][5]
*   [Convert IFC to PNG Image Programmatically using Java][6]

## IFC to JPG or PNG Image Converter – Java API Installation

[Aspose.CAD for Java][7] API supports converting IFC files to an image. Please configure the API by downloading the JAR file from the [New Releases][8] section or with the following Maven configurations:

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
        <version>21.8</version>        
   </dependency>
</dependencies>
```

## Convert IFC File to JPG Image Programmatically using Java

You can convert an IFC file to a JPG image with the following steps:

1.  Firstly, load source IFC file with the [Image][9] class constructor.
2.  Initialize [CadRasterizationOptions][10] class object.
3.  Create an instance of [JpegOptions][11] type.
4.  Convert the IFC to JPG image with [VectorRasterizationOptions][12].

The code snippet below shows how to convert an IFC file to a JPG image using Java:

{{< gist aspose-com-gists ca5756248317606c919feedbe045c5b5 "IFC-to-JPG.java" >}}

## Convert IFC to PNG Image with Java

You can convert an IFC file to a PNG image with the steps below:

1.  Load source IFC file with the [Image][13] class.
2.  Initialize an object of [CadRasterizationOptions][14] class.
3.  Instantiate [PngOptions][15] class object.
4.  Finally, convert IFC to PNG image using [VectorRasterizationOptions][16].

The following code sample explains how to convert an IFC file to a PNG image with Java:

{{< gist aspose-com-gists ca5756248317606c919feedbe045c5b5 "IFC-to-PNG.java" >}}

## Get Free Temporary License

You can request a [free temporary license][17] and test the API without any evaluation limitation.

## Conclusion

In conclusion, you have explored how to convert an IFC file to an image in JPG or PNG format with Java. Please visit the [documentation][18] section to learn the different other features of the API. Moreover, please feel free to write to us at the [free support forum][19] in case of any queries.

## See Also

[Convert DGN to JPEG, PNG, or TIFF Image with Java][20]




[1]: https://docs.fileformat.com/cad/ifc/
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
[20]: https://blog.aspose.com/2021/09/10/convert-dgn-to-png-jpeg-tiff-java/





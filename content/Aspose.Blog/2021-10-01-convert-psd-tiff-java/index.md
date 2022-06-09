---
title: 'Convert PSD to TIFF Image Programmatically with Java'
seoTitle: "Convert PSD to TIFF Image Programmatically with Java | PSD Converter"
description: "Convert a PSD file to a TIFF image programmatically using Java. PSD Converter with Advanced options lets you set different properties of PSD & TIFF."
date: Fri, 01 Oct 2021 17:16:00 +0000
draft: false
url: /2021/10/01/convert-psd-tiff-java/
author: Farhan Raza
summary: 'Images are often designed using Photoshop application. The output files are in the PSD format that can be opened or edited with a few programs. So you might need to convert a PSD file to a TIFF image programmatically using Java. The following sections explain the PSD conversion.'
tags: ['Convert PSD to TIFF', 'Convert PSD to TIFF in Java', 'PSD to TIFF', 'PSD to TIFF Image']
categories: ['Aspose.PSD Product Family']
---



{{< figure align=center src="images/PSD-to-TIFF.jpg" alt="PSD to TIFF">}}


Images are often designed using Photoshop application. The output files are in the PSD format that can be opened or edited with a few programs. So you might need to convert a [PSD][1] file to a [TIFF][2] image programmatically using Java. The following sections explain the PSD conversion:

*   [PSD to TIFF Image Converter – Java API Installation][3]
*   [Convert PSD to TIFF Image Programmatically using Java][4]
*   [Convert PSD to TIFF Image with Compression in Java][5]

## PSD to TIFF Image Converter – Java API Installation {#section1}

[Aspose.PSD for Java][6] API can be used to process Photoshop and image formats programmatically in your applications. You can quickly set up the API by downloading the JAR file from the [Downloads][7] section or with the following configurations in pom.xml file of your project:

### Repository```
<repository>
    <id>AsposeJavaAPI</id>
    <name>Aspose Java API</name>
    <url>http://repository.aspose.com/repo/</url>
</repository>
```

### Dependency```
<dependency>
     <groupId>com.aspose</groupId>
     <artifactId>aspose-psd</artifactId>
     <version>21.7</version>
     <classifier>jdk16</classifier>
</dependency>
```

## Convert PSD to TIFF Image Programmatically using Java {#section2}

You can convert a PSD file to a TIFF image with the following steps:

1.  Load an existing PSD image using the [Image][8] class.
2.  Create an instance of [TiffOptions][9] class.
3.  Convert the PSD file to TIFF image with the [Save][10] method.

The following code shows how to convert a PSD file to a TIFF image programmatically using Java:

{{< gist aspose-com-gists 6c6ccd35a9d4cda3d945e766554b9ae6 "PSD-to-TIFF.java" >}}

## Convert PSD to TIFF Image with Compression in Java {#section3}

You can convert a PSD file to a TIFF image with advanced options. Different options for specifying the compression type, bits per sample, etc. are exposed by the [TiffOptions][11] class. Please follow the steps below for converting a PSD file to TIFF with compression:

1.  Load a PSD file as an image and cast it into [PsdImage][12] object.
2.  Create an instance of [TiffOptions][13] for the resultant image.
3.  Set BitsPerSample, Compression, Photometric mode and graycale palette.
4.  Save output TIFF image with compression.

The following code explains how to convert a PSD file to a TIFF image with compression using Java:

{{< gist aspose-com-gists 6c6ccd35a9d4cda3d945e766554b9ae6 "PSD-to-TIFF-Compression.java" >}}

## Get Free Evaluation License

You can request a [Free Evaluation License][14] to test the API in its full capacity.

## Conclusion

In this article, you have learned how to convert a PSD file to a TIFF image. You can also perform image compression while rendering the TIFF image programmatically using Java. Moreover, please refer to [API Documentation][15] to explore several other features of the API. In case of any concerns, please feel free to contact us via the [Free Support Forum][16].

## See Also

*   [Convert PNG or JPG Image to PSD Programmatically using Java][17]
*   [Flatten or Merge the Layers of a PSD File in Java][18]




[1]: https://docs.fileformat.com/image/psd/
[2]: https://docs.fileformat.com/image/tiff/
[3]: #section1
[4]: #section2
[5]: #section3
[6]: https://products.aspose.com/psd/java
[7]: https://downloads.aspose.com/psd/java
[8]: https://apireference.aspose.com/psd/java/com.aspose.psd/Image
[9]: https://apireference.aspose.com/psd/java/com.aspose.psd.imageoptions/TiffOptions
[10]: https://apireference.aspose.com/psd/java/com.aspose.psd/Image#save--
[11]: https://apireference.aspose.com/psd/java/com.aspose.psd.imageoptions/TiffOptions
[12]: https://apireference.aspose.com/psd/java/com.aspose.psd.fileformats.psd/PsdImage
[13]: https://apireference.aspose.com/psd/java/com.aspose.psd.imageoptions/TiffOptions
[14]: https://purchase.aspose.com/temporary-license
[15]: https://docs.aspose.com/psd/java/
[16]: https://forum.aspose.com/c/psd
[17]: https://blog.aspose.com/2021/05/11/convert-png-or-jpg-image-to-psd-programmatically-using-java/
[18]: https://blog.aspose.com/2021/11/09/flatten-merge-layers-in-psd-using-java/





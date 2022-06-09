---
title: 'Convert PUB to Image Programmatically in Java'
seoTitle: "Convert PUB to Image Programmatically in Java | PUB to JPG PNG TIFF"
description: "Convert Microsoft Publisher PUB files to Image like JPG PNG TIFF Programmatically using Java. Export or Change PUB files in Java."
date: Mon, 31 May 2021 17:22:04 +0000
draft: false
url: /2021/05/31/convert-pub-to-image-programmatically-in-java/
author: Farhan Raza
summary: 'Microsoft Publisher Files are used for printing or publishing information. You can convert PUB to JPG, PNG, or TIFF images programmatically using Java. In this article, you will learn how to convert the PUB file to different image formats.'
tags: ['Convert PUB to Image', 'PUB to Image', 'PUB to Image in Java', 'PUB to JPG', 'PUB to JPG in Java', 'PUB to PNG', 'PUB to TIFF']
categories: ['Aspose.PUB Product Family']
---



{{< figure align=center src="images/PUB-to-PNG-JPG-TIF-Image.png" alt="Convert PUB to JPG PNG TIFF Image Java">}}


Microsoft Publisher Files are used for printing or publishing information. You can convert [PUB][1] to [JPG][2], [PNG][3], or [TIFF][4] images programmatically using Java. In this article, you will learn how to convert the PUB file to different image formats:

*   [PUB to Image Conversion – Java API Installation][5]
*   [Convert PUB to JPG Image Programmatically using Java][6]
*   [Convert PUB to PNG Image Programmatically with Java][7]
*   [PUB to TIFF Conversion Programmatically in Java][8]

## PUB to Image Conversion – Java APIs Installation {#section1}

[Aspose.PUB for Java][9] API supports working with PUB files. You can render the PUB files to PDF and then utilize [Aspose.PDF for Java][10] API to convert the output PDF file to image formats like JPG, PNG, TIFF, etc. You can download the JAR files for Aspose.PUB for Java and Aspose.PDF for Java API or specify the following configurations to download the APIs from the [Maven repository][11]:

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
        <artifactId>aspose-pub</artifactId>
        <version>20.8</version>
    </dependency>

    <dependency>
        <groupId>com.aspose</groupId>
        <artifactId>aspose-pdf</artifactId>
        <version>20.5</version>
    </dependency>

</dependencies>
```

## Convert PUB to JPG Image Programmatically using Java {#section2}

You can convert a Microsoft Publisher (PUB) file to JPG image with the following steps:

1.  Load input PUB file.
2.  Convert PUB to PDF file with [convertToPdf][12] method.
3.  Get page dimensions from the PDF document.
4.  Specify the [Resolution][13] and dimensions of the output image.
5.  Save output JPG image using [JpegDevice][14].

The code below explains how to convert PUB to JPG image using Java:

{{< gist aspose-com-gists c4c0ea9a3cf5466d2982fc037cabe802 "PUB-to-JPG.java" >}}

## Convert PUB to PNG Image Programmatically with Java {#section3}

You can convert a PUB file to PNG format image with the steps below:

1.  Load input PUB file with [createParser()][15] method.
2.  Convert PUB to PDF file.
3.  Specify width and height of output image.
4.  Finally, convert PUB to PNG image.

The following code shows how to convert PUB to PNG image with Java:

{{< gist aspose-com-gists c4c0ea9a3cf5466d2982fc037cabe802 "PUB-to-PNG.java" >}}

## PUB to TIFF Conversion Programmatically in Java {#section4}

You can convert PUB file to a TIFF image with the steps listed below:

1.  Firstly, load the input Publisher (PUB) file.
2.  Convert PUB to PDF file using [convertToPdf()][16] method.
3.  Specify properties for TIFF image using [TiffSettings][17] class.
4.  Finally, convert PUB to TIFF image with [TiffDevice][18] instance.

The following code demonstrates how to convert PUB to TIFF image programmatically using Java:

{{< gist aspose-com-gists c4c0ea9a3cf5466d2982fc037cabe802 "PUB-to-TIFF.java" >}}

## Get Free API License

You can evaluate the API in its full capacity by requesting a [Free Temporary License][19].

## Conclusion

In conclusion, you have learned how to convert Microsoft Publisher, PUB, files to different image formats like JPG, PNG, TIFF, etc, programmatically using Java. Moreover, you can learn about more features by visiting the [Documentation][20] of Aspose.PUB for Java API. Furthermore, please feel free to contact us via the [Free Support Forum][21] for any of your concerns.

## See Also

[Recognize Text by Performing OCR on Image from URL with Java][22]




[1]: https://en.wikipedia.org/wiki/PUB_(file_type)
[2]: https://docs.fileformat.com/image/jpeg/
[3]: https://docs.fileformat.com/image/png/
[4]: https://docs.fileformat.com/image/tiff/
[5]: #section1
[6]: #section2
[7]: #section3
[8]: #section4
[9]: https://products.aspose.com/pub/java/
[10]: https://products.aspose.com/pdf/java/
[11]: https://repository.aspose.com/webapp/#/artifacts/browse/tree/General/repo
[12]: https://apireference.aspose.com/pub/java/com.aspose.pub/IPdfConverter#convertToPdf-com.aspose.pub.Document-java.io.OutputStream-
[13]: https://apireference.aspose.com/pdf/java/com.aspose.pdf.devices/resolution
[14]: https://apireference.aspose.com/pdf/java/com.aspose.pdf.devices/JpegDevice
[15]: https://apireference.aspose.com/pub/java/com.aspose.pub/PubFactory
[16]: https://apireference.aspose.com/pub/java/com.aspose.pub/IPdfConverter
[17]: https://apireference.aspose.com/pdf/java/com.aspose.pdf.devices.class-use/tiffsettings
[18]: https://apireference.aspose.com/pdf/java/com.aspose.pdf.devices.class-use/tiffsettings#com.aspose.pdf.devices
[19]: https://purchase.aspose.com/temporary-license
[20]: https://docs.aspose.com/pub/java/
[21]: https://forum.aspose.com/c/pub
[22]: https://blog.aspose.com/2021/05/27/recognize-text-by-performing-ocr-on-image-from-url-with-java/






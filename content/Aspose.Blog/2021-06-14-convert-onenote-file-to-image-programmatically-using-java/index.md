---
title: 'Convert OneNote File to Image Programmatically using Java'
seoTitle: "Convert OneNote File to JPG PNG TIFF Image Programmatically in Java"
description: "Convert Note file to JPG PNG TIFF and other image formats programmatically using Java. Export or change microsoft OneNote files in your applications."
date: Mon, 14 Jun 2021 12:03:00 +0000
draft: false
url: /2021/06/14/convert-onenote-file-to-image-programmatically-using-java/
author: Farhan Raza
summary: 'Creating digital notes is like an everyday activity these days. Many people keep notes including text, drawings, pictures, and much more. You can convert such notes to images programmatically using Java. OneNote file can be rendered to JPG, PNG, as well as TIFF image with different color modes and compressions. The following sections discuss the conversions in detail.'
tags: ['Convert OneNote to Image', 'Convert OneNote to Picture in Java', 'Note to Image', 'Note to JPG', 'Note to PNG', 'Note to TIFF', 'OneNote to Image']
categories: ['Aspose.Note Product Family']
---



{{< figure align=center src="images/OneNote-to-Image.png" alt="OneNote to Image JPG PNG TIFF">}}


Creating digital notes is like an everyday activity these days. Many people keep notes including text, drawings, pictures, and much more. You can convert such notes to images programmatically using Java. OneNote file can be rendered to [JPG][1], [PNG][2], as well as [TIFF][3] image with different color modes and compressions. The following sections discuss the conversions in detail:

*   [OneNote to Image Converter – Java API Installation][4]
*   [Convert OneNote to JPG Image File Programmatically using Java][5]
*   [Convert OneNote to PNG Image Programmatically using Java][6]
*   [OneNote File to Grayscale TIFF Image Conversion in Java][7]
*   [Convert OneNote to TIFF in Black and White Color with Compression using Java][8]

## OneNote to Image Converter – Java API Installation {#section1}

You can convert a OneNote file to an Image with [Aspose.Note for Java][9] API. Simply configure the API by downloading the JAR file from the [New Releases][10] section, or with the following Maven configurations in pom.xml file of your project:

### Repository```
 <repositories>
    <repository>
        <id>AsposeJavaAPI</id>
        <name>Aspose Java API</name>
        <url>https://repository.aspose.com/repo/</url>
    </repository>
</repositories>
```

### Dependency```
 <dependencies>
    <dependency>
        <groupId>com.aspose</groupId>
        <artifactId>aspose-note</artifactId>
        <version>21.5</version>
        <classifier>jdk17</classifier>        
    </dependency>
</dependencies>
```

## Convert OneNote to JPG Image File Programmatically using Java {#section2}

You can convert a OneNote file to JPG image with the following steps:

1.  Load the input Note (.one) file using the Document class.
2.  Save output JPG image.

The code below shows how to convert a .one OneNote file to JPG image programmatically using Java:

{{< gist aspose-com-gists 31355c0db52fee1619cd6cb8488086c8 "OneNote-To-JPG.java" >}}

## Convert OneNote to PNG Image Programmatically using Java {#section3}

You can convert a OneNote file to PNG image with below steps:

1.  Load the input file using Document class.
2.  Initialize ImageSaveOptions class object.
3.  Save the output PNG image.

The following code explains how to convert OneNote file to a PNG image programmatically with Java:

{{< gist aspose-com-gists 31355c0db52fee1619cd6cb8488086c8 "OneNote-to-PNG.java" >}}

## OneNote File to Grayscale TIFF Image Conversion in Java {#section4}

You can convert .one files to image format while specifying the color modes as per your requirements. Please follow the following steps to convert a OneNote file to Grayscale TIFF image:

1.  Load the OneNote file using Document class.
2.  Initialize ImageSaveOptions and specify SaveFormat.
3.  Set color mode for GrayScale TIFF output.
4.  Save output image.

The code below demonstrates how to convert a .ONE file to a TIFF image with GrayScale color scheme programmatically using Java:

{{< gist aspose-com-gists 31355c0db52fee1619cd6cb8488086c8 "Note-to-TIFF-Grayscale.java" >}}

## Convert OneNote to TIFF in Black and White Color with Compression using Java {#section5}

Several compression algorithms are supported by the API and you can convert the OneNote file to black and white tiff image with compression using Java. You need to follow the steps below for converting the .one file to TIFF image:

1.  Load the note file using Document class.
2.  Initialize ImageSaveOptions and SaveFormat objects.
3.  Set ColorMode to Black and White.
4.  Set the compression type specific for the Black and White image.
5.  Finally, save the output TIFF file.

The following code explains how to convert a .ONE file to a black and white TIFF image programmatically with Java:

{{< gist aspose-com-gists 31355c0db52fee1619cd6cb8488086c8 "OneNote-to-tiff-BlackAndWhite-Compression.java" >}}

## Get Free API License

You can request a [Free Temporary License][11] to test the API in full capacity.

## Conclusion

In conclusion, you have learned how to convert OneNote files (.one) to different image formats like PNG, JPG, and TIFF with different color modes and compression algorithms programmatically using Java. Moreover, please take a look at API [Documentation][12] to explore other features. In case of any questions, please feel free to reach out to us at the [Free Support Forum][13].

## See Also

[Find and Replace Text in OneNote (.ONE) File in Java][14]




[1]: https://docs.fileformat.com/image/jpeg/
[2]: https://docs.fileformat.com/image/png/
[3]: https://docs.fileformat.com/image/tiff/
[4]: #section1
[5]: #section2
[6]: #section3
[7]: #section4
[8]: #section5
[9]: https://products.aspose.com/note/java
[10]: https://downloads.aspose.com/note/java
[11]: https://purchase.aspose.com/temporary-license
[12]: https://docs.aspose.com/note/java/
[13]: https://forum.aspose.com/c/note
[14]: https://blog.aspose.com/2021/02/03/find-and-replace-text-in-onenote-one-file-in-java/






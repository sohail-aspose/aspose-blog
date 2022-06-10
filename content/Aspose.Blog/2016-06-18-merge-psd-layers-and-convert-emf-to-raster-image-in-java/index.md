---
title: 'Merge PSD Layers and Convert EMF to Raster Image in Java'
date: Sat, 18 Jun 2016 12:26:59 +0000
draft: false
url: /2016/06/18/merge-psd-layers-and-convert-emf-to-raster-image-in-java/
author: Ikram Haq
summary: ''
tags: []
categories: ['Aspose.Imaging Product Family']
---



{{< figure align=center src="images/aspose_imaging-for-java.jpg" alt="">}}


We are pleased to announce the release of [Aspose.Imaging for Java][1] 3.6.0. The major developments in this release are to convert metafile (Emf/Emf+) to raster image formats and merging PSD layers while converting PSD to JPG.

## Export MetaFile To Raster Formats in Java

Using Aspose.Imaging for Java, developers can convert metafile (Emf/Emf+) to raster formats. Aspose.Imaging for Java provides the EmfImage class to load EMF files and same can be used to convert the PSD to raster formats. Below provided sample code demonstrate how to convert an EMF file to different raster formats.

```
String filePath = "TestEmfBezier.emf";

// Create EmfRasterizationOption class instance and set properties
com.aspose.imaging.imageoptions.EmfRasterizationOptions emfRasterizationOptions = 
        new com.aspose.imaging.imageoptions.EmfRasterizationOptions();

emfRasterizationOptions.setBackgroundColor(com.aspose.imaging.Color.getPapayaWhip());
emfRasterizationOptions.setPageWidth(300);
emfRasterizationOptions.setPageHeight(300);

// Load an existing EMF file as iamge and convert it to EmfImage class object
com.aspose.imaging.fileformats.emf.EmfImage image = 
        (com.aspose.imaging.fileformats.emf.EmfImage)com.aspose.imaging.Image.load(filePath);

// Convert EMF to BMP
com.aspose.imaging.imageoptions.BmpOptions objBMPo = 
        new com.aspose.imaging.imageoptions.BmpOptions();
objBMPo.setVectorRasterizationOptions(emfRasterizationOptions);

image.save(filePath + ".bmp", objBMPo);

// Convert EMF to GIF
com.aspose.imaging.imageoptions.GifOptions objGIFo = 
        new com.aspose.imaging.imageoptions.GifOptions();
objGIFo.setVectorRasterizationOptions(emfRasterizationOptions);

image.save(filePath + ".gif", objGIFo);

// Convert EMF to JPEG
com.aspose.imaging.imageoptions.JpegOptions objJPEGo = 
        new com.aspose.imaging.imageoptions.JpegOptions();
objJPEGo.setVectorRasterizationOptions(emfRasterizationOptions);

image.save(filePath + ".jpeg", objJPEGo );

// Convert EMF to J2K
com.aspose.imaging.imageoptions.Jpeg2000Options objJpeg2o = 
        new com.aspose.imaging.imageoptions.Jpeg2000Options();
objJpeg2o.setVectorRasterizationOptions(emfRasterizationOptions);

image.save(filePath + ".j2k", objJpeg2o);

// Convert EMF to PNG
com.aspose.imaging.imageoptions.PngOptions objPNGo = 
        new com.aspose.imaging.imageoptions.PngOptions();
objPNGo.setVectorRasterizationOptions(emfRasterizationOptions);

image.save(filePath + ".png", objPNGo);

// Convert EMF to PSD
com.aspose.imaging.imageoptions.PsdOptions objPSDo = 
        new com.aspose.imaging.imageoptions.PsdOptions();
objPSDo.setVectorRasterizationOptions(emfRasterizationOptions);

image.save(filePath + ".psd", objPSDo);

// Convert EMF to TIFF
com.aspose.imaging.imageoptions.TiffOptions objTIFFo = 
        new com.aspose.imaging.imageoptions.TiffOptions(TiffExpectedFormat.TiffLzwRgb);
objTIFFo.setVectorRasterizationOptions(emfRasterizationOptions);

image.save(filePath + ".tiff", objTIFFo );

// Convert EMF to WebP
com.aspose.imaging.imageoptions.WebPOptions objWebPo = 
        new com.aspose.imaging.imageoptions.WebPOptions();
objWebPo.setVectorRasterizationOptions(emfRasterizationOptions);

image.save(filePath + ".webp", objWebPo ); 
```

## Merge PSD Layers

Using Aspose.Imaging for Java API, developers can merge layers in a PSD file while converting PSD file to JPG. The following code example demonstrates how to merge layers of a PSD file.

```
String sourceFileName = "5_layers.psd";

//Load an existing PSD file as image
com.aspose.imaging.Image image = com.aspose.imaging.Image.load(sourceFileName);

// Convert the loaded image to PSDImage
com.aspose.imaging.fileformats.psd.PsdImage psdImage = (com.aspose.imaging.fileformats.psd.PsdImage)image;

// create a JPG file stream
java.io.FileInputStream fs = new java.io.FileInputStream("5_layers.jpg");

// Create JPEG option class object
JpegOptions jpgOptions = new JpegOptions();

// call the Save the method of PSDImage class to merge the layers and save it as jpg image.
psdImage.save("5_layers.jpg", jpgOptions);
```

## Enhancements

Following enhancements have been introduced in this release.

*   Process to convert PSD to TIFF format has been improved.
*   Memory management process while rendering metafiles has been improved.

Please refer to the release notes of [Aspose.Imaging for Java 3.6.0][2] for a full view of improvements along with sample code snippets for newly added features. If you are planning to upgrade the API to the latest revision, we strongly suggest you to check the Public API Changes section to know what has been changed in the public API since your current version.

## Aspose.Imaging for Java Resources

The resources, you may need to accomplish your tasks:

*   [Home page for Aspose.Imaging for Java API][3].
*   [Download Aspose.Imaging for Java][4].
*   [Aspose.Imaging for Java online documentation][5] – help documentation and API reference documents.
*   [Aspose.Imaging Product Family Forum][6] – post your technical questions and queries, or any other problem you are facing while working with Aspose.Imaging APIs.
*   [Enable blog Subscription][7] – Do not limit yourself, you can keep yourself updated with the latest news on Aspose.Imaging APIs, new features, fixes and other API related topics by subscribing to Aspose.Imaging blog.
*   [Aspose.Imaging for Java in Online Repository][8] – We have published the JAR files on the Maven repository. Anyone could explore the code examples for learning purposes.

As always we appreciate your feedback so if you ever have anything to tell us about this release or anything else, please head to the [Aspose.Imaging forum][9] for a chat.




[1]: https://products.aspose.com/imaging/java
[2]: https://downloads.aspose.com/imaging/java
[3]: https://products.aspose.com/imaging/java
[4]: https://downloads.aspose.com/imaging/java
[5]: https://docs.aspose.com/display/imagingjava/Home
[6]: http://forum.aspose.com
[7]: https://blog.aspose.com/category/aspose-products/aspose.imaging-product-family/
[8]: http://maven.aspose.com/repository/simple/ext-release-local/com/aspose/aspose-imaging/
[9]: http://forum.aspose.com





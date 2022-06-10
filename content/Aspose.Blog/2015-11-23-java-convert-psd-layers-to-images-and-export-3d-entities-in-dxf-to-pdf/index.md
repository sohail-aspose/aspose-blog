---
title: 'Convert PSD Layers to Raster Images and Export 3D Entities in DXF to PDF using Java'
date: Mon, 23 Nov 2015 09:42:55 +0000
draft: false
url: /2015/11/23/java-convert-psd-layers-to-images-and-export-3d-entities-in-dxf-to-pdf/
author: Ikram Haq
summary: ''
tags: []
categories: ['Aspose.Imaging Product Family']
---



{{< figure align=center src="images/aspose_imaging-for-java.jpg" alt="">}}


We are pleased to announce the release of Aspose.Imaging for Java 3.1.0. This release allows you to convert PSD layers to PNG, JPEG and TIFF image formats. Support to export 3D entities while converting DXF to PDF has also been incorporated in this release.

## Convert PSD Layers to Raster Images in Java

Using Aspose.Imaging for Java, developers can [convert PSD layers to PNG, JPEG and TIFF images][1]. Further, an exception with an appropriate message will be thrown in case of an unsupported layer. Following is the code snippet demonstrating how PSD layers can be converted to a PNG image.

```
// Create an instance of Image class
com.aspose.imaging.Image image = com.aspose.imaging.Image.load(sourceFileName);
        
// Cast image object to PSD image
com.aspose.imaging.fileformats.psd.PsdImage psdImage = (com.aspose.imaging.fileformats.psd.PsdImage)image;
    
// Create an instance of PngOptions class
PngOptions pngOptions = new PngOptions();
pngOptions.setColorType(com.aspose.imaging.fileformats.png.PngColorType.TruecolorWithAlpha);

// Access the list of layers in the PSD image object
com.aspose.imaging.fileformats.psd.layers.Layer[] allLayers = psdImage.getLayers();
        
for (int i = 0; i < allLayers.length; i++)
{
     // convert and save the layer to PNG file format.
     allLayers[i].save("layer" + i + 1 + ".png" , pngOptions);
}
```

## Export 3D Entities while Converting DXF to PDF

Aspose.Imaging for Java now enables the developers to export 3D entities while converting a DXF file to PDF file format. TypeOfEntities enumeration now has an integer value Entities3D. Setting TypeOfEntities property of the CadRasterizationOptions class will export the 3D entities to PDF.  
Following is the code demonstration of the said functionality.

```
// Create an instance of CadImage class and load the DXF file.
CadImage cadImage = (CadImage)Image.Load(fileName);

// Create an instance of CadRasterizationOptions class
CadRasterizationOptions rasterizationOptions = new CadRasterizationOptions();
rasterizationOptions.setPageWidth(1600);
rasterizationOptions.setPageHeight(1600);

// Set the Entities type property to Entities3D.
rasterizationOptions.setTypeOfEntities(TypeOfEntities.Entities3D);
rasterizationOptions.setScaleMethod(ScaleType.GrowToFit);

// Set Layouts
String[] sModelName = { "Model" };

rasterizationOptions.setLayouts(sModelName);

// Create an instance of PDF options class
PdfOptions pdfOptions = new PdfOptions();
pdfOptions.setVectorRasterizationOptions(rasterizationOptions);

// Export to PDF by calling the Save method.                    
string outPath = fileName + ".pdf";
cadImage.Save(outPath, pdfOptions);
```

## Enhancements

Conversion of DWG to PDF and exception handling were already supported, however, conversion and exception handling processes have been improved further.

*   EMF to PNG conversion functionality has been improved.
*   Converting color space from RGB to CMYK has been improved for JPEG images.
*   DWG to PDF functionality has been improved.
*   DWG to raster images functionality has been improved.
*   Maintaining image quality while resizing has been improved.
*   The functionality of HorizontalResolution & VerticalResolution properties have been improved.

Please refer to the release notes of [Aspose.Imaging for Java 3.1.0][2] for a full view of improvements along with sample code snippets for newly added features. If you are planning to upgrade the API to the latest revision, we strongly suggest you to check the Public API Changes section to know what has been changed in the public API since your current version.

## Aspose.Imaging for Java Resources

The resources, you may need to accomplish your tasks:

*   [Home page for Aspose.Imaging for Java API][3].
*   [Download Aspose.Imaging for Java][4].
*   [Aspose.Imaging for Java online documentation][5] – help documentation and API reference documents.
*   [Aspose.Imaging Product Family Forum][6] – post your technical questions and queries, or any other problem you are facing while working with Aspose.Imaging APIs.
*   [Enable blog Subscription][7] – Do not limit yourself, you can keep yourself updated with the latest news on Aspose.Imaging APIs, new features, fixes, and other API related topics by subscribing to Aspose.Imaging blog.
*   [Aspose.Imaging for Java in Online Repository][8] – We have published the JAR files on the Maven repository. Anyone could explore the code examples for learning purposes.

As always we appreciate your feedback so if you ever have anything to tell us about this release or anything else, please head to the [Aspose.Imaging forum][9] for a chat.




[1]: https://docs.aspose.com/display/psdjava/Manipulating+TIFF+Images
[2]: https://downloads.aspose.com/imaging/java
[3]: https://www.aspose.com/products/imaging/java
[4]: https://downloads.aspose.com/imaging/java
[5]: https://docs.aspose.com/display/imagingjava/Home
[6]: https://www.aspose.com/community/forums/aspose.imaging-product-family/498/showforum.aspx
[7]: https://blog.aspose.com/category/aspose-products/aspose.imaging-product-family/
[8]: http://maven.aspose.com/repository/simple/ext-release-local/com/aspose/aspose-imaging/
[9]: https://www.aspose.com/community/forums/aspose.imaging-product-family/498/showforum.aspx





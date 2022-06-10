---
title: 'Adjust CAD Drawing Size using Java API'
date: Fri, 24 Feb 2017 19:10:57 +0000
draft: false
url: /2017/02/24/adjust-autocad-drawing-size-using-java-autocad-file-manipulation-api/
author: Ikram Haq
summary: ''
tags: []
categories: ['Aspose.CAD Product Family']
---

We are pleased to announce that [Aspose.CAD for Java][1] 17.02 has been released. The major development in this release is the support for DWG 2007(AC1021) Format. This release supports determining the DWG external references and their file paths. The support for adjusting CAD drawing size has also been incorporated in this release.

## Adjust CAD Drawing Size using Java

Aspose.CAD for Java provides the setUnitType property to adjust the size of drawing during conversion of the CAD format. There are two ways to adjust the drawing size.

*   Automatic adjust size.
*   Adjust size using UnitType enumeration

UnitType enumeration gives the ability to adjust scaling when Width & Height properties are not set. Below provided code snippet demonstrate how to use UnitType.

```
 // Path to source file
String sourceFilePath = "sample.dwg";

// Load a CAD drawing in an instance of Image
com.aspose.cad.Image objImage = com.aspose.cad.Image.load("sourceFilePath");

// Create an instance of BmpOptions class
com.aspose.cad.imageoptions.BmpOptions bmpOptions = new com.aspose.cad.imageoptions.BmpOptions();

// Create an instance of CadRasterizationOptions and set its various properties
com.aspose.cad.imageoptions.CadRasterizationOptions cadRasterizationOptions = 
        new com.aspose.cad.imageoptions.CadRasterizationOptions();

bmpOptions.setVectorRasterizationOptions(cadRasterizationOptions);
cadRasterizationOptions.setCenterDrawing(true);

// Set the UnitType property
cadRasterizationOptions.setUnitType(com.aspose.cad.imageoptions.UnitType.Centimenter);

// Set the layouts property
cadRasterizationOptions.setLayouts( new String[] { "Model" } );

// Export layout to BMP format
String outPath = sourceFilePath + ".bmp";
objImage.save(outPath, bmpOptions); 
```

## Enhancements

Following enhancements have been introduced in this release.

*   Processing of entity order for DWG format has been improved.
*   Processing of converting DWG to PDF format has been improved.
*   Process of exporting external raster images linked with DWG file has been improved.

To view a complete list of new features and to download the latest release, please visit [Aspose.CAD for Java 17.02][2] page in downloads section.

## Aspose.CAD for Java Resources

The resources, you may need to accomplish your tasks:

*   [Homepage for Aspose.CAD for Java API][3]
*   [Download Aspose.CAD for Java][4]
*   [Aspose.CAD for Java Docs][5] – Help documentation
*   [Aspose.CAD Product Family Forum][6] – Post your technical questions and queries, or any other problem you faced while running Aspose.CAD APIs.
*   [Enable Email Subscription][7] – Don’t limit yourself, you can keep yourself updated with the latest news on Aspose.CAD APIs and new features, fixes, plus other API related topics by subscribing to Aspose.CAD blog.
*   [Aspose.CAD for Java Examples][8] – We have published our code examples on the social coding website GitHub.com. Anyone can explore the code examples for learning purposes.




[1]: https://products.aspose.com/cad/java
[2]: https://downloads.aspose.com/cad/java
[3]: https://products.aspose.com/cad/java
[4]: https://downloads.aspose.com/cad/java
[5]: https://docs.aspose.com/cad/java
[6]: http://forum.aspose.com
[7]: https://blog.aspose.com/category/aspose-products/aspose.cad-product-family/
[8]: https://github.com/aspose-cad/Aspose.CAD-for-Java





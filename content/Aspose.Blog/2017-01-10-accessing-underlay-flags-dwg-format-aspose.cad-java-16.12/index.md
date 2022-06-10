---
title: 'Accessing Underlay Flags for DWG Files using Java'
date: Tue, 10 Jan 2017 09:39:31 +0000
draft: false
url: /2017/01/10/accessing-underlay-flags-dwg-format-aspose.cad-java-16.12/
author: Ikram Haq
summary: ''
tags: []
categories: ['Aspose.CAD Product Family']
---

We are pleased to announce that [Aspose.CAD for Java][1] 16.12 has been released. The major development in this release is the implementation of the feature [drawing DGN format as a part of DWG format][2]. [Underlay flags for DWG format][3] are implementation in this release. Reading insert coordinate and rotation angle for DGN underlay feature also been incorporated in this release.

## Accessing underlay Flags for DWG Format in Java

Aspose.CAD for .NET has implemented the underlay flags for DWG format and allow developers to access them. Following is the simple code demonstration.

```
// Input file name and path
String fileName = getDwgFile("BlockRefDgn.dwg");

// Load an existing DWG file and convert it into CadImage 
CadImage image = (CadImage)Image.load(fileName);

// Go through each entity inside the DWG file
for (CadBaseEntity entity : image.getEntities())
{

   // Check if entity is of CadDgnUnderlay type
    if (entity instanceof CadDgnUnderlay)
    {
        // Access different underlay flags
        CadUnderlay underlay = (CadUnderlay) entity;
        System.out.println(underlay.getUnderlayPath());
        System.out.println(underlay.getUnderlayName());
        System.out.println(underlay.getInsertionPoint().getX());
        System.out.println(underlay.getInsertionPoint().getY());
        System.out.println(underlay.getRotationAngle());
        System.out.println(underlay.getScaleX());
        System.out.println(underlay.getScaleY());
        System.out.println(underlay.getScaleZ());
        System.out.println((underlay.getFlags() & UnderlayFlags.UnderlayIsOn) == UnderlayFlags.UnderlayIsOn);
        System.out.println((underlay.getFlags() & UnderlayFlags.ClippingIsOn) == UnderlayFlags.ClippingIsOn);
        System.out.println((underlay.getFlags() & UnderlayFlags.Monochrome) != UnderlayFlags.Monochrome);
        break;
    }
}
```

## Drawing DGN Format As Part of DWG

Aspose.CAD for .NET allows you to export a DWG file with embedded DGN underlay inside. Following is the code demonstrating how to access the DGN underlay inside a DWG file while exporting a DWG file.

```
 // Input and Output file paths
String fileName = getDwgFile("BlockRefDgn.dwg");
String outPath = getFileFromDesktop("BlockRefDgn.dwg.pdf");

// Create an instance of PdfOptions class as we are exporting the DWG file to PDF format
PdfOptions exportOptions = new PdfOptions();

// Load any existing DWG file as image and convert it to CadImage type
CadImage cadImage = (CadImage)Image.load(fileName);

// Go through each entity inside the DWG file
for (CadBaseEntity baseEntity : cadImage.getEntities())
{
    // Check if entity is an image definition
    if (baseEntity.getTypeName() == CadEntityTypeName.DGNUNDERLAY)
    {
        CadDgnUnderlay dgnFile = (CadDgnUnderlay)baseEntity;

        // Get external reference to object
        System.out.println(dgnFile.getUnderlayPath());
    }
}

// Define settings for CadRasterizationOptions object
CadRasterizationOptions vectorRasterizationOptions = new CadRasterizationOptions();
vectorRasterizationOptions.setPageWidth(1600);
vectorRasterizationOptions.setPageHeight(1600);
vectorRasterizationOptions.setCenterDrawing(true);
vectorRasterizationOptions.setLayouts(new String[] { "Model" });
vectorRasterizationOptions.setScaleMethod(ScaleType.None);
vectorRasterizationOptions.setBackgroundColor(Color.getBlack());
vectorRasterizationOptions.setDrawType(CadDrawTypeMode.UseObjectColor);

// Set Vector Rasterization Options
exportOptions.setVectorRasterizationOptions(vectorRasterizationOptions);

// Export the DWG to PDF by calling Save method
cadImage.save(outPath, exportOptions); 
```

## Enhancements

The following enhancements have been introduced in this release.

*   Process of loading DWG file has been improved.
*   Process of converting DWG to PDF format has been improved.
*   Process of converting DWG to PNG format in multithreading has been improved.

To view a complete list of new features and to download the latest release, please visit [Aspose.CAD for Java 16.12 page in downloads section][4].

## Aspose.CAD for Java Resources

The resources, you may need to accomplish your tasks:

*   [Homepage for Aspose.CAD for Java API][5]
*   [Download Aspose.CAD for Java][6]
*   [Aspose.CAD for Java Wiki Docs][7] – Help documentation
*   [Aspose.CAD Product Family Forum][8] – Post your technical questions and queries, or any other problem you faced while running Aspose.CAD APIs.
*   [Enable Email Subscription][9] – Don’t limit yourself, you can keep yourself updated with the latest news on Aspose.CAD APIs and new features, fixes, plus other API related topics by subscribing to Aspose.CAD blog.
*   [Aspose.CAD for Java Examples][10] – We have published our code examples on the social coding website GitHub.com. Anyone can explore the code examples for learning purposes.




[1]: https://products.aspose.com/cad/java
[2]: https://docs.aspose.com/cad/java/dgn-drawing/
[3]: https://docs.aspose.com/cad/java/dgn-drawing/#3d-entities-support-for-dgn-v7
[4]: http://www.aspose.com/downloads/cad/java
[5]: https://www.aspose.com/products/cad/java
[6]: https://downloads.aspose.com/cad/java
[7]: https://docs.aspose.com/cad/java/
[8]: http://forum.aspose.com
[9]: https://blog.aspose.com/category/aspose-products/aspose.cad-product-family/
[10]: https://github.com/aspose-cad/Aspose.CAD-for-Java





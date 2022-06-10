---
title: 'Search Text in DWG and Convert DGN to PDF or Images with Aspose.CAD for Java 1.1.0'
date: Thu, 29 Sep 2016 12:35:44 +0000
draft: false
url: /2016/09/29/search-text-in-dwg-file-and-dgn-file-conversion-with-aspose.cad-for-java-1.1.0/
author: Ikram Haq
summary: ''
tags: ['Convert DNG to Image', 'Convert DNG to PDF', 'Search Text in DWG in Java']
categories: ['Aspose.CAD Product Family']
---



{{< figure align=center src="images/aspose_cad-for-java-100x100.png" alt="">}}


We are pleased to announce that Aspose.CAD for Java 1.1.0 has been released. The major developments in this release are the ability to [search text within the DWG file][1] and support to [convert DGN file to PDF][2] & [raster image formats][3]. This release also supports to [retrieve block attribute values][4] from within a DWG file and its external references.

## Search Text in DWG File

Aspose.CAD for Java API allows you to [search text in a DWG AutCAD file][5]. Aspose.CAD API exposes **CadText** class that represents text entities in the DWG AutoCAD file. Class **CadMText** is also included in the Aspose.CAD API because some other entities may also contain text.

Following is the code demonstration of text search in DWG AutoCAD file.

```
String sourceFile = "sample.dwg";

// Load an existing DWG file as DgnImage.
com.aspose.cad.fileformats.dgn.DgnImage dgnImage =
                (com.aspose.cad.fileformats.dgn.DgnImage)com.aspose.cad.Image.load(file);

 // search for text in the file
for (com.aspose.cad.fileformats.cad.cadobjects.CadBaseEntity entity : cadImage.getEntities()) 
{
    // please, note: we iterate through CadText entities here, but some other entities
    // may contain text also, e.g. CadMText and others
    if (entity.getClass() == com.aspose.cad.fileformats.cad.cadobjects.CadText.class) 
    {
        com.aspose.cad.fileformats.cad.cadobjects.CadText text = 
                (com.aspose.cad.fileformats.cad.cadobjects.CadText)entity;
        System.out.println(text.getDefaultValue());
    }
}
```

## Exporting DGN AutoCAD Format To PDF

Aspose.CAD for Java API has introduced the functionality to load a DGN AutoCAD file and [convert it to PDF format][6]. **CadImage** class serves the purpose. You need to load an existing DGN file as **CadImage**. Create an instance of **CadRasterizationOptions** class and set different properties. Create an instance of **PdfOptions** class and pass the CadRasterizationOptions instance. Now call the **save** method of CadImage class instance.

Following is the code demonstration to convert/export DGN to PDF format.

```
String file = "sample.dgn";
String outFile = "sample.dgn.pdf";

// load an existing DGN file as DgnImage.
com.aspose.cad.fileformats.dgn.DgnImage dgnImage =
                (com.aspose.cad.fileformats.dgn.DgnImage)com.aspose.cad.Image.load(file);


java.io.OutputStream outStream = new java.io.FileOutputStream(outFile);

com.aspose.cad.imageoptions.DgnRasterizationOptions rasterizationOptions = 
        new com.aspose.cad.imageoptions.DgnRasterizationOptions();

// Create an object of CadRasterizationOptions class and define/set different properties
PdfOptions options = new PdfOptions();
rasterizationOptions.setPageWidth(600);
rasterizationOptions.setPageHeight(300);
rasterizationOptions.setCenterDrawing(true);
rasterizationOptions.setAutomaticLayoutsScaling(false);

options.setVectorRasterizationOptions(rasterizationOptions);

// Call the save method of the CadImage class object.
cadImage.save(outStream, options);
```

## Exporting DGN AutoCAD Format To Raster Image Format

Aspose.CAD for Java API has introduced the functionality to load a DGN AutoCAD file and [convert it to raster image][7]. **CadImage** class serves the purpose. You need to load an existing DGN file as CadImage. Create an instance of **DgnRasterizationOptions** class and set different properties. Create an instance of **JpegOptions** class and pass the DgnRasterizationOptions instance. Now call the **save** method of CadImage class instance.

Following is the code demonstration to convert/export DGN to JPEG image.

```
String file = "sample.dgn";
String outFile = "sample.dgn.jpg";

// load an existing DGN file as DgnImage.
com.aspose.cad.fileformats.dgn.DgnImage dgnImage =
                (com.aspose.cad.fileformats.dgn.DgnImage)com.aspose.cad.Image.load(file);

java.io.OutputStream outStream = new java.io.FileOutputStream(outFile);

// Create an object of DgnRasterizationOptions class and define/set different properties
com.aspose.cad.imageoptions.DgnRasterizationOptions rasterizationOptions = 
        new com.aspose.cad.imageoptions.DgnRasterizationOptions();

// Create an object of JpegOptions class as we are converting the DGN to jpeg and assign DgnRasterizationOptions object to it.
JpegOptions options = new JpegOptions();

rasterizationOptions.setPageWidth(600);
rasterizationOptions.setPageHeight(300);
rasterizationOptions.setCenterDrawing(true);
rasterizationOptions.setAutomaticLayoutsScaling(false);

options.setVectorRasterizationOptions(rasterizationOptions);

// Call the save method of the CadImage class object.
cadImage.save(outStream, options);
```

## Get Block Attribute Value Of External Reference

Aspose.CAD for Java API allows you to [get external reference of a block attribute][8]. Aspose.CAD API exposes **getXRefPathName** property to get the external reference of a block attribute in a **CadBlockDictionary** collection.

Following is the code demonstration of getting external reference of a block attribute.

```
// Path to the document.
String fileName = "sample.dwg";

// Load an existing DWG file as DgnImage.
com.aspose.cad.fileformats.dgn.DgnImage dgnImage =
                (com.aspose.cad.fileformats.dgn.DgnImage)com.aspose.cad.Image.load(file);

// Access the external path name property
String sXternalRef = cadImage.getBlockEntities().get_Item("Drawing1").getXRefPathName();
System.out.println(sXternalRef); 
```

## Enhancements

The following enhancements have been introduced in this release.

*   The process to convert CAD to BMP format has been improved.
*   The process of converting Face3D objects in DXF has been improved.

To view a complete list of new features and to download the latest release, please visit [Aspose.CAD for Java 1.1.0 page in downloads section][9].

## Aspose.CAD for Java Resources

The resources, you may need to accomplish your tasks:

*   [Homepage for Aspose.CAD for Java API][10]
*   [Download Aspose.CAD for Java][11]
*   [Aspose.CAD for Java Wiki Docs][12] – Help documentation
*   [Aspose.CAD Product Family Forum][13] – Post your technical questions and queries, or any other problem you faced while running Aspose.CAD APIs.
*   [Enable Email Subscription][14] – Don’t limit yourself, you can keep yourself updated with the latest news on Aspose.CAD APIs and new features, fixes, plus other API related topics by subscribing to Aspose.CAD blog.
*   [Aspose.CAD for Java Examples][15] – We have published our code examples on the social coding website GitHub.com. Anyone can explore the code examples for learning purposes.




[1]: https://docs.aspose.com/display/cadjava/DWG+Drawings#DWGDrawings-SearchTextInDWGAutoCADFile
[2]: https://docs.aspose.com/display/cadjava/Exporting+DGN+AutoCAD
[3]: https://docs.aspose.com/display/cadjava/Exporting+DGN+AutoCAD#ExportingDGNAutoCAD-ExportingDGNAutoCADFormatToRasterImageFormat
[4]: https://docs.aspose.com/display/cadjava/DWG+Drawings#DWGDrawings-GetBlockAttributeValueOfExternalReference
[5]: https://docs.aspose.com/display/cadjava/DWG+Drawings#DWGDrawings-SearchTextInDWGAutoCADFile
[6]: https://docs.aspose.com/display/cadjava/Exporting+DGN+AutoCAD
[7]: https://docs.aspose.com/display/cadjava/Exporting+DGN+AutoCAD#ExportingDGNAutoCAD-ExportingDGNAutoCADFormatToRasterImageFormat
[8]: https://docs.aspose.com/display/cadjava/DWG+Drawings#DWGDrawings-GetBlockAttributeValueOfExternalReference
[9]: https://downloads.aspose.com/cad/java
[10]: https://products.aspose.com/cad/java
[11]: https://downloads.aspose.com/cad/java
[12]: https://docs.aspose.com/display/cadjava/Home
[13]: http://forum.aspose.com
[14]: https://blog.aspose.com/category/aspose-products/aspose.cad-product-family/
[15]: https://github.com/aspose-cad/Aspose.CAD-for-Java





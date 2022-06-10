---
title: 'Convert CAD DWG and DXF to PDF and Raster Images using Java'
date: Tue, 09 Aug 2016 10:20:39 +0000
draft: false
url: /2016/08/09/work-with-cad-formats-including-dwg-and-dxf-using-aspose.cad-for-java/
author: Muhammad Ijaz
summary: ''
tags: ['Convert CAD DWG and DXF to Image in Java', 'Convert CAD to PDF in Java', 'Convert DWG to PDF in Java', 'Convert DXF to PDF in Java']
categories: ['Aspose.CAD Product Family']
---



{{< figure align=center src="images/aspose_cad-for-java-100x100.png" alt="">}}


We are pleased to announce the release of Aspose.CAD for Java 1.0.0. This is a new addition to Aspose for Java APIs and allows you to work with CAD formats including DWG and DXF formats. Aspose.Imaging for Java also supports CAD formats but these formats will be removed from Aspose.Imaging for Java in the next three months and all features related to CAD formats will be the part of Aspose.CAD only.

This release of Aspose.CAD for Java supports [converting DWG and DXF formats to PDF][1] and [raster image formats][2]. Converting CAD [layers][3] and [layouts][4] to PDF and [raster image formats][5] has also been supported by this release. You can also remove entities from DWG and DXF documents.

## Convert CAD to PDF using Java

Aspose.CAD for Java allows you to [convert CAD drawings to PDF format][6]. **com.aspose.cad.Image.load** method can be used to load CAD drawings, **com.aspose.cad.imageoptions.CadRasterizationOptions** can be used to set vector rasterization options, **com.aspose.cad.imageoptions.PdfOptions** can be used to set PDF options and **com.aspose.cad.Image.save** method can be used to save output PDF e.g.

{{< gist aspose-com-gists 49c1b75d9a84e149ecf374ece2c2597d "Examples-src-main-java-com-aspose-cad-examples-DWGDrawings-ConvertDWGFileToPDF-ConvertDWGFileToPDF.java" >}}

## Convert CAD Formats to Raster Image in Java

Aspose.CAD for Java allows you to [convert CAD drawings to raster image formats][7]. **com.aspose.cad.Image.load** method can be used to load CAD drawings, **com.aspose.cad.imageoptions.CadRasterizationOptions** can be used to set vector rasterization options, **com.aspose.cad.ImageOptionsBase** can be used to set image options and **com.aspose.cad.Image.save** method can be used to save output image e.g.

{{< gist aspose-com-gists 49c1b75d9a84e149ecf374ece2c2597d "Examples-src-main-java-com-aspose-cad-examples-CADConversion-ConvertCADDrawingToRasterImageFormat-ConvertCADDrawingToRasterImageFormat.java" >}}

## Remove Entities from CAD Documents

Aspose.CAD for Java allows you to remove specific entities from CAD drawings. **com.aspose.cad.Image.load** method can be used to load CAD drawings, **com.aspose.cad.fileformats.cad.CadImage.getEntities()** can be used to loop through each entity and **com.aspose.cad.fileformats.cad.CadImage.** **removeEntity** can be used to remove any entity e.g.

```
com.aspose.cad.fileformats.cad.CadImage image = (com.aspose.cad.fileformats.cad.CadImage) com.aspose.cad.Image
		.load("Input.dwg");

for (int i = 0; i < image.getEntities().length; i++) {
	CadBaseEntity baseEntity = image.getEntities()[i];
	if (baseEntity.getClass() == com.aspose.cad.fileformats.cad.cadobjects.CadArc.class) {
		com.aspose.cad.fileformats.cad.cadobjects.CadArc arc = (com.aspose.cad.fileformats.cad.cadobjects.CadArc) baseEntity;
		if (arc.getCenterPoint().getX() > 1e10) {
			// cadImage.RemoveEntityAt(i);
			image.removeEntity(baseEntity);
			i--;
		}
	}
}

image.updateSize();

// Create an instance of CadRasterizationOptions and set its various
// properties
com.aspose.cad.imageoptions.CadRasterizationOptions rasterizationOptions = new com.aspose.cad.imageoptions.CadRasterizationOptions();
rasterizationOptions.setBackgroundColor(com.aspose.cad.Color
		.getWhite());
rasterizationOptions.setLayouts(new String[] { "Model" });

rasterizationOptions.setPageWidth(1600);
rasterizationOptions.setPageHeight(1600);

rasterizationOptions.setCenterDrawing(true);
// Create an instance of PdfOptions
com.aspose.cad.imageoptions.PdfOptions pdfOptions = new com.aspose.cad.imageoptions.PdfOptions();
// Set the VectorRasterizationOptions property
pdfOptions.setVectorRasterizationOptions(rasterizationOptions);

image.save("Output.pdf", pdfOptions);
```

## Other Important Features

Following is a list of some important features included in this release.

*   [Convert CAD layers to PDF][8]
*   [Convert CAD layouts to PDF][9]
*   [Convert CAD layers to raster image formats][10]
*   [Convert CAD layouts to raster image formats][11]

To view a complete list of new features and to download the latest release, please visit [Aspose.CAD for Java 1.0.0 page in downloads section][12].

## Aspose.CAD for Java Resources

The resources, you may need to accomplish your tasks:

*   [Homepage for Aspose.CAD for Java API][13]
*   [Download Aspose.CAD for Java][14]
*   [Aspose.CAD for Java Wiki Docs][15] – Help documentation
*   [Aspose.CAD Product Family Forum][16] – Post your technical questions and queries, or any other problem you faced while running Aspose.CAD APIs.
*   [Enable Email Subscription][17] – Don’t limit yourself, you can keep yourself updated with the latest news on Aspose.CAD APIs and new features, fixes, plus other API related topics by subscribing to Aspose.CAD blog.
*   [Aspose.CAD for Java Examples][18] – We have published our code examples on the social coding website GitHub.com. Anyone can explore the code examples for learning purposes.




[1]: http://docs.aspose.com/display/cadjava/DWG+Drawings#DWGDrawings-ConvertDWGFilestoPDF
[2]: https://docs.aspose.com/display/cadjava/Converting+CAD+Drawings+to+PDF+and+Raster+Image+Formats#ConvertingCADDrawingstoPDFandRasterImageFormats-ConvertingCADDrawingstoRasterImageFormats
[3]: http://docs.aspose.com/display/cadjava/DXF+Drawings#DXFDrawings-ExportingSpecificLayerofDXFDrawingstoPDF
[4]: http://docs.aspose.com/display/cadjava/Exporting+CAD#ExportingCAD-ExportingCADLayoutstoPDF
[5]: https://docs.aspose.com/display/cadjava/Converting+CAD+Drawings+to+PDF+and+Raster+Image+Formats#ConvertingCADDrawingstoPDFandRasterImageFormats-ConvertingCADDrawingstoRasterImageFormats
[6]: http://docs.aspose.com/display/cadjava/DWG+Drawings#DWGDrawings-ConvertDWGFilestoPDF
[7]: https://docs.aspose.com/display/cadjava/Converting+CAD+Drawings+to+PDF+and+Raster+Image+Formats#ConvertingCADDrawingstoPDFandRasterImageFormats-ConvertingCADDrawingstoRasterImageFormats
[8]: http://docs.aspose.com/display/cadjava/DXF+Drawings#DXFDrawings-ExportingSpecificLayerofDXFDrawingstoPDF
[9]: http://docs.aspose.com/display/cadjava/Exporting+CAD#ExportingCAD-ExportingCADLayoutstoPDF
[10]: https://docs.aspose.com/display/cadjava/Converting+CAD+Drawings+to+PDF+and+Raster+Image+Formats
[11]: https://docs.aspose.com/display/cadjava/Converting+CAD+Drawings+to+PDF+and+Raster+Image+Formats
[12]: http://www.aspose.com/downloads/cad/java
[13]: http://www.aspose.com/products/cad
[14]: http://www.aspose.com/downloads/cad/java
[15]: http://docs.aspose.com/display/cadjava/Home
[16]: http://www.aspose.com/community/forums/aspose.cad-product-family/540/showforum.aspx
[17]: https://blog.aspose.com/
[18]: https://github.com/aspose-cad/Aspose.CAD-for-Java





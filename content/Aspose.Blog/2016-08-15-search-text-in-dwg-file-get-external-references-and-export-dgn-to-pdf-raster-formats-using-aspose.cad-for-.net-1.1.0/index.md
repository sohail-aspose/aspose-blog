---
title: 'Search Text in DWG Files and Convert DGN to PDF or Images using C# .NET'
date: Mon, 15 Aug 2016 06:44:11 +0000
draft: false
url: /2016/08/15/search-text-in-dwg-file-get-external-references-and-export-dgn-to-pdf-raster-formats-using-aspose.cad-for-.net-1.1.0/
author: Ikram Haq
summary: ''
tags: []
categories: ['Aspose.CAD Product Family']
---



{{< figure align=center src="images/aspose_cad-for-net.png" alt="">}}


We are pleased to announce the release of Aspose.CAD for .NET 1.1.0. The major developments in this release support for [searching text in DWG AutoCAD file][1] and [get external references of block attributes][2]. Support to [convert DGN AutoCAD format to PDF][3] and [convert DGN AutoCAD format to raster image format][4] has also been incorporated in this release.

## Search Text In DWG AutoCAD File

Aspose.CAD for .NET now supports searching text in the DWG file. Aspose.CAD API exposes CadText class that represents text entities in the DWG AutoCAD file.

Below provided sample code demonstrates how to [search text in DWG file][5].

{{< gist aspose-com-gists 88cdd0899132edaf0afff77d33d11ae5 "Src-DWG-Drawings-SearchText-SearchText.cs" >}}

## Get Block Attribute Value Of External Reference

Aspose.CAD for .NET allows you to get the block attribute value of the external reference. The API exposes XRefPathName property to get the external reference of a block attribute in a CadBlockDictionary collection.

The below-provided sample code demonstrates how to [get the block attribute value][6].

{{< gist aspose-com-gists 88cdd0899132edaf0afff77d33d11ae5 "Src-DWG-Drawings-GetBlockAttributeValue-GetBlockAttributeValue.cs" >}}

## Convert DGN AutoCAD Format To PDF

Aspose.CAD for .NET allows you to [convert DGN AutoCAD format to PDF][7]. **Aspose.CAD.Image.Load** method can be used to load DGN file, **Aspose.CAD.ImageOptions.CadRasterizationOptions** can be used to set vector rasterization options, **Aspose.CAD.ImageOptionsBase** can be used to set image options and **Aspose.CAD.Image.Save** method can be used to save output image e.g.

{{< gist aspose-com-gists 88cdd0899132edaf0afff77d33d11ae5 "Src-DXF-Drawings-ExportEmbeddedDGN-ExportEmbeddedDGN.cs" >}}

## Convert DGN AutoCAD Format To Raster Image Formats

Aspose.CAD for .NET allows you to [convert DGN AutoCAD format to raster images][8]. **Aspose.CAD.Image.Load** method can be used to load DGN file, **Aspose.CAD.ImageOptions.CadRasterizationOptions** can be used to set vector rasterization options, **Aspose.CAD.ImageOptionsBase** can be used to set image options and **Aspose.CAD.Image.Save** method can be used to save output image e.g.

{{< gist aspose-com-gists 88cdd0899132edaf0afff77d33d11ae5 "Src-DGN-Drawings-ExportDGNToRasterImage-ExportDGNToRasterImage.cs" >}}

## Other Important Features

The following enhancements have been introduced in this release.

*   EULA link has been introduced in the MSI file.
*   The memory management process while exporting CAD to BMP has been improved.
*   The process of accessing Face3D objects has been improved.

To view a complete list of new features and to download the latest release, please visit [Aspose.CAD for .NET 1.1.0 page in downloads section][9].

## Aspose.CAD for .NET Resources

The resources, you may need to accomplish your tasks:

*   [Homepage for Aspose.CAD for .NET API][10]
*   [Download Aspose.CAD for .NET][11]
*   [Aspose.CAD for .NET Wiki Docs][12] – Help documentation
*   [API Reference Documents][13]
*   [Aspose.CAD Product Family Forum][14] – Post your technical questions and queries, or any other problem you faced while running Aspose.CAD APIs.
*   [Enable Email Subscription][15] – Don’t limit yourself, you can keep yourself updated with the latest news on Aspose.CAD APIs and new features, fixes, plus other API related topics by subscribing to Aspose.CAD blog.
*   [Aspose.CAD for .NET Examples][16] – We have published our code examples on the social coding website GitHub.com. Anyone can explore the code examples for learning purposes.




[1]: http://docs.aspose.com/display/cadnet/Search+Text+In+DWG+AutoCAD+File
[2]: http://docs.aspose.com/display/cadnet/Get+Block+Attribute+Value+Of+External+Reference
[3]: https://docs.aspose.com/display/cadnet/Exporting+DGN+AutoCAD#ExportingDGNAutoCAD-ExportingDGNAutoCADFormatToPDF
[4]: https://docs.aspose.com/display/cadnet/Exporting+DGN+AutoCAD#ExportingDGNAutoCAD-ExportingDGNAutoCADFormatToRasterImageFormat
[5]: http://docs.aspose.com/display/cadnet/Search+Text+In+DWG+AutoCAD+File
[6]: http://docs.aspose.com/display/cadnet/Get+Block+Attribute+Value+Of+External+Reference
[7]: https://docs.aspose.com/display/cadnet/Exporting+DGN+AutoCAD#ExportingDGNAutoCAD-ExportingDGNAutoCADFormatToPDF
[8]: https://docs.aspose.com/display/cadnet/Home
[9]: https://downloads.aspose.com/cad/net
[10]: https://products.aspose.com/cad/net
[11]: https://downloads.aspose.com/cad/net
[12]: https://docs.aspose.com/display/cadnet/Home
[13]: https://apireference.aspose.com/net/cad
[14]: http://forum.aspose.com
[15]: https://blog.aspose.com/category/aspose-products/aspose.cad-product-family/
[16]: https://github.com/aspose-cad/Aspose.CAD-for-.NET





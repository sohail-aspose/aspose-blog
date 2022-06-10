---
title: 'Support for DWG 2007 Format, Normalize Size for a DWG'
date: Fri, 24 Feb 2017 09:21:35 +0000
draft: false
url: /2017/02/24/support-dwg-2007-format-normalize-size-drawing-determine-external-references-dwg-aspose.cad-.net-17.02/
author: Ikram Haq
summary: ''
tags: []
categories: ['Aspose.CAD Product Family']
---

We are pleased to announce the release of Aspose.CAD for .NET 17.02. The major development in this release is the support for DWG 2007(AC1021) Format. This release supports determining the DWG external references and their file paths. The support for [adjusting CAD drawing size][1] has also been incorporated in this release.

## Adjusting CAD Drawing Size

Aspose.CAD for .Net provides the UnitType enumeration to [adjust the size of drawing][2] during conversion of the CAD format. There are two ways to adjust the drawing size.

*   Automatic adjust size.
    
*   Adjust size using UnitType enumeration
    

UnitType enumeration gives the ability to adjust scaling when Width and Height properties are not set. Below provided code snippet demonstrate how to use UnitType.

```

// Path to source file
string sourceFilePath = "sample.dwg";
            
// Load a CAD drawing in an instance of Image
using (var image = Aspose.CAD.Image.Load(sourceFilePath))
{
    // Create an instance of BmpOptions class
    Aspose.CAD.ImageOptions.BmpOptions bmpOptions = new Aspose.CAD.ImageOptions.BmpOptions();

    // Create an instance of CadRasterizationOptions and set its various properties
    Aspose.CAD.ImageOptions.CadRasterizationOptions cadRasterizationOptions = new Aspose.CAD.ImageOptions.CadRasterizationOptions();
    bmpOptions.VectorRasterizationOptions = cadRasterizationOptions;
    cadRasterizationOptions.CenterDrawing = true;

    // Set the UnitType property
    cadRasterizationOptions.UnitType = Aspose.CAD.ImageOptions.UnitType.Centimenter;

    // Set the layouts property
    cadRasterizationOptions.Layouts = new string\[\] { "Model" };

    // Export layout to BMP format
    string outPath = fileName + ".bmp";
    image.Save(outPath, bmpOptions);
}


```

## Enhancements

Following enhancements have been introduced in this release.

*   Processing of entity order for DWG format has been improved.
    
*   Processing of converting DWG to PDF format has been improved.
    
*   Process of exporting external raster images linked with DWG file has been improved.
    

To view a complete list of new features and to download the latest release, please visit [Aspose.CAD for .NET 17.02][3] page in downloads section.

## Aspose.CAD for .NET Resources

The resources, you may need to accomplish your tasks:

*   [Homepage for Aspose.CAD for .NET API][4]
*   [Download Aspose.CAD for .NET][5]
*   [Aspose.CAD for .NET Wiki Docs][6] – Help documentation
*   [API Reference Documents][7]
*   [Aspose.CAD Product Family Forum][8] – Post your technical questions and queries, or any other problem you faced while running Aspose.CAD APIs.
*   [Enable Email Subscription][9] – Don’t limit yourself, you can keep yourself updated with the latest news on Aspose.CAD APIs and new features, fixes, plus other API related topics by subscribing to Aspose.CAD blog.
*   [Aspose.CAD for .NET Examples][10] – We have published our code examples on the social coding website GitHub.com. Anyone can explore the code examples for learning purposes.




[1]: https://docs.aspose.com/display/cadnet/Adjusting+CAD+Drawing+Size
[2]: https://docs.aspose.com/display/cadnet/Adjusting+CAD+Drawing+Size
[3]: http://www.aspose.com/downloads/cad-family/net
[4]: https://www.aspose.com/products/cad/net
[5]: https://downloads.aspose.com/cad/net
[6]: https://docs.aspose.com/display/cadnet/Home
[7]: https://apireference.aspose.com/net/cad
[8]: https://www.aspose.com/community/forums/aspose.cad-product-family/540/showforum.aspx
[9]: https://blog.aspose.com/category/aspose-products/aspose.cad-product-family/
[10]: https://github.com/aspose-cad/Aspose.CAD-for-.NET





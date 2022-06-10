---
title: 'Export PSD Layer to Raster Image and 3D AutoCAD Images to PDF with Aspose.Imaging for .NET 3.1.0'
date: Wed, 07 Oct 2015 12:13:48 +0000
draft: false
url: /2015/10/07/export-psd-layer-to-raster-image-and-3d-autocad-images-to-pdf-with-aspose.imaging-for-.net-3.1.0/
author: Ikram Haq
summary: ''
tags: []
categories: ['Aspose.Total Product Family', 'Aspose.Imaging Product Family']
---

![](https://blog.aspose.com/wp-content/uploads/sites/2/2013/09/aspose-Imaging-for-net_100.png "aspose-Imaging-for-net_100") We are pleased to announce the release of Aspose.Imaging for .NET 3.1.0. This release contains two very useful features namely exporting PSD Layer to Raster Image and exporting 3D AutoCAD Images to PDF.

## Export PSD Layer to Raster Image

Aspose.Imaging for .NET API has introduced the functionality to export layer(s) in a PSD file to Raster image. Save method of the Layer class can be used to export a layer in a PSD file to raster image. Here is the code to Export the PSD Layer to Raster Image.

```
 //Load an existing PSD file as image.
using (Image image = Image.Load(dataDir + "sample.psd"))
{
    // Cast into PSD image.
    var psdImage = (FileFormats.Psd.PsdImage)image;

    // Create an instance of ImageOptions class.
    var pngOptions = new ImageOptions.PngOptions();
    pngOptions.ColorType = FileFormats.Png.PngColorType.TruecolorWithAlpha;

    // iterate through the layers in the PSD.
    for (int i = 0; i < psdImage.Layers.Length; i++)
    {
        // Access a layer and save it as PNG image.
        psdImage.Layers[i].Save(dataDir + "layer-" + i +".png", pngOptions);
    }
} 
```

## Export 3D AutoCAD Images to PDF

Aspose.Imaging for .NET API has introduced the functionality to export 3D AutoCAD images to PDF. Save method of the CadImage class, 3D AutoCAD Images (DxF) can be used to export to PDF format. You have to use the Aspose.Imaging.ImageOptions.TypeOfEntities.Entities3D class to activate the 3D settings. Here is the code to Export the 3D AutoCAD Images to PDF.

```
 //Load an existing DxF file as CAD image.
using (CadImage cadImage = (CadImage)Image.Load(dataDir + "conic_pyramid.dxf"))
{
    // Create an instance of CadRasterizationOptions class to set the preferences.
    CadRasterizationOptions rasterizationOptions = new CadRasterizationOptions();
    rasterizationOptions.PageWidth = 500;
    rasterizationOptions.PageHeight = 500;

    // Set/Activate the 3D option.
    rasterizationOptions.TypeOfEntities = TypeOfEntities.Entities3D;
    rasterizationOptions.Layouts = new string[] { "Model" };
    
    // Create an instance of PdfOptions class.
    PdfOptions pdfOptions = new PdfOptions();
    pdfOptions.VectorRasterizationOptions = rasterizationOptions;

    // Save the CAD image into PDF format.
    cadImage.Save(dataDir + "output.pdf", pdfOptions);
} 
```

## Enhancements

Fix to an exception "Cannot open an image. The image file format may be not supported at the moment. at Image.load" while loading DWG file format has also been taken care. Some problems were noticed while exporting DWG to PDF format, JPEG image get distorted after saving with CMYK colorspace setting and quality of the image decreases while re-sizing the image. All such issues have been fixed.

*   Fixed: ExifData and Comment properties in JpegImage class are always set to null after reading a JPEG image that contains these data.
    
*   Fixed: ImageLoadException: Cannot process loading further due to incorrect file format structure. Index was out of range. Must be non-negative and less than the size of the collection, while loading DWG.
    
*   Fixed: Image quality (Sharpness) decreases while resizing the image.
    
*   Fixed: Converting DWG to raster image formats Tiff renders in blank image with no Layout specified.
    
*   Fixed: ImageLoadException: Unable to read file.
    
*   Fixed: System.OverflowException: Arithmetic operation resulted in an overflow, at Image.Resize.
    
*   Fixed: Conversion of DWG to PDF generated a huge file in size.
    

Many reported bug fixes have also been included. Please refer to the release notes of [Aspose.Imaging for .NET 3.1.0][1] for a full view of improvements along with sample code snippets for newly added features. If you are planning to upgrade the API to the latest revision, we strongly suggest you to check the Public API Change section to know what has been changed in the public API since your current version.

## Aspose.Imaging for .Net Resources

The resources, you may need to accomplish your tasks:

*   Home page for Aspose.Imaging for .Net API.
*   [Download Aspose.Imaging for .NET][2].
*   Aspose.Imaging for .NET online documentation – help documentation and API reference documents.
*   [Aspose.Imaging Product Family Forum][3] – post your technical questions and queries, or any other problem you are facing while working with Aspose.Imaging APIs.
*   [Enable blog Subscription][4] – Do not limit yourself, you can keep yourself updated with the latest news on Aspose.Imaging APIs, new features, fixes and other API related topics by subscribing to Aspose.Imaging blog.
*   [Aspose.Imaging for .NET Examples][5] – We have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.

As always we appreciate your feedback so if you ever have anything to tell us about this release or anything else, please head to the [Aspose.Imaging forum][6] for a chat.




[1]: http://www.aspose.com/community/files/51/.net-components/aspose.imaging-for-.net/default.aspx
[2]: http://www.aspose.com/community/files/51/.net-components/aspose.imaging-for-.net/default.aspx
[3]: http://www.aspose.com/community/forums/aspose.imaging-product-family/498/showforum.aspx
[4]: https://blog.aspose.com/
[5]: https://github.com/aspose-imaging/Aspose.Imaging-for-.NET
[6]: http://www.aspose.com/community/forums/aspose.imaging-product-family/498/showforum.aspx





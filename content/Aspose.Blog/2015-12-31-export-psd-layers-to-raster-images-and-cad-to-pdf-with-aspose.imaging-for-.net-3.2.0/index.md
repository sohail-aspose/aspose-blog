---
title: 'Export PSD Layers to Raster Images using C#'
date: Thu, 31 Dec 2015 14:13:39 +0000
draft: false
url: /2015/12/31/export-psd-layers-to-raster-images-and-cad-to-pdf-with-aspose.imaging-for-.net-3.2.0/
author: Ikram Haq
summary: ''
tags: []
categories: ['Aspose.Imaging Product Family']
---



{{< figure align=center src="images/aspose-Imaging-for-net_100.png" alt="">}}


We are pleased to announce the release of Aspose.Imaging for .NET 3.2.0. This release allows you to use [Bradley's threshold algorithm][1] during image conversion and define settings to [expand or crop the image][2].

## Use Bradley's Threshold Algorithm while Converting Images

Aspose.Imaging for .NET API has introduced the functionality to use Bradley's threshold algorithm during process of image conversion. Here is the code to define the threshold value and use it.

```
string sourcepath = @"sourcefile.png";
string outputPath = @"binarized\_output.png";

//Load an existing image.
using (var image = (PngImage)Image.Load(sourcepath))
{
        // Define threshold value
        double threshold = 0.15;

        // Call BinarizeBradley method and pass the threshold value as parameter
        image.BinarizeBradley(threshold);

        // Save the output image
        image.Save(savePath);
}

```

## Expand and Crop an Image

Using Aspose.Imaging for .Net, developers can expand or crop an image during image conversion process. Following is the code snippet demonstrating how Rectangle class can be used to crop or expand raster images.

```
string fileName = @"imageToResize.bmp";
string outputFileName = @"imageResized.Jpeg";

//Load an existing image.
using (RasterImage rasterImage = (RasterImage)Image.Load(fileName))
{
        // setting for image data to be cashed
        rasterImage.CacheData();

        // Create an instance of Rectangle class and define X,Y and Width, height of the rectangle.
        Rectangle destRect = new Rectangle() { X = -200, Y = -200, Width = 300, Height = 300 };

        // Save output image by passing output file name, image options and rectangle object.
        rasterImage.Save(outputFileName, new JpegOptions(), destRect);
}

```

## Export PSD Layers to Raster Images

Using Aspose.Imaging for .Net, developers can convert PSD layers to PNG, JPEG and TIFF images. Following is the code snippet demonstrating how PSD layers can be converted to PNG image.

```
string sourceFileName = @"source.psd";

// Create an instance of Image class and load PSD file as image.
using (Aspose.Imaging.Image image = Aspose.Imaging.Image.Load(sourceFileName))
{

    // Cast image object to PSD image
    var psdImage = (Aspose.Imaging.FileFormats.Psd.PsdImage)image;

    // Create an instance of PngOptions class
    var pngOptions = new PngOptions();
    pngOptions.ColorType = Aspose.Imaging.FileFormats.Png.PngColorType.TruecolorWithAlpha;

    // Loop through the list of layers
    for (int i = 0; i < psdImage.Layers.Length; i++)
    {
        // convert and save the layer to PNG file format.
        psdImage.Layers\[i\].Save(string.Format("layer{0}.png", i + 1), pngOptions);
    }
}

```

## Export CAD Layouts to PDF

Aspose.Imaging for .Net provides functionality to export CAD to PDF file format. Save method of the CadImage class can be used to export to PDF format. Initialize the CadRasterizationOptions class, define the type of entities using Aspose.Imaging.ImageOptions.TypeOfEntities class and set the layout(s) that you want to export. Following is the code demonstration of the said functionality.

```
// Create an instance of CadImage class and load the file.
using (CadImage cadImage = (CadImage)Image.Load(fileName))
{
       // Create an instance of CadRasterizationOptions class
        CadRasterizationOptions rasterizationOptions = new CadRasterizationOptions();
        rasterizationOptions.PageWidth = 1600;
        rasterizationOptions.PageHeight = 1600;

        // Set the Entities type property to Entities3D.
        rasterizationOptions.TypeOfEntities = TypeOfEntities.Entities3D;
        
        rasterizationOptions.ScaleMethod = ScaleType.GrowToFit;
        rasterizationOptions.ContentAsBitmap = true;

        // Set Layouts
        rasterizationOptions.Layouts = new string\[\] { "Model" };
        
        // Create an instance of PDF options class
        PdfOptions pdfOptions = new PdfOptions();
        pdfOptions.VectorRasterizationOptions = rasterizationOptions;
        
        string outPath = fileName + ".pdf";

        // Set Graphics options
        rasterizationOptions.GraphicsOptions.SmoothingMode = SmoothingMode.HighQuality;
        rasterizationOptions.GraphicsOptions.TextRenderingHint = TextRenderingHint.AntiAliasGridFit;
        rasterizationOptions.GraphicsOptions.InterpolationMode = InterpolationMode.HighQualityBicubic;

        // Export to PDF by calling the Save method
        cadImage.Save(outPath, pdfOptions);
}

```

## Enhancements

The following enhancements have been introduced in this release.

*   The functionality of ExifData with NULL properties has been improved.
*   Loading and saving PSD to raster image functionality has been improved.
*   DWG file to PDF conversion process has been improved.
*   Converting DXF file to PNG or TIFF process has been improved.
*   Process of handling large images while resizing has been improved.

Please refer to the release notes of [Aspose.Imaging for .NET 3.2.0][3] for a full view of improvements along with sample code snippets for newly added features. If you are planning to upgrade the API to the latest revision, we strongly suggest you to check the [Public API Change][4] section to know what has been changed in the public API since your current version.

## Aspose.Imaging for .Net Resources

The resources, you may need to accomplish your tasks:

*   [Home page for Aspose.Imaging for .NET API][5].
*   [Download Aspose.Imaging for .NET][6].
*   [Aspose.Imaging for .NET online documentation][7] – help documentation and API reference documents.
*   [Aspose.Imaging Product Family Forum][8] – post your technical questions and queries, or any other problem you are facing while working with Aspose.Imaging APIs.
*   [Enable blog Subscription][9] – Do not limit yourself, you can keep yourself updated with the latest news on Aspose.Imaging APIs, new features, fixes and other API related topics by subscribing to Aspose.Imaging blog.
*   [Aspose.Imaging for .NET Examples][10] – We have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.

As always we appreciate your feedback so if you ever have anything to tell us about this release or anything else, please head to the [Aspose.Imaging forum][11] for a chat.




[1]: https://docs.aspose.com/display/imagingnet/Applying+Median+and+Wiener+Filters#ApplyingMedianandWienerFilters-UseBradleythresholdalgorithm
[2]: https://docs.aspose.com/display/imagingnet/Converting+Images#ConvertingImages-ExpandandCropImages
[3]: https://downloads.aspose.com/imaging/net
[4]: http://docs.aspose.com/display/imagingnet/Migrating+from+Earlier+Versions+of+Aspose.Imaging
[5]: https://www.aspose.com/products/imaging/net
[6]: https://downloads.aspose.com/imaging/net
[7]: https://docs.aspose.com/display/imagingnet/Home
[8]: https://www.aspose.com/community/forums/aspose.imaging-product-family/498/showforum.aspx
[9]: https://blog.aspose.com/category/aspose-products/aspose.imaging-product-family/
[10]: https://github.com/aspose-imaging/Aspose.Imaging-for-.NET
[11]: http://forum.aspose.com





---
title: 'Convert EMF to Raster Image Formats using C#'
date: Wed, 08 Jun 2016 20:34:55 +0000
draft: false
url: /2016/06/08/convert-emf-to-raster-image-formats-using-csharp/
author: Ikram Haq
summary: ''
tags: []
categories: ['Aspose.Imaging Product Family']
---



{{< figure align=center src="images/aspose-Imaging-for-net_100.png" alt="">}}


We are pleased to announce the release of [Aspose.Imaging for .NET][1] 3.6.0. The major development in this release is to convert metafile (Emf/Emf+) to raster image formats. Support to merge PSD layers while converting PSD to JPG has also been incorporated in this release.

## Export MetaFile To Raster Formats using C#

Using Aspose.Imaging for .Net, developers can convert metafile (Emf/Emf+) to raster formats. Aspose.Imaging for .Net provides the EmfImage class to load EMF files and the same can be used to convert the PSD to raster formats. Below the provided sample code demonstrates how to convert an EMF file to different raster formats.

```
string filePath = "TestEmfBezier.emf";

// Create EmfRasterizationOption class instance and set properties
EmfRasterizationOptions emfRasterizationOptions = new EmfRasterizationOptions();
emfRasterizationOptions.BackgroundColor = Aspose.Imaging.Color.PapayaWhip;
emfRasterizationOptions.PageWidth = 300;
emfRasterizationOptions.PageHeight = 300;

// Load an existing EMF file as iamge and convert it to EmfImage class object
using (var image = (Aspose.Imaging.FileFormats.Emf.EmfImage)Aspose.Imaging.Image.Load(filePath))
{
    if (!image.Header.EmfHeader.Valid)
    {
        throw new Aspose.Imaging.CoreExceptions.ImageLoadException(string.Format("The file {0} is not valid", filePath));
    }

    // Convert EMF to BMP
    image.Save(filePath + ".bmp", new BmpOptions() { VectorRasterizationOptions = emfRasterizationOptions });

    // Convert EMF to GIF
    image.Save(filePath + ".gif", new GifOptions() { VectorRasterizationOptions = emfRasterizationOptions });

    // Convert EMF to JPEG
    image.Save(filePath + ".jpeg", new JpegOptions() { VectorRasterizationOptions = emfRasterizationOptions });

    // Convert EMF to J2K
    image.Save(filePath + ".j2k", new Jpeg2000Options() { VectorRasterizationOptions = emfRasterizationOptions });

    // Convert EMF to PNG
    image.Save(filePath + ".png", new PngOptions() { VectorRasterizationOptions = emfRasterizationOptions });

    // Convert EMF to PSD
    image.Save(filePath + ".psd", new PsdOptions() { VectorRasterizationOptions = emfRasterizationOptions });

    // Convert EMF to TIFF
    image.Save(filePath + ".tiff", new TiffOptions(TiffExpectedFormat.TiffLzwRgb) { VectorRasterizationOptions = emfRasterizationOptions });

    // Convert EMF to WebP
    image.Save(filePath + ".webp", new WebPOptions() { VectorRasterizationOptions = emfRasterizationOptions });
}
```

## Merge PSD Layers using C#

Using Aspose.Imaging for .NET API, developers can merge layers in a PSD file while converting PSD file to JPG. The following code example demonstrates how to merge layers of a PSD file.

```
string sourceFileName = "5_layers.psd";

//Load an existing PSD file as image
using (Aspose.Imaging.Image image = Aspose.Imaging.Image.Load(sourceFileName))
{
       // Convert the loaded image to PSDImage
       var psdImage = (Aspose.Imaging.FileFormats.Psd.PsdImage)image;

       // create a JPG file stream
       using (Stream stream = File.Create(sourceFileName.Replace("psd", "jpg")))
       {

             // Create JPEG option class object
             var jpgOptions = new JpegOptions();

            // Set the source property to jpg file stream.
            jpgOptions.Source = new Aspose.Imaging.Sources.StreamSource(stream);

            // call the Save the method of PSDImage class to merge the layers and save it as jpg image.
            psdImage.Save(stream, jpgOptions);
       }
}
```

## Enhancements

The following enhancements have been introduced in this release.

*   Process to convert PSD to TIFF format has been improved.
*   Memory management process while rendering metafiles has been improved.

Please refer to the release notes of [Aspose.Imaging for .NET 3.6.0][2] for a full view of improvements along with sample code snippets for newly added features. If you are planning to upgrade the API to the latest revision, we strongly suggest you to check the Public API Change section to know what has been changed in the public API since your current version.

## Aspose.Imaging for .NET Resources

The resources, you may need to accomplish your tasks:

*   [Home page for Aspose.Imaging for .NET API][3].
*   [Download Aspose.Imaging for .NET][4].
*   [Aspose.Imaging for .NET online documentation][5] – help documentation and API reference documents.
*   [Aspose.Imaging Product Family Forum][6] – post your technical questions and queries, or any other problem you are facing while working with Aspose.Imaging APIs.
*   [Enable blog Subscription][7] – Do not limit yourself, you can keep yourself updated with the latest news on Aspose.Imaging APIs, new features, fixes and other API related topics by subscribing to Aspose.Imaging blog.
*   [Aspose.Imaging for .NET Examples][8] – We have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.

As always we appreciate your feedback so if you ever have anything to tell us about this release or anything else, please head to the [Aspose.Imaging forum][9] for a chat.




[1]: https://products.aspose.com/imaging/net
[2]: https://downloads.aspose.com/imaging/net
[3]: https://products.aspose.com/imaging/net
[4]: https://downloads.aspose.com/imaging/net
[5]: https://docs.aspose.com/imaging/net
[6]: https://www.aspose.com/community/forums/aspose.imaging-product-family/498/showforum.aspx
[7]: https://blog.aspose.com/category/aspose-products/aspose.imaging-product-family/
[8]: https://github.com/aspose-imaging/Aspose.Imaging-for-.NET
[9]: http://forum.aspose.com





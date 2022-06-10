---
title: 'Export Webp and Update Text Layer In PSD using C#'
date: Sun, 28 Feb 2016 10:09:18 +0000
draft: false
url: /2016/02/28/create-and-export-webp-update-psd-text-layer-using-csharp/
author: Ikram Haq
summary: ''
tags: []
categories: ['Aspose.Imaging Product Family']
---



{{< figure align=center src="images/aspose-Imaging-for-net_100.png" alt="">}}


We are pleased to announce the release of [Aspose.Imaging for .NET][1] 3.3.0. This release allows you to Create Webp image, export Webp image to other image formats, extract a particular frame from Webp image and convert frame of a GIF image to Webp image. Support to update text layer in the PSD file and read/ write XMP data to image has also been incorporated in this release.

## Create WebP Image using C#

Using Aspose.Imaging for .NET API, developers can create WebP image. Following is the code demonstrating the use of WebPOptions class to create a WebP image.

```
// Create an instance of WebPOptions class
Aspose.Imaging.ImageOptions.WebPOptions imageOptions = new Aspose.Imaging.ImageOptions.WebPOptions();

// Set LossLess property
imageOptions.Lossless = true;

// Set Source property with the path and image file name where you want to create the WebP image.
imageOptions.Source = new Aspose.Imaging.Sources.FileCreateSource(@"Test_create.webp", false);

// Create an instance of image class by using WebOptions instance that you have just created.
using (Aspose.Imaging.Image image = Aspose.Imaging.Image.Create(imageOptions, 500, 500))
{
     // Save the image.
     image.Save();
}
```

## Exporting WebP to Other Image Formats using C#

Using Aspose.Imaging for .NET API, developers can convert WebP image to other image formats. Here is the code to convert Webp image to BMP format.

```
// Load WebP image into the instance of image class.
using (Aspose.Imaging.Image image = Aspose.Imaging.Image.Load(@"sample.webp"))
{
      // Save the image in WebP format.
      image.Save(@"sample_out.bmp", new Aspose.Imaging.ImageOptions.BmpOptions());
}
```

## Extract Frames From WebP Image using C#

Using Aspose.Imaging, developers can extract a particular frame from any existing Webp image and convert it to other image formats. Following is the code snippet demonstrating how to extract a particular frame can from a WebP image and convert it to a Raster image.

```
// Load an existing WebP image into the instance of WebPImage class.
using (Aspose.Imaging.FileFormats.Webp.WebPImage image = new Aspose.Imaging.FileFormats.Webp.WebPImage(@"D:\animation.webp"))
{
       if (image.Blocks.Length > 2)
       {
           // Access a particular frame from WebP image and cast it to Raster Image
           RasterImage block = (image.Blocks[2] as RasterImage);

           if (block != null)
           {
               // Save the Raster Image to a BMP image.
               block.Save(@"D:\animation.bmp", new BmpOptions());
           }
       }
}
```

## Convert GIFF Image Frame to WebP Image using C#

Using Aspose.Imaging for .NET API, developers can extract a frame from any existing GIFF image and convert it to WebP format. Following is the code demonstration of GifImage.Blocks property to extract a GIFF frame and WebPFrameBlock class to add WebP frame to WebP image block list to create a WebP image.

```
// Load GIFF image into the instance of image class.
using (Aspose.Imaging.Image image = Aspose.Imaging.Image.Load(@"D:\animation.gif"))
{
      // Create an instance of GIFF image class.
      Aspose.Imaging.FileFormats.Gif.GifImage gif = image as Aspose.Imaging.FileFormats.Gif.GifImage;

      if (gif == null) return;

      // Load an existing WebP image into the instance of WebPImage class.
      using (Aspose.Imaging.FileFormats.Webp.WebPImage webp = new Aspose.Imaging.FileFormats.Webp.WebPImage(image.Width, image.Height, null))
      {
             // Loop through the GIFF frames
             for (int i = 0; i < gif.Blocks.Length; i++)
             {
                    // Convert GIFF block to GIFF Frame
                    Aspose.Imaging.FileFormats.Gif.Blocks.GifFrameBlock gifBlock = gif.Blocks[i] as Aspose.Imaging.FileFormats.Gif.Blocks.GifFrameBlock;
                    if (gifBlock == null)
                    {
                            continue;
                    }

                    // Create an instance of WebP Frame instance by passing GIFF frame to class constructor.
                    Aspose.Imaging.FileFormats.Webp.WebPFrameBlock block = new Aspose.Imaging.FileFormats.Webp.WebPFrameBlock(gifBlock)
                    {
                            Top = (short)gifBlock.Top,
                            Left = (short)gifBlock.Left,
                           Duration = (short)gifBlock.ControlBlock.DelayTime
                    };

                    // Add WebP frame to WebP image block list
                    webp.AddBlock(block);
            }

            // Set Properties of WebP image.
            webp.Options.AnimBackgroundColor = 0xff; //black
            webp.Options.AnimLoopCount = 0; //infinity
            webp.Options.Qualitty = 50;
            webp.Options.Lossless = false;

            // Save WebP image.
            webp.Save(@"D:\saveAnimation.webp");
      }
}
```

## Update Text Layer In PSD File using C#

Aspose.Imaging provides functionality to update text layer in PSD file. TextLayer.UpdateText method of the TextLayer class can be used to update text in the text layer of a PSD file. TextLayer class can be found under namespace Apose.Imaging.FileFormats.Psd.Layers. Method TextLayer.UpdateText takes a string that is to be added, top left coordinates as starting point (Aspose.Imaging.Point), font size and color (Aspose.Imaging.Color) as parameters. Following is the code demonstration of the said functionality.

```
using (Aspose.Imaging.Image image = Aspose.Imaging.Image.Load(sourceFileName))
{
      Aspose.Imaging.FileFormats.Psd.PsdImage psdImage = (Aspose.Imaging.FileFormats.Psd.PsdImage)image;
                
      Apose.Imaging.FileFormats.Psd.Layers.TextLayer textLayer1 = (Aspose.Imaging.FileFormats.Psd.Layers.TextLayer)psdImage.Layers[1];
      Aspose.Imaging.FileFormats.Psd.Layers.TextLayer textLayer2 = (Aspose.Imaging.FileFormats.Psd.Layers.TextLayer)psdImage.Layers[2];

      textLayer2.UpdateText("test update", new Aspose.Imaging.Point(100, 100), 72.0f, Aspose.Imaging.Color.Purple);

      psdImage.Save(outputFile, new PsdOptions() { CompressionMethod = Aspose.Imaging.FileFormats.Psd.CompressionMethod.RLE });
}
```

## Read and Write XMP Data To Images

Using Aspose.Imaging for .NET API, developers can read or write XMP metadata to images. Xmp namespace can be used for XMP data manipulation.

Following is the complete code demonstrating how to use the XmpHeaderPi, XmpTrailerPi, XmpMeta, XmpPacketWrapper, PhotoshopPackage and DublinCorePackage packages contained in Xmp namespace to read and write XMP metadata into the image.

```
// Specify the size of image by defining a Rectangle 
Aspose.Imaging.Rectangle rect = new Aspose.Imaging.Rectangle(0, 0, 100, 200);

TiffOptions tiffOptions = new TiffOptions(TiffExpectedFormat.TiffJpegRGB);
tiffOptions.Photometric = TiffPhotometrics.MinIsBlack;
tiffOptions.BitsPerSample = new ushort[] { 8 };

// create the brand new image just for sample purposes
using (var image = new TiffImage(new TiffFrame(tiffOptions, rect.Width, rect.Height)))
{
      // create an instance of XMP-Header
      Aspose.Imaging.Xmp.XmpHeaderPi xmpHeader = new Aspose.Imaging.Xmp.XmpHeaderPi(System.Guid.NewGuid().ToString());

      // create an instance of Xmp-TrailerPi 
      Aspose.Imaging.Xmp.XmpTrailerPi xmpTrailer = new Aspose.Imaging.Xmp.XmpTrailerPi(true);

      // create an instance of XMPmeta class to set different attributes
      Aspose.Imaging.Xmp.XmpMeta xmpMeta = new Aspose.Imaging.Xmp.XmpMeta();
      xmpMeta.AddAttribute("Author", "Mr Smith");
      xmpMeta.AddAttribute("Description", "The fake metadata value");

      // create an instance of XmpPacketWrapper that contains all metadata
      Aspose.Imaging.Xmp.XmpPacketWrapper xmpData = new Aspose.Imaging.Xmp.XmpPacketWrapper(xmpHeader, xmpTrailer, xmpMeta);

      // create an instacne of Photoshop package and set photoshop attributes
      Aspose.Imaging.Xmp.Schemas.Photoshop.PhotoshopPackage photoshopPackage = new Aspose.Imaging.Xmp.Schemas.Photoshop.PhotoshopPackage();
      photoshopPackage.SetCity("London");
      photoshopPackage.SetCountry("England");
      photoshopPackage.SetColorMode(Aspose.Imaging.Xmp.Schemas.Photoshop.ColorMode.Rgb);
      photoshopPackage.SetCreatedDate(DateTime.UtcNow);

      // add photoshop package into XMP metadata
      xmpData.AddPackage(photoshopPackage);

      // create an instacne of DublinCore package and set dublinCore attributes
      Aspose.Imaging.Xmp.Schemas.DublinCore.DublinCorePackage dublinCorePackage = new Aspose.Imaging.Xmp.Schemas.DublinCore.DublinCorePackage();
      dublinCorePackage.SetAuthor("Charles Bukowski");
      dublinCorePackage.SetTitle("Confessions of a Man Insane Enough to Live With the Beasts");
      dublinCorePackage.AddValue("dc:movie", "Barfly");

      // add dublinCore Package into XMP metadata
      xmpData.AddPackage(dublinCorePackage);

      using (var ms = new MemoryStream())
      {
                    // update XMP metadata into image
                    image.XmpData = xmpData;

                    // Save image on the disk or in memory stream
                    image.Save(ms);

                    ms.Seek(0, System.IO.SeekOrigin.Begin);

                    // Load the image from moemory stream or from disk to read/get the metadata
                    using (var img = (TiffImage)Aspose.Imaging.Image.Load(ms))
                    {
                        // getting the XMP metadata
                        Aspose.Imaging.Xmp.XmpPacketWrapper imgXmpData = img.XmpData;
                        foreach (Aspose.Imaging.Xmp.XmpPackage package in imgXmpData.Packages)
                        {
                            // use package data ...
                        }
                    }
     }
}
```

## Enhancements

Following enhancements have been introduced in this release.

*   Process of JPEG2000 image conversion JP2 has been improved.
*   Process of TIFF image conversion to other image format has been improved.
*   Functionality of EXIF data in TIFF image has been improved.
*   DWG file to PDF conversion process has been improved.
*   Process of converting raster images process has been improved.
*   JPEG image encoding algorithm has been upgraded.
*   Functionality of HorizontalResolution & VerticalResolution properties has been improved.
*   Resizing GIF image functionality has been improved.

Please refer to the release notes of [Aspose.Imaging for .NET 3.3.0][2] for a full view of improvements along with sample code snippets for newly added features. If you are planning to upgrade the API to the latest revision, we strongly suggest you to check the Public API Change section to know what has been changed in the public API since your current version.

## Aspose.Imaging for .Net Resources

The resources, you may need to accomplish your tasks:

*   [Home page for Aspose.Imaging for .Net API][3].
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
[6]: http://forum.aspose.com
[7]: https://blog.aspose.com/category/aspose-products/aspose.imaging-product-family/
[8]: https://github.com/aspose-imaging/Aspose.Imaging-for-.NET
[9]: http://forum.aspose.com





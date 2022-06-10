---
title: 'Aspose.Imaging for .NET 2.0.0 Introduces AutoCAD DXF to PDF Conversion Support'
date: Thu, 26 Sep 2013 03:53:32 +0000
draft: false
url: /2013/09/26/aspose.imaging-for-.net-2.0.0-introduces-autocad-dxf-to-pdf-conversion-support/
author: Tilal Ahmad
summary: ''
tags: ['Babar Raza']
categories: ['Aspose.Imaging Product Family']
---

[![][1]](https://blog.aspose.com/wp-content/uploads/sites/2/2013/09/aspose-Imaging-for-net_100.png)We are pleased to announce the long awaited release of Aspose.Imaging for .NET 2.0.0. It includes several major and highly demanded features along with some bug fixes.

This month’s release includes an exciting feature which lets you read AutoCAD DXF drawing entities and render them as an entire drawing into PDF format. At the moment, we fully support the AutoCAD DXF 2010 file format with all widespread 2D entities and their basic default parameters. However, we plan to support other AutoCAD file formats in the future. We have also introduced another feature for reading and editing an image's EXIF data in this release. Please check the following code snippet for the details.

```
using (Aspose.Imaging.Image image = Aspose.Imaging.Image.Load("Test.jpg"))
     {
        ExifData exif = (image as JpegImage).ExifData;

        if (exif != null)
         {
          Console.WriteLine("Exif WhiteBalance: " + exif.WhiteBalance);
          Console.WriteLine("Exif PixelXDimension: " + exif.PixelXDimension);
          Console.WriteLine("Exif PixelYDimension: " + exif.PixelYDimension);
          Console.WriteLine("Exif ISOSpeed: " + exif.ISOSpeed);
          Console.WriteLine("Exif FocalLength: " + exif.FocalLength);
          Console.ReadKey();
         }
     }
```

To see a complete list of features and fixes, and to download Aspose.Imaging for .NET 2.0.0, [please visit the download page][2].




[1]: https://blog.aspose.com/wp-content/uploads/sites/2/2013/09/aspose-Imaging-for-net_100.png "aspose-Imaging-for-net_100"
[2]: http://www.aspose.com/community/files/51/.net-components/aspose.imaging-for-.net/entry497656.aspx





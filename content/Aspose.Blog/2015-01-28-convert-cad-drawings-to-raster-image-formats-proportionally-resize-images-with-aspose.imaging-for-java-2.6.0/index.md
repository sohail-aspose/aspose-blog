---
title: 'Convert AutoCAD Drawings to Raster Images using Java'
date: Wed, 28 Jan 2015 11:08:00 +0000
draft: false
url: /2015/01/28/convert-cad-drawings-to-raster-image-formats-proportionally-resize-images-with-aspose.imaging-for-java-2.6.0/
author: Babar Raza
summary: ''
tags: ['Babar Raza']
categories: ['Aspose.Imaging Product Family']
---

Aspose.Imaging for Java 2.6.0 has been released and we are pleased to announce that this release contains many useful improvements, including the long-awaited feature of AutoCAD drawings to raster image conversion. Please refer to the release notes of [Aspose.Imaging for Java 2.6.0][1] for a full list of bug fixes and improvements. If you are planning to upgrade the API from any previous version, we strongly recommend you to first check the Public API Changes section.

While you are downloading the latest build, here is a look at the biggest features in this release.

## Convert AutoCAD to Raster Image using Java

Aspose.Imaging for Java API now supports the conversion of CAD drawing formats such as DXF & DWG to raster image formats such as PNG, BMP, TIFF, JPEG and GIF. Aspose.Imaging for Java API has exposed the VectorRasterizationOptions and CadRasterizationOptions classes to the com.aspose.imaging.ImageOptions package that serve an efficient and easy to use interface for CAD to Raster Image Conversion.

The said conversion can be achieved by following the 4 simple steps as elaborated below.

1.  Load the CAD file into an instance of Image.
2.  Create an instance of CadRasterizationOptions and set its mandatory properties such as PageWidth & PageHeight.
3.  Create an instance of ImageOptionsBase and set its VectorRasterizationOptions property to the instance of CadRasterizationOptions created in previous step.
4.  Call Image.save by passing the file path as well as the instance of ImageOptionsBase created in previous step.

## Proportionally Re-size Images

Aspose.Imaging APIs already support the feature of re-sizing existing images by passing the new height & width values as parameters to the Image.resize method but in that case the user had to calculate the aspect ratio himself. This is because when the width or height of an image is altered, the image either scales or shrinks to fill the new size. If the changes to the width and height of an image are not in proportion this could lead to stretched and distorted result.

Aspose.Imaging for Java 2.6.0 has exposed the resizeWidthProportionally and resizeHeightProportionally methods for the Image class that can be used to re-size existing images on the fly while keeping the aspect ratio as demonstrated below.

```
//Load an image from source
Image image = Image.load(sourceFile);

//Specify only width
int newWidth = image.getWidth() / 2;
image.resizeWidthProportionally(newWidth);

//Specify only height
int newHeight = image.getHeight() / 2;
image.resizeHeightProportionally(newHeight);

//Save result
image.save(outputFile);
```

Aspose.Imaging for Java 2.6.0 has also exposed overload versions of the resizeWidthProportionally and resizeHeightProportionally methods that can accept ResizeType as second parameter to achieve desired results. An important point to note is that if you intend to get quality result after applying the re-size then it is suggested that you should always use ResizeType.LanczosResample because it will output highly qualitative results but may work slower than ResizeType.NearestNeighbourResample. On the other hand, ResizeType.NearestNeighbourResample algorithm is specifically used for fast re-sizing while compromising on the image quality. This method may be useful for thumbnail generation in real time or similar processes where performance is required.

As always we appreciate your feedback so if you ever have anything to tell us about this release or anything else, please head to the [Aspose.Imaging forum][2] for a chat.




[1]: https://products.aspose.com/imaging/java
[2]: http://forum.aspose.com





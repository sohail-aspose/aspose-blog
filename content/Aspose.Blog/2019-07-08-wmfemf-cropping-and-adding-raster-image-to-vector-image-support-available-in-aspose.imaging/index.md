---
title: 'Crop WMF or EMF and Add Raster Image to Vector Image with Aspose.Imaging'
date: Mon, 08 Jul 2019 15:45:59 +0000
draft: false
url: /2019/07/08/wmfemf-cropping-and-adding-raster-image-to-vector-image-support-available-in-aspose.imaging/
author: Mudassir
summary: ''
tags: []
categories: ['Aspose.Imaging Product Family']
---



{{< figure align=center src="images/aspose-Imaging-for-net_100.png" alt="Crop WMF or EMF">}}


Hello readers, in this blog I would like to introduce you with new features included in Aspose.Imaging 19.6. The good thing about the Aspose team is that it releases both .NET and Java-based APIs simultaneously every month. This way both API users remain recurrent with changes being made in APIs every month.

In subsequent sections, I am going to give you a walkthrough of what new features have been included in API.

## Crop EMF/WMF Images

Image cropping usually refers to the removal of the outer parts of an image to help improve the framing. Cropping may also be used to cut out some portion of an image to increase the focus on a particular area. The **EmfImage\\WmfImage** class provides **Crop** method that accepts an instance of the **Rectangle** class. One can cut out any portion of an image by providing the desired boundaries to the **Rectangle** object.

The following examples demonstrate the cropping of a rectangular region in EMF and WMF images.  

{{< gist aspose-com-gists 2d1bcb9853315458808ffbcd9e7e3e02 "Examples-CSharp-ModifyingAndConvertingImages-CropEMFFile-CropEMFFile.cs" >}} {{< gist aspose-com-gists 2d1bcb9853315458808ffbcd9e7e3e02 "Examples-CSharp-ModifyingAndConvertingImages-CropWMFFile-CropWMFFile.cs" >}}

The similar Java-based implementation is like as under:

{{< gist aspose-com-gists 07be292db0a393dc95f153f84b28c069 "Examples-src-main-java-com-aspose-imaging-examples-EMF-CropEMFFile-CropEMFFile.java" >}} {{< gist aspose-com-gists 07be292db0a393dc95f153f84b28c069 "Examples-src-main-java-com-aspose-imaging-examples-wmf-CropWMFFile-CropWMFFile.java" >}}

## Drawing Raster Images on SVG, EMF, and WMF

Now, Aspose.Imaging supports drawing **Raster**(JPEG, GIF, TIFF, BMP) images to **Vector** (SVG, EMF, WMF) images. **Raster** images are based on pixels and thus lose clarity when scaled, while **Vector-ba**sed images can be scaled indefinitely without degrading quality. Using Aspose.Imaging you can draw a raster or vector image on another vector image.

## Adding Vector Image on another Vector Image

In the following example, I have shared the mechanism for adding a **Vector** image on another **Vector** image.

{{< gist aspose-com-gists 2d1bcb9853315458808ffbcd9e7e3e02 "Examples-CSharp-DrawingAndFormattingImages-DrawVectorImageToRasterImage-DrawVectorImageToRasterImage.cs" >}}

The similar Java based implementation is like as under:

{{< gist aspose-com-gists 07be292db0a393dc95f153f84b28c069 "Examples-src-main-java-com-aspose-imaging-examples-images-DrawVectorImageToRasterImage-DrawVectorImageToRasterImage.java" >}}

## Adding Raster Image on SVG

Using Aspose.Imaging, you can draw raster image on SVG. In following example, I have shared the mechanism for adding a **raster** image on another **SVG** image.

{{< gist aspose-com-gists 2d1bcb9853315458808ffbcd9e7e3e02 "Examples-CSharp-DrawingAndFormattingImages-DrawRasterImageOnSVG-DrawRasterImageOnSVG.cs" >}}

The similar Java based implementation is like as under:

{{< gist aspose-com-gists 07be292db0a393dc95f153f84b28c069 "Examples-src-main-java-com-aspose-imaging-examples-images-DrawRasterImageOnSVG-DrawRasterImageOnSVG.java" >}}

## Adding Raster Image on EMF

Using Aspose.Imaging, you can draw raster image on EMF. In following example, I have shared the mechanism for adding a **raster** image on another **EMF** image.

{{< gist aspose-com-gists 2d1bcb9853315458808ffbcd9e7e3e02 "Examples-CSharp-DrawingAndFormattingImages-DrawRasterImageOnEMF-DrawRasterImageOnEMF.cs" >}}

The similar Java based implementation is like as under:

{{< gist aspose-com-gists 07be292db0a393dc95f153f84b28c069 "Examples-src-main-java-com-aspose-imaging-examples-images-DrawRasterImageOnEMF-DrawRasterImageOnEMF.java" >}}

## Adding Raster Image on WMF

Using Aspose.Imaging, you can draw raster image on WMF. In following example, I have shared the mechanism for adding a **raster** image on another **WMF** image.

{{< gist aspose-com-gists 2d1bcb9853315458808ffbcd9e7e3e02 "Examples-CSharp-DrawingAndFormattingImages-DrawRasterImageOnWMF-DrawRasterImageOnWMF.cs" >}}

The similar Java based implementation is like as under:

{{< gist aspose-com-gists 07be292db0a393dc95f153f84b28c069 "Examples-src-main-java-com-aspose-imaging-examples-images-DrawRasterImageOnWMF-DrawRasterImageOnWMF.java" >}}

## Improved Image Processing

In this new release, we have improved the API performance in terms of adding support for multi-threading to manipulate the images along with options for optimizing memory usage during rendering

### Image processing using multi-threading

Aspose.Imaging is multi-thread safe as long as only one thread works on a document at a time. It is a typical scenario to have one thread working on one document. In the following example, we have demonstrated the use of parallel DJVU images processing using multi-threading.

{{< gist aspose-com-gists 2d1bcb9853315458808ffbcd9e7e3e02 "Examples-CSharp-ModifyingAndConvertingImages-DjVu-ParallelDJVUImagesProcessingUsingMultithreading-ParallelDJVUImagesProcessingUsingMultithreading.cs" >}}

The similar Java-based implementation is like as under:

{{< gist aspose-com-gists 07be292db0a393dc95f153f84b28c069 "Examples-src-main-java-com-aspose-imaging-examples-djvu-ParallelDJVUImagesProcessingUsingMultithreading-ParallelDJVUImagesProcessingUsingMultithreading.java" >}}

## Optimizing Memory Usage {#mce_43}

When reading a big PNG file, the total amount of RAM the process will take is always a concern. There are measures that can be adapted to cope with the challenge. Aspose.Imaging provides some relevant options and API calls to lower, reduce, and optimize memory use. Moreover, it can help the process work more efficiently and run faster.

The following example shows how to read a large PNG file in optimized mode.

{{< gist aspose-com-gists 2d1bcb9853315458808ffbcd9e7e3e02 "Examples-CSharp-ModifyingAndConvertingImages-PNG-ReadLargePNGFile-ReadLargePNGFile.cs" >}}

The similar Java-based implementation is like as under:

{{< gist aspose-com-gists 07be292db0a393dc95f153f84b28c069 "Examples-src-main-java-com-aspose-imaging-examples-ManipulatingPNGImages-ReadLargePNGFile-ReadLargePNGFile.java" >}}

Wait, there are many other features, enhancement, and bug fixes included in this release. [Here you can get the detail!][1]

When time allows you can check out API [examples at Github][2], talk about this release and other API related issues in our [forum][3].




[1]: https://docs.aspose.com/display/imagingnet/Aspose.Imaging+for+.NET+19.6+-+Release+Notes
[2]: https://github.com/aspose-imaging/
[3]: https://forum.aspose.com/c/imaging





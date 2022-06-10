---
title: 'Work with Device Independent Bitmap (DIB) Files in C# and Java'
date: Thu, 16 May 2019 20:50:18 +0000
draft: false
url: /2019/05/16/device-independent-bitmap-dib-file-format-support-included-in-aspose.imaging-19.4/
author: Mudassir
summary: ''
tags: []
categories: ['Aspose.Imaging Product Family']
---



{{< figure align=center src="images/aspose-Imaging-for-net_100.png" alt="">}}


Hello guys, in this blog I would like to introduce you with new enhancements being made in Aspose.Imaging 19.4. The good thing about the Aspose team is that it releases both .NET and Java-based APIs simultaneously every month. The latest release provides you the ability to work with **Device Independent Bitmap (DIB)** files in C# applications.

In subsequent sections, I am going to give you a walk through the new features that have been included in API.

## Work with Devise Independent Bitmap (DIB) Files

The DIB file format was developed to allow free image transfer regardless of the display device or operating system. It is similar to bitmap files, the only thing differentiating them being the lack of a file header and the fact that they're not device-dependent. The DIB file format contains all the information required for displaying a bitmap including color palette and metric resolution. DIB files can store 2D images of various resolutions, widths or heights and with color depths of 1, 4, 8, 16, 24 or 32 bits per pixel.

Using Aspose.Imaging, now you can access the DIB files and may convert them to other file formats like PNG, BMP, or JPEG. In the following example, the demonstration of loading an existing DIB file, and its conversion to PNG is exhibited.

{{< gist aspose-com-gists 2d1bcb9853315458808ffbcd9e7e3e02 "Examples-CSharp-ModifyingAndConvertingImages-SupportOfDIB-SupportOfDIB.cs" >}}

The similar Java-based implementation is like as under:

{{< gist aspose-com-gists 07be292db0a393dc95f153f84b28c069 "Examples-src-main-java-com-aspose-imaging-examples-images-SupportOfDIB-SupportOfDIB.java" >}}

## Word with CorelDRAW Drawing File (CDR)

CDR files are created with CorelDRAW. The CDR file format is proprietary and it is used by Corel as the default for saving images. It can store simple drawings and vector images. It is also capable of storing data used by CorelDraw such as nodes, layers, or segments.

In this version of Aspose.Imaging the support for CDR files has been included. In the following example below, an existing CDR file is loaded by passing the file path to the **Image** class static Load method.

{{< gist aspose-com-gists 2d1bcb9853315458808ffbcd9e7e3e02 "Examples-CSharp-ModifyingAndConvertingImages-CDR-SupportOfCDR-SupportOfCDR.cs" >}}

The similar Java-based implementation is like as under:

{{< gist aspose-com-gists 07be292db0a393dc95f153f84b28c069 "Examples-src-main-java-com-aspose-imaging-examples-CDR-SupportOfCDR-SupportOfCDR.java" >}}

## Raster Image Masking

The process of Masking involves setting some of the pixel values in an image to zero, or some other "background" value. Aspose.Imaging supports both Manual and Automatic masking features.



{{< figure align=center src="images/Colored-by-Faith_small-1.png" alt="">}}
</li><li class="blocks-gallery-item">

{{< figure align=center src="images/Colored-by-Faith_small.psd_._with_non_transparent_bg-1.png" alt="">}}
</li></ul></figure>

### Manual Masking

The following exhibit how to apply manual masking to a raster image.

{{< gist aspose-com-gists 2d1bcb9853315458808ffbcd9e7e3e02 "Examples-CSharp-ModifyingAndConvertingImages-ManualImageMasking-ManualImageMasking.cs" >}}

The similar Java-based implementation is like as under:

{{< gist aspose-com-gists 07be292db0a393dc95f153f84b28c069 "Examples-src-main-java-com-aspose-imaging-examples-ModifyingImages-ManualImageMasking-ManualImageMasking.java" >}}

### Automatic Masking {#mce_43}

The following sample demonstrates how to apply auto masking to a raster image.

{{< gist aspose-com-gists 2d1bcb9853315458808ffbcd9e7e3e02 "Examples-CSharp-ModifyingAndConvertingImages-AutoImageMasking-AutoImageMasking.cs" >}} {{< gist aspose-com-gists 2d1bcb9853315458808ffbcd9e7e3e02 "Examples-CSharp-ModifyingAndConvertingImages-AutoImageMasking-FillInputPoints.cs" >}}

The similar Java-based implementation is like as under:

{{< gist aspose-com-gists 07be292db0a393dc95f153f84b28c069 "Examples-src-main-java-com-aspose-imaging-examples-ModifyingImages-AutoImageMasking-AutoImageMasking.java" >}} {{< gist aspose-com-gists 07be292db0a393dc95f153f84b28c069 "Examples-src-main-java-com-aspose-imaging-examples-ModifyingImages-AutoImageMasking-FillInputPoints.java" >}} {{< gist aspose-com-gists 07be292db0a393dc95f153f84b28c069 "Examples-src-main-java-com-aspose-imaging-examples-ModifyingImages-AutoImageMasking-LEIntegerReader.java" >}}

Wait, there are many other features, enhancement, and bug fixes included in this release. [Here you can get the detail!][1]

When time allows you can check out API [examples at Github][2], talk about this release and other API related issues in our [forum][3].




[1]: https://docs.aspose.com/display/imagingnet/Aspose.Imaging+for+.NET+19.4+-+Release+Notes
[2]: https://github.com/aspose-imaging/
[3]: https://forum.aspose.com/c/imaging





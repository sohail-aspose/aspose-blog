---
title: 'Load and Save JPEG 2000 and DjVu with Optimized Memory in C# and Java'
date: Thu, 26 Dec 2019 07:25:15 +0000
draft: false
url: /2019/12/26/memory-optimization-for-jpeg2000-and-djvu-aspose-imaging-net-java/
author: Usman Aziz
summary: ''
tags: ['.NET', 'Aspose.Imaging API', 'C#', 'DjVu', 'JP2', 'JPEG 2000', 'Memory Optimization', 'java']
categories: ['Aspose.Imaging Product Family']
---



{{< figure align=center src="images/aspose_imaging-min.png" alt="C#.NET Java Library to Load and Save JPEG2000 and DjVu">}}


Memory optimization is an important factor to be considered when performing any computation or processing on digital data. Different optimization strategies are applied to minimize memory utilization as well as processing delay. This is the reason we have implemented the feature of memory optimization for loading and creating the [JPEG 2000][1] (JP2) and [DjVu][2] images in [Aspose.Imaging][3] for .NET and Java 19.12.

## Memory Optimization for JPEG 2000 Images

Aspose.Imaging for .NET and Java APIs support working with JPEG 2000 images. You can load the existing JPEG 2000 images as well as create and save JPEG 2000 images specifying different Jpeg2000 Codec options in C# or Java. In order to optimize memory consumption when loading and saving JPEG 2000 images, you can define the memory optimization strategy and limit the memory buffer size to be used.

Let's have a look at how to specify the memory buffer size when loading and creating JPEG 2000 images.

### Load JPEG 2000 Image

You can specify the memory buffer size when loading a JPEG 2000 image using _BufferSizeHint_ property in the _LoadOptions_ class as shown in the following C# and Java code samples.

#### **C#**

{{< gist aspose-com-gists ba8e70ccced6ac4a71f57cc3cfed2321 "LoadJPEG2000.cs" >}}

#### **Java**

{{< gist aspose-com-gists ba8e70ccced6ac4a71f57cc3cfed2321 "LoadJPEG2000.java" >}}

### Create or Save JPEG 2000 Image

Similar to the loading of JPEG 2000 images, you can specify memory buffer size when creating or saving the images using _BufferSizeHint_ property in _Jpeg2000Options_ class.

#### **C#**

{{< gist aspose-com-gists ba8e70ccced6ac4a71f57cc3cfed2321 "CreateJPEG2000.cs" >}}

#### **Java**

{{< gist aspose-com-gists ba8e70ccced6ac4a71f57cc3cfed2321 "CreateJPEG2000.java" >}}

## Memory Optimization for DjVu Images {#mce_24}

Aspose.Imaging for .NET and Java APIs also support working with DjVu images. You can load a DjVu image and perform the conversion from DjVu to raster image formats such as TIFF, PNG, etc. Similar to JEPG 2000 images, you can optimize memory utilization when loading a DjVu image as shown in the following C# and Java code samples.

#### **C#**

{{< gist aspose-com-gists ba8e70ccced6ac4a71f57cc3cfed2321 "LoadDjVu.cs" >}}

#### **Java**

{{< gist aspose-com-gists ba8e70ccced6ac4a71f57cc3cfed2321 "LoadDjVu.java" >}}

Well, you have seen that how to limit the memory buffer size when loading or creating JP2 or DjVu images using Aspose.Imaging. So, if you are working with JPEG 2000 and DjVu images and want to optimize the memory consumption, we recommend you to download and use Aspose.Imaging 19.12 within your .NET or Java applications.

As always, if you would have any questions or queries, do let us know via our [forum][4].




[1]: https://wiki.fileformat.com/image/jp2/
[2]: https://wiki.fileformat.com/image/djvu/
[3]: https://downloads.aspose.com/imaging
[4]: https://forum.aspose.com/c/imaging





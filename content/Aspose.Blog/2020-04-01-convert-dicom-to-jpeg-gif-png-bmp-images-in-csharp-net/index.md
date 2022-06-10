---
title: 'C# Convert DICOM to JPEG, GIF, PNG, and BMP Images'
seoTitle: "C# Convert DICOM to Images | DICOM to JPEG GIF PNG BMP Converter"
description: "Convert DICOM to JPEG, DICOM to GIF, DICOM to PNG, DICOM to BMP in C#. Create Online DICOM Converter using C# in ASP.NET MVC or WebForms."
date: Wed, 01 Apr 2020 16:03:45 +0000
draft: false
url: /2020/04/01/convert-dicom-to-jpeg-gif-png-bmp-images-in-csharp-net/
author: Usman Aziz
summary: ''
tags: ['DICOM to BMP', 'DICOM to GIF', 'DICOM to JPEG', 'DICOM to PNG', 'Online DICOM Converter']
categories: ['Aspose.Imaging Product Family']
---



{{< figure align=center src="images/DICOM-to-Image.png" alt="DICOM to Image ">}}


[DICOM][1] (**Digital Imaging and Communications in Medicine**) is a standard file format for storing medical imaging information. The information stored in the DICOM images is managed in the form of datasets including the header and the image data set. Most often, DICOM images contain medical scans such as ultrasounds, MRIs and etc. which are exchanged between multiple entities to share the patient's medical information.

In order to view the DICOM images, various offline and online DICOM viewers are available in the market. However, if you want to embed DICOM images in presentations or webpages, you will have to convert them into **JPEG**, **GIF**, **PNG**, **BMP** or some other image format. In accordance with this scenario, in this article, you will learn how to **convert DICOM** images **programmatically** in **C#**. Ultimately, you will be able to convert DICOM to the following image formats:

*   JPEG
*   GIF
*   PNG
*   BMP

## C# DICOM Converter API

In order to convert DICOM images, we'll use [Aspose.Imaging for .NET][2] which is an easy to use API for creating and manipulating various types of images within .NET applications. _Aspose.Imaging for .NET_ is hosted on [NuGet][3] as well as available as downloadable [binaries][4].

## Convert DICOM to JPEG in C#

The following are the steps to convert DICOM to JPEG in C#:

*   Load the DICOM file into a [FileStream][5] object.
*   Create an object of [DicomImage][6] class and initialize it with the _FileStream_ object.
*   Select the active page in DICOM that you want to convert to JPEG (if it is not set, the default active page will be converted).
*   Save the converted JPEG image using [DicomImage.Save(string, ImageOptionsBase)][7] method.

The following code sample converts a page in DICOM to JPEG in C#.

{{< gist aspose-com-gists 8f1fa6e4f45927c74554ba9c1e1531f2 "convert-DICOM-to-JPEG.cs" >}}

### Input DICOM



{{< figure align=center src="images/DICOM-to-JPG.png" alt="DICOM to JPEG">}}


### DICOM to JPEG



{{< figure align=center src="images/DICOM-to-JPG-Converted.png" alt="Convert DICOM to JPEG C#">}}


## Convert DICOM to GIF in C#

Converting DICOM to GIF is as simple as pie. Just access the DICOM file and save it with **.gif** extension. The following are the steps to convert DICOM to animated GIF in C#:

*   Access the DICOM file using [DicomImage][8] class.
*   Save the converted GIF image using [DicomImage.Save(string, ImageOptionsBase)][9] method.

The following code sample shows how to convert DICOM to GIF in C#.

{{< gist aspose-com-gists 8f1fa6e4f45927c74554ba9c1e1531f2 "convert-DICOM-to-GIF.cs" >}}

**Info**: You may find Aspose [Text to GIF][10] web app interesting.

## Convert DICOM to PNG in C#

Converting DICOM to PNG is as same as converting DICOM to JPEG. Simply access the DICOM file using [DicomImage][11] class and save it with **.png** extension. The following code sample shows how to convert a DICOM to PNG in C#.

{{< gist aspose-com-gists 8f1fa6e4f45927c74554ba9c1e1531f2 "convert-DICOM-to-PNG.cs" >}}

## Convert DICOM to BMP in C#

In order to convert DICOM to BMP, you can repeat the same steps to access the DICOM file using the [DicomImage][12] class. Once done, use [DicomImage.Save(string, ImageBaseOptions)][13] method to save DICOM as BMP. The following code sample shows how to convert DICOM to BMP in C#.

{{< gist aspose-com-gists 8f1fa6e4f45927c74554ba9c1e1531f2 "convert-DICOM-to-BMP.cs" >}}

## Learn more about Aspose.Imaging for .NET

Explore more about [working with images][14] using Aspose.Imaging for .NET API.

## See also

*   [Convert PSD to PDF, JPG, PNG and Other Image Formats in C#][15]




[1]: https://wiki.fileformat.com/image/dicom/
[2]: https://products.aspose.com/imaging/net
[3]: https://www.nuget.org/packages/Aspose.Imaging/
[4]: https://downloads.aspose.com/imaging/net
[5]: https://docs.microsoft.com/en-us/dotnet/api/system.io.filestream?view=netframework-4.8
[6]: https://apireference.aspose.com/net/imaging/aspose.imaging.fileformats.dicom/dicomimage
[7]: https://apireference.aspose.com/net/imaging/aspose.imaging.image/save/methods/3
[8]: https://apireference.aspose.com/net/imaging/aspose.imaging.fileformats.dicom/dicomimage
[9]: https://apireference.aspose.com/net/imaging/aspose.imaging.image/save/methods/3
[10]: https://products.aspose.app/slides/text-to-gif
[11]: https://apireference.aspose.com/net/imaging/aspose.imaging.fileformats.dicom/dicomimage
[12]: https://apireference.aspose.com/net/imaging/aspose.imaging.fileformats.dicom/dicomimage
[13]: https://apireference.aspose.com/net/imaging/aspose.imaging.image/save/methods/3
[14]: https://docs.aspose.com/display/imagingnet/Introduction
[15]: https://blog.aspose.com/2020/03/27/convert-psd-to-pdf-jpg-png-tiff-gif-bmp-jp2-in-csharp-net/






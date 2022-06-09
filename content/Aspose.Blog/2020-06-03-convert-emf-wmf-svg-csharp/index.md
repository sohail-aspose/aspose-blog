---
title: 'Convert EMF, WMF and SVG Images Programmatically using C#'
seoTitle: ""
description: ""
date: Wed, 03 Jun 2020 22:08:58 +0000
draft: false
url: /2020/06/03/convert-emf-wmf-svg-csharp/
author: Farhan Raza
summary: 'You can convert EMF images to EMZ or WMF images to WMZ as well as SVG images to SVGZ and other way around. Convert EMF, WMF and SVG to PNG images.'
tags: ['Convert EMF to EMz', 'Convert EMF to PNG', 'Convert EMZ to EMF', 'Convert SVG to PNG', 'Convert SVG to SVGZ', 'Convert SVGZ to SVG', 'Convert WMF to PNG', 'Convert WMF to WMZ', 'Convert WMZ to WMF']
categories: ['Aspose.Imaging Product Family']
---



{{< figure align=center src="images/aspose-Imaging-for-net_100.png" alt="Convert SVG">}}


Images are everywhere on the internet. Let us explore working with a few of the popular image formats including EMF, WMF, and SVG images. In this article, you will be considering the compression of EMF, WMF, and SVG vector images to EMZ, WMZ, and SVGZ respectively. Moreover, we will also learn how to convert EMF, WMF, and SVG vector images to raster images such as PNG using C#. Following are the use cases we will be exploring:

*   [Convert EMF to EMZ using C#][1]
*   [Convert EMZ to EMF using C#][2]
*   [Convert WMF to WMZ using C#][3]
*   [Convert WMZ to WMF using C#][4]
*   [Convert SVG to SVGZ using C#][5]
*   [Convert SVGZ to SVG using C#][6]
*   [Convert EMZ to PNG using C#][7]
*   [Convert WMZ to PNG using C#][8]
*   [Convert SVGZ to PNG using C#][9]

Vector image files are often huge in size so the compression and uncompression of such images are helpful when you need to transfer files over a network. Let us learn the conversions with Aspose.Imaging for .NET API.

## Convert EMF to EMZ using C# {#section1}

EMZ file is actually the compressed form of EMF image. You can convert EMF to EMZ by following below steps:

1.  Load source EMF image
2.  Initialize [VectorRasterizationOptions][10] object
3.  Save image while specifying [EmfOptions][11]

Below code snippet shows how to convert an EMF to EMZ using C#:

{{< gist aspose-cloud 7b6fd21096e2fbbda3548cdd8c565b96 "EMFtoEMZ.cs" >}}

## Convert EMZ to EMF using C# {#section2}

If you have received a compressed EMZ file and then you want to convert EMZ to EMF then follow the steps below:

1.  Load source EMZ file
2.  Initialize [EmfRasterizationOptions][12] object
3.  Save image while specifying [EmfOptions][13]

The code snippet below explains how to convert EMZ to EMF using C#:

{{< gist aspose-cloud 7b6fd21096e2fbbda3548cdd8c565b96 "EMZtoEMF.cs" >}}

## Convert WMF to WMZ using C# {#section3}

You can compress WMF images with Aspose.Imaging for .NET API. The compression process converts WMF to WMZ by following below steps:

1.  Load source WMF file
2.  Initialize [WmfRasterizationOptions][14] object
3.  Save the image using [WmfOptions][15]

Below code snippet shows how to convert WMF to WMZ using C#:

{{< gist aspose-cloud 7b6fd21096e2fbbda3548cdd8c565b96 "WMFtoWMZ.cs" >}}

## Convert WMZ to WMF using C# {#section4}

As we have already learned to compress WMF image. Aspose.Imaging for .NET API lets you uncompress WMZ files and convert such WMZ to WMF file. You should follow the following steps for conversion:

1.  Load input WMZ file
2.  Declare an instance of [WmfRasterizationOptions][16] class
3.  Save output image as WMF file

The code snippet below shows how to convert WMZ to WMF using C#:

{{< gist aspose-cloud 7b6fd21096e2fbbda3548cdd8c565b96 "WMZtoWMF.cs" >}}

## Convert SVG to SVGZ using C# {#section5}

SVG images are widely used to display high quality and complex graphics. You can compress such vector images and convert SVG to SVGZ with below steps:

1.  Load input SVG file
2.  Initialize [VectorRasterizationOptions][17] object
3.  Save output SVGZ image using [SvgOptions][18]

Following code snippet shows how to convert SVG to SVGZ using C#:

{{< gist aspose-cloud 7b6fd21096e2fbbda3548cdd8c565b96 "SVGtoSVGZ.cs" >}}

## Convert SVGZ to SVG using C# {#section6}

You can uncompress an SVGZ file and convert an SVGZ to SVG with simple steps below:

1.  Load input SVGZ file
2.  Specify [SvgRasterizationOptions][19] instance
3.  Save SVG image with [SvgOptions][20]

The following code snippet shows how to convert SVGZ to SVG using C#:

{{< gist aspose-cloud 7b6fd21096e2fbbda3548cdd8c565b96 "SVGZtoSVG.cs" >}}

So you have learned how to compress and uncompress vector format images including EMZ, WMZ and, SVGZ images. Let us move forward and understand how to convert such image files to raster images.

## Convert EMZ to PNG using C# {#section7}

EMZ is the compressed form of EMF image. You can directly convert it to a raster image format like PNG or JPG. You do not need to uncompress the image first and then convert it. Please follow below steps to convert EMZ to PNG image:

1.  Load input EMZ image
2.  Initialize an instance of [VectorRasterizationOptions][21] Class
3.  Save putput PNG image with [PngOptions][22]

The code snippet below shows how to convert EMZ to PNG image using C#:

{{< gist aspose-cloud 7b6fd21096e2fbbda3548cdd8c565b96 "EMZtoPNG.cs" >}}

## Convert WMZ to PNG using C# {#section8}

Now, let us learn the conversion of compressed WMF files, WMZ, directly to PNG. Below steps convert WMZ to PNG:

1.  Load source WMZ image file
2.  Declare an object of [VectorRasterizationOptions][23] class
3.  Save PNG image file using [PngOptions][24] class

The below code snippet follows these steps and shows how to convert WMZ to PNG using C#:

{{< gist aspose-cloud 7b6fd21096e2fbbda3548cdd8c565b96 "WMZtoPNG.cs" >}}

## Convert SVGZ to PNG using C# {#section9}

The exciting feature of SVGZ to PNG conversion has been introduced based on several requests from our customers. This feature lets you efficiently convert SVGZ to PNG images with high fidelity results. All you need to do is to follow the steps below:

*   Load source SVGZ image file
*   Initialize an object of [VectorRasterizationOptions][25] class
*   Save output PNG file by specifying [PngOptions][26]

The code snippet below is based on these steps which explain how to convert SVGZ to PNG with C#:

{{< gist aspose-cloud 7b6fd21096e2fbbda3548cdd8c565b96 "SVGZtoPNG.cs" >}}

## Conclusion

We have discussed the compression and uncompression of vector image formats which is helpful for transferring files. The approach is also suitable when you want to archive such images. For example, you can compress such vector images before archiving and later uncompress as per your requirements. Moreover, we have also explored the conversion of compressed vector images to raster images with Aspose.Imaging for .NET API. Furthermore, you may explore [API Reference][27] and [API Documentation][28]. Feel free to contact us at the [Free Support Forum][29] in case of any concern.

## See Also

[Generate HTML5 Canvas Programmatically using C#][30]




[1]: #section1
[2]: #section2
[3]: #section3
[4]: #section4
[5]: #section5
[6]: #section6
[7]: #section7
[8]: #section8
[9]: #section9
[10]: https://apireference.aspose.com/cad/net/aspose.cad.imageoptions/vectorrasterizationoptions
[11]: https://apireference.aspose.com/imaging/net/aspose.imaging.imageoptions/emfoptions
[12]: https://apireference.aspose.com/imaging/net/aspose.imaging.imageoptions/emfrasterizationoptions
[13]: https://apireference.aspose.com/imaging/net/aspose.imaging.imageoptions/emfoptions
[14]: https://apireference.aspose.com/imaging/net/aspose.imaging.imageoptions/wmfrasterizationoptions
[15]: https://apireference.aspose.com/imaging/net/aspose.imaging.imageoptions/wmfoptions
[16]: https://apireference.aspose.com/imaging/net/aspose.imaging.imageoptions/wmfrasterizationoptions
[17]: https://apireference.aspose.com/cad/net/aspose.cad.imageoptions/vectorrasterizationoptions
[18]: https://apireference.aspose.com/imaging/net/aspose.imaging.imageoptions/svgoptions
[19]: https://apireference.aspose.com/imaging/net/aspose.imaging.imageoptions/svgrasterizationoptions
[20]: https://apireference.aspose.com/imaging/net/aspose.imaging.imageoptions/svgoptions
[21]: https://apireference.aspose.com/cad/net/aspose.cad.imageoptions/vectorrasterizationoptions
[22]: https://apireference.aspose.com/imaging/net/aspose.imaging.imageoptions/pngoptions
[23]: https://apireference.aspose.com/cad/net/aspose.cad.imageoptions/vectorrasterizationoptions
[24]: https://apireference.aspose.com/imaging/net/aspose.imaging.imageoptions/pngoptions
[25]: https://apireference.aspose.com/cad/net/aspose.cad.imageoptions/vectorrasterizationoptions
[26]: https://apireference.aspose.com/imaging/net/aspose.imaging.imageoptions/pngoptions
[27]: https://apireference.aspose.com/imaging/net
[28]: https://docs.aspose.com/display/imagingnet/Home
[29]: https://forum.aspose.com/c/imaging
[30]: https://blog.aspose.com/2020/06/01/generate-html5-canvas-programmatically-using-csharp-vb.net/






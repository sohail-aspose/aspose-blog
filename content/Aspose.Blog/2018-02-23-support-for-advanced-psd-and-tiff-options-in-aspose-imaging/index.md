---
title: 'Convert PSD to PDF and Use Advanced PSD and TIFF Options using C#'
date: Fri, 23 Feb 2018 16:48:50 +0000
draft: false
url: /2018/02/23/support-for-advanced-psd-and-tiff-options-in-aspose-imaging/
author: Mudassir
summary: ''
tags: ['Convert PSD to PDF in CSharp']
categories: ['Aspose.Imaging Product Family']
---

We like to share the release announcement for [Aspose.Imaging for .NET][1] 18.2. In this release, we have added support for many features along with the resolution of outstanding issues in API.

## Convert PSD to PDF 

The following code sample shows how to convert PSD to PDF in C#

{{< gist aspose-imaging b93073a27bcdd4fefc2821e113f0cb3a "Examples-CSharp-ModifyingAndConvertingImages-PSD-PSDtoPDF-PSDtoPDF.cs" >}}

## Other Features

The following features have been introduced in this release.

*   [Support TIFF deflate Images with Alpha][2].
*   [Convert Image to grayscale with setting 16bit][3]

## Enhancements

The following enhancements have been introduced in this release.

*   Fix PSD export of multiple styles for a single text layer.
*   EMF to PDF generated blank document.
*   Support the \[interlaced Gif to non-interlaced PNG\] conversion.
*   Coordinate of the left top corner is incorrect at update.
*   Incorrect exporting EMF+ to SVG.
*   Wrong FileFormat returned on loading BMP Images.
*   Implement \[Jpeg DCT extended sequential, Huffman. 12-bit\] decoder.
*   Improve performance Jpeg2000 decoder.
*   Improper export of SVG export to PNG, JPEG, and BMP formats.
*   chart axis values are improperly positioned when exporting SVG to PNG.
*   System.IndexOutOfRangeException when loading pixels from the Tiff image.
*   A bad quality image is generated for Tiff.
*   Applying MedianFilterOptions on an image is blurring the resultant image.
*   Converting WMF to SVG format is not working properly. It is generating SVG file but SVG file is empty.
*   Converting EMF to SVG format is not working properly. It is generating SVG file but SVG file is empty.
*   Converting JPEG to gray scale at 300DPI and 8BIT not working if we save the resultant image in a stream.
*   Unable to convert 360MB TIFF file to PDF.

Please refer to the release notes of [Aspose.Imaging for .NET 18.2][4] for a full view of improvements along with sample code snippets for newly added features. If you are planning to upgrade the API to the latest revision, we strongly suggest you check the [Public API Change][5] section to know what has been changed in the public API since your current version.

## Aspose.Imaging for .NET Resources

The resources, you may need to accomplish your tasks:

*   [Home page for Aspose.Imaging for .NET API][6].
*   [Download Aspose.Imaging for .NET][7].
*   [Aspose.Imaging for .NET online documentation][8] – help documentation and API reference documents.
*   [Aspose.Imaging Product Family Forum][9] – post your technical questions and queries, or any other problem you are facing while working with Aspose.Imaging APIs.
*   [Enable blog Subscription][10] – Do not limit yourself, you can keep yourself updated with the latest news on Aspose.Imaging APIs, new features, fixes, and other API related topics by subscribing to Aspose.Imaging blog.
*   [Aspose.Imaging for .NET Examples][11] – We have published our code examples on the social coding website GitHub.com. Anyone can explore the code examples for learning purposes.

As always, we appreciate your feedback so if you ever have anything to share with us about this release or anything else, please feel free to contact us in [Aspose.Imaging forum][12].




[1]: https://products.aspose.com/imaging/net
[2]: https://docs.aspose.com/display/imagingnet/Manipulating+TIFF+Images#ManipulatingTIFFImages-SupportTiffdeflateImageswithAlpha
[3]: https://docs.aspose.com/display/imagingnet/Converting+Images#ConvertingImages-ConvertImagetograyscalewithSetting16bit
[4]: https://docs.aspose.com/display/imagingnet/Aspose.Imaging+for+.NET+18.2+-+Release+Notes
[5]: https://docs.aspose.com/display/imagingnet/Aspose.Imaging+for+.NET+18.2+-+Release+Notes
[6]: https://products.aspose.com/imaging/net
[7]: https://www.nuget.org/packages/Aspose.Imaging/18.2.0
[8]: https://docs.aspose.com/display/imagingnet/Home
[9]: https://forum.aspose.com/c/imaging
[10]: https://blog.aspose.com/category/aspose-products/aspose.imaging-product-family/
[11]: https://github.com/aspose-imaging/Aspose.Imaging-for-.NET
[12]: https://forum.aspose.com/c/imaging





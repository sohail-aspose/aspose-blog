---
title: 'Convert CMX to PNG, JPEG, BMP, or TIFF in C#'
date: Tue, 19 Mar 2019 18:02:47 +0000
draft: false
url: /2019/03/19/convert-cmx-to-png-jpeg-bmp-or-tiff-images-in-csharp-asp.net/
author: Mannanfazil
summary: ''
tags: ['CMX to BMP', 'CMX to JPEG', 'CMX to TIFF', 'Convert CMX to PNG']
categories: ['Aspose.Imaging Product Family']
---

Corel Metafile Exchange (CMX) is a metafile format that supports bitmap and vector information and the full range of PANTONE, RGB and CMYK colors. This format is used for data exchange in programs that work with vector graphics. It contains image data and also the metadata that describes it. The purpose of this post is to demonstrate how you can export the existing CMX file to other formats (PNG, JPEG, BMP, TIFF) using Aspose.Imaging.

## Convert CMX to PNG in C#

Using **Aspose.Imaging.ImageOptions.PngOptions** class you can export existing CMX file to PNG format. **CmxRasterizationOptions** class is used to set different properties as per requirement.

Using **CmxRasterizationOptions.Positioning** parameter, you can set the Positioning and size-types of a graphics scene. **CmxRasterizationOptions.Positioning** parameter can take one of the following three values.

**Value**

**Description**

DefinedByDocument

The absolute positioning on the page that is defined by document page settings.  
  

DefinedByOptions

The absolute positioning on the page that is defined by options page settings.  
  

Relative

The relative positioning and size. Determined by the boundary of all graphics objects.

**CmxRasterizationOptions.SmoothingMode** parameter specifies whether smoothing (antialiasing) is applied to lines and curves and the edges of filled areas. **CmxRasterizationOptions.SmoothingMode** parameter can take one of the following six values.

<figure class="wp-block-table is-style-stripes"><table class=""><tbody><tr><td>**Value</strong></td><td><strong>Description**</td></tr><tr><td>Invalid</td><td>Specifies an invalid mode.<br><br></td></tr><tr><td>Default</td><td>Specifies no antialiasing.<br><br></td></tr><tr><td>HighSpeed</td><td>Specifies no antialiasing.<br><br></td></tr><tr><td>None</td><td>Specifies no antialiasing<br><br></td></tr><tr><td>AntiAlias</td><td>Specifies antialiased rendering.<br><br></td></tr><tr><td>HighQuality</td><td>Specifies antialiased rendering.<br></td></tr></tbody></table></figure>

The following code is loading existing CMX files using Image class and setting Positioning to DefinedByDocument and SmoothingMode to AntiAlias and exporting loaded CMX file to PNG.

{{< gist aspose-com-gists 2d1bcb9853315458808ffbcd9e7e3e02 "Examples-CSharp-ModifyingAndConvertingImages-CMX-CMXToPNGConversion-CMXToPNGConversion.cs" >}}

Finally, after exporting the CMX file to PNG, the output PNG looks as follows:



{{< figure align=center src="images/CMXToPNG.png" alt="CMX to PNG C#">}}


The complete code of this post is available on [GitHub][1].




[1]: https://github.com/aspose-imaging/Aspose.Imaging-for-.NET/blob/master/Examples/CSharp/ModifyingAndConvertingImages/CMX/CMXToPNGConversion.cs





---
title: 'Find Layers and Update Layer's Text or Image in Photoshop Files using C#'
seoTitle: "C# Update Text and Image in Photoshop Layers (PSD)"
description: "Find layer and update the layer's text and image in Photoshop PSD files using C# or VB.NET. Find PSD layers by name and update the layer's content using C#."
date: Mon, 08 Jun 2020 17:23:47 +0000
draft: false
url: /2020/06/08/find-and-update-text-or-image-layers-in-psd-files-using-csharp/
author: Usman Aziz
summary: ''
tags: ['Csharp PSD Library', 'Find and Replace Layer in PSD using Csharp', 'Update image layer in PSD using Csharp', 'Update text layer in PSD using Csharp']
categories: ['Aspose.PSD Product Family']
---

In this article, you will learn how to find layers and update the layer's text or image within Photoshop's PSD files dynamically using C# .NET.

[PSD][1] is the default format used by Adobe Photoshop for saving its documents in a multilayered structure where each layer contains the text, images, graphical objects, and other supported elements. There could be the case when you have a PSD template and you need to create several resultant images by populating the text and image layers within the template. An example of such a scenario is creating employee cards within an organization. In order to automate this process, I'll show you how to:

*   [find and update text layers in PSD files using C#][2]
*   [find and update image layers in PSD files using C#][3]

## C# Library to Find and Update PSD Layers

[Aspose.PSD for .NET][4] allows creating and modifying PSD files without installing Adobe Photoshop or Illustrator. The API can be handy in the scenario where you need to update PSD layers dynamically using C# or VB.NET. You can install the API using [NuGet Package Manager][5] or download and reference its [DLLs][6] manually.

## Find and Update Text Layers in PSD Files using C# {#find-and-replace-text-layers-in-Photoshop-PSD-files-using-CSharp}

Aspose.PSD for .NET allows you to find the desired layer in PSD files using the layer's name. Once you find the layer, you can update its content. The following are the steps to find and update a text layer in a PSD file.

*   Create an instance of the [PsdImage][7] class and initialize it with the PSD file's path.
*   Access the layers in the PSD using [PsdImage.Layers][8] property.
*   Match each layer's display name to get the desired layer into the [TextLayer][9] object.
*   Update the text using [TextLayer.UpdateText(String)][10] method.
*   Save the updated image using [PsdImage.Save(String)][11] method.

The following code sample shows how to find and update the text layer in the PSD file using C#.

{{< gist aspose-com-gists 15000fd8740fd1f404dce8a1276fe94d "update-text-layer-in-psd.cs" >}}

Below is the screenshot of the input PSD file we have used in this example:



{{< figure align=center src="images/template.jpg" alt="Find layer in PSD using C#">}}


The following is the resultant PSD file having updated text layer:



{{< figure align=center src="images/Find-and-replace-text-in-PSD-C.jpg" alt="Update text layer in PSD using C#">}}


## Find and Update Image Layers in PSD Files using C# {#find-and-replace-image-layers-in-PSD-files-using-CSharp}

In order to deal with graphical objects such as images, Aspose.PSD for .NET exposes [Graphics][12] class. This class is used to clear or draw the graphics within the PSD layers. The following are the steps to find a PSD layer and update its image.

*   Create an object of the [PsdImage][13] class to load the PSD file.
*   Find the layer in the PSD file from [PsdImage.Layers][14] object.
*   Load the image you want to draw in the layer in a [Stream][15] object.
*   Create a new Layer object and initialize it with the _Stream_ object created in the previous step.
*   Create an instance of the [Graphics][16] class and initialize it with layer to be replaced.
*   Clear the layer using [Graphics.Clear()][17] method.
*   Draw the image in the layer using [Graphics.DrawImage(Image, Rectangle)][18] method.
*   Save the file using [PsdImage.Save(String)][19] method.

The following code sample shows how to find and update image layers in the PSD file using C#.

{{< gist aspose-com-gists 15000fd8740fd1f404dce8a1276fe94d "update-image-layer-in-psd.cs" >}}

The following is the screenshot of the PSD file after updating the image layer using the above-mentioned code:



{{< figure align=center src="images/Find-and-replace-image-in-PSD-C.jpg" alt="Update image layer in PSD using C#">}}


## Conclusion

In this article, we have seen how to find and update the layers in a Photoshop file (PSD) using C#. The step by step guide and code samples demonstrate how to find layers and update their text or image in the Photoshop PSD files. You can explore more about Aspose.PSD for .NET using [documentation][20].

## See Also

*   [Convert PSD to PDF, JPG, PNG and Other Raster Image Formats in C#][21]




[1]: https://wiki.fileformat.com/image/psd/
[2]: #find-and-replace-text-layers-in-Photoshop-PSD-files-using-CSharp
[3]: #find-and-replace-image-layers-in-PSD-files-using-CSharp
[4]: https://products.aspose.com/psd/net
[5]: https://www.nuget.org/packages/Aspose.PSD
[6]: https://downloads.aspose.com/psd/net
[7]: https://apireference.aspose.com/psd/net/aspose.psd.fileformats.psd/psdimage
[8]: https://apireference.aspose.com/psd/net/aspose.psd.fileformats.psd/psdimage/properties/layers
[9]: https://apireference.aspose.com/psd/net/aspose.psd.fileformats.psd.layers/textlayer
[10]: https://apireference.aspose.com/psd/net/aspose.psd.fileformats.psd.layers/textlayer/methods/updatetext
[11]: https://apireference.aspose.com/psd/net/aspose.psd.datastreamsupporter/save/methods/2
[12]: https://apireference.aspose.com/psd/net/aspose.psd/graphics
[13]: https://apireference.aspose.com/psd/net/aspose.psd.fileformats.psd/psdimage
[14]: https://apireference.aspose.com/psd/net/aspose.psd.fileformats.psd/psdimage/properties/layers
[15]: https://docs.microsoft.com/en-us/dotnet/api/system.io.stream?view=netcore-3.1
[16]: https://apireference.aspose.com/psd/net/aspose.psd/graphics
[17]: https://apireference.aspose.com/psd/net/aspose.psd/graphics/methods/clear
[18]: https://apireference.aspose.com/psd/net/aspose.psd.graphics/drawimage/methods/10
[19]: https://apireference.aspose.com/psd/net/aspose.psd.datastreamsupporter/save/methods/2
[20]: https://docs.aspose.com/display/psdnet/Product+Description
[21]: https://blog.aspose.com/2020/03/27/convert-psd-to-pdf-jpg-png-tiff-gif-bmp-jp2-in-csharp-net/






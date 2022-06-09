---
title: 'Flatten or Merge Layers in PSD Image using C#'
seoTitle: "Flatten or Merge Layers in PSD Image Programmatically using C#"
description: "You can flatten or merge layers in PSD image files programmatically using C#. Work with PSD image layers in your .NET applications."
date: Fri, 10 Dec 2021 06:27:00 +0000
draft: false
url: /2021/12/10/flatten-merge-layers-in-psd-csharp/
author: Farhan Raza
summary: 'PSD images are popularly used to create logos, brochures, and other images where the PSD files contain several layers. In certain situations, you might need to manipulate the layers like flatten or merge layers in a PSD file. This article covers how to **flatten or merge layers in a PSD file programmatically in C#**.'
tags: ['Flatten PSD Layers csharp', 'Merge PSD Layers C#', 'flatten layers in PSD image', 'merge layers in PSD Image']
categories: ['Aspose.PSD Product Family']
---



{{< figure align=center src="images/Merge-Flatten-PSD-Layer.png" alt="Flatten Merge Layers in PSD C#">}}


PSD images are popularly used to create logos, brochures, and other images where the PSD files contain several layers. In certain situations, you might need to manipulate the layers like flatten or merge layers in a PSD file. This article covers how to flatten or merge layers in a PSD file programmatically in C#:

*   [C# API to Flatten or Merge Layers in PSD Image][1]
*   [Flatten Layers in PSD Image using C#][2]
*   [Merge Layers in PSD File using C#][3]

## C# API to Flatten or Merge Layers in PSD Image {#section1}

[Aspose.PSD for .NET][4] API supports creating, editing, or manipulating PSD and several other [supported file formats][5]. You can easily install the API by downloading the DLL file from the [New Releases][6] section or by using the following [NuGet][7] command:

```
PM> Install-Package Aspose.PSD
```

## Flatten Layers in PSD Image using C# {#section2}

You can flatten layers in a PSD image with the following steps:

1.  Load the input PSD image using the [Image][8] class.
2.  Call the [FlattenImage][9] method.
3.  Write the output file using the [Save][10] method.

The following code snippet explains how to flatten layers in a PSD image programmatically in C#:

{{< gist aspose-com-gists 46dc6ef2aa8ffb86fc381b8b1b20e0a0 "Flatten-PSD-Layers.cs" >}}

## Merge Layers in PSD File using C# {#section3}

You can merge two or more layers in a PSD file by following the steps below:

1.  Load the input PSD image using the [Image][11] class.
2.  Read the layers from the PSD file.
3.  Merge the layers using the [MergeLayers][12] method.
4.  Set up the merged layers and save the output file.

The following code snippet explains how to merge layers in PSD file using C#:

{{< gist aspose-com-gists 46dc6ef2aa8ffb86fc381b8b1b20e0a0 "Merge-PSD-Layers.cs" >}}

## Get Free Evaluation License

You can evaluate the API in full capacity without any evaluation limitations by requesting a [free temporary license][13].

## Conclusion

In this article, you have learned how to flatten or merge layers in a PSD image programmatically using C#. These features can be helpful in scenarios like when you do not want to share the editable files with anyone for avoiding any changes. Moreover, please take a look at the [documentation][14] to learn different features supported by the API. Please feel free to contact us at the [forum][15] in case of any concerns.

## See Also

[Convert PSD to TIFF Image in C#][16]

[Rotate or Crop PSD Image using C#][17]




[1]: #section1
[2]: #section2
[3]: #section3
[4]: https://products.aspose.com/psd/net/
[5]: https://docs.aspose.com/psd/net/supported-file-formats/
[6]: https://downloads.aspose.com/psd/net
[7]: https://www.nuget.org/packages/Aspose.Psd/
[8]: https://apireference.aspose.com/psd/net/aspose.psd/image
[9]: https://apireference.aspose.com/psd/net/aspose.psd.fileformats.psd/psdimage/methods/flattenimage
[10]: https://apireference.aspose.com/psd/net/aspose.psd/image/methods/save/index
[11]: https://apireference.aspose.com/psd/net/aspose.psd/image
[12]: https://apireference.aspose.com/psd/net/aspose.psd.fileformats.psd/psdimage/methods/mergelayers
[13]: https://purchase.aspose.com/temporary-license
[14]: https://docs.aspose.com/psd/net/
[15]: https://forum.aspose.com/c/psd
[16]: https://blog.aspose.com/2021/11/18/convert-psd-to-tiff-image-csharp/
[17]: https://blog.aspose.com/2021/09/25/crop-rotate-psd-csharp/





---
title: 'Create Clipping Path in TIFF Images using C#'
seoTitle: ""
description: ""
date: Mon, 31 Aug 2020 14:30:34 +0000
draft: false
url: /2020/08/31/create-clipping-path-in-tiff-images-using-csharp/
author: Usman Aziz
summary: ''
tags: ['create clipping path in tiff', 'create clipping path in tiff using csharp', 'export tiff with clipping path to psd', 'tiff to psd']
categories: ['Aspose.Imaging Product Family']
---

[Clipping Path][1] is a closed vector path used to select a part of the image that should be visible. Once the clipping path is created, the part of the image outside the clipping path becomes transparent or invisible. In Adobe Photoshop, the clipping path technique is most often used to remove the background from the images and photographs. In this article, you will learn how to **create a clipping path in [TIFF][2] images** programmatically using C#. Furthermore, you'll come to know how to **export TIFF images to [PSD][3]** format along with the clipping path.

*   [.NET API for Creating Clipping Path in TIFF][4]
*   [Create Clipping Path in TIFF Image using C#][5]
*   [Export TIFF with Clipping Path to PSD using C#][6]

## .NET API for Creating Clipping Path in TIFF {#NET-API-for-Creating-Clipping-Path-in-TIFF}

[Aspose.Imaging for .NET][7] is a well-known image processing API that allows you to process and work with a wide range of image formats. In addition, the API lets you create the clipping paths in TIFF programmatically and transfer the clipping path from TIFF to the PSD image with a few lines of code. You can install the API within your .NET application using [NuGet][8] or download its DLL from [here][9].

## Create Clipping Path in TIFF Image using C# {#Create-Clipping-Path-in-TIFF-Image-using-CSharp}

For creating the clipping path in a TIFF image, you would need to define the points of the path in a TXT file. You can either create the points manually or using the Pen tool in Photoshop. The following is a sample TXT file containing the Bezier points of a clipping path that will be used in the examples below.



{{< figure align=center src="images/Path-Points.jpg" alt="">}}


Once you have created the path points, you can insert them into the Path Resources of the TIFF image. Below is the targetted TIFF image that is being used in the examples.



{{< figure align=center src="images/Tiff-Image-for-Clipping-Path.jpg" alt="Sample TIFF Image">}}


The following code sample shows how to create a clipping path in a Tiff image.

{{< gist aspose-com-gists 2d1bcb9853315458808ffbcd9e7e3e02 "Examples-Create-Clipping-Path-Tiff-Psd-Manually.cs" >}}

The following is the screenshot of the resultant TIFF image along with the clipping path in Photoshop.



{{< figure align=center src="images/Tiff-Image-with-Clipping-Path.jpg" alt="TIFF with Clipping Path">}}


## Export TIFF with Clipping Path to PSD using C# {#Export-TIFF-with-Clipping-Path-to-PSD-using-CSharp}

You can also export the TIFF image having a clipping path to a PSD image for further processing in Photoshop. This can be done in a couple of lines of code.

*   Load the TIFF image using [Image.Load(String)][10] method.
*   Export TIFF to PSD using [Image.Save(String, PsdOptions)][11] method.

The following code sample shows how to export a TIFF image having a clipping path to PSD using C#.

{{< gist aspose-com-gists 2d1bcb9853315458808ffbcd9e7e3e02 "Examples-Transfer-Tiff-Path-To-Psd.cs" >}}

### PSD File



{{< figure align=center src="images/PSD-with-Clipping-Path.jpg" alt="TIFF to PSD with Clipping Path">}}


## Conclusion

In this article, you have seen how to create a clipping path in a TIFF image programmatically using C#. Furthermore, you have also learned how to export a TIFF image to PSD along with the clipping path using Aspose.Imaging for .NET API. You can explore more about Aspose's image processing API using the [documentation][12].

## See Also

*   [Create Animated PNG Images using C# or VB.NET][13]




[1]: https://en.wikipedia.org/wiki/Clipping_path
[2]: https://docs.fileformat.com/image/tiff/
[3]: https://docs.fileformat.com/image/psd/
[4]: #NET-API-for-Creating-Clipping-Path-in-TIFF
[5]: #Create-Clipping-Path-in-TIFF-Image-using-CSharp
[6]: #Export-TIFF-with-Clipping-Path-to-PSD-using-CSharp
[7]: https://products.aspose.com/imaging/net
[8]: http://nuget.org/packages/Aspose.Imaging
[9]: https://downloads.aspose.com/imaging/net
[10]: https://apireference.aspose.com/imaging/net/aspose.imaging.image/load/methods/2
[11]: https://apireference.aspose.com/imaging/net/aspose.imaging.image/save/methods/3
[12]: https://docs.aspose.com/imaging/net/getting-started/
[13]: https://blog.aspose.com/2020/07/02/create-animated-png-using-csharp-or-vb.net/






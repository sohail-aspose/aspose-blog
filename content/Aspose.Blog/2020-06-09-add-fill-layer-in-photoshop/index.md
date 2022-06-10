---
title: 'Add Fill Layer in Photoshop Document (PSD file) - Easy Guide'
seoTitle: "Add Fill Layer in Photoshop | Add Fill Layer in PSD File using C#"
description: "Add fill layer in Photoshop document with C#. Insert fill layer in PSD at runtime as well as in existing files. Pattern, gradient, and color fill supported."
date: Tue, 09 Jun 2020 18:29:58 +0000
draft: false
url: /2020/06/09/add-fill-layer-in-photoshop/
author: Farhan Raza
summary: ''
tags: ['add fill layer in photoshop', 'add layer in photoshop', 'add layer in psd']
categories: ['Aspose.PSD Product Family']
---



{{< figure align=center src="images/Add_Fill_Layer_in_Photoshop-300x300.png" alt="Add fill layer in photoshop">}}


Photos are a very useful way of reflecting information. [PSD][1] format files are used to create images. However, there could be scenarios like editing several Photoshop files along the same lines. For instance, a photo processing application may need to add a layer in multiple Photoshop documents, along with other operations. [Aspose.PSD for .NET][2] API offers many features to work with PSD, PSB, AI, and many other file formats. Let us explore the following use cases related to adding a layer in PSD files:

*   [Add Fill Layer at Runtime in PSD file using C#][3]
*   [Add Existing Fill Layer in PSD file using C#][4]
    *   [Add a Fill Layer with Pattern Fill][5]
    *   [Add a Fill Layer with Gradient Fill][6]
    *   [Add a Fill Layer with Color Fill][7]

## Add Fill Layer at Runtime in Photoshop Document using C# {#section1}

Aspose.PSD for .NET API supports creating a fill layer in a PSD file. You do not necessarily need to load the layer from an existing file. Simply follow below steps to add a fill layer at runtime in the PSD file:

1.  Initialize an instance of [PsdImage][8] class with page dimensions
2.  Create an instance of [FillLayer][9] class
3.  Set Display Name for the layer
4.  Add the layer to the image

Following code snippet shows how to add fill layer in Photoshop using C#:

\[gist id="7b6fd21096e2fbbda3548cdd8c565b96" file="Add\_Layer\_in\_Photoshop.cs"\]

This code snippet will generate a PSD file of specified dimensions where the screenshot below is showing names of three fill layers exactly as set by C# code above:



{{< figure align=center src="images/Add-Layer-in-Photoshop-1024x514.png" alt="Add Layer in Photoshop">}}


## Add Existing Fill Layer in PSD file using C# {#section2}

We have already learned about creating and adding new fill layers. Let us check out how to add layer from existing Photoshop file. Following are the possibilities of adding existing fill layers:

### i) Add a Fill Layer with Pattern Fill using C# {#section3}

A pattern fill may have an image, line, or shadow to fill the area. You need to follow the steps below for adding a layer with Patten Fill in a PSD image:

1.  Load source PSD file
2.  Iterate through all layers and check for [FillLayer][10]
3.  Set different settings for the layer
4.  Edit the Fill Layer
5.  Save the image

The code snippet below shows how to add fill layer with Pattern fill using C#:

\[gist id="7b6fd21096e2fbbda3548cdd8c565b96" file="Add\_Layer\_Pattern\_Fill.cs"\]

### ii) Add a Fill Layer with Gradient Fill using C# {#section4}

You can also use Gradient fill for filling a layer in Photoshop Document. Aspose.PSD for .NET API supports the following types of Gradient fills:

*   **Linear**
*   **Diamond**
*   **Radial**
*   **Reflected**
*   **Angle**

Below are the steps for adding a layer with a gradient fill:

*   Load source PSD file
*   Initialize a collection of [GradientType][11]
*   Declare an instance of [GradientFillSettings][12] Class
*   Specify [GradientType][13] and update layer
*   Save PSD image

The code snippet below is based on these steps and shows how to add GradientFill layer in Photoshop document using C#:

\[gist id="7b6fd21096e2fbbda3548cdd8c565b96" file="Add\_Layer\_Gradient\_Fill.cs"\]

This code snippet will generate five different files, each with a different kind of Gradient fill in the layer of the PSD file.

### iii) Add a Fill Layer with Color Fill using C# {#section5}

You can add a layer with Color fill in Photoshop Document, a PSD file. Follow the steps below for adding or creating a Fill Layer with Color Fill:

1.  Load source PSD image
2.  Check all layers and find [FillLayer][14]
3.  Read fill settings of the layer
4.  Set fill color and update the layer
5.  Save the PSD image

The code snippet below is based on the aforementioned steps that show how to add fill layer in Photoshop Document using C#:

\[gist id="7b6fd21096e2fbbda3548cdd8c565b96" file="Add\_Layer\_Color\_Fill.cs"\]

## Conclusion

In this article, you have explored a few of the many possibilities for adding a fill layer in PSD files. You have learned how to add a layer from scratch, as well as how to add a layer from existing PSD files. Different types of Gradient fill layers are also addressed along with examples. There are many other exciting features offered by [Aspose.PSD for .NET][15] API. Please feel free to get in touch with us via [Free Support Forums][16] in case of any concerns.

## See Also

[Find Layers and Update Layer’s Text or Image in Photoshop Files][17]



[1]: https://wiki.fileformat.com/image/psd/
[2]: https://products.aspose.com/psd/net
[3]: #section1
[4]: #section2
[5]: #section3
[6]: #section4
[7]: #section5
[8]: https://apireference.aspose.com/psd/net/aspose.psd.fileformats.psd/psdimage
[9]: https://apireference.aspose.com/psd/net/aspose.psd.fileformats.psd.layers.filllayers/filllayer
[10]: https://apireference.aspose.com/psd/net/aspose.psd.fileformats.psd.layers.filllayers/filllayer
[11]: https://apireference.aspose.com/psd/net/aspose.psd.fileformats.psd.layers.fillsettings/gradienttype
[12]: https://apireference.aspose.com/psd/net/aspose.psd.fileformats.psd.layers.fillsettings/gradientfillsettings
[13]: https://apireference.aspose.com/psd/net/aspose.psd.fileformats.psd.layers.fillsettings/gradienttype
[14]: https://apireference.aspose.com/psd/net/aspose.psd.fileformats.psd.layers.filllayers/filllayer
[15]: https://products.aspose.com/psd/net
[16]: https://forum.aspose.com/c/psd
[17]: https://blog.aspose.com/2020/06/08/find-and-update-text-or-image-layers-in-psd-files-using-csharp/






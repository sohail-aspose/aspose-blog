---
title: 'Working with Layer Properties using Aspose.PSD'
date: Wed, 09 Oct 2019 07:39:42 +0000
draft: false
url: /2019/10/09/support-for-working-with-layer-properties-using-aspose.psd/
author: Adnan Ahmad
summary: ''
tags: []
categories: ['Aspose.PSD Product Family']
---

[![Aspose.PSD for .NET logo][1]](https://blog.aspose.com/wp-content/uploads/sites/2/2018/07/Aspose_PSD-for-net-128x128.png)Here comes new release of Aspose.PSD for .NET 19.9, which has been enriched with new features. This is a relatively new product and we tend to include new features regularly in almost every release. Like in this release, we have introduced support for working with Layer Properties for different layers in a PSD file. In following section, I will be giving you an overview of new features introduced in API.

## Create Layer Group

In [PSD][2] files, you need to work with different layers. We have introduced the feature of creating layers group by adding layers in it and It helps to organize similar or related layers. For this purpose, a new method AddLayerGroup has been added in a** PsdImage** class to add the layer group**.**

The following code snippet shows how you can create layer Group in a PSD file.

{{< gist aspose-com-gists 8a4c9d34ce856d1642fc7c0ce974175c "Examples-CSharp-Aspose-ModifyingAndConvertingImages-PSD-CreateLayerGroups-CreateLayerGroups.cs" >}}

## Rename Layer {#title-heading}

This time we have enhanced the capability of Aspose.PSD to allow renaming of layers in PSD files. This is a good utility as you can set a custom layer name as per your own understanding and future reference. For this purpose, a new property [DisplayName][3]has been added in Layer class to display a layer name properly. It has been observed that when Photoshop saves a layer name using the **Name** property, then Korean characters are stored as byte 63'?' in ASCII. So, if you want to display a layer name properly then use the **DisplayName** property because the **Name** property does not support Korean characters.

The following code snippet shows you how to rename layer in a PSD file.

{{< gist aspose-com-gists 8a4c9d34ce856d1642fc7c0ce974175c "Examples-CSharp-Aspose-ModifyingAndConvertingImages-PSD-RenameLayer-RenameLayer.cs" >}}

## Support for Getting Text Properties from Text Layer

Working with text layer is one of day to day requirement when working with PSD files. Now, using Aspose.PSD for .NET, you can get and update the text properties of different portions of text available in PSD text layer. This article demonstrates how you can get Paragraphs, Styles and Textual properties of the text layer and update them.

The following code snippet shows you how get text properties from text layer in a PSD file.

{{< gist aspose-com-gists 8a4c9d34ce856d1642fc7c0ce974175c "Examples-CSharp-Aspose-ModifyingAndConvertingImages-PSD-GetTextPropertiesFromTextLayer-GetTextPropertiesFromTextLayer.cs" >}}

## Support of Scale Property for Gradient Fill Layer

When working with Gradient fill layers, scaling of gradient which ensure the size of the gradient is one of useful proeprties. Using Aspose.PSD for .NET. For this purpose, a new property [Scale][4] has been added in **IGradientFillSettings.** This article demonstrates how to scale FillLayer with gradient fill using Aspose.PSD for .NET.

Following is the code demonstration that shows how to use **Scale** property.  

{{< gist aspose-com-gists 8a4c9d34ce856d1642fc7c0ce974175c "Examples-CSharp-Aspose-ModifyingAndConvertingImages-PSD-SupportOfScaleProperty-SupportOfScaleProperty.cs" >}}

You can check the official product release notes for many other issues and enhancement carried out in product as well. [Here you can get the detail!][5]

When time allows you can check out API [examples at Github][6], talk about this release and other API related issues in our [forum][7].




[1]: https://blog.aspose.com/wp-content/uploads/sites/2/2018/07/Aspose_PSD-for-net-128x128.png "Aspose.PSD for .NET logo"
[2]: https://wiki.fileformat.com/image/psd/
[3]: https://apireference.aspose.com/net/psd/aspose.psd.fileformats.psd.layers/layer/properties/displayname
[4]: https://apireference.aspose.com/net/psd/aspose.psd.fileformats.psd.layers.fillsettings/igradientfillsettings/properties/scale
[5]: https://docs.aspose.com/display/psdnet/Aspose.PSD+for+.NET+19.9+-+Release+Notes
[6]: https://github.com/aspose-psd
[7]: https://forum.aspose.com/c/psd





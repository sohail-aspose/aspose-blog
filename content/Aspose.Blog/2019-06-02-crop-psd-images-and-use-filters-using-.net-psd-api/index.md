---
title: 'Crop PSD Images and Use Filters using .NET PSD API'
date: Sun, 02 Jun 2019 04:50:16 +0000
draft: false
url: /2019/06/02/crop-psd-images-and-use-filters-using-.net-psd-api/
author: Mudassir
summary: ''
tags: []
categories: ['Aspose.PSD Product Family']
---

[![Aspose.PSD for .NET logo][1]](https://blog.aspose.com/wp-content/uploads/sites/2/2018/07/Aspose_PSD-for-net-128x128.png)Hello viewers! In today's blog, I am back with giving you a walk through of the latest [Aspose.PSD for .NET][2] 19.5 release. This is a relatively new product and we tend to include new features to it in every monthly release. In the following section, I will be giving you an overview of new features along with sample examples for how to use them.

## Support of Fill layers: Pattern

In Photoshop Creative Suite 6, one can apply preset patterns as fills. To fill a layer or selection with a preset pattern, one needs to select a layer in edit mode and set either preset or custom panel for selected panel.

Likewise, Aspose.PSD now also support setting for filling PSD layer with Pattern fill. For this, Aspose.PSD.FileFormats.Psd.Layers.FillLayer is used to add Pattern in PSD layer. In the following example, we have demonstrated loading of a PSD file, accessing the Filllayer class and setting the Pattern using the PatternFillSettings properties.

{{< gist aspose-com-gists 8a4c9d34ce856d1642fc7c0ce974175c "Examples-CSharp-Aspose-ModifyingAndConvertingImages-PSD-PatternFillLayer-PatternFillLayer.cs" >}}

## Support for New Resources {#title-heading}

Aspose.PSD for .NET now introduces support for working with resources like PtFlResource and VsmsResource. For this, one needs to use PtFlResource and VsmsResource classes for resources available PSD layers. In the following examples, we have demonstrated the use of PtFlResource and VsmsResource respectively.

{{< gist aspose-com-gists 8a4c9d34ce856d1642fc7c0ce974175c "Examples-CSharp-Aspose-ModifyingAndConvertingImages-PSD-SupportOfPtFlResource-SupportOfPtFlResource.cs" >}} {{< gist aspose-com-gists 8a4c9d34ce856d1642fc7c0ce974175c "Examples-CSharp-Aspose-ModifyingAndConvertingImages-PSD-SupportOfVsmsResource-SupportOfVsmsResource.cs" >}} 

You can check the official product release notes for many other issues and enhancement carried out in product as well. [Here you can get the detail!][3]

When time allows you can check out API [examples at Github][4], talk about this release and other API related issues in our [forum][5].




[1]: https://blog.aspose.com/wp-content/uploads/sites/2/2018/07/Aspose_PSD-for-net-128x128.png "Aspose.PSD for .NET logo"
[2]: https://products.aspose.com/psd/net
[3]: https://docs.aspose.com/psd/net/aspose-psd-for-net-19-5-release-notes/
[4]: https://github.com/aspose-psd
[5]: https://forum.aspose.com/c/psd





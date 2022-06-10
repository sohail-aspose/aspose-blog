---
title: 'Use Adjustment Layer For Invert and Color Balance in PSD Files using C#'
date: Tue, 05 Nov 2019 19:38:45 +0000
draft: false
url: /2019/11/05/adjustment-layer-support-for-invert-and-color-balance-available-in-aspose.psd/
author: Mudassir
summary: ''
tags: []
categories: ['Aspose.PSD Product Family']
---

[![Aspose.PSD for .NET logo][1]](https://blog.aspose.com/wp-content/uploads/sites/2/2018/07/Aspose_PSD-for-net-128x128.png)Hello readers, let me share the the good news of release announcement for [Aspose.PSD for .NET][2] 19.10. We have introduced support for many new exciting features including Bicubic re-sampling for PSD, invert and color balance adjustment layer support and improvements in rendering PSD to PDF. In following section, I will be giving you an overview of new features introduced in API.

## Implement Bicubic Re-sampling

Re-sampling means you ought to change the pixel dimensions of an image. When you down-sample, you are actually eliminating pixels and therefore deleting information and detail from your image. When you up-sample, you are adding pixels and enhancing details. Photoshop adds these pixels by using interpolation. In following example, we have demonstrated how you can perform the Bicubic Re-sampling by using Aspose.PSD for .NET.

{{< gist aspose-com-gists 8a4c9d34ce856d1642fc7c0ce974175c "Examples-CSharp-Aspose-DrawingAndFormattingImages-ImplementBicubicResampler-ImplementBicubicResampler.cs" >}}

## Color Balance Adjustment Layer {#title-heading}

The color balance adjustment layer gives you the ability to make adjustments to the coloring of their images. It presents the three color channels and their complementary colors and you can adjust the balance of these pairs to change the appearance of an image.

This article demonstrates the usage of Aspose.PSD for .NET to perform the **Color Balance adjustment layer** on an image.



## Invert Adjustment Layer

An adjustment layer is a special kind of layer used mostly for color correction. Rather than having content of their own, they adjust the information on the layers below them. The Invert adjustment layer makes a photo negative effect by inverting the colors of an image.

This following example demonstrates how you can perform the **Invert adjustment layer** by using Aspose.PSD for .NET. 

{{< gist aspose-com-gists 8a4c9d34ce856d1642fc7c0ce974175c "Examples-CSharp-Aspose-DrawingAndFormattingImages-InvertAdjustmentLayer-InvertAdjustmentLayer.cs" >}}

## PSD to PDF with Clipping Mask

A clipping mask allows you to apply a mask to multiple layers at once. In the following example, we have demonstrated the use of exporting PSD to PDF with clipping mask.feature.

{{< gist aspose-com-gists 8a4c9d34ce856d1642fc7c0ce974175c "Examples-CSharp-Aspose-ModifyingAndConvertingImages-PSD-PSDToPDFWithClippingMask-PSDToPDFWithClippingMask.cs" >}}

You can check the official product release notes for many other issues and enhancement carried out in product as well. [Here you can get the detail!][3]

When time allows you can check out API [examples at Github][4], talk about this release and other API related issues in our [forum][5].




[1]: https://blog.aspose.com/wp-content/uploads/sites/2/2018/07/Aspose_PSD-for-net-128x128.png "Aspose.PSD for .NET logo"
[2]: https://products.aspose.com/psd/net
[3]: https://docs.aspose.com/display/psdnet/Aspose.PSD+for+.NET+19.10+-+Release+Notes
[4]: https://github.com/aspose-psd
[5]: https://forum.aspose.com/c/psd





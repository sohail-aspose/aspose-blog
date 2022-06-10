---
title: 'Load Images with Memory Optimization using Aspose.Imaging'
date: Wed, 09 Oct 2019 10:31:42 +0000
draft: false
url: /2019/10/09/controlled-memory-optimization-support-for-loading-images-in-aspose-imaging/
author: Mudassir
summary: ''
tags: []
categories: ['Aspose.Imaging Product Family']
---



{{< figure align=center src="images/aspose-Imaging-for-net_100.png" alt="">}}


Hello readers, in this blog I would like to introduce you with new features included in [Aspose.Imaging][1] 19.10 especially support for controlled memory optimization techniques for loading images using API. The best thing about the Aspose team is that it releases both .NET and Java-based APIs simultaneously every month. This way both API user remains recurrent with changes being made in APIs every month.

In the following sections, I am going to give you a glance at the features that have been included in API.

## Load Images with Memory Optimization

At times there is a requirement to load huge images and you don't have enough RAM available on the machine. In such cases, **OutOfMemory** exception is thrown on loading images. We have introduced the support for controlled memory specification in this new API. Now, you can have memory controlled limitation for loading image by specifying buffer size and it will guarantee that memory usage will be in those bounds. So, if you set memory optimization and your machine RAM memory is not enough, the image related operation will begin to work using hard drive. It will guarantee that operation will be performed in such a way without out of memory exception but it will take much time than using RAM. The controlled memory optimization techniques support has been provided for images like JPEG, CMX, and PNG.

The following examples demonstrate the use of memory optimization while loading the CMX images using API.

### Memory Optimization in C#{{< gist aspose-com-gists 2d1bcb9853315458808ffbcd9e7e3e02 "MemoryStrategyOptimizationCMX.cs" >}}

Likewise, the following examples demonstrate the use of memory optimization while loading JPEG images using API.

{{< gist aspose-com-gists 2d1bcb9853315458808ffbcd9e7e3e02 "MemoryStrategyOptimizationJPEG.cs" >}}

### Memory Optimization in Java

The similar Java-based implementation of loading CMX images is the following:



The similar Java-based implementation of memory optimization for JPEG images is the following:

{{< gist ESidenko 7e927e66d3f218bae75da311c4a4ee0e "MemoryStrategyOptimizationJPEG.java" >}}

## Performance Improvements in API

As against previous API versions, we have tended to improve the API performance in many areas when performing different operations including:

*   Rendering to PDF has been improved
*   Issues related to SVG rendering have been addressed

Wait, there are many other features, enhancement, and bug fixes included in this release. [Here you can get the detail!][2]

When time allows you can check out API [examples at Github][3], talk about this release and other API related issues in our [forum][4].




[1]: https://products.aspose.com/imaging
[2]: https://docs.aspose.com/display/imagingnet/Aspose.Imaging+for+.NET+19.10+-+Release+Notes
[3]: https://github.com/aspose-imaging/
[4]: https://forum.aspose.com/c/imaging





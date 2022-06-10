---
title: 'Resize SVG Images using C# and Java'
date: Thu, 05 Dec 2019 18:41:42 +0000
draft: false
url: /2019/12/05/support-for-svg-resize-and-monitoring-document-conversion-using-aspose.imaging/
author: Adnan Ahmad
summary: ''
tags: []
categories: ['Aspose.Total Product Family']
---



{{< figure align=center src="images/aspose-Imaging-for-net_100.png" alt="">}}


Hi guys! I am pleased to share release announcement for [Aspose.Imaging 19.11][1], which has been enhanced with new features including support for [resizing SVG Images][2] and monitoring document conversion progress. One of the best things about Aspose team is that it publishes both .NET and Java APIs simultaneously every month. This way users of both APIs can use the newly added features simultaneously.

In the following sections, I am going to give you a walk through of new features and enhancements made in API.

## Resize SVG using C# and Java

SVG is a Scalable Vector Graphics file format and utilizes XML based content to depict the graphics. The SVG file format can be scaled to various sizes without affecting the quality as the content is utilized to render the graphics in the image. In other words, SVG format is independent of resolution. For this purpose a new method [resize][3] has been added in Aspose.Imaging that can be used to get the desired dimension size for SVG files.

The following example demonstrate use of this feature:

{{< gist aspose-com-gists 2d1bcb9853315458808ffbcd9e7e3e02 "SvgNativeResize.cs" >}}

The similar Java based implementation is as under:

{{< gist ESidenko 2bff5c26321d6d3fb35dffce2c4033d3 "SvgNativeResize.java" >}}

## Support for Document Conversion Progress

Some times, you work with large image files and when rendering such files to other format there is a long wait depending on size of file to complete rendering process. In such circumstances, it is very convenient to determine the progress of the conversion as it can be useful when if you intend to show some status to the end user regarding conversion process. For this purpose a new property [ProgressCallback][4] has been added in Aspose.Imaging.

The following examples demonstrate use of this feature:

{{< gist aspose-com-gists 2d1bcb9853315458808ffbcd9e7e3e02 "ProgressCallback.cs" >}}

The similar Java based implementation is as under:

{{< gist ESidenko 749eb4262bef8ba92cc5ac65087624f4 "ProgressCallback.java" >}}

Hold on, there are many other features, enhancements, and bug fixes included in this release. You can refer to our [Release Notes section][5] to get more details.

When time allows you can also check out ready made [examples at Github][6]. You may also talk about this release and other API related issues in our [product support forum][7].




[1]: https://products.aspose.com/imaging/net
[2]: https://apireference.aspose.com/net/imaging/aspose.imaging.fileformats.svg/svgimage/methods/resize/index
[3]: https://apireference.aspose.com/net/imaging/aspose.imaging/image/methods/resize
[4]: https://apireference.aspose.com/
[5]: https://docs.aspose.com/display/imagingnet/Aspose.Imaging+for+.NET+19.11+-+Release+Notes
[6]: https://github.com/aspose-imaging/
[7]: https://forum.aspose.com/c/imaging





---
title: 'Create and Export WebP Images Programmatically using Java'
date: Mon, 11 Apr 2016 07:21:41 +0000
draft: false
url: /2016/04/11/create-and-export-webp-images-using-java-imaging-api/
author: Ikram Haq
summary: ''
tags: []
categories: ['Aspose.Imaging Product Family']
---



{{< figure align=center src="images/aspose_imaging-for-java.jpg" alt="">}}


We are pleased to announce the release of Aspose.Imaging for Java 3.3.0. This release allows you to [Create WebP image][1], [export WebP image to other image formats][2], and [convert frame of a GIF image to WebP image][3]. Support to [update text layer in the PSD file][4] and [read/write XMP data to image][5] has also been incorporated in this release.

## Create a WebP Image using Java

Using Aspose.Imaging for Java API, you can [create WebP image][6].  
The ollowing is the code demonstrating the use of WebPOptions class to create a WebP image using Java.

{{< gist aspose-com-gists 07be292db0a393dc95f153f84b28c069 "CreatingWebPImage.java" >}}

## Export WebP to Other Image Formats using Java

Using Aspose.Imaging for Java API, you can [convert WebP image to other image formats][7]. Here is the code to convert WebP image to BMP format using Java.

{{< gist aspose-com-gists 07be292db0a393dc95f153f84b28c069 "ExportWebPToOtherImageFormats.java" >}}

## Convert GIFF Image Frame to WebP Image using Java

Using Aspose.Imaging for Java API, you can [extract a frame from any existing GIFF image and convert it to WebP format][8]. Following is the code demonstration of GifImage. Blocks property to extract a GIFF frame and WebPFrameBlock class to add WebP frame to the WebP image blocklist to create a WebP image.

{{< gist aspose-com-gists 07be292db0a393dc95f153f84b28c069 "ConvertGIFFImageFrame.java" >}}

## Update Text Layer in PSD File

Aspose.Imaging provides functionality to [update text layer in the PSD file][9]. TextLayer.UpdateText method of the TextLayer class can be used to update text in the text layer of a PSD file. TextLayer class can be found under package com.apose.imaging.fileformats.psd.Layers. Method TextLayer.UpdateText takes a string that is to be added, top left coordinates as starting point (com.aspose.imaging.Point), font size and color (com.aspose.imaging.Color) as parameters. Following is the code demonstration of the said functionality.

{{< gist aspose-imaging 8c9bd83e0d07145ba0c1 "Examples-src-main-java-com-aspose-imaging-examples-Photoshop-UpdateTextInTextLayerInsidePSDFile-UpdateTextInTextLayerInsidePSDFile.java" >}}

## Enhancements

The following enhancements have been introduced in this release.

*   Process of JPEG2000 image conversion JP2 has been improved.
*   Process of TIFF image conversion to other image format has been improved.
*   Functionality of EXIF data in TIFF image has been improved.
*   DWG file to PDF conversion process has been improved.
*   Process of converting raster images has been improved.
*   JPEG image encoding algorithm has been upgraded.
*   Functionality of getHorizontalResolution & getVerticalResolution properties has been improved.
*   Resizing GIF image functionality has been improved.

Please refer to the release notes of [Aspose.Imaging for Java 3.3.0][10] for a full view of improvements along with sample code snippets for newly added features. If you are planning to upgrade the API to the latest revision, we strongly suggest you to check the [Public API Changes][11] section to know what has been changed in the public API since your current version.

## Aspose.Imaging for Java Resources

The resources, you may need to accomplish your tasks:

*   [Home page for Aspose.Imaging for Java API][12].
*   [Download Aspose.Imaging for Java][13].
*   [Aspose.Imaging for Java online documentation][14] – help documentation and API reference documents.
*   [Aspose.Imaging Product Family Forum][15] – post your technical questions and queries, or any other problem you are facing while working with Aspose.Imaging APIs.
*   [Enable blog Subscription][16] – Do not limit yourself, you can keep yourself updated with the latest news on Aspose.Imaging APIs, new features, fixes, and other API related topics by subscribing to Aspose.Imaging blog.
*   [Aspose.Imaging for Java in Online Repository][17] – We have published the JAR files on the Maven repository. Anyone could explore the code examples for learning purposes.

As always we appreciate your feedback so if you ever have anything to tell us about this release or anything else, please head to the [Aspose.Imaging forum][18] for a chat.




[1]: https://docs.aspose.com/display/imagingjava/Manipulating+WebP+Images#ManipulatingWebPImages-CreateWebPImage
[2]: https://docs.aspose.com/display/imagingjava/Manipulating+WebP+Images#ManipulatingWebPImages-ExportingWebPtoOtherImageFormats
[3]: https://docs.aspose.com/display/imagingjava/Manipulating+WebP+Images#ManipulatingWebPImages-ConvertGIFFImageFrametoWebPImage
[4]: https://docs.aspose.com/display/imagingjava/Update+Text+In+Text+Layer+Inside+PSD+File
[5]: https://docs.aspose.com/display/imagingjava/Converting+Images#ConvertingImages-ReadandWriteXMPDataToImages
[6]: https://docs.aspose.com/display/imagingjava/Manipulating+WebP+Images#ManipulatingWebPImages-CreateWebPImage
[7]: https://docs.aspose.com/display/imagingjava/Manipulating+WebP+Images#ManipulatingWebPImages-ExportingWebPtoOtherImageFormats
[8]: https://docs.aspose.com/display/imagingjava/Manipulating+WebP+Images#ManipulatingWebPImages-ConvertGIFFImageFrametoWebPImage
[9]: https://docs.aspose.com/display/imagingjava/Update+Text+In+Text+Layer+Inside+PSD+File
[10]: https://downloads.aspose.com/imaging/java
[11]: http://docs.aspose.com/display/imagingjava/Migrating+from+Earlier+Versions+of+Aspose.Imaging
[12]: https://products.aspose.com/imaging/java
[13]: https://downloads.aspose.com/imaging/java
[14]: http://docs.aspose.com/display/imagingjava/Home
[15]: http://forum.aspose.com
[16]: https://blog.aspose.com/
[17]: http://maven.aspose.com/repository/simple/ext-release-local/com/aspose/aspose-imaging/
[18]: http://forum.aspose.com





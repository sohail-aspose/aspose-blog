---
title: 'Convert Raster Images to Metafiles using Java with Aspose.Imaging for Java'
date: Tue, 07 Jul 2015 12:12:58 +0000
draft: false
url: /2015/07/07/convert-raster-images-to-metafiles-emf-wmf-using-java-imaging-library/
author: Babar Raza
summary: ''
tags: ['Babar Raza', 'Convert Raster Images to Metafiles using Java']
categories: ['Aspose.Imaging Product Family']
---



{{< figure align=center src="images/aspose_imaging-for-java.jpg" alt="">}}


We are pleased to announce July's release of Aspose.Imaging for Java. This month's release contains many useful improvements that will certainly ease the task of processing Metafiles with Aspose.Imaging for Java. Please refer to the release notes of [Aspose.Imaging for Java 2.9.1][1] for a full list of bug fixes and improvements along with sample code snippets for newly added features. If you are planning to upgrade the API to the latest revision, we strongly suggest you to check the [Public API Change][2] section to know what has been changed in the public API since your current version.

While you are downloading the latest build, here is a look at just a few of the showcased features of this release.

## Storing Image in BufferedImage using Java

While working with images in Java applications, we may encounter scenarios where we need to [save the images generated with Aspose.Imaging for Java in an instance of BufferedImage][3]. This simple conversion is now available with the help of ImageExtensions.toJava factory method.

Aspose.Imaging for Java 2.9.1 has exposed two versions of the ImageExtensions.toJava method to suit most of the application requirements. The first revision of the aforesaid method can accept an instance of com.aspose.imaging.Image and returns an object of java.awt.image.BufferedImage. Whereas the other revision of the ImageExtensions.toJava method can also accept an instance of com.aspose.imaging.Rectangle as the second parameter to return a part of image as an object of java.awt.image.BufferedImage.

## Cropping Metafiles using Java

This release has exposed two versions of the MetafileImage.crop method to perform the [cropping on Metafiles][4] such as EMF. Both revisions of the MetafileImage.crop method accept different types of parameters and perform a different type of cropping as elaborated below:

*   Cropping by Shifts: The first overload of crop method can accept 4 integer values denoting Left, Right, Top & Bottom. Based on these four values, the crop method moves the image boundaries toward the center of the image while discarding the outer portion.
*   Cropping by Rectangle: The other overloaded version of the crop method can accept an instance of the com.aspose.imaging.Rectangle class to cut out any portion of an image by providing the desired boundaries to the Rectangle object.

For now, the resultant cropped image can only be stored in raster image formats such as BMP, PNG, TIFF, GIF & JPEG. In case the result has to be stored back in Metafile format then the changes will not take effect. We have already planned to enhance this feature for Metafile formats as well, and hope to publish the enhancements with the next release of the Aspose.Imaging for Java API.

## Watermarking Metafiles in Java

Aspose.Imaging for Java has exposed the getWatermarkDrawer method for all classes that represent Metafiles such as EmfMetafileImage, MetafileImage, and WmfMetafileImage. The getWatermarkDrawer method returns an instance of java.awt.Graphics2D object which in turn allows to [create custom watermarks for Metafiles][5].

The following code example demonstrates the usage of Aspose.Imaging for Java API to watermark EMF images and store the result in raster image format.

{{< gist aspose-imaging 8c9bd83e0d07145ba0c1 "Examples-src-main-java-com-aspose-imaging-examples-metafile-WatermarkMetafiles-WatermarkMetafiles.java" >}}

## Converting a Raster Image to Metafile using Java

This release has exposed the EmfMetafileImage.createEmfRecorderGraphics method that returns an instance of EmfRecorderGraphics2D that in turn can be used to call the drawImage method while specifying the instance of Image to be inserted in EMF image.

The following code demonstrates the usage of EmfMetafileImage.createEmfRecorderGraphics method to [add a raster image to EMF file][6].

{{< gist aspose-com-gists 07be292db0a393dc95f153f84b28c069 "Examples-src-main-java-com-aspose-imaging-examples-images-DrawRasterImageOnEMF-DrawRasterImageOnEMF.java" >}}

## Aspose.Imaging for Java Resources

The resources, you may need to accomplish your tasks:

*   [Home page for Aspose.Imaging for Java API][7].
*   [Download Aspose.Imaging for Java][8].
*   Aspose.Imaging for Java online documentation – help documentation and API reference documents.
*   [Aspose.Imaging Product Family Forum][9] – post your technical questions and queries, or any other problem you are facing while working with Aspose.Imaging APIs.
*   [Enable blog Subscription][10] – Do not limit yourself, you can keep yourself updated with the latest news on Aspose.Imaging APIs, new features, fixes, and other API related topics by subscribing to Aspose.Imaging blog.
*   [Aspose.Imaging for Java Examples][11] – We have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: https://downloads.aspose.com/imaging/java
[2]: https://docs.aspose.com/display/imagingjava/Migrating+from+Earlier+Versions+of+Aspose.Imaging
[3]: https://docs.aspose.com/display/imagingjava/Saving+Image+to+BufferedImage
[4]: https://docs.aspose.com/display/imagingjava/Manipulating+Metafiles#ManipulatingMetafiles-CroppingEMFImage
[5]: https://docs.aspose.com/display/imagingjava/Manipulating+Metafiles#ManipulatingMetafiles-WatermarkingMetafiles
[6]: https://docs.aspose.com/display/imagingjava/Drawing+Raster+Images+on+Vector+Images#DrawingRasterImagesonVectorImages-DrawRasterImageonEMF
[7]: https://products.aspose.com/imaging/java
[8]: https://downloads.aspose.com/imaging/java
[9]: http://forum.aspose.com
[10]: https://blog.aspose.com/aspose-products/aspose.imaging-product-family
[11]: https://github.com/asposeimaging/Aspose_Imaging_Java





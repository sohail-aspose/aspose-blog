---
title: 'Aspose.Metafiles has been Completely Merged into Aspose.Imaging for Java with 2.1.0'
date: Thu, 20 Mar 2014 13:34:47 +0000
draft: false
url: /2014/03/20/aspose.metafiles-has-been-completely-merged-into-aspose.imaging-for-java-with-2.1.0/
author: Babar Raza
summary: ''
tags: ['Aspose.Imaging for Java', 'Aspose.Metafiles for Java. Aspose.Metafiles', 'Babar Raza', 'EMF', 'EMF to BMP', 'EMF to JPEG', 'EMF to PNG', 'Merged API', 'Porting Guide', 'WMF', 'WMF to PNG', 'conversion', 'metafiles']
categories: ['Aspose.Imaging Product Family']
---



{{< figure align=center src="images/aspose_imaging-for-java.jpg" alt="">}}


We are pleased to announce the release of [Aspose.Imaging for Java 2.1.0][1] with all enhancements, features and bug fixes from [Aspose.Imaging for .NET 2.1.0][2]. More to that, Aspose.Metafiles for Java has been completely merged into the Aspose.Imaging for Java API with this release. An important point to note here is that [Aspose will no longer sell licenses for Aspose.Metafiles][3], instead we are offering a richer library that meets all imaging requirements in the shape of Aspose.Imaging for Java.

Existing users of Aspose.Metafiles can go through the [Porting Guide][4] to find out what has changed, and what they should do to integrate Aspose.Imaging for Java into their existing applications. We've tried our best to keep everything intact as it was originally in Aspose.Metafiles but have standardized the loading and saving mechanisms according to Aspose.Imaging's object model.

When migrating from Aspose.Metafiles to Aspose.Imaging the following facts should be taken into account:

*   The **MetafileImage** class no longer contains the **write** method, instead of a standard Aspose.Imaging approach using the **save** method should be used as it provides the same functionality.
*   The **MetafileImage** class no longer contains the static **loadMetafile** method, instead, a standard factory method, **load**, should be used as it provides the same functionality.
*   The **EmfMetafile** and **WmfMetafile** classes have been renamed **EmfMetafileImage** and **WmfMetafileImage** respectively.

Merging Aspose.Metafiles into Aspose.Imaging for Java has enabled us to provide the much asked for feature that [converts metafiles to raster images][5]. Now application developers can use Aspose.Imaging for Java to convert EMF and WMF files to other supported image formats such as PNG, JPEG, BMP, and many more.

As always we appreciate your feedback so if you ever have anything to tell us about this release or anything else, please head to the [Aspose.Imaging forum][6] for a chat.




[1]: https://downloads.aspose.com/imaging/java
[2]: https://products.aspose.com/imaging/java
[3]: https://purchase.aspose.com/policies/discontinued-products
[4]: https://docs.aspose.com/display/imagingjava/How+to+Migrate+from+Aspose.Metafiles+to+Aspose.Imaging
[5]: https://docs.aspose.com/display/imagingjava/Manipulating+Metafiles#ManipulatingMetafiles-ConvertingMetafilestoOtherImageFormats
[6]: https://forum.aspose.com/c/imaging





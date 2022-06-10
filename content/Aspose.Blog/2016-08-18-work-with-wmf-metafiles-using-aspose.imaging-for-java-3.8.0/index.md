---
title: 'Work with WMF metafiles using Aspose.Imaging for Java 3.8.0'
date: Thu, 18 Aug 2016 06:41:51 +0000
draft: false
url: /2016/08/18/work-with-wmf-metafiles-using-aspose.imaging-for-java-3.8.0/
author: Ikram Haq
summary: ''
tags: []
categories: ['Aspose.Imaging Product Family']
---

[![Aspose.Imaging for Java logo][1]](http://www.aspose.com/java/imaging-component.aspx "Aspose.Imaging for Java API") We are pleased to announce the release of Aspose.Imaging for Java 3.8.0. The major development in this release is support for WMF metafile. This release allows you to get last modified date of a raster image.

## Support for WMF metafiles

Aspose.Imaging for Java now supports the WMF metafile image format. WMF stands for Windows Media Format (Microsoft). Following is the list of operations that can be performed on a WMF image using Aspose.Imaging:

*   Converting WMF To PDF
    
*   Converting WMF To Raster Format
    
*   Converting WMF To Webp
    
*   Cropping WMF File While Converting To Raster Format
    
*   Resize WMF File While Converting To Raster Format
    

## Get last modified date of an image

Using Aspose.Imaging for Java, developers can get last modified date of a raster format. Below provided sample code demonstrate how to get the last modified date of an image.

```
 //Declare variable to store file path for input image
String path = "path_to_image\\cat_eye.jpg";

com.aspose.imaging.RasterImage image = (com.aspose.imaging.RasterImage)Image.load(path);
try
{
        // gets the date from [FileInfo]
        String modifyDate = image.getModifyDate(true).toString();
        System.out.format("Last modify date using FileInfo: %s\n", modifyDate);

        // gets the date from XMP metadata of [FileInfo] as long as it's not default case
        modifyDate = image.getModifyDate(false).toString();
        System.out.format("Last modify date using info from FileInfo and XMP metadata: %s\n", modifyDate);
}
finally
{
        image.dispose();
} 
```

## Enhancements

Following enhancements have been introduced in this release.

*   SVG to Raster Image conversion process has been improved.
    
*   Diacom to Raster Image conversion process has been improved.
    
*   Process of loading TIFF image has been improved.
    
*   Process of loading PNG image has been improved.
    
*   process of loading JPG image has been improved.
    
*   Exporting process of image in multi threaded environment has been improved.
    

Please refer to the release notes of Aspose.Imaging for Java 3.8.0 for a full view of improvements along with sample code snippets for newly added features. If you are planning to upgrade the API to the latest revision, we strongly suggest you to check the Public API Changes section to know what has been changed in the public API since your current version.

## Aspose.Imaging for Java Resources

The resources, you may need to accomplish your tasks:

*   [Home page for Aspose.Imaging for Java API][2].
*   [Download Aspose.Imaging for Java][3].
*   [Aspose.Imaging for Java online documentation][4] – help documentation and API reference documents.
*   [Aspose.Imaging Product Family Forum][5] – post your technical questions and queries, or any other problem you are facing while working with Aspose.Imaging APIs.
*   [Enable blog Subscription][6] – Do not limit yourself, you can keep yourself updated with the latest news on Aspose.Imaging APIs, new features, fixes and other API related topics by subscribing to Aspose.Imaging blog.
*   [Aspose.Imaging for Java in Online Repository][7] – We have published the JAR files on the Maven repository. Anyone could explore the code examples for learning purposes.

As always we appreciate your feedback so if you ever have anything to tell us about this release or anything else, please head to the [Aspose.Imaging forum][8] for a chat.




[1]: https://docs.aspose.com/display/emailproductfamily/Home "Aspose.Imaging for Java logo"
[2]: https://www.aspose.com/products/imaging/java
[3]: https://downloads.aspose.com/imaging/java
[4]: https://docs.aspose.com/display/imagingjava/Home
[5]: https://www.aspose.com/community/forums/aspose.imaging-product-family/498/showforum.aspx
[6]: https://blog.aspose.com/category/aspose-products/aspose.imaging-product-family/
[7]: http://maven.aspose.com/repository/simple/ext-release-local/com/aspose/aspose-imaging/
[8]: https://www.aspose.com/community/forums/aspose.imaging-product-family/498/showforum.aspx





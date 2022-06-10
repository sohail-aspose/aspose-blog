---
title: 'Work with WMF metafiles and get last modified date of raster image with Aspose.Imaging for .NET 3.8.0'
date: Tue, 19 Jul 2016 05:54:26 +0000
draft: false
url: /2016/07/19/work-with-wmf-metafiles-and-get-last-modified-date-of-raster-image-with-aspose.imaging-for-.net-3.8.0/
author: Ikram Haq
summary: ''
tags: []
categories: ['Aspose.Imaging Product Family']
---

![](https://blog.aspose.com/wp-content/uploads/sites/2/2013/09/aspose-Imaging-for-net_100.png "aspose-Imaging-for-net_100") We are pleased to announce the release of Aspose.Imaging for .NET 3.8.0. The major development in this release is support for WMF metafile. This release allows you to get last modified date of a raster image.

## Support for WMF metafiles

Aspose.Imaging for .Net now supports the WMF metafile image format. WMF stands for Windows Media Format (Microsoft). Following is the list of operations that can be performed on a WMF image using Aspose.Imaging:

*   Converting WMF To PDF
    
*   Converting WMF To Raster Format
    
*   Converting WMF To Webp
    
*   Cropping WMF File While Converting To Raster Format
    
*   Resize WMF File While Converting To Raster Format
    

## Get last modified date of an image

Using Aspose.Imaging for .Net, developers can get last modified date of a raster format. Below provided sample code demonstrate how to get the last modified date of an image.

```
 //Declare variable to store file path for input image
string path = @"path_to_image\cat_eye.jpg";

using (Aspose.Imaging.RasterImage image = (Aspose.Imaging.RasterImage)Aspose.Imaging.Image.Load(path))
{
    // Get the date from [FileInfo]
    string modifyDate = image.GetModifyDate(true).ToString();

    Console.WriteLine("Last modify date using [FileInfo]: {0}", modifyDate);

    // Get the date from XMP metadata of [FileInfo] as long as it is not default case
    modifyDate = image.GetModifyDate(false).ToString();
                
    Console.WriteLine("Last modify date using info from [FileInfo] and XMP metadata: {0}", modifyDate);
} 
```

## Enhancements

Following enhancements have been introduced in this release.

*   Process of loading TIFF image has been improved.
    
*   Process of loading PNG image has been improved.
    
*   process of loading JPG image has been improved.
    
*   Exporting process of image in multi threaded environment has been improved.
    

Please refer to the release notes of [Aspose.Imaging for .NET 3.8.0][1] for a full view of improvements along with sample code snippets for newly added features. If you are planning to upgrade the API to the latest revision, we strongly suggest you to check the Public API Change section to know what has been changed in the public API since your current version.

## Aspose.Imaging for .Net Resources

The resources, you may need to accomplish your tasks:

*   [Home page for Aspose.Imaging for .Net API][2].
*   [Download Aspose.Imaging for .NET][3].
*   [Aspose.Imaging for .NET online documentation][4] – help documentation and API reference documents.
*   [Aspose.Imaging Product Family Forum][5] – post your technical questions and queries, or any other problem you are facing while working with Aspose.Imaging APIs.
*   [Enable blog Subscription][6] – Do not limit yourself, you can keep yourself updated with the latest news on Aspose.Imaging APIs, new features, fixes and other API related topics by subscribing to Aspose.Imaging blog.
*   [Aspose.Imaging for .NET Examples][7] – We have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.

As always we appreciate your feedback so if you ever have anything to tell us about this release or anything else, please head to the [Aspose.Imaging forum][8] for a chat.




[1]: http://www.aspose.com/community/files/51/.net-components/aspose.imaging-for-.net/default.aspx
[2]: https://www.aspose.com/products/imaging/net
[3]: https://downloads.aspose.com/imaging/net
[4]: https://docs.aspose.com/display/imagingnet/Home
[5]: https://www.aspose.com/community/forums/aspose.imaging-product-family/498/showforum.aspx
[6]: https://blog.aspose.com/category/aspose-products/aspose.imaging-product-family/
[7]: https://github.com/aspose-imaging/Aspose.Imaging-for-.NET
[8]: https://www.aspose.com/community/forums/aspose.imaging-product-family/498/showforum.aspx





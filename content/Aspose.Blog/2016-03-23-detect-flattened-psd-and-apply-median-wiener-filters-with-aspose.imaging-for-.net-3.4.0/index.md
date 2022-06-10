---
title: 'Detect Flattened PSD And Apply Median &amp; Wiener Filters With Aspose.Imaging for .Net 3.4.0'
date: Wed, 23 Mar 2016 14:48:11 +0000
draft: false
url: /2016/03/23/detect-flattened-psd-and-apply-median-wiener-filters-with-aspose.imaging-for-.net-3.4.0/
author: Ikram Haq
summary: ''
tags: []
categories: ['Aspose.Imaging Product Family']
---

![](https://blog.aspose.com/wp-content/uploads/sites/2/2013/09/aspose-Imaging-for-net_100.png "aspose-Imaging-for-net_100") We are pleased to announce the release of Aspose.Imaging for .NET 3.4.0. This release allows you to detect flattened PSD. Support to apply median & wiener filters have also been incorporated in this release.

## Detect Flattened PSD

Using Aspose.Imaging for .NET API, developers can detect flattened PSD. Following is the code demonstrating the use of IsFlatten property of the PsdImage class.

```
 string flattenPath = "flatten.psd";

// create an instance of PsdImage class and load the PSD file.
using (Aspose.Imaging.FileFormats.Psd.PsdImage image = (Aspose.Imaging.FileFormats.Psd.PsdImage)Image.Load(flattenPath))
{
     // do processing

    // Get the true value if PSD is flatten and false in case the PSD is not flatten.
    Console.WriteLine(image.IsFlatten);
} 
```

## Apply Median and Wiener Filters

Using Aspose.Imaging for .NET API, developers can apply median & wiener filters on an image. Following is the code to apply median & wiener filters.

### Apply Median Filter```
 string inputFilePath = @"median_test_noise.gif";
string outputFilePath = @"median_test_denoise.gif";

// Load the noisy image
using (Aspose.Imaging.Image image = Aspose.Imaging.Image.Load(inputFilePath))
{
        // caste the image into RasterImage
        Aspose.Imaging.RasterImage rasterImage = image as Aspose.Imaging.RasterImage;

        if (rasterImage == null)
        {
            return;
        }

       // Create an instance of MedianFilterOptions class and set the size.
       Aspose.Imaging.ImageFilters.FilterOptions.MedianFilterOptions options = new Aspose.Imaging.ImageFilters.FilterOptions.MedianFilterOptions(4);

       // apply MedianFilterOptions filter to RasterImage object.
       rasterImage.Filter(image.Bounds, options);

       // Save the resultant image
       image.Save(outputFilePath);
} 
```

### Apply Gauss Wiener Filter```
 string inputFilePath = @"gauss_test_image.gif";
string outputFilePath = @"gauss_test_result.gif";

// Load the image
using (Aspose.Imaging.Image image = Aspose.Imaging.Image.Load(inputFilePath))
{
     // caste the image into RasterImage
     Aspose.Imaging.RasterImage rasterImage = image as Aspose.Imaging.RasterImage;
     if (rasterImage == null)
     {
         return;
     }

     // Create an instance of GaussWienerFilterOptions class and set the radius size and smooth value.
     Aspose.Imaging.ImageFilters.FilterOptions.GaussWienerFilterOptions options = new Aspose.Imaging.ImageFilters.FilterOptions.GaussWienerFilterOptions(12, 3);
     options.Grayscale = true;

     // apply MedianFilterOptions filter to RasterImage object.
     rasterImage.Filter(image.Bounds, options);

     // Save the resultant image
     image.Save(outputFilePath);
} 
```

### Apply Motion Wiener Filter```
 string inputFilePath = @"gauss_test_image.gif";
string outputFilePath = @"gauss_test_result.gif";

// Load the image
using (Aspose.Imaging.Image image = Aspose.Imaging.Image.Load(inputFilePath))
{
     // caste the image into RasterImage
     Aspose.Imaging.RasterImage rasterImage = image as Aspose.Imaging.RasterImage;
     if (rasterImage == null)
     {
         return;
     }

     // Create an instance of MotionWienerFilterOptions class and set the length, smooth value and angle.
     Aspose.Imaging.ImageFilters.FilterOptions.MotionWienerFilterOptions options = new Aspose.Imaging.ImageFilters.FilterOptions.MotionWienerFilterOptions(50, 9, 90);
     options.Grayscale = true;

     // apply MedianFilterOptions filter to RasterImage object.
     rasterImage.Filter(image.Bounds, options);

     // Save the resultant image
     image.Save(outputFilePath);
} 
```

## Enhancements

Following enhancements have been introduced in this release.

*   Process of creating BMP image with RLE8 compression has been improved.
    
*   Functionality of processing JPEG image with CMYK color mode has been improved.
    
*   DWG file to PDF conversion process has been improved.
    
*   JPEG image compression has been upgraded.
    

Please refer to the release notes of [Aspose.Imaging for .NET 3.4.0][1] for a full view of improvements along with sample code snippets for newly added features. If you are planning to upgrade the API to the latest revision, we strongly suggest you to check the Public API Change section to know what has been changed in the public API since your current version.

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





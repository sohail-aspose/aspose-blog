---
title: 'Apply Median and Wiener Filters and Detect Flattened PSD using Java'
date: Sun, 24 Apr 2016 18:49:06 +0000
draft: false
url: /2016/04/24/apply-median-wiener-filters-and-detect-flattened-psd-with-aspose.imaging-for-java-3.4.0/
author: Ikram Haq
summary: ''
tags: []
categories: ['Aspose.Imaging Product Family']
---



{{< figure align=center src="images/aspose_imaging-for-java.jpg" alt="">}}


We are pleased to announce the release of Aspose.Imaging for Java 3.4.0. This release allows you to [apply median & wiener filters][1] on an image. Support to [detect flattened PSD][2] have also been incorporated in this release.

## Apply Median and Wiener Filters

Using Aspose.Imaging for Java API, developers can apply median & wiener filters on an image. Following is the code to apply median & wiener filters.

### Apply Median Filter```
 String inputFilePath = @"median_test_noise.gif";
String outputFilePath = @"median_test_denoise.gif";

// Create an instance of Image class and load noisy image.
com.aspose.imaging.Image image = com.aspose.imaging.Image.load(inputFilePath);

// caste the image into RasterImage
com.aspose.imaging.RasterImage rasterImage = (com.aspose.imaging.RasterImage) image;

if (rasterImage == null)
{
    return;
}

// Create an instance of MedianFilterOptions class and set the size.
com.aspose.imaging.imagefilters.filteroptions.MedianFilterOptions options = new com.aspose.imaging.imagefilters.filteroptions.MedianFilterOptions(4);

// apply MedianFilterOptions filter to RasterImage object.
rasterImage.filter(image.Bounds, options);

// Save the resultant image
image.save(outputFilePath);
```

### Apply Gauss Wiener Filter```
 String inputFilePath = @"gauss_test_image.gif";
String outputFilePath = @"gauss_test_result.gif";

// Load the image
com.aspose.imaging.Image image = com.aspose.imaging.Image.load(inputFilePath);

// caste the image into RasterImage
com.aspose.imaging.RasterImage rasterImage = (com.aspose.imaging.RasterImage) image;

if (rasterImage == null)
{
   return;
}

// Create an instance of GaussWienerFilterOptions class and set the radius size and smooth value.
com.aspose.imaging.imagefilters.filteroptions.GaussWienerFilterOptions options = new com.aspose.imaging.imagefilters.filteroptions.GaussWienerFilterOptions(12, 3);
options.setGrayscale(true);

// apply MedianFilterOptions filter to RasterImage object.
rasterImage.filter(image.Bounds, options);

// Save the resultant image
image.save(outputFilePath);
```

### Apply Motion Wiener Filter```
 String inputFilePath = @"gauss_test_image.gif";
String outputFilePath = @"gauss_test_result.gif";

// Load the image
com.aspose.imaging.Image image = com.aspose.imaging.Image.load(inputFilePath);

// caste the image into RasterImage
com.aspose.imaging.RasterImage rasterImage = (com.aspose.imaging.RasterImage) image;

if (rasterImage == null)
{
    return;
}

// Create an instance of MotionWienerFilterOptions class and set the length, smooth value and angle.
com.aspose.imaging.imagefilters.filteroptions.MotionWienerFilterOptions options = new com.aspose.imaging.imagefilters.filteroptions.MotionWienerFilterOptions(50, 9, 90);
options.setGrayscale(true);

// apply MedianFilterOptions filter to RasterImage object.
rasterImage.filter(image.Bounds, options);

// Save the resultant image
image.save(outputFilePath); 
```

## Detect Flattened PSD

Using Aspose.Imaging for Java API, developers can [detect flattened PSD][3]. Following is the code demonstrating the use of isFlatten property of the PsdImage class.

```
 String flattenPath = "flatten.psd";

// Create an instance of Image class and load PSD file as image.
com.aspose.imaging.Image objImage = com.aspose.imaging.Image.load(flattenPath);

// Cast image object to PSD image
com.aspose.imaging.fileformats.psd.PsdImage psdImage = (com.aspose.imaging.fileformats.psd.PsdImage)objImage;

// do processing

// Get the true value if PSD is flatten and false in case the PSD is not flatten.
System.out.println(psdImage.isFlatten()); 
```

## Enhancements

The following enhancements have been introduced in this release.

*   Process of creating BMP image with RLE8 compression has been improved.
*   DWG file to PDF conversion process has been improved.
*   JPEG image compression has been upgraded.

Please refer to the release notes of [Aspose.Imaging for Java 3.4.0][4] for a full view of improvements along with sample code snippets for newly added features. If you are planning to upgrade the API to the latest revision, we strongly suggest you to check the Public API Changes section to know what has been changed in the public API since your current version.

## Aspose.Imaging for Java Resources

The resources, you may need to accomplish your tasks:

*   [Home page for Aspose.Imaging for Java API][5].
*   [Download Aspose.Imaging for Java][6].
*   [Aspose.Imaging for Java online documentation][7] – help documentation and API reference documents.
*   [Aspose.Imaging Product Family Forum][8] – post your technical questions and queries, or any other problem you are facing while working with Aspose.Imaging APIs.
*   [Enable blog Subscription][9] – Do not limit yourself, you can keep yourself updated with the latest news on Aspose.Imaging APIs, new features, fixes and other API related topics by subscribing to Aspose.Imaging blog.
*   [Aspose.Imaging for Java in Online Repository][10] – We have published the JAR files on the Maven repository. Anyone could explore the code examples for learning purposes.

As always we appreciate your feedback so if you ever have anything to tell us about this release or anything else, please head to the [Aspose.Imaging forum][11] for a chat.




[1]: https://docs.aspose.com/display/imagingjava/Applying+Median+and+Wiener+Filters
[2]: https://docs.aspose.com/display/imagingjava/Manipulating+Photoshop+Formats#ManipulatingPhotoshopFormats-DetectingFlattenedPSD
[3]: https://docs.aspose.com/display/imagingjava/Manipulating+Photoshop+Formats#ManipulatingPhotoshopFormats-DetectingFlattenedPSD
[4]: https://downloads.aspose.com/pdf/java
[5]: https://www.aspose.com/products/imaging/java
[6]: https://downloads.aspose.com/imaging/java
[7]: https://docs.aspose.com/display/imagingjava/Home
[8]: https://www.aspose.com/community/forums/aspose.imaging-product-family/498/showforum.aspx
[9]: https://blog.aspose.com/category/aspose-products/aspose.imaging-product-family/
[10]: http://maven.aspose.com/repository/simple/ext-release-local/com/aspose/aspose-imaging/
[11]: https://www.aspose.com/community/forums/aspose.imaging-product-family/498/showforum.aspx





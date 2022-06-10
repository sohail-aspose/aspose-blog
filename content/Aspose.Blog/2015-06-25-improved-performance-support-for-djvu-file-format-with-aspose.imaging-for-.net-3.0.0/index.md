---
title: 'Improved Performance &amp; Support for DjVu File Format with Aspose.Imaging for .NET 3.0.0'
date: Thu, 25 Jun 2015 13:53:34 +0000
draft: false
url: /2015/06/25/improved-performance-support-for-djvu-file-format-with-aspose.imaging-for-.net-3.0.0/
author: Babar Raza
summary: ''
tags: ['Babar Raza']
categories: ['Aspose.Imaging Product Family']
---

![](https://blog.aspose.com/wp-content/uploads/sites/2/2013/09/aspose-Imaging-for-net_100.png "aspose-Imaging-for-net_100")Aspose.Imaging for .NET 3.0.0 has been released, and we are pleased to announce that this month’s release contains many useful improvements where the most worth mentioning enhancement is the new improved imaging core. Moreover, this release has provided the support for the famous DjVu file format. You can [download][1] the latest build and start exploring the newly added features & enhancements. In case you are planning to upgrade the API from any previous revision then we strongly recommend you to check the Public API Change section to know what has been changed since your current version of the API.

While you are waiting for the latest release to download, here is a look at a few of the worth mentioning features in this month’s release.

## Improved Imaging Core

Aspose.Imaging for .NET API has improved the imaging core for performance considerations by converting the internal structure to utilize the byte array instead of the Aspose.Imaging.Color array. With these changes in place, the latest revision of the Aspose.Imaging for .NET 3.0.0 is less resource consuming and more efficient as compared to any of its predecessors.

Previously, the imaging core used the Aspose.Imaging.Color array to store the pixel information due to which each pixel had to occupy 24 bytes in the memory. This schema proved to be the performance bottleneck in scenarios where images having huge dimensions have to be processed, reason being; the image required more memory to process and hence more time to flush the data. Since the release of Aspose.Imaging for .NET 3.0.0, the API has added new interfaces and methods which are available in public API as well as being used internally for core processing. Now, the Color is represented as 32-bit ARGB integer structure where there are 4 color channels stored in the order of ARGB. For more details, please check the Public API Changes in Aspose.Imaging for .NET 3.0.0.

## Support for DjVu File Format

DjVu file format is becoming popular as an alternative to PDF because it has smaller file size as compared to PDF. DjVu format can also be considered as a superior alternative to PDF for digital documents, to TIFF for scanned bitonal documents, to JPEG and JPEG2000 for photographs and pictures, and to GIF for large palatalized images.

With the release of Aspose.Imaging for .NET 3.0.0, the API has provided the support for loading DjVu files for possible conversion to raster image formats as well as PDF. In order to provide this support, the API has exposed DjvuImage class along with many new helping classes, methods & properties listed in the Public API Changes in Aspose.Imaging for .NET 3.0.0.

## Conversion of DjVu to Multi Frame Raster Formats

Like PDF & TIFF, the DjVu files can have multiple pages/frames therefore while converting the DjVu files to raster formats such as TIFF & GIF, all pages of DjVu are rendered to the resultant image by default. Here is the code to convert all pages of DjVu to TIFF format.

```
 //Load a DjVu image
using (var image = (DjvuImage)Image.Load(sourceFilename))
{
    //Create an instance of TiffOptions & use preset options for Black n While with Deflate compression
    var exportOptions = new TiffOptions(TiffExpectedFormat.TiffDeflateBW);

    //Initialize the DjvuMultiPageOptions
    exportOptions.MultiPageOptions = new DjvuMultiPageOptions();

    //Call Save method while passing instance of TiffOptions
    image.Save(destinationFilename, exportOptions);
} 
```

## Conversion of DjVu to PDF Format

Aspose.Imaging for .NET 3.0.0 can also be used to convert the DjVu files to PDF format while using the existing PdfOptions class. It is up to the user requirement if all DjVu pages or a subset of the pages are to be exported in PDF format.

Following code snippet demonstrates the usage of Aspose.Imaging for .NET 3.0.0 to convert a subset of DjVu pages to PDF format.

```
 //Load a DjVu image
using (DjvuImage image = (DjvuImage)Image.Load(sourceFilename))
{
    //Create an instance of PdfOptions
    PdfOptions exportOptions = new PdfOptions();

    //Initialize the metadata for Pdf document
    exportOptions.PdfDocumentInfo = new Aspose.Imaging.FileFormats.Pdf.PdfDocumentInfo();

    //Create an instance of IntRange and initialize it with the range of DjVu pages to be exported
    IntRange range = new IntRange(0, 5); //Export first 5 pages

    //Initialize an instance of DjvuMultiPageOptions with range of DjVu pages to be exported 
    exportOptions.MultiPageOptions = new DjvuMultiPageOptions(range);

    //Save the result in PDF format
    image.Save(destinationFilename, exportOptions);
} 
```

## Conversion of Specific DjVu Pages to Multi Frame Raster Formats

Aspose.Imaging for .NET 3.0.0 has exposed a new class IntRange that can be used to specify a range that in turn can be passed to an instance of DjvuMultiPageOptions for the conversion of specific range of DjVu pages to TIFF or GIF.

Following piece of code uses the IntRange & DjvuMultiPageOptions classes to render a subset of DjVu pages to TIFF.

```
 //Load a DjVu image
using (DjvuImage image = (DjvuImage)Image.Load(sourceFilename))
{
    //Create an instance of TiffOptions with preset options
    TiffOptions exportOptions = new TiffOptions(TiffExpectedFormat.TiffDeflateBW);

    //Create an instance of IntRange and initialize it with range of pages to be exported
    IntRange range = new IntRange(0, 2); //Export first 2 pages

    //Initialize an instance of DjvuMultiPageOptions while passing instance of IntRange
    exportOptions.MultiPageOptions = new DjvuMultiPageOptions(range);

    //Call Save method while passing instance of TiffOptions
    image.Save(destinationFilename, exportOptions);
} 
```

## Conversion of DjVu Pages to Separate Images

It is also possible to store each DjVu page to separate raster image. In order to achieve this goal, the latest version of Aspose.Imaging for .NET 3.0.0 has exposed an overload constructor of DjvuMultiPageOptions that could accept an integer value to export the specific page. This mechanism can be extended to render individual DjVu pages to raster formats.

Following piece of code uses the DjvuMultiPageOptions class to export 2 DjVu pages to separate BMP images.

```
 //Load a DjVu image
using (DjvuImage image = (DjvuImage) Image.Load(sourceFilename))
{
    //Create an instance of BmpOptions
    BmpOptions exportOptions = new BmpOptions();

    //Set BitsPerPixel for resultant images
    exportOptions.BitsPerPixel = 32;

    //Create an instance of IntRange and initialize it with range of pages to be exported
    IntRange range = new IntRange(0, 2); //Export first 2 pages

    int counter = 0;
    //Loop over the specified range
    foreach (var i in range.Range)
    {
        //Save each page in separate file, as BMP do not support layering
        exportOptions.MultiPageOptions = new DjvuMultiPageOptions(range.GetArrayOneItemFromIndex(counter));
        image.Save(string.Format("{0}.bmp", counter++), exportOptions);
    }
} 
```

## Conversion of Specific Portion of DjVu Page to Image

Another overload constructor of DjvuMultiPageOptions class can accept an integer value as well as an instance of Rectangle to export a specific portion of DjVu page to raster image format.

Following piece of code creates an instance of Rectange to specify the location and size of the desired area to be exported in PNG format.

```
 //Load a DjVu image
using (DjvuImage image = (DjvuImage) Image.Load(sourceFilename))
{
      //Create an instance of PngOptions
      PngOptions exportOptions = new PngOptions();

      //Set ColorType to Grayscale
      exportOptions.ColorType = Aspose.Imaging.FileFormats.Png.PngColorType.Grayscale;

      //Create an instance of Rectange and specify the portion on DjVu page
      Aspose.Imaging.Rectangle exportArea = new Aspose.Imaging.Rectangle(0, 0, 500, 500);

      //Specify the DjVu page index
      int exportPageIndex = 2;

      //Initialize an instance of DjvuMultiPageOptions
      //while passing index of DjVu page index and instance of Rectange covering the area to be exported
      exportOptions.MultiPageOptions = new DjvuMultiPageOptions(exportPageIndex, exportArea);

      //Save the image
      image.Save(destinationFilename, exportOptions);
} 
```

As always we appreciate your feedback so if you ever have anything to tell us about this release or anything else, please head to the [Aspose.Imaging forum][2] for a chat.




[1]: http://www.aspose.com/community/files/51/.net-components/aspose.imaging-for-.net/entry636170.aspx "Download Aspose.Imaging for .NET 3.0.0"
[2]: http://www.aspose.com/community/forums/aspose.imaging-product-family/498/showforum.aspx





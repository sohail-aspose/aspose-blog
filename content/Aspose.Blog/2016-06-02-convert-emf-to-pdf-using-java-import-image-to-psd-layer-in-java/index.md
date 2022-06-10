---
title: 'Convert EMF to PDF and Import Image to PSD Layer using Java'
date: Thu, 02 Jun 2016 18:02:44 +0000
draft: false
url: /2016/06/02/convert-emf-to-pdf-using-java-import-image-to-psd-layer-in-java/
author: Ikram Haq
summary: ''
tags: ['Convert EMF to PDF using Java', 'Import Image to PSD Layer in Java']
categories: ['Aspose.Imaging Product Family']
---



{{< figure align=center src="images/aspose_imaging-for-java.jpg" alt="">}}


We are pleased to announce the release of Aspose.Imaging for Java 3.5.0. The major development in this release is [support for DICOM image][1] and [support for EMF format][2]. This release allows you to [blur an image][3] and [import image to PSD layer][4]. Support to [apply correction filters on images][5] has also been incorporated in this release.

## Convert EMF To PDF using Java

Using Aspose.Imaging for Java, developers can convert EMF metafile to PDF format. Aspose.Imaging provides the EmfImage class to load EMF files and the same can be used to save the image to PDF format. Below provided sample code demonstrates how to convert EMF to PDF.

```
String[] filePaths = new String[] {
                    "input\\FilledRectangleRotateMode_c.emf",
                    "input\\image5.emf",
                    "input\\LinearGradientBrushCircuitMode.emf",
                    "input\\Pict.emf",
                    "input\\Picture1.emf",
                    "input\\test.emf",
                    "input\\wrong-font-size.emf"
                 };

        for (String filePath : filePaths)
        {
              String outPath = filePath + ".pdf";

              com.aspose.imaging.fileformats.emf.EmfImage image = com.aspose.imaging.fileformats.emf.EmfImage.load(filePath);
              try
              {
                   com.aspose.imaging.system.io.FileStream outputStream = 
                           new com.aspose.imaging.system.io.FileStream(outPath, com.aspose.imaging.system.io.FileMode.Create);
                   try
                   {
                         if(!image.getHeader().getEmfHeader().getValid())
                         {
                              throw new com.aspose.imaging.exceptions.ImageLoadException("The file" + outPath +" is not valid");
                         }

                         com.aspose.imaging.imageoptions.EmfRasterizationOptions emfRasterization = 
                                 new com.aspose.imaging.imageoptions.EmfRasterizationOptions();
                         
                         emfRasterization.setPageWidth(image.getWidth());
                         emfRasterization.setPageHeight(image.getHeight());
                         emfRasterization.setBackgroundColor(com.aspose.imaging.Color.getWhiteSmoke());

                         PdfOptions pdfOptions = new PdfOptions();
                         pdfOptions.setVectorRasterizationOptions(emfRasterization);

                         image.save(outputStream.toOutputStream(), pdfOptions);
                    }
                    finally
                    {
                         outputStream.close();
                         outputStream.dispose();
                    }
              }
              finally
              {
                  image.dispose();
              }
        } 
```

## Support for DICOM image

Aspose.Imaging for Java now [supports the DICOM image format(.dicom)][6]. DICOM stands for Digital Imaging and Communications in Medicine. DICOM is a standard for handling, storing, printing, and transmitting information in medical imaging. It includes a file format definition and a network communications protocol.

Following is the list of operations that can be performed on a DICOM image using Aspose.Imaging:

*   [Adjusting Brightness, Contrast and Gamma][7]
*   [Applying Filters][8]
*   [Applying Binarization][9]
*   [Cropping Image][10]
*   [Cropping by Shifts][11]
*   [Dithering For DICOM Image][12]
*   [Resizing DICOM Image][13]
*   [Rotate and Flip DICOM Image][14]
*   [Export to DICOM][15]

## Blur An Image

Using Aspose.Imaging for Java API, developers can [create blur effect on an image][16]. Following is the code demonstrating the use of the GaussianBlurFilterOptions class.

```
//Declare variables to store file paths for input and output images
String sourcePath = "D:\blur_test_before.jpg";
String outPath = "D:\blur_test_after.jpg";

// Load an image 
com.aspose.imaging.Image image = com.aspose.imaging.Image.load(sourcePath);

//Convert the image into RasterImage.
com.aspose.imaging.RasterImage rasterImage = (com.aspose.imaging.RasterImage)image;

//Pass Bounds[rectangle] of image and GaussianBlurFilterOptions instance to Filter method.
rasterImage.filter(rasterImage.getBounds(), new com.aspose.imaging.imagefilters.filteroptions.GaussianBlurFilterOptions(5, 5));

//Save the results to output path.
rasterImage.save(outPath);
```

## Import Image To PSD Layer

Using Aspose.Imaging for Java API, developers can import image [into a PSD file. Aspose.Imaging for Java has exposed the DrawImage method][17] of the Layer class to add/import an image into a PSD file. DrawImage method needs location and image values to add/import an image into a PSD file. The following code example demonstrates how to import an image into PSD file.

```
//Declare variables to store file paths for input and output.
String sourceFileName = "source.psd";
String outputFileName = "result.psd";

// Load a PSD file as an image and caste it into PsdImage
com.aspose.imaging.fileformats.psd.PsdImage image = (com.aspose.imaging.fileformats.psd.PsdImage)com.aspose.imaging.Image.load(sourceFileName);

// Extract a layer from PSDImage
com.aspose.imaging.fileformats.psd.layers.Layer layer = image.getLayers()[1];

// Load the image that is needed to be imported into the PSD file.
String normalImagePath = "png_normal.png";

com.aspose.imaging.RasterImage drawImage = (com.aspose.imaging.RasterImage)com.aspose.imaging.Image.load(normalImagePath);

// Call DrawImage method of the Layer class and pass the image instance.
layer.drawImage(new com.aspose.imaging.Point(10, 10), drawImage);

//Save the results to output path.
image.save(outputFileName, new com.aspose.imaging.imageoptions.PsdOptions());
```

## Apply Correction Filter On An Image

Using Aspose.Imaging for .NET API, developers can [apply correction filters on an image][18]. Aspose.Imaging for .NET has exposed the BilateralSmoothingFilterOptions and SharpenFilterOptions classes for filtration. BilateralSmoothingFilterOptions class needs an integer as size. The following code example demonstrates how to apply correction filter.

```
//Declare variables to store file paths for input and output images
String inputFilePath = "a1.jpg";
String outputFilePath = "a1_out.jpg";

// Load an image 
com.aspose.imaging.Image image = com.aspose.imaging.Image.load(inputFilePath);

//Convert the image into RasterImage.
com.aspose.imaging.RasterImage rasterImage = (com.aspose.imaging.RasterImage)image;
if (rasterImage == null)
{
    return;
}

//Get Bounds[rectangle] of image.
com.aspose.imaging.Rectangle rect = image.getBounds();

// Create an instance of BilateralSmoothingFilterOptions class with size parameter.
com.aspose.imaging.imagefilters.filteroptions.BilateralSmoothingFilterOptions bilateralOptions = 
        new com.aspose.imaging.imagefilters.filteroptions.BilateralSmoothingFilterOptions(3);

// Create an instance of SharpenFilterOptions class.
com.aspose.imaging.imagefilters.filteroptions.SharpenFilterOptions sharpenOptions = 
        new com.aspose.imaging.imagefilters.filteroptions.SharpenFilterOptions();

// Supply the filters to raster image.
rasterImage.filter(rect, bilateralOptions);
rasterImage.filter(rect, sharpenOptions);

// Adjust the contrast accordingly.
rasterImage.adjustContrast(-10);

// Set brightness using Binarize Bradley
rasterImage.binarizeBradley(80);

//Save the results to output path.
rasterImage.save(outputFilePath);
```

## Enhancements

The following enhancements have been introduced in this release.

*   The process of digital signing of assembly has been improved.
*   The processing of the PSD file has been improved.
*   DXF to PDF conversion process has been improved.
*   JPG to JPG2000 format conversion process has been improved.
*   The processing of YCBCR format has been upgraded.
*   The processing of JPEG & TIFF formats have been improved.

Please refer to the release notes of [Aspose.Imaging for Java 3.5.0][19] for a full view of improvements along with sample code snippets for newly added features. If you are planning to upgrade the API to the latest revision, we strongly suggest you to check the [Public API Changes][20] section to know what has been changed in the public API since your current version.

## Aspose.Imaging for Java Resources

The resources, you may need to accomplish your tasks:

*   [Home page for Aspose.Imaging for Java API][21].
*   [Download Aspose.Imaging for Java][22].
*   [Aspose.Imaging for Java online documentation][23] – help documentation and API reference documents.
*   [Aspose.Imaging Product Family Forum][24] – post your technical questions and queries, or any other problem you are facing while working with Aspose.Imaging APIs.
*   [Enable blog Subscription][25] – Do not limit yourself, you can keep yourself updated with the latest news on Aspose.Imaging APIs, new features, fixes and other API related topics by subscribing to Aspose.Imaging blog.
*   [Aspose.Imaging for Java in Online Repository][26] – We have published the JAR files on the Maven repository. Anyone could explore the code examples for learning purposes.

As always we appreciate your feedback so if you ever have anything to tell us about this release or anything else, please head to the [Aspose.Imaging forum][27] for a chat.




[1]: https://docs.aspose.com/display/imagingjava/Manipulating+DICOM+Formats
[2]: https://docs.aspose.com/
[3]: https://docs.aspose.com/display/imagingjava/Modifying+Images#ModifyingImages-BluranImage
[4]: https://docs.aspose.com/display/imagingjava/Manipulating+Photoshop+Formats#ManipulatingPhotoshopFormats-ImportingimagetoPSDlayer
[5]: https://docs.aspose.com/display/imagingjava/Applying+Median+and+Wiener+Filters#ApplyingMedianandWienerFilters-ApplyCorrectionFilterOnAnImage
[6]: https://docs.aspose.com/display/imagingjava/Manipulating+DICOM+Formats
[7]: https://docs.aspose.com/display/imagingjava/Manipulating+DICOM+Formats#ManipulatingDICOMFormats-AdjustingBrightness,ContrastandGamma
[8]: https://docs.aspose.com/display/imagingjava/Manipulating+DICOM+Formats#ManipulatingDICOMFormats-ApplyingFilters
[9]: https://docs.aspose.com/display/imagingjava/Manipulating+DICOM+Formats#ManipulatingDICOMFormats-ApplyingBinarization
[10]: https://docs.aspose.com/display/imagingjava/Manipulating+DICOM+Formats#ManipulatingDICOMFormats-CroppingImage
[11]: https://docs.aspose.com/display/imagingjava/Manipulating+DICOM+Formats#ManipulatingDICOMFormats-CroppingbyShifts
[12]: https://docs.aspose.com/display/imagingjava/Manipulating+DICOM+Formats#ManipulatingDICOMFormats-DitheringForDICOMImage
[13]: https://docs.aspose.com/display/imagingjava/Manipulating+DICOM+Formats#ManipulatingDICOMFormats-ResizingDICOMImage
[14]: https://docs.aspose.com/display/imagingjava/Manipulating+DICOM+Formats#ManipulatingDICOMFormats-RotateandFlipDICOMImage
[15]: https://docs.aspose.com/display/imagingjava/Manipulating+DICOM+Formats#ManipulatingDICOMFormats-ExporttoDICOM
[16]: https://docs.aspose.com/display/imagingjava/Modifying+Images#ModifyingImages-BluranImage
[17]: https://docs.aspose.com/display/imagingjava/Manipulating+Photoshop+Formats#ManipulatingPhotoshopFormats-ImportingimagetoPSDlayer
[18]: https://docs.aspose.com/display/imagingjava/Applying+Median+and+Wiener+Filters#ApplyingMedianandWienerFilters-ApplyCorrectionFilterOnAnImage
[19]: https://downloads.aspose.com/imaging/java
[20]: http://docs.aspose.com/display/imagingjava/Migrating+from+Earlier+Versions+of+Aspose.Imaging
[21]: https://www.aspose.com/products/imaging/java
[22]: https://downloads.aspose.com/imaging/java
[23]: https://docs.aspose.com/display/imagingjava/Home
[24]: http://forum.aspose.com
[25]: https://blog.aspose.com/category/aspose-products/aspose.imaging-product-family/
[26]: http://maven.aspose.com/repository/simple/ext-release-local/com/aspose/aspose-imaging/
[27]: http://forum.aspose.com





---
title: 'Render Multiple CAD Layouts, Specify Transparency for PNG and ICC Profiles for JPEG with Aspose.Imaging for Java 2.7.0'
date: Wed, 22 Apr 2015 17:42:33 +0000
draft: false
url: /2015/04/22/render-multiple-cad-layouts-specify-transparency-for-png-and-icc-profiles-for-jpeg-with-aspose.imaging-for-java-2.7.0/
author: Babar Raza
summary: ''
tags: ['Babar Raza']
categories: ['Aspose.Imaging Product Family']
---

[![Aspose.Imaging for Java logo][1]](http://www.aspose.com/java/imaging-component.aspx "Aspose.Imaging for Java API")Aspose.Imaging for Java 2.7.0 has been released and we are pleased to announce that this release contains many useful improvements & features. Most worth mentioning enhancement is the support for DWG 2005 revision 16.1, 2010 revision 18.0 and 2013 revision 19.0 AutoCAD formats. Please refer to the release notes of [Aspose.Imaging for Java 2.7.0][2] for a full list of bug fixes and improvements along with sample code snippets to the newly added features. If you are planning to upgrade the Aspose.Imaging for Java API to the latest revision, we would strongly suggest you to check the Public API Change section to know what has been changed in the API since your current version.

## Code Baseline Moved to Java 6

Starting with this release, Aspose.Imaging for Java has dropped the support for Java versions prior to v6 and has moved its codebase to Java 6 (Java 7 and 8 are also supported). Reason being, Sun/Oracle has discontinued the support for all JDK revisions prior to 1.6. Now the Aspose.Imaging for Java package contains a single Jar that works well with Java 6, 7 & 8.

## Support for Multiple Layout Rendering

Aspose.Imaging for Java API can load AutoCAD drawings for possible conversion to PDF and raster image formats. With this release, the API has extended it's support for the said conversion by allowing the users to select multiple layouts from a given DWG or DXF drawing, and render them to PDF or raster image formats. The API has exposed the CadRasterizationOptions.Layouts property of type String\[\] so you may specify more than one layouts at a time. While specifying multiple layouts for the CadRasterizationOptions.Layouts property, the resultant PDF and TIFF image would have multiple pages, GIF image would have multiple frames and PSD format would have multiple layers, where each page/frame/layer represents an individual AutoCAD layout. In case any other image format such as PNG, BMP, JPEG is selected to store the result then the API will render only the default layout; that is "Model".

The following code snippet demonstrates the usage of CadRasterizationOptions.Layouts property to export CAD drawings to PDF format.

```
 //Load an existing CAD in an instance of Image
Image image = Image.load(source);

//Create an instance of CadRasterizationOptions and set its various properties
CadRasterizationOptions rasterizationOptions = new CadRasterizationOptions();
rasterizationOptions.setPageWidth(1600);
rasterizationOptions.setPageHeight(1600);
//Specify desired layout names
rasterizationOptions.setLayouts(new String [] {"Model", "Layout1"});

//Create an instance of PdfOptions
PdfOptions pdfOptions = new PdfOptions();

//Set the VectorRasterizationOptions property
pdfOptions.setVectorRasterizationOptions(rasterizationOptions);

//Export the CAD to PDF
image.save(output, pdfOptions); 
```

## Color Space Conversion for JPEG through ICC Profiles

Aspose.Imaging for Java API conceals the ugly details and provide an easy to use mechanism to specify ICC profiles via JpegImage class. Moreover, Aspose.Imaging uses the sample profiles of SWOP CMYK and sRGB embedded into it's core therefore in most common usage cases, you do not need to seek for any specific profiles.

The following code snippet demonstrates the usage of Aspose.Imaging for Java API to specify RGB and CMYK color profiles for YCCK JPEG image saving process.

```
 //Load an existing CAD in an instance of Image
JpegImage image = (JpegImage)Image.load(source);

//Load profiles from disk
StreamSource rgbprofile = new StreamSource(new FileInputStream("rgb.icc"));
StreamSource cmykprofile = new StreamSource(new FileInputStream("cmyk.icc"));

//Set RGB & CMYK profiles
image.setDestinationRGBColorProfile(rgbprofile);
image.setDestinationCMYKColorProfile(cmykprofile);

//Save the result
image.save(); 
```

## Support for PNG & GIF Transparent & Background Colors

Previously, Aspose.Imaging allowed to set the transparency color for PNG format. With this release, the API has extended it's support for the GIF image, and have improved the public API to make the usability even simpler by exposing the relevant properties to the RasterImage class.

Here is the simplest code to set the transparent & background color for the RasterImage object and save the result in PNG format.

```
 //Load the source image (any format) in an instance of RasterImage
RasterImage image = (RasterImage)Image.load(source);

//Set the background color for the image
image.setBackgroundColor(Color.getWhite());

//Set the transparent color for the image
image.setTransparentColor(Color.getBlack());

//Set the HasTransparentColor & HasBackgroundColor properties to true
image.setBackgroundColor(true);
image.setTransparentColor(true);

//Save the image on disc in PNG format
image.save(output, new PngOptions()); 
```

As always we appreciate your feedback so if you ever have anything to tell us about this release or anything else, please head to the [Aspose.Imaging forum][3] for a chat.




[1]: https://docs.aspose.com/display/emailproductfamily/Home "Aspose.Imaging for Java logo"
[2]: http://www.aspose.com/community/files/72/java-components/aspose.imaging-for-java/entry622353.aspx "Download Aspose.Imaging for Java 2.7.0"
[3]: http://www.aspose.com/community/forums/aspose.imaging-product-family/498/showforum.aspx





---
title: 'Set Fonts’ Location, Export PSD Layers to Raster Images and CAD to PDF With Aspose.Imaging for Java 3.2.0'
date: Sat, 30 Jan 2016 20:10:24 +0000
draft: false
url: /2016/01/30/set-fonts%e2%80%99-location-export-psd-layers-to-raster-images-and-cad-to-pdf-with-aspose.imaging-for-java-3.2.0/
author: Ikram Haq
summary: ''
tags: []
categories: ['Aspose.Imaging Product Family']
---

[![Aspose.Imaging for Java logo][1]](http://www.aspose.com/java/imaging-component.aspx "Aspose.Imaging for Java API") We are pleased to announce the release of Aspose.Imaging for Java 3.2.0. This release allows you to use Bradley's threshold algorithm during image conversion and define settings to expand or crop the image. Support to export PSD layers to raster images, CAD file to PDF format and font folder setting while converting DXF files has also been incorporated in this release.

## Set Font Folder While Exporting DXF Files

Using Aspose.Imaging for Java, developers can specify the font folder path used while converting CAD (DXF) files. Following is the code explaining how to use the said functionality.

```
 com.aspose.imaging.FontSettings.addFontsFolder("/home/username/.fonts"); 
```

## Use Bradley's Threshold Algorithm While Converting Images

Aspose.Imaging has introduced the functionality to use Bradley's threshold algorithm during process of image conversion. Here is the code to define the threshold value and use it.

```
 String sourcepath = "sourcefile.png";
String outputPath = "binarized_output.png";

//Load an existing image.
com.aspose.imaging.fileformats.png.PngImage objimage = 
        (com.aspose.imaging.fileformats.png.PngImage)com.aspose.imaging.Image.load(sourcepath);
        
// Define threshold value
double threshold = 0.15;
        
// Call BinarizeBradley method and pass the threshold value as parameter
objimage.binarizeBradley(threshold);

// Save the output image
objimage.save(outputPath); 
```

## Expand and Crop an Image

Using Aspose.Imaging, developers can expand or crop an image during image conversion process. Following is the code snippet demonstrating how Rectangle class can be used to crop or expand raster images.

```
 String fileName = "imageToResize.bmp";
String outputFileName = "imageResized.Jpeg";
        
//Load an existing image.
com.aspose.imaging.RasterImage rasterImage = (com.aspose.imaging.RasterImage)com.aspose.imaging.Image.load(fileName);
        
// setting for image data to be cashed
rasterImage.cacheData();
        
// Create an instance of Rectangle class and define X,Y and Width, height of the rectangle.
com.aspose.imaging.Rectangle destRect = new com.aspose.imaging.Rectangle();
destRect.setX(-200);
destRect.setY(-200);
destRect.setWidth(300);
destRect.setHeight(300);
        
// Save output image by passing output file name, image options and rectangle object.
rasterImage.save(outputFileName, new JpegOptions(), destRect); 
```

## Export PSD Layers to Raster Images

Using Aspose.Imaging, developers can convert PSD layers to PNG, JPEG and TIFF images. Following is the code snippet demonstrating how PSD layers can be converted to PNG image.

```
 String sourceFileName = "source.psd";

// Create an instance of Image class and load PSD file as image.
com.aspose.imaging.Image objImage = com.aspose.imaging.Image.load(sourceFileName);
        
// Cast image object to PSD image
com.aspose.imaging.fileformats.psd.PsdImage psdImage = (com.aspose.imaging.fileformats.psd.PsdImage)objImage;
        
// Create an instance of PngOptions class
com.aspose.imaging.imageoptions.PngOptions pngOptions = new com.aspose.imaging.imageoptions.PngOptions();
pngOptions.setColorType(com.aspose.imaging.fileformats.png.PngColorType.TruecolorWithAlpha);
        
// Loop through the list of layers
for (int i = 0; i < psdImage.getLayers().length; i++)
{
    // convert and save the layer to PNG file format.
    psdImage.getLayers()[i].save("layer_" + i + 1 + ".png", pngOptions);
} 
```

## Export CAD Layouts to PDF

Aspose.Imaging provides functionality to export CAD to PDF file format. save method of the CadImage class can be used to export to PDF format. Initialize the CadRasterizationOptions class, define the type of entities using com.aspose.imaging.ImageOptions.TypeOfEntities class and set the layout(s) that you want to export. Following is the code demonstration of the said functionality.

```
 String sourceFile = "test.dwg";
        
com.aspose.imaging.fileformats.cad.CadImage cadImage = 
        (com.aspose.imaging.fileformats.cad.CadImage) com.aspose.imaging.fileformats.cad.CadImage.load(sourceFile);
        
//Create an instance of CadRasterizationOptions and set its various properties
CadRasterizationOptions rasterizationOptions = new CadRasterizationOptions();

rasterizationOptions.setPageWidth(1600);
rasterizationOptions.setPageHeight(1600);
        
// Set the Entities type property to Entities3D.
rasterizationOptions.setTypeOfEntities(TypeOfEntities.Entities3D);
        
rasterizationOptions.setScaleMethod(com.aspose.imaging.fileformats.cad.ScaleType.GrowToFit);
rasterizationOptions.setContentAsBitmap(true);
        
// Set Layouts
rasterizationOptions.setLayouts(new String[] { "Model" });
        
// Create an instance of PDF options class
PdfOptions pdfOptions = new PdfOptions();
        
//Set the VectorRasterizationOptions property
pdfOptions.setVectorRasterizationOptions(rasterizationOptions);

String outPath = "output.pdf";

// Set Graphics options
rasterizationOptions.getGraphicsOptions().setSmoothingMode(com.aspose.imaging.SmoothingMode.HighQuality);
rasterizationOptions.getGraphicsOptions().setTextRenderingHint(com.aspose.imaging.TextRenderingHint.AntiAliasGridFit);
rasterizationOptions.getGraphicsOptions().setInterpolationMode(com.aspose.imaging.InterpolationMode.HighQualityBicubic);

// Export CAD to PDF by calling the Save method
cadImage.save(outPath, pdfOptions); 
```

## Enhancements

Following are the enhancements incorporated in this release.

*   StreamContainer, FileStreamContainer and TiffStreamFactory classes are now public for developers.
    
*   Functionality of ExifData with NULL properties has been improved.
    
*   Read/Loading process has been improved for TIFF images.
    
*   DWG to PDF functionality has been improved.
    
*   DXF to raster images functionality has been improved.
    
*   Process of handling large size images in memory has been improved. Maintaining image quality while resizing has been improved.
    
*   TIFF to JPEG conversion process have been improved.
    

Please refer to the release notes of [Aspose.Imaging for Java 3.2.0][2] for a full view of improvements along with sample code snippets for newly added features. If you are planning to upgrade the API to the latest revision, we strongly suggest you to check the Public API Changes section to know what has been changed in the public API since your current version.

## Aspose.Imaging for Java Resources

The resources, you may need to accomplish your tasks:

*   [Home page for Aspose.Imaging for Java API][3].
*   [Download Aspose.Imaging for Java][4].
*   [Aspose.Imaging for Java online documentation][5] – help documentation and API reference documents.
*   [Aspose.Imaging Product Family Forum][6] – post your technical questions and queries, or any other problem you are facing while working with Aspose.Imaging APIs.
*   [Enable blog Subscription][7] – Do not limit yourself, you can keep yourself updated with the latest news on Aspose.Imaging APIs, new features, fixes and other API related topics by subscribing to Aspose.Imaging blog.
*   [Aspose.Imaging for Java in Online Repository][8] – We have published the JAR files on the Maven repository. Anyone could explore the code examples for learning purposes.

As always we appreciate your feedback so if you ever have anything to tell us about this release or anything else, please head to the [Aspose.Imaging forum][9] for a chat.




[1]: https://docs.aspose.com/display/emailproductfamily/Home "Aspose.Imaging for Java logo"
[2]: http://www.aspose.com/community/files/72/java-components/aspose.imaging-for-java/default.aspx
[3]: https://www.aspose.com/products/imaging/java
[4]: https://downloads.aspose.com/imaging/java
[5]: https://docs.aspose.com/display/imagingjava/Home
[6]: https://www.aspose.com/community/forums/aspose.imaging-product-family/498/showforum.aspx
[7]: https://blog.aspose.com/category/aspose-products/aspose.imaging-product-family/
[8]: http://maven.aspose.com/repository/simple/ext-release-local/com/aspose/aspose-imaging/
[9]: https://www.aspose.com/community/forums/aspose.imaging-product-family/498/showforum.aspx





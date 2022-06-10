---
title: 'Work with SVG Images and Apply Font Settings for EMF Files in Java'
date: Mon, 25 Jul 2016 06:58:07 +0000
draft: false
url: /2016/07/25/work-with-svg-images-and-applying-font-settings-for-emf-files-with-aspose.imaging-for-java-3.7.0/
author: Ikram Haq
summary: ''
tags: ['Convert SVG to BMP', 'Convert SVG to GIF', 'Convert SVG to JPEG', 'Convert SVG to PNG', 'Convert SVG to TIFF']
categories: ['Aspose.Imaging Product Family']
---



{{< figure align=center src="images/aspose-Imaging-for-Java-e1378110009543.png" alt="Aspose.Imaging for Java logo">}}


We are pleased to announce the release of Aspose.Imaging for Java 3.7.0. The major development in this release is [support for Scalable Vector Graphics image][1]. [Support to apply font setting for metafiles (EMF)][2] has also been incorporated in this release.

## Support for SVG image

Aspose.Imaging for Java now supports the SVG image format (.svg). SVG stands for Scalable Vector Graphics. Aspose.Imaging for Java provides the SvgImage class to load SVG files and the same can be used to convert the SVG to raster formats.

Below provided sample code demonstrates how to [convert a SVG file to PNG format][3].

{{< gist aspose-com-gists 0420a5530f73658aebea7f98ea4d705f "Examples-CSharp-LoadSaveConvert-ConvertSVGToImage-ConvertSVGToPNG.cs" >}}

## Applying Font Settings For Metafiles

Using Aspose.Imaging for Java API, developers can apply font settings for metafiles (EMF). Following is the code demonstrates how to specify font folder settings for EMF image while converting it to PNG image.

```
// Create an instance of EmfRasterizationOptions class
com.aspose.imaging.imageoptions.EmfRasterizationOptions emfRasterizationOptions = 
        new com.aspose.imaging.imageoptions.EmfRasterizationOptions();

// Set different properties
emfRasterizationOptions.setBackgroundColor(com.aspose.imaging.Color.getWhiteSmoke());

// Create an instance of PngOptions class
PngOptions pngOptions = new PngOptions();

// Pass the instance of EmfRasterizationOptions class
pngOptions.setVectorRasterizationOptions(emfRasterizationOptions);

//Declare variables to store file path
String filePath = ".\\alphabet.emf";

// Create an instance of EmfImage class and Load an existing EMF image.
com.aspose.imaging.fileformats.emf.EmfImage image = 
        (com.aspose.imaging.fileformats.emf.EmfImage)com.aspose.imaging.fileformats.emf.EmfImage.load(filePath);
try
{
    // Cache the image data for speed
    image.cacheData();

    // Set width & height of resultant image
    pngOptions.getVectorRasterizationOptions().setPageWidth(300);
    pngOptions.getVectorRasterizationOptions().setPageHeight(350);

    // Reset font font settings
    com.aspose.imaging.FontSettings.reset();

    // Call the Image.save() method to create the resultant image with default settings.
    // image.save(filePath + "_default_fonts.png", pngOptions); // un-comment this line for testing

    //Declare variable to store font file path
    String fontPath = ".\\Fonts";

    // Create an instance of Array list and add all default font paths to it.
    List fonts = new ArrayList();
    java.util.Collections.addAll(fonts, com.aspose.imaging.FontSettings.getDefaultFontsFolders());

    // Now add the new font path
    fonts.add(fontPath);

    // Call the setFontsFolders method of the FontSettings class and supply the array of font paths
    com.aspose.imaging.FontSettings.setFontsFolders(fonts.toArray(new String[0]), true);

    // Save the results to disk with new fonts
    image.save(filePath + "_with_my_fonts.png", pngOptions);
}
finally
{
    image.dispose();
}
```

## Enhancements

The following enhancements have been introduced in this release.

*   The process of loading WMF files has been improved.
*   Aspose.Imaging drawing engine has been improved.
*   The calculation process of Horizontal and Vertical resolution values has been improved.

Please refer to the release notes of [Aspose.Imaging for Java 3.7.0][4] for a full view of improvements along with sample code snippets for newly added features. If you are planning to upgrade the API to the latest revision, we strongly suggest you check the [Public API Changes][5] section to know what has been changed in the public API since your current version.

## Aspose.Imaging for Java Resources

The resources, you may need to accomplish your tasks:

*   [Home page for Aspose.Imaging for Java API][6].
*   [Download Aspose.Imaging for Java][7].
*   [Aspose.Imaging for Java online documentation][8] – help documentation and API reference documents.
*   [Aspose.Imaging Product Family Forum][9] – post your technical questions and queries, or any other problem you are facing while working with Aspose.Imaging APIs.
*   [Enable blog Subscription][10] – Do not limit yourself, you can keep yourself updated with the latest news on Aspose.Imaging APIs, new features, fixes and other API related topics by subscribing to Aspose.Imaging blog.
*   [Aspose.Imaging for Java in Online Repository][11] – We have published the JAR files on the Maven repository. Anyone could explore the code examples for learning purposes.

As always we appreciate your feedback so if you ever have anything to tell us about this release or anything else, please head to the [Aspose.Imaging forum][12] for a chat.




[1]: https://docs.aspose.com/display/imagingjava/Home
[2]: https://docs.aspose.com/display/imagingjava/Home
[3]: https://docs.aspose.com/
[4]: http://docs.aspose.com/display/imagingjava/Aspose.Imaging+for+Java+3.7.0+Release+Notes
[5]: http://docs.aspose.com/display/imagingjava/Migrating+from+Earlier+Versions+of+Aspose.Imaging
[6]: https://www.aspose.com/products/imaging/java
[7]: https://downloads.aspose.com/imaging/java
[8]: https://docs.aspose.com/display/imagingjava/Home
[9]: https://forum.aspose.com/
[10]: https://blog.aspose.com/category/aspose-products/aspose.imaging-product-family/
[11]: http://maven.aspose.com/repository/simple/ext-release-local/com/aspose/aspose-imaging/
[12]: https://forum.aspose.com/





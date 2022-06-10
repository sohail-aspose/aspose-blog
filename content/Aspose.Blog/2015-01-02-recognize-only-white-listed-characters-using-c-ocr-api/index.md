---
title: 'Recognize Only White Listed Characters using C# OCR API'
date: Fri, 02 Jan 2015 13:53:59 +0000
draft: false
url: /2015/01/02/recognize-only-white-listed-characters-using-c-ocr-api/
author: Babar Raza
summary: ''
tags: ['Babar Raza']
categories: ['Aspose.OCR Product Family']
---



{{< figure align=center src="images/aspose-OCR-for-net_100.png" alt="Aspose.OCR for .NET logo">}}


We are pleased to announce that the [Aspose.OCR for .NET 2.2.0][1] is now available for public use. This release contains many useful improvements, including the long-awaited feature of Character White Listing. Please refer to the release notes of v2.2.0 for a full list of bug fixes and improvements. If you are planning to upgrade the API from any previous version, we would suggest you to check the Public API Changes section first.

While you are downloading the latest build, here is a look at the biggest features in this release.

## Recognize Only White Listed Characters

Aspose.OCR for .NET API has exposed Whitelist property for the OcrConfig class in order to provide the feature of Character White Listing. Now the developers can add a list of characters for recognition purposes, and while performing the OCR operation the OcrEngine recognizes only the specified characters. The list of characters can be added to the OcrConfig class using its Whitelist property. As a default behavior, the OcrEngine recognizes only the white-listed characters if OcrConfig.Whitelist property is not null or not empty.

## OCR Preprocessed Images

Aspose.OCR for .NET API has exposed the PreprocessedImages class that allows the users to see how original input image changes during the OCR pre-processing. PreprocessedImages class has the following useful properties that can retrieve the image at a particular stage of the OCR pre-processing.

*   BinarizedImage represents the source image after binarization and/or background correction.
*   FilteredImage represents the source image after applying user specified correction filters.
*   NonTextRemovedImage represents the source image after detecting and removing the non-textual fragments such as graphics.
*   RotatedImage represents the source image after the skew correction has been applied.
*   TextBlocksImage represents the source image after text block detection. This image contains the red rectangles around all the detected textual blocks on the source image.

All of the above mentioned forms of the preprocessed images can be saved on the disc for performance evaluation of OCR configurations

```
 //Initialize an instance of OcrEngine
OcrEngine ocrEngine = new OcrEngine();

//Set the Image property by loading the image from file path location or an instance of MemoryStream 
ocrEngine.Image = ImageStream.FromFile(imageFile);

//Process the image
if (ocrEngine.Process())
{
    //Save binarized image on disc
    ocrEngine.PreprocessedImages.BinarizedImage.Save(@"D:\BinarizedImage.png", ImageFormat.Png);

    //Save filtered image on disc
    ocrEngine.PreprocessedImages.FilteredImage.Save(@"D:\FilteredImage.png", ImageFormat.Png);

    //Save image after removing non-textual fragments
    ocrEngine.PreprocessedImages.NonTextRemovedImage.Save(@"D:\NonTextRemovedImage.png", ImageFormat.Png);

    //Save image after skew correction
    ocrEngine.PreprocessedImages.RotatedImage.Save(@"D:\RotatedImage.png", ImageFormat.Png);

    //Save image after textual block detection
    ocrEngine.PreprocessedImages.TextBlocksImage.Save(@"D:\TextBlocksImage.png", ImageFormat.Png);
} 
```

## Part Hierarchy of Recognized Text

Aspose.OCR for .NET API allows to extract the text either as a whole or by parts whereas each part has its own Style, Font, Text Size and Location in the image, and all of this information can easily be extracted using the IRecognizedPartInfo and IRecognizedTextPartInfo class. The API also allows to retrieve the hierarchy of each recognized part on the image as TextBlock, Line, Word or Character. Hierarchy of the recognized part can be extracted using the TextPartLevel class that has been exposed to the public API with this release. The IRecognizedTextPartInfo class has two useful properties such as Level and Children that provides the access to the hierarchical level and lower level textual parts respectively.

As always we appreciate your feedback so if you ever have anything to tell us about this release or anything else, please head to the [Aspose.OCR forum][2] for a chat.




[1]: https://products.aspose.com/ocr/net
[2]: http://forum.aspose.com





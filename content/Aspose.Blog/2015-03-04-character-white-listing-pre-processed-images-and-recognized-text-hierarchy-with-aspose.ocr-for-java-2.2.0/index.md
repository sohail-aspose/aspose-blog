---
title: 'Character White Listing, Pre-processed Images and Recognized Text Hierarchy with Aspose.OCR for Java 2.2.0'
date: Wed, 04 Mar 2015 14:43:54 +0000
draft: false
url: /2015/03/04/character-white-listing-pre-processed-images-and-recognized-text-hierarchy-with-aspose.ocr-for-java-2.2.0/
author: Babar Raza
summary: ''
tags: ['Babar Raza']
categories: ['Aspose.OCR Product Family']
---

[![Aspose.OCR for Java logo][1]](http://www.aspose.com/java/ocr-component.aspx "Aspose.OCR for Java Overview")This month's release of [Aspose.OCR for Java 2.2.0][2] is now available with some great new feature, including the long awaited feature of Character White Listing. Please refer to the release notes of v2.2.0 for a full list of bug fixes and improvements. If you are planning to upgrade the API from any previous version, we would suggest you to check the Public API Changes section first.

While you are downloading the latest build, here is a look at the biggest features and worth mentioning changes in this release.

## Code Baseline Moved to Java 6

Starting with this release, Aspose.OCR for Java has dropped the support for Java versions prior to v6 and has moved its codebase to Java 6 (Java 7 and 8 are also supported). Reason being, Sun/Oracle has discontinued the support for all JDK revisions prior to 1.6. Now the Aspose.OCR for Java package contains a single Jar for Aspose.OCR & another for Aspose.OMR that works well with Java 6, 7 & 8.

## Recognize Only White Listed Characters

Aspose.OCR for Java API has exposed the Whitelist property for the OcrConfig class in order to provide the feature of Character White Listing. Now the developers can add a list of characters for recognition purposes. When Whitelist property is not null or empty, the OcrEngine recognizes only the specified characters while skipping everything else on the input image. The list of characters can be added to the OcrConfig class using its Whitelist property to enable this feature.

## OCR Preprocessed Images

Aspose.OCR for Java API has now exposed the PreprocessedImages class that allows the users to see how original input image is transformed during the OCR pre-processing steps. PreprocessedImages class has the following useful properties that can retrieve the image at any particular stage of the OCR pre-processing.

*   BinarizedImage represents the source image after binarization and/or background correction.
*   FilteredImage represents the source image after applying user specified correction filters.
*   NonTextRemovedImage represents the source image after detecting and removing the non-textual fragments such as graphics.
*   RotatedImage represents the source image after the skew correction has been applied.
*   TextBlocksImage represents the source image after text block detection. This image contains the red rectangles around all the detected textual blocks on the source image.

All of the above mentioned forms of the pre-processed images can be saved on the disc for performance evaluation of OCR configurations using the following simple piece of code.

```
 //Initialize an instance of OcrEngine
OcrEngine ocrEngine = new OcrEngine();

//Set the Image property by loading the image from file path location
ocrEngine.setImage(ImageStream.fromFile(imagePath));

//Process the image
if (ocrEngine.process())
{	
	//Save binarized image on disc
	ImageIO.write(ocrEngine.getPreprocessedImages().getBinarizedImage(), "PNG", new File("D:/BinarizedImage.png"));

	//Save filtered image on disc
	ImageIO.write(ocrEngine.getPreprocessedImages().getFilteredImage(), "PNG", new File("D:/FilteredImage.png"));

	//Save image after removing non-textual fragments
	ImageIO.write(ocrEngine.getPreprocessedImages().getNonTextRemovedImage(),"PNG", new File("D:/NonTextRemovedImage.png"));

	//Save image after skew correction
	ImageIO.write(ocrEngine.getPreprocessedImages().getRotatedImage(), "PNG", new File("D:/RotatedImage.png"));

	//Save image after textual block detection
       	ImageIO.write(ocrEngine.getPreprocessedImages().getTextBlocksImage(), "PNG", new File("D:/TextBlocksImage.png"));
} 
```

## Part Hierarchy of Recognized Text

Aspose.OCR for Java API allows to extract the text either as a whole or by parts whereas each part has its own Style, Font, Text Size and Location in the image, and all of this information can easily be extracted using the IRecognizedPartInfo and IRecognizedTextPartInfo class. The API also allows to retrieve the hierarchy of each recognized part on the image as TextBlock, Line, Word or Character. Hierarchy of the recognized part can be extracted using the TextPartLevel class that has been exposed to the public API with this release. The IRecognizedTextPartInfo class has two useful properties such as Level and Children that provides the access to the hierarchical level and lower level textual parts respectively.

As always we appreciate your feedback so if you ever have anything to tell us about this release or anything else, please head to the [Aspose.OCR forum][3] for a chat.




[1]: https://blog.aspose.com/wp-content/uploads/sites/2/2013/07/aspose-OCR-for-Java_100.png "Aspose.OCR for Java"
[2]: http://www.aspose.com/community/files/72/java-components/aspose.ocr-for-java/entry609926.aspx "Download Aspose.OCR for Java 2.2.0"
[3]: http://www.aspose.com/community/forums/aspose.ocr-product-family/493/showforum.aspx





---
title: 'C# OCR API - Add User Defined Recognition Blocks and Auto-Detect Text Blocks'
date: Sat, 28 Jun 2014 12:25:50 +0000
draft: false
url: /2014/06/28/add-user-defined-recognition-blocks-auto-detect-text-blocks/
author: Babar Raza
summary: ''
tags: ['.NET API', 'Aspose.OCR', 'Babar Raza', 'Enhanced OCR', 'Non-Textual Block Removal', 'OCR', 'Spelling Correction', 'Text Block Detection']
categories: ['Aspose.Total Product Family', 'Aspose.OCR Product Family']
---



{{< figure align=center src="images/aspose-OCR-for-net_100.png" alt="Aspose.OCR for .NET logo">}}


We are pleased to announce the monthly release of [Aspose.OCR for .NET][1], version 2.0.0. Our team has been hard at work bringing many useful improvements to this edition of the Aspose.OCR API. You can start exploring the newly added features & enhancements immediately, but before you head to the [download section][2], here is a look at just a few of the biggest features in this month’s release. For a full list of bug fixes and improvements please refer to the download pages in the link above. If you are going to upgrade the API, please refer to the Public API Changes in reference to v2.0.0 of Aspose.OCR for .NET article.

## Custom Recognition Blocks

Users may now define custom recognition blocks on the document image. These will be processed by the OcrEngine while other areas of the image are skipped. However, if user defined recognition blocks are not set prior to processing, the OcrEngine automatically calculate the recognition blocks using its default behavior.

## Detect the Reading Order

Images with text can be divided into many text recognition blocks. It is sometimes important to apply a special sorting so that the correct text block order is maintained. The OcrConfig class has exposed the DetectReadingOrder property to handle situations where an image within the main document image may contain text blocks of its own. Setting the DetectReadingOrder property to true instructs the OcrEngine to maintain the order of text regions for better recognition result. However, performance degradation can be observed for images with a large number of text blocks. In such cases, it is advised to turn this feature off by setting the DetectReadingOrder property to false.

## Automatic Spelling Correction

In order to improve the accuracy of the recognized data, the Aspose.OCR for .NET API has exposed the DoSpellingCorrection property for the OcrConfig class. A Boolean property, it can be either set to true or false indicating whether automatic spelling correction should be applied on the recognized text or not. Setting the DoSpellingCorrection property to true will improve the OCR results, however, the process may take more time to complete. Please check the detailed article on setting the OcrEngine to automatically correct spelling.

## Ignore Non-Textual Blocks

Document images to be processed with OcrEngine may contain graphics. During the OCR process, these graphics may not contain any text to be recognized although they are detected as a separate block. If developers wish to ignore the non-textual blocks such as graphics from the recognition process, they just have to set the RemoveNonText property exposed by the OcrConfig class to true.

## Enhancements to the OcrEngine

Last but not the least, we have completely overhauled the OcrEngine with new recognition algorithm for better accuracy of the recognized data and performance considerations. Moreover, Aspose.OCR API now uses a resource file that is just of 5.5MB in size unlike previous resource files of 88MB.

As always we appreciate your feedback so if you ever have anything to tell us about this release or anything else, please head to the [Aspose.OCR forum][3] for a chat.




[1]: https://products.aspose.com/ocr/net
[2]: https://downloads.aspose.com/ocr/net
[3]: http://forum.aspose.com





---
title: 'Custom Recognition Blocks, Detect Reading Order and Other Enhancements with Aspose.OCR for Java 2.0.0'
date: Wed, 13 Aug 2014 05:46:26 +0000
draft: false
url: /2014/08/13/custom-recognition-blocks-detect-reading-order-and-other-enhancements-with-aspose.ocr-for-java-2.0.0/
author: Babar Raza
summary: ''
tags: ['Aspose.OCR', 'Aspose.OCR for Java 2.0.0', 'Babar Raza', 'Custom Recognition Blocks', 'Non-Textual Blocks', 'OCR API', 'OcrEngine', 'Reading Order']
categories: ['Aspose.OCR Product Family']
---



{{< figure align=center src="images/aspose-OCR-for-Java_100.png" alt="Aspose.OCR for Java logo">}}


We have just released this month’s improvements to Aspose.OCR for Java, and have upgraded the API to version 2.0.0. This release contains 12 improvements, including the showcased feature discussed below. You can download the latest Aspose.OCR for Java release from the [download section][1] now, and start exploring the newly added features. However, if you are planning to upgrade your project to use the latest build, we recommend you to check the Public API Changes section first.

## Custom Recognition Blocks

Setting custom recognition blocks is useful when documents of the same layout have to be processed. Programmers can specify custom recognition blocks and direct the API to focus on a particular area of the image. The latest build allows the users to define custom recognition blocks on the document image. These blocks are processed by the OcrEngine while other areas are skipped completely. If user-defined recognition blocks are not set prior to processing, the OcrEngine automatically calculates the recognition blocks using its default behavior.

## Detect the Reading Order

Images with text can be divided into many text blocks on which the recognition process can be performed. It is sometimes important to apply a special sorting so that the correct text block order is maintained. The OcrConfig class has exposed the DetectReadingOrder property to handle situations where an image within the main document image may contain text blocks of its own. Setting the DetectReadingOrder property to true instructs the OcrEngine to maintain the order of text regions for better recognition results. However, performance degradation can be observed for images with a large number of text blocks. In such cases, it is advised to turn this feature off by setting the DetectReadingOrder property to false.

## Automatic Spelling Correction

In order to improve the accuracy of the recognized data, the Aspose.OCR for Java API has exposed the DoSpellingCorrection property for the OcrConfig class. Setting the DoSpellingCorrection property to true will improve the OCR results, however, the process may take more time to complete. Please check the detailed article on setting the OcrEngine to automatically correct spelling.

## Ignore Non-Textual Blocks

Document images to be processed with OcrEngine may contain graphics. During the OCR process, these graphics may not contain any text to be recognized although they are detected as a separate block. If developers wish to ignore the non-textual blocks such as graphics from the recognition process, they just have to set the RemoveNonText property exposed by the OcrConfig class to true.

## Enhancements to the OcrEngine

Last but not the least, we have completely overhauled the OcrEngine with a new recognition algorithm for better accuracy of the recognized data and performance considerations. Moreover, [Aspose.OCR API now uses a resource file that is just of 5.5MB in size][2] unlike previous resource files of 88MB.

Please visit the [documentation][3] for details, and if you still have any questions, we always welcome inquiries on [Aspose.OCR Support Forum][4].




[1]: https://downloads.aspose.com/ocr/java
[2]: https://downloads.aspose.com/ocr/java
[3]: http://docs.aspose.com/display/OCRJAVA/Home
[4]: http://forum.aspose.com





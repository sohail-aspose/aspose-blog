---
title: 'Merged OCR &amp; OMR Features with Aspose.OCR for Java 2.4.0'
date: Sat, 02 May 2015 17:00:40 +0000
draft: false
url: /2015/05/02/merged-ocr-omr-features-with-aspose.ocr-for-java-2.4.0/
author: Babar Raza
summary: ''
tags: ['Babar Raza']
categories: ['Aspose.OCR Product Family']
---

[![Aspose.OCR for Java logo][1]](http://www.aspose.com/java/ocr-component.aspx "Aspose.OCR for Java Overview")We're pleased to announce the release of the first version of merged Aspose.OCR for Java. In this merged version, we have combined the com.aspose.ocr & com.aspose.omr packages in one jar and published it as [Aspose.OCR for Java 2.4.0][2]. Now you can use the single component to work with both OCR & OMR features without even changing your existing code. If you are planning to upgrade the API from any revision prior to v2.3.0, we suggest you to check the Public API Changes section first.

## What Has Been Changed

From API point of view, nothing has changed. All the classes, method, enumerations & properties that were previously present in com.aspose.omr package still reside there, whereas all the APIs relevant to OCR features still belong to com.aspose.ocr package.  In order to keep this transition simple, we haven't changed anything in the public API so you do not need to worry about changing your existing code to accommodate this merger. However, number of jars for the Aspose.OCR for Java package have been reduced to one, that mean; you can use the single jar (Aspose.OCR.jar) for both OCR & OMR features from now onward. Please review the Public API Changes in reference to Aspose.OCR for Java 2.4.0 for more details.

## Enhancements & Fixes

This release has addressed a few critical issues and has incorporated some enhancements as detailed below.

*   Enhanced the OmrEngine to support the template version 4.
*   Fixed the implementation of IRecognitionBlock.RecognitionData that used to return null for the custom recognition blocks. Due to this issue, the API didn't allow to retrieve the symbols & words that belongs to a specific block on the image.
*   Improved the exception handling for the cases where OMR elements have invalid dimensions.

As always we appreciate your feedback so if you ever have anything to tell us about this release or anything else, please head to the [Aspose.OCR forum][3] for a chat.




[1]: https://blog.aspose.com/wp-content/uploads/sites/2/2013/07/aspose-OCR-for-Java_100.png "Aspose.OCR for Java"
[2]: http://www.aspose.com/community/files/72/java-components/aspose.ocr-for-java/entry625131.aspx "Download Aspose.OCR for Java 2.4.0"
[3]: http://www.aspose.com/community/forums/aspose.ocr-product-family/493/showforum.aspx





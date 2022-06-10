---
title: 'Configure Threshold for OMR with Aspose.OCR for .NET'
date: Mon, 07 Apr 2014 10:10:54 +0000
draft: false
url: /2014/04/07/configure-threshold-for-omr/
author: Babar Raza
summary: ''
tags: ['Aspose.OCR', 'Aspose.OCR for .NET', 'Aspsoe.OMR', 'Babar Raza', 'Element Level Threshold', 'OMR', 'OMR Template Editor', 'Optical Mark Recognition', 'Page Level Threshold', 'Recognition Threshold', 'Template Level Threshold', 'Threshold']
categories: ['Aspose.OCR Product Family']
---



{{< figure align=center src="images/aspose-OCR-for-net_100.png" alt="Threshold Optical Mark Recognition">}}


[](https://blog.aspose.com/wp-content/uploads/sites/2/2012/10/imgLogoOCR128x128.png)[][1]Aspose.OCR 1.9.0 has been released and we are pleased to announce that this month’s release contains many useful improvements and bug fixes reported for previous versions. You can download the latest release of [Aspose.OCR for .NET 1.9.0][2] from the download section along with the required resource files.

Here is a look at a few of the features in this month’s release. For a full list of bug fixes and improvements please refer to the download pages in the link above.

## Optical Mark Recognition Threshold

The threshold specifies the percentage of black pixels over which the option is considered selected. A threshold can be set before initializing the OMR procedure to determine the amount of pixels (as a percent) that is required before a field or a mark is considered checked or filled. Aspose.OCR for .NET now supports setting the threshold for a template, template page and even for a specific template element . Please check the detailed article on Setting OMR Thresholds.

### Template Level Threshold

A threshold can be configured on the template level so that all pages and elements use the rules set globally. The OmrConfig class now contains the FillThreshold property that accepts a value between 0 to 1, corresponding to the threshold percentage where 1 means 100% and thus requires the mark to be filled completely.

## Page Level Threshold

OmrPage now contains the FillThreshold property for the page configurations. Like above this property also accepts a value between 0 to 1 where 0 is the most lenient interpretation of OMR marks and 1 means the most strict.

## Element Level Threshold

All the supported OMR elements now contain the TrimWhitePixels property for their configurations. TrimWhitePixels accepts a Boolean (true/false) value indicating whether the area that contains a OMR mark should be reduced to a minimum size that contains all black pixels.

As always we appreciate your feedback so if you ever have anything to tell us about this release or anything else, please head to the [Aspose.OCR forum][3] for a chat.




[1]: https://blog.aspose.com/wp-content/uploads/sites/2/2013/07/OCRDotNet.png
[2]: http://www.aspose.com/community/files/51/.net-components/aspose.ocr-for-.net/default.aspx "Aspose.OCR for .NET 1.9.0"
[3]: http://www.aspose.com/community/forums/aspose.ocr-product-family/493/showforum.aspx





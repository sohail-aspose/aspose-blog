---
title: 'Configure Threshold for Optical Markers using Java OMR API'
date: Sun, 13 Apr 2014 09:34:57 +0000
draft: false
url: /2014/04/13/configure-threshold-for-optical-markers-with-aspose.ocr-for-java-1.9.0/
author: Babar Raza
summary: ''
tags: ['Aspose.OCR', 'Aspsoe.OMR', 'Babar Raza', 'Element Level Threshold', 'OMR', 'OMR Template Editor', 'Optical Mark Recognition', 'Page Level Threshold', 'Recognition Threshold', 'Template Level Threshold', 'Threshold']
categories: ['Aspose.OCR Product Family']
---



{{< figure align=center src="images/aspose-OCR-for-Java_100.png" alt="Aspose.OCR for Java logo">}}


We are pleased to announce the release of Aspose.OMR for Java 1.9.0. This month's release contains all the features, enhancements and bug fixes from Aspose.OMR for .NET 1.8.0 and 1.9.0.

This outlines the most significant changes. Check the detailed release notes for all enhancements and fixes when downloading the latest version of [Aspose.OMR for Java 1.9.0][1].

## Optical Mark Recognition Threshold

The threshold specifies the percentage of black pixels over which the option is considered to be selected. Setting a lower threshold allows the OmrEngine to consider any partially filled marker as selected; a higher threshold may require the marker to be filled completely. Usually, the threshold is set to an acceptable higher average value before initializing the OMR procedure to determine the number of pixels (as a percent) that is required before a field or a mark is considered checked or filled. Aspose.OCR for Java now supports setting the threshold for a template, template page and even for a specific template element. Please check the detailed article on [Setting OMR Thresholds][2].

## Equal Spacing Between the Markers

This enhancement has been made for the OmrEngine to accommodate markers that are equally distributed on the OMR template. Unfortunately, the Template Editor for the Java version of the product isn't yet available for public use. We are working to provide a Java-based template editor with future releases of Aspose.OMR for Java.

Please visit the documentation for details, and if you still have any questions, we always welcome inquiries on [Aspose.OMR Support Forum][3].




[1]: https://downloads.aspose.com/omr/java
[2]: https://docs.aspose.com/display/omrjava/Perform+OMR+on+Images#PerformOMRonImages-PerformOMRoperationwithathresholdsetting
[3]: https://forum.aspose.com/





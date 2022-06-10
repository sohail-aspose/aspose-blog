---
title: 'Determine Line Break Scenario in PDF Documents using Java'
date: Sun, 13 May 2018 20:44:15 +0000
draft: false
url: /2018/05/13/determine-line-break-scenario-and-performance-improvements-during-pdf-to-html-conversion/
author: Asad Ali
summary: ''
tags: ['Asad Ali']
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/aspose-Pdf-for-Java.png" alt="">}}


As per the regular monthly update process, we are pleased to announce [Aspose.PDF for Java 18.4][1]. The new version of Aspose.PDF for Java API has been released and available on Aspose Artifactory for download and to be used in Java Projects. Like every release of Java API, we have ported features from .NET library of Aspose.PDF as well as made several bug fixes in [Aspose.PDF for Java 18.4][2]. Public API Changes are given in the [release notes][3] page of Aspose.PDF for Java 18.4 and we recommend you to go through release notes of the API before using it.

## Process Line Breaking

Some of our customers have requirements to determine the points/positions where an Enter/Line Break was added to create new line or contents of a line were moved to the subsequent line, after content reaching to the edge of the page. We have implemented tracking background processing of multi-line text fragments in text adding scenarios. You can use [getNotifications()][4] method of Page Class, in order to log the line breaks. You may please check respective example in API documentation on following link, where code snippet for such functionality has been showcased:

*   [Track Line Breaking of Multi-Line TextFragments][5]

We already have been planning to add features in our API regarding such scenarios, and we are working over providing support for these features in scenarios of manipulating existing PDF documents as well. We hope to provide more enhancements in API regarding this feature in upcoming versions. For now, only notifications about paragraph events in text adding scenarios are supported.

## PDF to HTML Conversion Performance

Regarding the performance of the API during PDF to HTML conversion, there were some issues reported for earlier versions of Aspose.PDF for Java. For some particular PDF documents (i.e. containing images and annotations), API was taking more time than expected in order to render them as HTML. However, we have improved API for such type of conversions, and processing time is much reduced in Aspose.PDF for Java 18.4.

Along with the improvements and enhancements mentioned above, we have made following bug fixes in this release of API:

*   Cannot retrieve the watermark text of PDF
*   Security error on setting custom font directory
*   PDF to HTML: Header text is not been rendered correctly
*   PDF to HTML: Text rendered incorrectly
*   RedactArea corrupts the PDF if with setLicense method

## Miscellaneous Fixes

As it is always recommended to use the latest release of our API’s because they include the latest features/improvements and fixes related to issues reported in earlier released versions. Therefore, please download the latest release of [Aspose.PDF for Java 18.4.][6]

*   [Home page for Aspose.PDF for Java][7]
*   [Download Aspose.PDF for Java 18.4][8]
*   [Aspose.PDF product family forum][9] – Post your technical questions and queries, or any other problem you faced while running Aspose.PDF APIs.
*   [Aspose.PDF for Java online documentation][10]– Help documentation and API reference documents.
*   [Enable Blog Subscription][11]– Do not limit yourself, you can keep yourself updated with the latest news on Aspose.PDF APIs, new features, fixes, and other API related topics by subscribing to Aspose.PDF blog.




[1]: https://artifact.aspose.com/webapp/#/artifacts/browse/tree/General/repo/com/aspose/aspose-pdf/18.4
[2]: https://artifact.aspose.com/webapp/#/artifacts/browse/tree/General/repo/com/aspose/aspose-pdf/18.4
[3]: https://docs.aspose.com/display/pdfjava/Aspose.PDF+for+Java+18.4+Release+Notes
[4]: https://apireference.aspose.com/java/pdf/com.aspose.pdf/Page#getNotifications--
[5]: https://docs.aspose.com/display/pdfjava/Determine+Line+Break
[6]: https://artifact.aspose.com/webapp/#/artifacts/browse/tree/General/repo/com/aspose/aspose-pdf/18.4
[7]: https://products.aspose.com/pdf/java
[8]: https://artifact.aspose.com/webapp/#/artifacts/browse/tree/General/repo/com/aspose/aspose-pdf/18.4
[9]: https://forum.aspose.com/c/pdf
[10]: https://docs.aspose.com/display/pdfjava/Home
[11]: https://blog.aspose.com/category/aspose-products/aspose-pdf-product-family/





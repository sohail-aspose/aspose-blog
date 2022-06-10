---
title: 'Support for Portuguese Language &amp; Improved Notifiers with Aspose.OCR for Java 2.3.0'
date: Mon, 30 Mar 2015 12:13:39 +0000
draft: false
url: /2015/03/30/support-for-portuguese-language-improved-notifiers-with-aspose.ocr-for-java-2.3.0/
author: Babar Raza
summary: ''
tags: ['Babar Raza']
categories: ['Aspose.OCR Product Family']
---

[![Aspose.OCR for Java logo][1]](http://www.aspose.com/java/ocr-component.aspx "Aspose.OCR for Java Overview")Aspose.OCR for Java 2.3.0 has been released. This month’s release contains useful improvements and features including the support for Portuguese language. Please refer to the release notes of [Aspose.OCR for Java 2.3.0][2] for a full list of bug fixes and improvements. If you are planning to upgrade the Aspose.OCR for Java API to the latest revision, we would strongly suggest you to check the complete Public API Changes section to know what has been changed in the API so far.

While you are downloading the latest build, here is a look at the showcased features of this release.

## Support for Portuguese Language

Aspose.OCR for Java API has extended the support for languages by including Portuguese to its neural network. In order to perform OCR operation for Portuguese language, Aspose.OCR for Java 2.3.0 has provided the specific resources that are required by the OcrEngine to correctly identify the language specific characters. These resources are available for download in an archive at [Aspose download section][3].

Important point to note here is that while setting up OcrEngine to recognize Portuguese language characters, it is required to specify the language specific resource while using LanguageFactory.load method and adding them to the LanguageContainer using the addLanguage method. Please check more details on How to setup OCR process for different languages.

## Creating Recognition Notifications

Aspose.OCR for Java API has exposed the NotifierFactory class that allows the users to create objects of type INotifier that in turn can be used to enable the notifications during the OCR process. The com.aspose.ocr.NotifierFactory class supports 5 types of different notifiers as detailed below.

*   symbolNotifier method can be used to create the notifier that causes an event on each recognized symbol.
*   wordNotifier method can be used to create the notifier that causes an event on each recognized word.
*   lineNotifier method can be used to create the notifier that causes an event on each recognized line.
*   blockNotifier method can be used to create the notifier that causes an event on each recognized text block.
*   pageNotifier method can be used to create the notifier that causes an event when a page from a multipage document is recognized.

Source code snippets and more details on this subject are available at Usage of NotifierFactory Class.

As always we appreciate your feedback so if you ever have anything to tell us about this release or anything else, please head to the [Aspose.OCR forum][4] for a chat.




[1]: https://blog.aspose.com/wp-content/uploads/sites/2/2013/07/aspose-OCR-for-Java_100.png "Aspose.OCR for Java"
[2]: http://www.aspose.com/community/files/72/java-components/aspose.ocr-for-java/entry617531.aspx "Download Aspose.OCR for Java 2.3.0"
[3]: http://www.aspose.com/community/files/51/.net-components/aspose.ocr-for-.net/entry609348.aspx "Aspose Download Section"
[4]: http://www.aspose.com/community/forums/aspose.ocr-product-family/493/showforum.aspx





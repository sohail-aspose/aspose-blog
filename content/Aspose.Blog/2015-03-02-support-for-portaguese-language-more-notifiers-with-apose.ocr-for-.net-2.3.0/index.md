---
title: 'Perform OCR for Portuguese Language using C# or VB.NET'
date: Mon, 02 Mar 2015 11:00:24 +0000
draft: false
url: /2015/03/02/support-for-portaguese-language-more-notifiers-with-apose.ocr-for-.net-2.3.0/
author: Babar Raza
summary: ''
tags: ['Babar Raza']
categories: ['Aspose.OCR Product Family']
---



{{< figure align=center src="images/aspose-OCR-for-net_100.png" alt="Aspose.OCR for .NET logo">}}


We are pleased to announce that the [Aspose.OCR for .NET 2.3.0][1] is now available for public use. This release contains many useful improvements, including the support for Portuguese/Brazilian Portuguese language. Please refer to the release notes of v2.3.0 for a full list of bug fixes and improvements. If you are planning to upgrade the API from any previous version, we would suggest you to check the Public API Changes section first.

While you are downloading the latest build, here is a look at the biggest features in this release.

## OCR for Portuguese Language in C#

Aspose.OCR for .NET API has extended the support for languages by including Portuguese to its neural network. In order to perform OCR operation for the Portuguese language, Aspose.OCR for .NET 2.3.0 has provided the specific resources that are required by the OcrEngine to correctly identify the language-specific characters. These resources are available for download in an archive at the Aspose download section.

An important point to note here is that while setting up OcrEngine to recognize Portuguese language characters, it is required to specify the language specific resource while using LanguageFactory.Load method and adding them to the LanguageContainer using the AddLanguage method. Please check more details on [how to setup OCR process for different languages][2].

## Creating Recognition Notifications

Aspose.OCR for .NET API has exposed the NotifierFactory class that allows the users to create objects of type INotifier that in turn can be used to enable the notifications during the OCR process.

The Aspose.OCR.NotifierFactory class supports 5 types of different notifiers as detailed below.

*   SymbolNotifier method can be used to create the notifier that causes an event on each recognized symbol.
*   WordNotifier method can be used to create the notifier that causes an event on each recognized word.
*   LineNotifier method can be used to create the notifier that causes an event on each recognized line.
*   BlockNotifier method can be used to create the notifier that causes an event on each recognized text block.
*   PageNotifier method can be used to create the notifier that causes an event when a page from a multipage document is recognized.

## Other Enhancements & Fixes

Along with above-mentioned features, the Aspose.OCR for .NET 2.3.0 has enhanced the OMR Template Editor to load images of type GIF, BMP, TIFF, JPEG, PNG for possible optical marker extraction. The OMR Template Editor can now accept Aspose.OCR for .NET assembly without requiring the additional resources and Aspose.BarCode for .NET assembly to recognize barcodes from an OMR form.

As always we appreciate your feedback so if you ever have anything to tell us about this release or anything else, please head to the [Aspose.OCR forum][3] for a chat.




[1]: https://downloads.aspose.com/ocr/net
[2]: https://docs.aspose.com/display/ocrnet/Working+with+Different+Languages
[3]: http://forum.aspose.com





---
title: 'Barcode Recognition in WPF and Separate Binary for .NET Compact Framework 3.5 in Aspose.BarCode for .NET 6.1.0'
date: Fri, 21 Mar 2014 19:18:45 +0000
draft: false
url: /2014/03/21/barcode-recognition-in-wpf-and-separate-binary-for-.net-compact-framework-3.5-in-aspose.barcode-for-.net-6.1.0/
author: Imran Rafique
summary: ''
tags: ['Imran.Rafique']
categories: ['Aspose.BarCode Product Family']
---

[![][1]](https://blog.aspose.com/wp-content/uploads/sites/2/2013/07/aspose-Barcode-for-net_100.png)Aspose.BarCode for .NET 6.1.0 has been released. We are pleased to share with everyone that this new release is quite a plus for WPF application projects because barcode recognition has been added. Previously, there was no way to read barcodes in WPF projects. You can find the details of this feature in the following help topic: Recognizing Barcode in WPF Project. With this release, we have also shipped a separate Aspose.BarCode library for .NET Compact Framework 3.5.

## Combining Generation and Recognition

We have merged the recognition and generation modules so that now there is a single library for both APIs. This means that developers don’t have to apply a license for each module. As a result, we have removed the Aspose.BarCodeRecognition.License class because there's no need for it. Simply apply a license once using the Aspose.BarCode.License class. Please see the updated help topics: Licensing Information, Setting a License in Aspose.BarCode for .NET.

## Fixed Issues and Improvements

We have included a number of bug fixes and improvements. They are mostly based on customer feedback, scenarios and earlier experience. With these fixes and improvements, recognition and generation techniques are now better than in previous releases.

In this release, the recognition rate of various symbologies, for example Code128 from PDF, JPG, and TIFF, PDF417 from PDF, GS1Code128 from PNG, OneCode from JPG, DataMatrix from PNG, and TIFF, AustralianPosteParcel from GIF and Code39 from TIFF, are a little more mature. Partial recognition is downgraded with respect to the PLANET and POSTNET symbologies from JPEG. Two fixes were about incorrect recognition so the accuracy of EAN13 and Code128 symbologies from PDF can increase.

We can now generate a DataMatrix code in a small size of JPG format. Based on this, resolution support has automatically added to the BarCodeBuilder.GetCustomSizeBarCodeImage(Size, bool) and BarCodeBuilder.GetOnlyBarCodeImage() methods. These methods work as expected, taking resolution into account. Please see a complete example topic: [Generate Barcode Using Custom Width  Support][2].

Also, the appearance of Interleaved2of5 symbology is now better because there are no addition lines around the code. Aspose.BarCode binaries support dual signing with SHA1 & SHA2.

To view a complete list of new features, fixes and enhancements [download the new release of Aspose.BarCode for .NET][3].




[1]: https://blog.aspose.com/wp-content/uploads/sites/2/2013/07/aspose-Barcode-for-net_100.png "Aspose.BarCode for .NET logo"
[2]: https://blog.aspose.com/ "Generate Barcode Using Custom Width Support"
[3]: http://www.aspose.com/community/files/51/.net-components/aspose.barcode-for-.net/default.aspx





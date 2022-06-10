---
title: 'Improved Garbage Element Recognition and New Page Notifier in Aspose.OCR for .NET 1.5.0'
date: Thu, 04 Apr 2013 13:02:39 +0000
draft: false
url: /2013/04/04/improved-garbage-element-recognition-and-introduction-of-page-notifier-in-aspose.ocr-for-.net-1.5.0/
author: Tilal Ahmad
summary: ''
tags: ['.NET', 'Babar Raza', 'OCR', 'Page Notifier', 'product release']
categories: ['Aspose.OCR Product Family']
---

[](https://blog.aspose.com/wp-content/uploads/sites/2/2012/10/imgLogoOCR128x128.png)[![][1]](https://blog.aspose.com/wp-content/uploads/sites/2/2013/04/OCRDotNet.png)We are pleased to announce the release of Aspose.OCR for .NET 1.5.0.

In this release we have introduced some improvements and bug fixes along with a new feature.  It includes improvement in garbage element detection to increase the recognition accuracy. Rotation and flip parameters are exposed in the public API; the default value is none. Users can specify these parameters to improve recognition speed and accuracy as well.

This release also fixed an issue with recognition notification as well as other issues. We have also introduced a page notifier feature in this release. It usage is similar to other notifiers.

```
`INotifier processorPage = Notifier.Page();
processorPage.Elapsed += delegate 
 {
 totalPages++;` `};
ocrEngine.AddNotifier(processorPage);`
```

Please visit the following link for further details on what’s new in [Aspose.OCR for .NET 1.5.0][2].




[1]: https://blog.aspose.com/wp-content/uploads/sites/2/2013/04/OCRDotNet.png "OCRDotNet"
[2]: http://www.aspose.com/community/files/51/.net-components/aspose.ocr-for-.net/entry455864.aspx





---
title: 'Extract Text from Headers and Footers and Watermark Count from PDF using C#'
date: Thu, 18 Oct 2012 14:01:10 +0000
draft: false
url: /2012/10/18/extract-text-from-headerfooter-section-get-watermark-count-set-default-font-for-form-field/
author: Codewarior
summary: ''
tags: ['Nayyer Shahbaz']
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/aspose.pdf-logo2.jpg" alt="Aspose.Pdf icon">}}


We're pleased to announce the release of [Aspose.PDF for .NET 7.4.0][1]. In this release, we have introduced many new features. A new feature to manipulate watermarks or artifacts in PDF document has been introduced and now you can also count the number of watermarks of a particular type in a PDF document. Some further details regarding this feature can be found over at working with existing watermarks. A highly demanded feature, setting form fields fonts to other than the 14 core fonts, has been implemented. With this new release, any font present in FontRepository can be set as the default font for form fields. Please check out the following documentation article for further details on how to use this feature: Set Form Field Font to Other than the 14 Core Fonts.

In earlier releases, the PdfExtractor was used to extract images defined in resources. With this release, we've added another approach to extract images in the system: ImagePlacementAbsorber. A new enumeration - ExtractImageMode - has been introduced and now images can be extracted in ActuallyUsed or DefinedInResources mode.

```
PdfExtractor extractor = new PdfExtractor();
extractor.BindPdf(TestSettings.GetInputFile("pic.pdf")); 
extractor.ExtractImageMode = ExtractImageMode.ActuallyUsed;  
extractor.ExtractImage();  
while (extractor.HasNextImage())  
{ extractor.GetNextImage(imgFileName, ImageFormat.Png); }
```

Please visit the following link for further details on what's new & fixed in [Aspose.PDF for .NET 7.4.0][2].




[1]: https://products.aspose.com/pdf/net
[2]: https://downloads.aspose.com/pdf/net





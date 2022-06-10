---
title: 'Find Minimum Required Height And Width for A BarCode Image With Aspose.BarCode for SSRS 17.7'
date: Thu, 03 Aug 2017 17:47:59 +0000
draft: false
url: /2017/08/03/find-minimum-required-hight-width-barcode-image-aspose.barcode-ssrs-17.7/
author: Ikram Haq
summary: ''
tags: []
categories: ['Aspose.BarCode Product Family']
---

We are pleased to announce the release of Aspose.BarCode for Reporting Services 17.7. The major development in this release is the functionality to get the minimun size (height & width) required for the barcode image. Improved functionality of GetOnlyBarCodeImage method has also been incorporated in this release.

## Get Minimum BarCode Size

Aspose.BarCode for Reporting Services now enables its users to get the minimum height & width required for a barcode image to be generated. How a developer can get the minimum size (height & width) is very simple and is demonstrated in the code snippet given below. The code snippet contains comments that makes it self explanatory.

```
// Create an instance of BarCodeBuilder class
// Set barcode text
// Set encoding type
using (Aspose.BarCode.BarCodeBuilder builder = new Aspose.BarCode.BarCodeBuilder("1234567890", Aspose.BarCode.Generation.EncodeTypes.Code128))
{
    // Set graphic unit
    builder.GraphicsUnit = System.Drawing.GraphicsUnit.Pixel;

    // Call GetMinimumBarCodeSize method to get the minimum size required
    System.Drawing.SizeF minSize = builder.GetMinimumBarCodeSize();

    // Set Auto size to false
    builder.AutoSize = false;

    // Set image height & width with the help of min size got from GetMinimumBarCodeSize method
    builder.ImageWidth = minSize.Width;
    builder.ImageHeight = minSize.Height;

    // Save the barcode image
    using (System.Drawing.Bitmap image = builder.BarCodeImage)
        image.Save("minimumresult.png");
}
```

## Enhancements

The following issues have been fixed in this release.

*   Functionality of GetOnlyBarCodeImage method has been improved. The working of GetOnlyBarCodeImage method with a small size has been enhanced.

To view the complete list of new features and fixes, please visit the [release notes][1] page. You can download the latest version by visiting the [Aspose.BarCode for Reporting Services 17.7][2] page in the downloads section.

## Aspose.BarCode for Reporting Services Resources

The following resources will help you work with Aspose.BarCode for SSRS:

*   [Homepage for Aspose.BarCode for SSRS API][3]
*   [Download Aspose.BarCode for SSRS][4]
*   [Aspose.BarCode for SSRS Wiki docs][5] – Help documentation and API reference documents.
*   [Aspose.BarCode Product Family Forum][6] – Post your technical questions and queries, or any other problem you faced while running Aspose.BarCode APIs.
*   [Enable Email Subscription][7] – You can keep yourself updated with the latest news on Aspose.BarCode APIs and new features, fixes, plus other API related topics by subscribing to Aspose.BarCode blog.




[1]: https://docs.aspose.com/display/barcodereportingservices/Aspose.BarCode+for+Reporting+Services+17.7+Release+Notes
[2]: http://www.aspose.com/downloads/barcode/reportingservices
[3]: https://www.aspose.com/products/barcode/reporting-services
[4]: https://downloads.aspose.com/barcode/reportingservices
[5]: https://docs.aspose.com/display/barcodereportingservices/Home
[6]: https://forum.aspose.com/c/barcode
[7]: https://blog.aspose.com/category/aspose-products/aspose-barcode-product-family/





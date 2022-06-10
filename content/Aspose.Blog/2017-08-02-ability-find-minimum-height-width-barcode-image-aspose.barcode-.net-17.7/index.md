---
title: 'Find Out Minimum Height and Width of Barcode using C#'
date: Wed, 02 Aug 2017 17:52:13 +0000
draft: false
url: /2017/08/02/ability-find-minimum-height-width-barcode-image-aspose.barcode-.net-17.7/
author: Ikram Haq
summary: ''
tags: []
categories: ['Aspose.BarCode Product Family']
---



{{< figure align=center src="images/aspose-Barcode-for-net_100.png" alt="Aspose.Barcode for .NET">}}


We are pleased to announce the release of Aspose.Barcode for .NET 17.7. The major development in this release is the support to [get minimum barcode image size][1]. Improved functionality of GetOnlyBarCodeImage method has also been incorporated in this release.

## Get Minimum BarCode Size using C#

Aspose.BarCode now supports the functionality to [get the minimum height & width required for a barcode image][2]. How a developer can get the minimum size (height & width) required for a barcode image is very simple and is demonstrated in the code snippet given below. The code snippet contains comments that makes it self explanatory.

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

This month’s release also includes enhancements. Details about the enhancements are listed below.

*   Functionality of GetOnlyBarCodeImage method has been improved. The working of GetOnlyBarCodeImage method with small size has been enhanced.

To view a complete list of new features and fixes, please visit the [release notes][3] page. You can download the latest version by visiting the [Aspose.Barcode for .NET 17.7][4] page in downloads section.

## Aspose.BarCode for .NET Resources

You can get started with Aspose.BarCode for .NET by making use of information available in the following:

*   [Homepage for Aspose.BarCode for .NET API][5]
*   [Download Aspose.BarCode for .NET][6]
*   [Aspose.BarCode for .NET Wiki docs][7] – Help documentation and API reference documents.
*   [Aspose.BarCode Product Family Forum][8] – Post your technical questions and queries, or any other problem you faced while running Aspose.BarCode APIs.
*   [Enable Email Subscription][9] – You can keep yourself updated with the latest news on Aspose.BarCode APIs, new features, fixes and other API related topics by subscribing to Aspose.BarCode blog.
*   [Aspose.BarCode for .NET Examples][10] – We have published our code examples on the social coding website GitHub.com. You can explore the code examples for learning purposes.




[1]: https://docs.aspose.com/display/barcodenet/Saving+Barcode+Image
[2]: https://docs.aspose.com/display/barcodenet/Saving+Barcode+Image
[3]: https://docs.aspose.com/display/barcodenet/Aspose.BarCode+for+.NET+17.7+Release+Notes
[4]: http://www.aspose.com/community/files/51/.net-components/aspose.barcode-for-.net/default.aspx
[5]: https://www.aspose.com/products/barcode/net
[6]: https://downloads.aspose.com/barcode/net
[7]: https://docs.aspose.com/display/barcodenet/Home
[8]: https://forum.aspose.com/c/barcode
[9]: https://blog.aspose.com/
[10]: https://github.com/aspose-barcode/Aspose.BarCode-for-.NET





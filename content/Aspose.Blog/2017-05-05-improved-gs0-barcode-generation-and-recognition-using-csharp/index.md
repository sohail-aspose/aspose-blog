---
title: 'Improved GS0 Barcode Generation And Recognition using C#'
date: Fri, 05 May 2017 05:48:28 +0000
draft: false
url: /2017/05/05/improved-gs0-barcode-generation-and-recognition-using-csharp/
author: Ikram Haq
summary: ''
tags: []
categories: ['Aspose.BarCode Product Family']
---



{{< figure align=center src="images/aspose-Barcode-for-net_100.png" alt="Aspose.Barcode for .NET 17.4">}}


We are pleased to announce the next release of [Aspose.Barcode for .NET][1] 17.4. The major development in this release is the improved functionality of GS1 coded barcode. Many times GS1 code texts contain complex combinations of digits and letters. The functionality of the GS1 barcode has been upgraded in such a way that it can parse and validate those complex combinations. The functionality of QR coded barcode recognition has also been improved and incorporated in this release.

## Improved API to Work With GS1 Barcode

Aspose.BarCode for .NET allows developers to generate GS1 coded barcode according to AI **(Application Identifier)** specifications. Checksum calculation and validation for many AI specifications have been implemented. For example, consider code text **“(703)123”**, which is an incorrect code text (ref: 703 AI, with letters - 324a, with more than 4 symbols). Aspose.BarCode will throw the following exception if the user tries to generate the barcode with **EncodeTypes** as **GS1Code128**. The following exception message will be displayed for such an incorrect barcode.

### Exception Message:

Wrong format of GS1 Code128 input string.

## Enhanced QR Barcode Working

Algorithm to detect **QR** coded barcode has been improved. Its targets detection logic has been updated. **QR** coded barcode can now be detected in combination with **MaxQuality** mode for better accuracy. This is as illustrated in the following code sample.

```
//Initialize reader object
using (BarCodeReader reader = new BarCodeReader("sample_QR_barcode.bmp", DecodeType.QR))
{
    // Set recognition mode to MaxQuality
    reader.RecognitionMode = RecognitionMode.MaxQuality;

    // Read the barcode
    while (reader.Read())
    {
        // print output
        Console.WriteLine("{0}:{1}", reader.GetCodeType(), reader.GetCodeText());
    }
}
```

## Enhancements

This month’s release also includes few bug fixes that were reported by our customers in the previous release. Details about these fixes are listed below.

*   Recognition process of QR barcode in MaxBarCodes mode has been improved.
*   Functionality of ExportToXml method has been improved. ExportToXml method now export dimension properties along with other properties of the newly define barcode into XML file.

To view a complete list of new features and fixes, please visit the [release notes][2] page. You can download the latest version by visiting the [Aspose.Barcode for .NET 17.4][3] page in downloads section.

## Aspose.BarCode for .NET Resources

You can get started with Aspose.BarCode for .NET by making use of information available in the following:

*   [Homepage for Aspose.BarCode for .NET API][4]
*   [Download Aspose.BarCode for .NET][5]
*   [Aspose.BarCode for .NET docs][6] – Help documentation and API reference documents.
*   [Aspose.BarCode Product Family Forum][7] – Post your technical questions and queries, or any other problem you faced while running Aspose.BarCode APIs.
*   [Enable Email Subscription][8] – You can keep yourself updated with the latest news on Aspose.BarCode APIs, new features, fixes and other API related topics by subscribing to Aspose.BarCode blog.
*   [Aspose.BarCode for .NET Examples][9] – We have published our code examples on the social coding website GitHub.com. You can explore the code examples for learning purposes.




[1]: https://products.aspose.com/barcode/net
[2]: https://docs.aspose.com/barcode/net
[3]: http://www.aspose.com/community/files/51/.net-components/aspose.barcode-for-.net/default.aspx
[4]: https://products.aspose.com/barcode/net
[5]: https://downloads.aspose.com/barcode/net
[6]: https://docs.aspose.com/barcode/net
[7]: https://forum.aspose.com/c/barcode
[8]: https://blog.aspose.com/
[9]: https://github.com/aspose-barcode/Aspose.BarCode-for-.NET





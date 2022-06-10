---
title: 'Apply Codabar Checksum Validation using C# with Aspose.BarCode for .NET 17.03'
date: Tue, 04 Apr 2017 20:42:38 +0000
draft: false
url: /2017/04/04/codabar-checksum-validation-aspose.barcode-.net-17.03/
author: Ikram Haq
summary: ''
tags: []
categories: ['Aspose.BarCode Product Family']
---



{{< figure align=center src="images/aspose-Barcode-for-net_100.png" alt="">}}


We are pleased to announce the release of [Aspose.Barcode for .NET][1] 17.03. The major development in this release is the support to [apply checksum validation on Codabar][2] coded barcode. Functionality to [get barcode text along with checksum value in a single call][3] has also been incorporated in this release.

## Applying Checksum Validation On Codabar

Aspose.BarCode for .NET allows developers to [apply checksum validation on Codabar][4]. The API now exposes the CodabarChecksumMode enumeration to specify the checksum mode. EnableChecksum property of the BarCodeBuilder class is needed to be set to TRUE before setting the checksum mode. This is as illustrated in the following code sample.

```
// The path to the documents directory.
string dataDir = RunExamples.GetDataDir_ManageBarCodes();

//Generation
//Instantiate BarCodeBuilder object
Aspose.BarCode.BarCodeBuilder builder = new Aspose.BarCode.BarCodeBuilder();

//Set the Code text for the barcode
builder.CodeText = "1234567890";

//Set the symbology type to Code128
builder.EncodeType = Aspose.BarCode.Generation.EncodeTypes.Codabar;

//Set the EnableChecksum property to yes
builder.EnableChecksum = Aspose.BarCode.EnableChecksum.Yes;

//Set the CodabarChecksumMode
builder.CodabarChecksumMode = Aspose.BarCode.CodabarChecksumMode.Mod10;

//Save the image on the system
builder.Save("Codabar_Mod10.png");

//Recognition
//Initialize reader object
using (Aspose.BarCode.BarCodeRecognition.BarCodeReader reader = new Aspose.BarCode.BarCodeRecognition.BarCodeReader("Codabar_Mod10.png", Aspose.BarCode.BarCodeRecognition.DecodeType.Codabar))
{
    //Set ChecksumValidation property of the reader to On
    reader.ChecksumValidation = Aspose.BarCode.BarCodeRecognition.ChecksumValidation.On;
    while (reader.Read())
    {
        //Get code text
        Console.WriteLine("{0}:{1}", reader.GetCodeType(), reader.GetCodeText());

        //Get checksum value
        Console.WriteLine("Checksum:" + reader.GetCheckSum());
    }
}
```

## Get Barcode With Checksum Value

Aspose.BarCode for .NET allows developers to [get barcode text along with checksum value][5]. Aspose.BarCode API now exposes an overloaded method GetCodeText of the BarCodeReader class to accomplish the task. This is illustrated in the following code sample.

```
//Initialize reader object
using (Aspose.BarCode.BarCodeRecognition.BarCodeReader reader = new Aspose.BarCode.BarCodeRecognition.BarCodeReader("error5.jpg", Aspose.BarCode.BarCodeRecognition.DecodeType.EAN13))
{
    while (reader.Read())
    {
        //Get code text by passing TRUE to get the Barcode along with checksum value
        Console.WriteLine("{0}: {1}", reader.GetCodeType(), reader.GetCodeText(true));
    }
}
```

## Enhancements

This month’s release also includes several bug fixes that were reported by our users in the previous release. Details about these fixes and improvements are listed below.

*   Process of reading GS1DataMatrix barcode has been improved.
*   Process of reading Code39Standard barcode has been improved.
*   Recognition process of DutchKIX barcode in MaxBarCodes mode has been improved.
*   Processing of GS1DataMatrix barcode generation has been improved.

To view a complete list of new features and fixes, please visit the [release notes][6] page. You can download the latest version by visiting the [Aspose.Barcode for .NET 17.03][7] page in downloads section.

## Aspose.BarCode for .NET Resources

The resources, you may need to accomplish your tasks:

*   [Homepage for Aspose.BarCode for .NET API][8]
*   [Download Aspose.BarCode for .NET][9]
*   [Aspose.BarCode for .NET docs][10] – Help documentation and API reference documents.
*   [Aspose.BarCode Product Family Forum][11] – Post your technical questions and queries, or any other problem you faced while running Aspose.BarCode APIs.
*   [Enable Email Subscription][12] – You can keep yourself updated with the latest news on Aspose.BarCode APIs, new features, fixes and other API related topics by subscribing to Aspose.BarCode blog.
*   [Aspose.BarCode for .NET Examples][13] – We have published our code examples on the social coding website GitHub.com. You can explore the code examples for learning purposes.




[1]: https://products.aspose.com/barcode/net
[2]: https://docs.aspose.com/barcode/net/use-checksum-and-supplement-data/#applying-checksum-validation-on-codabar
[3]: https://docs.aspose.com/barcode/net/use-checksum-and-supplement-data/#get-barcode-with-checksum-value
[4]: https://docs.aspose.com/barcode/net/use-checksum-and-supplement-data/#applying-checksum-validation-on-codabar
[5]: https://docs.aspose.com/barcode/net/use-checksum-and-supplement-data/#get-barcode-with-checksum-value
[6]: https://docs.aspose.com/barcode/net/aspose-barcode-for-net-17-03-release-notes/
[7]: https://downloads.aspose.com/barcode/net
[8]: https://products.aspose.com/barcode/net/
[9]: https://downloads.aspose.com/barcode/net
[10]: https://docs.aspose.com/barcode/net/
[11]: https://forum.aspose.com/c/barcode
[12]: https://blog.aspose.com/
[13]: https://github.com/aspose-barcode/Aspose.BarCode-for-.NET





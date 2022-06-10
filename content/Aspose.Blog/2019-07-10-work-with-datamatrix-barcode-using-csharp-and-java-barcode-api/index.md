---
title: 'Enhancements for DataMatrix Barcode using Aspose.BarCode 19.5'
date: Wed, 10 Jul 2019 15:34:40 +0000
draft: false
url: /2019/07/10/work-with-datamatrix-barcode-using-csharp-and-java-barcode-api/
author: Ahsaniqbal
summary: ''
tags: []
categories: ['Aspose.BarCode Product Family']
---



{{< figure align=center src="images/aspose-BarCode-for-Java_100-grey.png" alt="">}}


Here comes the new release Aspose.BarCode 19.5 for [Java][1] and [.NET][2]/) containing a lot of enhancements. This time we have targetted the DataMatrix barcode reading and IMB barcode recognition. For detailed information about the enhancements in this release follow the release notes for [Java][3] and [.NET][4]. Let us have a look at what is new there in this release.

## Enhancements

As usual, we have put a lot of effort into bringing our product to exceed customer satisfaction. There were a few shortcomings that were observed while working with the library. Enhancements are done to tackle all these shortcomings and the new version is far better for handling these situations.

### Upgradations while Reading the DataMatrix Barcode

Reading a barcode is quite tricky and sometimes the minutest dots can result in wrong values. Similarly, we observed issues in reading the DataMatrix barcode from a 200 DPI TIFF image. This issue was investigated in detail and all the issues are handled now as follows:

*   We have supported the recognition if invasion in the quite zones of data matrix.
*   Resolved the issues incurred due to low scanner resolution which produces lot of errors.
*   Effort is made to recognise black dots around the barcode.
*   Irregular grids were also causing issues. We have identified them and these are no more an issue now.
*   There were some problems in the bits in the data matrix recognition which is sorted out and results are amazing now.

### Barcode Recognized on Low-Resolution TIFF

This is very common that we come across barcodes in tiff formats that have very low resolutions. In this case, sometimes we may get garbled data out of these barcodes. An in-depth investigation is done in this regard and a new public property AllowOneDWipedBarsRestoration has been added to the QualitySettings. It allows the engine for 1D barcodes to recognize barcodes with single wiped/glued bars in pattern. Property is enabled by default in HighQuality, MaxBarCodes modes. Currently the property is used for Code128, GS1Code128, SCC14, EAN14, SSCC18, AustralianPosteParcel, SwissPostParcel barcode types. To use this feature, just set this property to true while reading the barcode from TIFF image as follows:

```
reader.QualitySettings.AllowOneDWipedBarsRestoration = true;
```

## Other Enhancements

*   IMB barcodes were failing sometimes to be recognized. Enhancements are done to overcome this issue.
*   There was a need to enhance the recognition capability in .NET Core environment, which is also done successfully.

## Aspose.BarCode for Java/.NET Resources

You may visit the following links for documentation, source code, API reference, and other details of this product.

*   [Aspose.BarCode for Java][5]
*   [Aspose.BarCode for .NET][6]

Similarly, for downloading this version using NuGet package manager visit [here][7] and for Java user it is available on [Maven][8] also.




[1]: https://downloads.aspose.com/barcode/java/new-releases/aspose.barcode-for-java-19.5/
[2]: https://downloads.aspose.com/barcode/net/new-releases/aspose.barcode-for-.net-19.5-(dlls-only
[3]: https://docs.aspose.com/display/barcodejava/Aspose.BarCode+for+Java+19.5+Release+Notes
[4]: https://docs.aspose.com/display/barcodenet/Aspose.BarCode+for+.NET+19.5+Release+Notes
[5]: https://products.aspose.com/barcode/java
[6]: https://products.aspose.com/barcode/net
[7]: https://www.nuget.org/packages/Aspose.BarCode/19.5.0
[8]: https://repository.aspose.com/repo/com/aspose/aspose-barcode/19.5/





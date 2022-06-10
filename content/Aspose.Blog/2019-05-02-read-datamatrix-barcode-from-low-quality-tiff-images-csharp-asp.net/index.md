---
title: 'Read Data Matrix Barcode from Low-Quality​ TIFF Images with Aspose.BarCode 19.4.0'
date: Thu, 02 May 2019 13:36:09 +0000
draft: false
url: /2019/05/02/read-datamatrix-barcode-from-low-quality-tiff-images-csharp-asp.net/
author: Ahsaniqbal
summary: ''
tags: []
categories: ['Aspose.BarCode Product Family']
---



{{< figure align=center src="images/aspose-BarCode-for-JasperReports_100.png" alt="Aspose.BarCode for JasperReports">}}


So, you want to know what is new there in the latest Aspose.BarCode release. Pleasure is mine to share the details about the latest release Aspose.BarCode 19.4.0. You will find enhancements providing a rich experience while using this product with a variety of barcodes used nowadays. A summary of details about all the upgrades in this release can be reviewed [here][1]. Let us start exploring this new release. Are you ready?

As you know barcode reading is quite a complex task as a lot of issues can be there in the barcodes (especially received via Fax), like slim white modules, invasion of the quiet zone, small modules (1-2px), broken time pattern, incorrect bits location and a ragged border of the l-time pattern. Remember that there is a limit for any barcode reader to read an image and may have difficulties to read images with a lot of blurs or too poor image quality. Don't you think so? Also, it was possible to read such barcodes by adding clear whitespace around the barcode but this workaround was not practical in all the cases due to extra effort and process involvement. We have worked hard on these issues and have improved our library a lot to handle all the above-mentioned issues and can read most of such barcodes.

## Read DataMatrix Barcode in C#

The following code sample shows how to read data matrix barcode with high performance:

{{< gist aspose-com-gists f801733f5eb53b0777dd38da9db8366a "Examples-CSharp-ManageAndOptimizeBarcodeRecognition-DetectDecoratedDatamatrix-DetectDecoratedDatamatrix.cs" >}}

## Improvements

Following is a list of few improvements which are made in this release:

*   Detect region on an image with the heterogeneous brightness
*   Support recognition of invasion in the quiet zone for data matrix
*   Recognize data matrix with a lot of errors because of low scanner resolution
*   Recognize a DataMatrix with black dots around
*   Correct the bits in DataMatrix recognition
*   Identify cells of poor quality
*   IMB barcode was failing to be recognized. This issue is resolved and it works fine now like the following sample IMB barcode can be read.
*   There were some issues while detecting 1D and 2D barcode images in .NET Core environment due to some error while using Skia Graphics Library. Those issues are resolved now and you can read barcode images without any error.




[1]: https://docs.aspose.com/display/barcodenet/Aspose.BarCode+for+.NET+19.4+Release+Notes





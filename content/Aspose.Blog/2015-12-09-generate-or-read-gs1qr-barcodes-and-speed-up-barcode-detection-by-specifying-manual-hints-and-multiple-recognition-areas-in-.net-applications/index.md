---
title: 'Generate or read GS1QR barcodes and speed up barcode detection by specifying manual hints and multiple recognition areas in .NET applications'
date: Wed, 09 Dec 2015 06:03:41 +0000
draft: false
url: /2015/12/09/generate-or-read-gs1qr-barcodes-and-speed-up-barcode-detection-by-specifying-manual-hints-and-multiple-recognition-areas-in-.net-applications/
author: Muhammad Ijaz
summary: ''
tags: ['Muhammad Ijaz']
categories: ['Aspose.BarCode Product Family']
---

[![][1]](https://blog.aspose.com/wp-content/uploads/sites/2/2013/07/aspose-Barcode-for-net_100.png) We are pleased to announce the release of Aspose.Barcode for .NET 7.5.0. This release supports encoding and decoding GS1QR barcodes, and specifying manual hints and multiple recognition areas to speed up the recognition process.

## Speed up barcode recognition process using manual hints

Aspose.Barcode for .NET allows you to specify manual hints and speed up recognition process. BarCodeReader.ManualHints property can be set to appropriate ManualHint enumeration value e.g.

```
 Stopwatch watch = new Stopwatch();
string filename = @"Barcode.jpg";
using (BarCodeReader reader = new BarCodeReader(filename, BarCodeReadType.DataMatrix))
{
	watch.Start();
	reader.RecognitionMode = RecognitionMode.ManualHints;
	reader.ManualHints = ManualHint.MedianSmoothing;

	while (reader.Read())
	{
		Console.WriteLine(reader.GetReadType() + ": " + reader.GetCodeText());
	}
	watch.Stop();
	Console.WriteLine("Time: " + watch.ElapsedMilliseconds + "ms.");
} 
```

## Read barcodes from multiple regions

Aspose.Barcode for .NET allows you to read barcodes from certain regions of the images. A new constructor of BarCodeReader class has been introduced with accepts a list of rectangles to read barcodes from those rectangular areas only e.g.

```
 Bitmap bitmap = new Bitmap("Three_Barcodes.png");

Rectangle[] areas = new Rectangle[3];
areas[0] = new Rectangle (50, 50, 300, 300);
areas[1] = new Rectangle (400, 40, 350, 350);
areas[2] = new Rectangle (40, 500, 700, 150);

using (BarCodeReader reader = new BarCodeReader(bitmap, areas, BarCodeReadType.AllSupportedTypes))
{
	while (reader.Read())
	{
		Console.WriteLine(reader.GetReadType() + ": " + reader.GetCodeText());
	}
} 
```

## Enhancements

Following is a list of improvements included in this release.

*   Support encoding GS1QR code
*   Remove unwanted white space from the bottom of barcode image
*   Reorganize the logic of recognition in manual hint mode to speed up the detection
*   Improve encoding GS1DataMatrix
*   Improve encoding GS1Code128
*   Improve reading Aztec code from the JPG images
*   Improve barcode reading
*   Implement a BarCodeReader constructor that accepts a list of rectangles

To view a complete list of new features and fixes and to download the latest release, please visit [Aspose.Barcode for .NET 7.5.0 page in downloads section][2].

## Aspose.BarCode for .NET Resources

The resources, you may need to accomplish your tasks:

*   [Homepage for Aspose.BarCode for .NET API][3]
*   [Download Aspose.BarCode for .NET][4]
*   Aspose.BarCode for .NET Wiki docs – Help documentation and API reference documents.
*   [Aspose.BarCode Product Family Forum][5] – Post your technical questions and queries, or any other problem you faced while running Aspose.BarCode APIs.
*   [Enable Email Subscription][6] – Don’t limit yourself, you can keep yourself updated with the latest news on Aspose.BarCode APIs and new features, fixes, plus other API related topics by subscribing to Aspose.BarCode blog.
*   [Aspose.BarCode for .NET Examples][7] – We have published our code examples on the social coding website GitHub.com. Anyone can explore the code examples for learning purposes.




[1]: https://blog.aspose.com/wp-content/uploads/sites/2/2013/07/aspose-Barcode-for-net_100.png "Aspose.BarCode for .NET logo"
[2]: http://www.aspose.com/community/files/51/.net-components/aspose.barcode-for-.net/default.aspx
[3]: https://products.aspose.com/barcode
[4]: http://www.aspose.com/community/files/51/.net-components/aspose.barcode-for-.net/default.aspx
[5]: http://www.aspose.com/community/forums/aspose.barcode-product-family/193/showforum.aspx
[6]: https://blog.aspose.com/
[7]: https://github.com/asposebarcode/Aspose_BarCode_NET





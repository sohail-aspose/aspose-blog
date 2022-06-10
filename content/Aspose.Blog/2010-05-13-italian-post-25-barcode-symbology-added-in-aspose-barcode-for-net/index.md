---
title: 'Italian Post 25 barcode symbology added in Aspose.BarCode for .NET'
date: Thu, 13 May 2010 20:05:00 +0000
draft: false
url: /2010/05/13/italian-post-25-barcode-symbology-added-in-aspose-barcode-for-net/
author: Saqib Razzaq
summary: ''
tags: []
categories: ['Aspose.BarCode Product Family']
---

We have recently released a new version of Aspose.BarCode for .NET 3.4. It supports both generation and recognition of Italian Post 25 barcodes. Now, you can also specify a rectangular region within the image for barcode scanning. This is useful and more efficient in case you have a large size image and the barcode is placed at a specific location that you already know.  
  

BarCodeReader reader = new BarCodeReader(new Bitmap("test.png"), new Rectangle(0, 0, 300, 300), BarCodeReadType.Pdf417);  
while (reader.Read())  
{  
      Console.WriteLine("Codetext found: " + reader.GetCodeText());  
}  
reader.Close();

  
Some bugs were also fixed in this release.  
  
For release notes and download, please visit [http://www.aspose.com/community/files/51/.net-components/aspose.barcode-for-.net/default.aspx][1].




[1]: http://www.aspose.com/community/files/51/.net-components/aspose.barcode-for-.net/default.aspx





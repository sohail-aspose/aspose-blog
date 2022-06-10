---
title: 'Improved Barcode Recognition Performance in Aspose.BarCode for .NET 3.9'
date: Fri, 28 Jan 2011 19:16:00 +0000
draft: false
url: /2011/01/28/improved-barcode-recognition-performance-in-aspose-barcode-for-net-3-9/
author: Saqib Razzaq
summary: ''
tags: []
categories: ['Aspose.BarCode Product Family']
---

We are pleased to announce a new version of Aspose.BarCode for .NET v3.9. It now supports exclusive locking of the barcode image, which can result in improved barcode recognition performance for large sized images.

  

BarCodeReader reader = new BarCodeReader(image, BarCodeReadType.Code128);  
// Acquire an exclusive lock on the image  
reader.SetHints(RecognitionHints.ImageAccessHints.Exclusive);  
while (reader.Read() == true)  
{  
      Console.WriteLine("Codetext: " + reader.GetCodeText());  
}  
reader.Close();

  

For release notes and download, please visit [http://www.aspose.com/community/files/51/.net-components/aspose.barcode-for-.net/default.aspx][1].




[1]: http://www.aspose.com/community/files/51/.net-components/aspose.barcode-for-.net/default.aspx





---
title: 'Aztec Barcode Recognition Support Added in Aspose.BarCode for .NET 3.6.1'
date: Mon, 02 Aug 2010 17:44:00 +0000
draft: false
url: /2010/08/02/aztec-barcode-recognition-support-added-in-aspose-barcode-for-net-3-6-1/
author: Saqib Razzaq
summary: ''
tags: []
categories: ['Aspose.BarCode Product Family']
---

We have just released Aspose.BarCode for .NET hotfix v3.6.1. It supports reading Aztec barcodes. Sample code:

  

// read or decode Aztec barcode  
BarCodeReader reader = new BarCodeReader("aztec.png", BarCodeReadType.Aztec);  
while (reader.Read() == true)  
{  
// display the detected codetext  
      Console.WriteLine("Codetext: " + reader.GetCodeText());  
}  
// close the reader  
reader.Close();

  

Some bugs were also fixed in this hotfix. For release notes and download, please visit [http://www.aspose.com/community/files/51/.net-components/aspose.barcode-for-.net/default.aspx][1].




[1]: http://www.aspose.com/community/files/51/.net-components/aspose.barcode-for-.net/default.aspx





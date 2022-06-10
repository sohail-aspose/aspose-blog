---
title: 'OPC and Leitcode Barcodes Support Now Available in Aspose.BarCode for .NET 4.0'
date: Tue, 26 Apr 2011 01:32:11 +0000
draft: false
url: /2011/04/26/opc-and-leticode-barcodes-support-now-available-in-aspose.barcode-for-.net-4.0/
author: Saqib Razzaq
summary: ''
tags: []
categories: ['Aspose.BarCode Product Family']
---

We are pleased to announce the release of a new version of Aspose.BarCode for .NET 4.0. In this version, we added support for OPC and Deutsche Post Leitcode barcode symbologies. You can generate as well as recognize both of these symbologies. // Create OPC barcode  
BarCodeBuilder builder = new BarCodeBuilder(strCodetext, Symbology.OPC);  
// Save the barcode to stream  
MemoryStream imgStream = new MemoryStream();  
builder.Save(imgStream, ImageFormat.Png);  
imgStream.Position = 0;  
  
// Read OPC barcode  
BarCodeReader reader = new BarCodeReader(imgStream, BarCodeReadType.OPC);  
while (reader.Read())  
{  
Console.WriteLine("codetext: " + reader.GetCodeText());  
Console.WriteLine("Orientation" + orientation.ToString());  
}  
reader.Close();  
  
For release notes and download, please visit [http://www.aspose.com/community/files/51/.net-components/aspose.barcode-for-.net/default.aspx][1].




[1]: http://www.aspose.com/community/files/51/.net-components/aspose.barcode-for-.net/default.aspx





---
title: 'EMF Image Format Now Supported in Aspose.BarCode for .NET'
date: Mon, 25 Oct 2010 10:04:00 +0000
draft: false
url: /2010/10/25/emf-image-format-now-supported-in-aspose-barcode-for-net/
author: Saqib Razzaq
summary: ''
tags: []
categories: ['Aspose.BarCode Product Family']
---

We are pleased to announce the release of Aspose.BarCode for .NET v3.7. In this version, we added support of saving barcode images in EMF format (Vector graphics). 

  

Sample code for generating and saving the barcode in EMF format:

// Initialize barcode builder  
BarCodeBuilder builder = new BarCodeBuilder("test-123", Symbology.Code128);  
// Save barcode image in EMF format  
builder.SaveAsEmf("test.emf");

  

We also introduced generation of two new barcode symbologies (Royal Mail 4-state Customer Code and Vehicle Identification Number). Some bug fixes were also included.

  

For release notes and download, please visit [http://www.aspose.com/community/files/51/.net-components/aspose.barcode-for-.net/default.aspx][1].




[1]: http://www.aspose.com/community/files/51/.net-components/aspose.barcode-for-.net/default.aspx





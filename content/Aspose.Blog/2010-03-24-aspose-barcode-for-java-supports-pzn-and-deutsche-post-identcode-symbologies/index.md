---
title: 'Aspose.BarCode for Java supports PZN and Deutsche Post Identcode symbologies'
date: Wed, 24 Mar 2010 23:00:00 +0000
draft: false
url: /2010/03/24/aspose-barcode-for-java-supports-pzn-and-deutsche-post-identcode-symbologies/
author: Saqib Razzaq
summary: ''
tags: []
categories: ['Aspose.BarCode Product Family']
---

We just released a new version of Aspose.BarCode for Java 2.0.0. It supports generation and recognition of PZN and Deutsche Post Identcode symbology types.  
  
A new class has also been added to generate Code128 barcodes with user defined codeset patterns. Sample code is given below:  
  

Code128CodeBuilder builder = new Code128CodeBuilder(Code128Set.A);  
String codeText = builder.Append("1234").Switch(Code128Set.B).Append("5678").toString();  
BarCodeBuilder b = new BarCodeBuilder(Symbology.CODE128, codeText);  
b.setCode128Set(Code128Set.Customized);  
String file = "code128.png";  
b.save(file);

  
For release notes and download, please visit [http://www.aspose.com/community/files/72/java-components/aspose.barcode-for-java/default.aspx][1].




[1]: http://www.aspose.com/community/files/72/java-components/aspose.barcode-for-java/default.aspx





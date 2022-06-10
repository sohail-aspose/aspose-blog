---
title: 'Adding Checksum Validation On Codabar with Aspose.BarCode for Java 17.3'
date: Wed, 03 May 2017 04:16:11 +0000
draft: false
url: /2017/05/03/adding-checksum-validation-codabar-aspose.barcode-java-17.03/
author: Ikram Haq
summary: ''
tags: []
categories: ['Aspose.BarCode Product Family']
---

[](https://www.aspose.com/products/barcode/java)We are pleased to announce the release of Aspose.Barcode for Java 17.3. This month’s release provides the capability to [add checksum validation on Codabar][1] coded barcode. An enhancement has also been made in this version to control fake/additional recognition of DutchKIX while MaxBarCodes mode is applied. Other than above mentioned new features, the API also fixes several bugs reported in the last version by the customers.

## Adding Checksum Validation On Codabar

Aspose.BarCode for Java allows developers to [add checksum validation on Codabar][2] barcode. The API now exposes the CodabarChecksumMode enumeration to specify the checksum mode. BarCodeBuilder class has a property setEnableChecksum that needs to be set to **TRUE** before setting the checksum mode. Following code illustrates how to set this property and use the checksum enumeration.

```
 //Generation
//Instantiate BarCodeBuilder object
com.aspose.barcode.BarCodeBuilder builder = new com.aspose.barcode.BarCodeBuilder();
        
//Set the Code text for the barcode
builder.setCodeText("1234567890");
        
//Set the symbology type to CodaBar
builder.setEncodeType(com.aspose.barcode.EncodeTypes.CODABAR);
        
//Set the EnableChecksum property to yes
builder.setEnableChecksum(com.aspose.barcode.EnableChecksum.Yes);
        
//Set the CodabarChecksumMode
builder.setCodabarChecksumMode(com.aspose.barcode.CodabarChecksumMode.Mod10);
        
//Save the image on the system
builder.save("Codabar_Mod10.png");

//Recognition
//Initialize reader object
BarCodeReader reader = new BarCodeReader("Codabar_Mod10.png", com.aspose.barcode.barcoderecognition.DecodeType.CODABAR);
        
//Set ChecksumValidation property of the reader to On
reader.setChecksumValidation(com.aspose.barcode.barcoderecognition.ChecksumValidation.On);
while (reader.read())
{
      //Get code text
      System.out.println(" codetext: " + reader.getCodeText());
            
      //Get type of barcode
      System.out.println(" type: " + reader.getCodeType());
            
      //Get checksum value
      System.out.println(" Checksum: " + reader.getCheckSum());
} 
```

## Enhancements

Complete list of enhancements and fixes in this release is as follows.

*   Functionality to recognize barcode with checksum has been improved.
*   New changes have been incorporated into the detection algorithm to read GS1DataMatrix barcode.
*   Improved the functionality to not detect fake/additional DutchKIX coded barcode.
*   GS1DataMatrix barcode generation algorithm has been updated generate much more clear tt>GS1DataMatrix barcode image.

To view a complete list of new features, fixes and to download the latest release, please visit [Aspose.Barcode for Java 17.3][3] page in downloads section.

## Aspose.BarCode for Java Resources

The following API resources can be of help to you in getting started with Aspose.BarCode:

*   [Homepage for Aspose.BarCode for Java API][4]
    
*   [Download Aspose.BarCode for Java][5]
    
*   [Aspose.BarCode for Java Wiki docs][6] - help documentation and API reference documents.
    
*   [Aspose.BarCode Product Family Forum][7] - post your technical questions and queries, or any other problem you faced while running Aspose.BarCode APIs.
    
*   [Enable Email Subscription][8] - Don't limit yourself, you can keep yourself updated with the latest news on Aspose.BarCode APIs and new features, fixes, plus other API related topics by subscribing to Aspose.BarCode blog.
    
*   [Aspose.BarCode for Java Examples][9] - We have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: https://docs.aspose.com/display/barcodejava/Applying+Checksum+Validation+On+OneCode+And+AustraliaPost+Barcodes#ApplyingChecksumValidationOnOneCodeAndAustraliaPostBarcodes-ApplyingChecksumValidationOnCodabar
[2]: https://docs.aspose.com/display/barcodejava/Applying+Checksum+Validation+On+OneCode+And+AustraliaPost+Barcodes#ApplyingChecksumValidationOnOneCodeAndAustraliaPostBarcodes-ApplyingChecksumValidationOnCodabar
[3]: http://www.aspose.com/downloads/barcode/java
[4]: https://www.aspose.com/products/barcode/java
[5]: https://downloads.aspose.com/barcode/java
[6]: https://docs.aspose.com/display/barcodejava/Home
[7]: https://forum.aspose.com/c/barcode
[8]: https://blog.aspose.com/category/aspose-products/aspose-barcode-product-family/
[9]: https://github.com/aspose-barcode/Aspose.BarCode-for-Java





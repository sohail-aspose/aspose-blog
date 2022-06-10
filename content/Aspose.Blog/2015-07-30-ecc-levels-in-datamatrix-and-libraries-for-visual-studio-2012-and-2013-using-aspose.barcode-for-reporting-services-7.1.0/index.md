---
title: 'ECC Levels in DataMatrix and Libraries for Visual Studio 2012 and 2013 using Aspose.BarCode for Reporting Services 7.1.0'
date: Thu, 30 Jul 2015 20:53:34 +0000
draft: false
url: /2015/07/30/ecc-levels-in-datamatrix-and-libraries-for-visual-studio-2012-and-2013-using-aspose.barcode-for-reporting-services-7.1.0/
author: Imran Rafique
summary: ''
tags: ['Imran.Rafique']
categories: ['Aspose.BarCode Product Family']
---

[![Aspose.BarCode for SSRS icon][1]](https://blog.aspose.com/wp-content/uploads/sites/2/2013/08/aspose-BarCode-for-SSRS-e1377591419756.png)We're pleased to announce the new release version 7.1.0 of Aspose.BarCode for Reporting Services. The error correction levels are now supported in the DataMatrix symbology. Users can set an ECC level while encoding DataMatrix code. This new release has also included separate libraries for Visual Studio 2012 and 2013 configurations. We have fixed many other defects those leads to better performance in reading and writing codes.

## Set ECC Level While Writing DataMatrix Code

The DataMatrix symbology adopts two types of error correction algorithm, depending on the ECC level employed. The ECC levels 000 to 140, which offer five different error correction levels. However, the commonly used ECC 200 level uses Reed-Solomon error correction. Following help topic shows, how to write DataMatrix code along with the ECC algorithm: Select an ECC Level to Encode a Barcode.

## Visual Studio 2012 and 2013 Configurations

We have provided two separate libraries to manage configuration of Microsoft Visual Studio 2012 and 2013. Previously, users were facing an error while adding barcode control in the toolbox. It has now been fixed. These assemblies are located in the Bin\\VS2012 and Bin\\VS2013 directories. These assemblies can also be used with respective Business Intelligence for Visual Studio version.

We have enhanced encoding part of Code128 symbology. It was throwing an error while encoding FNC 3 character. Please check a list of key fixes that help us improve Aspose.BarCode APIs.

*   Fixed: Can't add barcode control in the toolbox of Visual Studio 2012 and 2013.
    
*   Fixed: Business Intelligence for Visual Studio 2013 - Can't preview barcode using Reporting Services 2014.
    
*   Fixed: Error message when tried to encode Code128 with FNC 3 character.
    

## Public API Changes

The following API changes in the new version are also worth noting:

*   The new DatamatrixECC property is added to the BarCodeBuilder class in order to select an appropriate ECC level while encoding DataMatrix barcode.
    
*   The new DataMatrixEccType Enum has been added to specify the type of the ECC to encode.
    

## Aspose.BarCode for SSRS Resources

The resources, you may need to accomplish your tasks:

*   [Homepage for Aspose.BarCode for SSRS APIs][2]
    
*   [Download Aspose.BarCode for SSRS][3]
    
*   Aspose.BarCode for SSRS Wiki docs - help documentation and API reference documents.
    
*   [Aspose.BarCode Product Family Forum][4] - post your technical questions and queries, or any other problem you faced while running Aspose.BarCode APIs.
    
*   [Enable Email Subscription][5] - Don't limit yourself, you can keep yourself updated with the latest news on Aspose.BarCode APIs and new features, fixes, plus other API related topics by subscribing to Aspose.BarCode blog.




[1]: https://blog.aspose.com/wp-content/uploads/sites/2/2013/08/aspose-BarCode-for-SSRS-e1377591419756.png "Aspose.BarCode for SSRS icon"
[2]: https://products.aspose.com/barcode
[3]: http://www.aspose.com/community/files/52/ssrs-rendering-extensions/aspose.barcode-for-reporting-services/default.aspx
[4]: http://www.aspose.com/community/forums/aspose.barcode-product-family/193/showforum.aspx
[5]: https://blog.aspose.com/





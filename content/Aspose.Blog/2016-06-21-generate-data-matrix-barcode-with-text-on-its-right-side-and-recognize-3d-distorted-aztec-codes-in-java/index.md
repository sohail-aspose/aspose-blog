---
title: 'Generate data matrix barcode with text on its right side and recognize 3D-distorted Aztec codes in Java'
date: Tue, 21 Jun 2016 08:09:04 +0000
draft: false
url: /2016/06/21/generate-data-matrix-barcode-with-text-on-its-right-side-and-recognize-3d-distorted-aztec-codes-in-java/
author: Muhammad Ijaz
summary: ''
tags: []
categories: ['Aspose.BarCode Product Family']
---

[![Aspose.BarCode for Java logo][1]](https://blog.aspose.com/wp-content/uploads/sites/2/2013/06/aspose-BarCode-for-Java_100.png)We are pleased to announce the release of Aspose.Barcode for Java 7.9.0. This release supports showing the code text on the right side of the barcode. A new algorithm has also been implemented which allows you to read 3D-distorted Aztec codes.

## Set the code text location to the right side of a barcode

Aspose.Barcode for Java allows you to set the code text location to the right side of the barcode. This is helpful in showing the code text on the right side of a data matrix barcode. **BarCodeBuilder.** **setCodeLocation** can be set to **CodeLocation.Right** e.g.

```
 BarCodeBuilder builder = new BarCodeBuilder(
"GTIN:898978777776665655
  UID: 121212121212121212
  Batch:GH768
  Exp.Date:150923", Symbology.DataMatrix);

builder.setCodeLocation(CodeLocation.Right);
builder.setMargins(new MarginsF(0,0,0,0));
//builder.setCodeTextSpace(0); // not recommended small space
builder.save("codetextRight.png"); 
```

## Enhancements

Following is a list of improvements included in this release.

*   Aztec codes recognition has been improved 
*   QR barcode recognition has been improved

To view a complete list of new features and fixes and to download the latest release, please visit [Aspose.Barcode for Java 7.8.0 page in downloads section][2].

## Aspose.BarCode for Java Resources

The resources, you may need to accomplish your tasks:

*   [Homepage for Aspose.BarCode for Java API][3]
*   [Download Aspose.BarCode for Java][4]
*   Aspose.BarCode for Java Wiki docs – Help documentation and API reference documents.
*   [Aspose.BarCode Product Family Forum][5] – Post your technical questions and queries, or any other problem you faced while running Aspose.BarCode APIs.
*   [Enable Email Subscription][6] – Don’t limit yourself, you can keep yourself updated with the latest news on Aspose.BarCode APIs and new features, fixes, plus other API related topics by subscribing to Aspose.BarCode blog.
*   [Aspose.BarCode for Java Examples][7] – We have published our code examples on the social coding website GitHub.com. Anyone can explore the code examples for learning purposes.




[1]: https://blog.aspose.com/wp-content/uploads/sites/2/2013/06/aspose-BarCode-for-Java_100.png "Aspose.BarCode for Java logo"
[2]: http://www.aspose.com/downloads/barcode/java
[3]: http://www.aspose.com/products/barcode/java
[4]: http://www.aspose.com/downloads/barcode/java
[5]: http://www.aspose.com/community/forums/aspose.barcode-product-family/193/showforum.aspx
[6]: https://blog.aspose.com/
[7]: https://github.com/aspose-barcode/Aspose.BarCode-for-Java





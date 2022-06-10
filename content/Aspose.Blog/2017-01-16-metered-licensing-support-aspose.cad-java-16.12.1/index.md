---
title: 'Metered licensing support in Aspose.CAD for Java 16.12.1'
date: Mon, 16 Jan 2017 08:56:21 +0000
draft: false
url: /2017/01/16/metered-licensing-support-aspose.cad-java-16.12.1/
author: Ikram Haq
summary: ''
tags: []
categories: ['Aspose.CAD Product Family']
---

We are pleased to announce that Aspose.CAD for Java 16.12.1 has been released. The major development in this release is support for metered license mechanism. The new licensing mechanism will be used along with existing licensing method. Those customers who want to be billed based on the usage of the API features can use the metered licensing.

## Metered Licensing

Aspose.CAD for Java provides the functionality to use metered licensing mechanism. We have introduced Metered class in API to accomplish this job. The following sample code will demonstrate, how to calculate the consumed CAD API requests.

```
 // Create an instance of OCR Metered class
com.aspose.cad.Metered metered = new com.aspose.cad.Metered();

// Access the setMeteredKey property and pass public and private keys as parameters
metered.setMeteredKey("", "");

// Get consumed qantity value before accessing API
double quantityOld = com.aspose.cad.Metered.getConsumptionQuantity();
System.out.println("Consumption quantity" + quantityOld);

// DO PROCESSING
//com.aspose.cad.fileformats.cad.CadImage image = 
//        (com.aspose.cad.fileformats.cad.CadImage)com.aspose.cad.Image.load("BlockRefDgn.dwg");


// Get consumed qantity value after accessing API
double quantity = com.aspose.cad.Metered.getConsumptionQuantity();
System.out.println("Consumption quantity" + quantity); 
```

## Enhancements

Following enhancements have been introduced in this release.

*   Process of loading DWG file has been improved.
    
*   Process of converting DWG to PDF format has been improved.
    
*   Process of converting DWG to PNG format in multithreading has been improved.
    

To view a complete list of new features and to download the latest release, please visit [Aspose.CAD for Java 16.12.1 page in downloads section][1].

## Aspose.CAD for Java Resources

The resources, you may need to accomplish your tasks:

*   [Homepage for Aspose.CAD for Java API][2]
*   [Download Aspose.CAD for Java][3]
*   [Aspose.CAD for Java Wiki Docs][4] – Help documentation
*   [Aspose.CAD Product Family Forum][5] – Post your technical questions and queries, or any other problem you faced while running Aspose.CAD APIs.
*   [Enable Email Subscription][6] – Don’t limit yourself, you can keep yourself updated with the latest news on Aspose.CAD APIs and new features, fixes, plus other API related topics by subscribing to Aspose.CAD blog.
*   [Aspose.CAD for Java Examples][7] – We have published our code examples on the social coding website GitHub.com. Anyone can explore the code examples for learning purposes.




[1]: http://www.aspose.com/downloads/cad/java
[2]: https://www.aspose.com/products/cad/java
[3]: https://downloads.aspose.com/cad/java
[4]: https://docs.aspose.com/display/cadjava/Home
[5]: https://www.aspose.com/community/forums/aspose.cad-product-family/540/showforum.aspx
[6]: https://blog.aspose.com/category/aspose-products/aspose.cad-product-family/
[7]: https://github.com/aspose-cad/Aspose.CAD-for-Java





---
title: 'Metered licensing support in Aspose.CAD for .Net 16.12.1'
date: Mon, 16 Jan 2017 08:53:01 +0000
draft: false
url: /2017/01/16/metered-licensing-support-aspose.cad-.net-16.12.1/
author: Ikram Haq
summary: ''
tags: []
categories: ['Aspose.CAD Product Family']
---

We are pleased to announce the release of Aspose.CAD for .NET 16.12.1. The major development in this release is support for metered license mechanism. The new licensing mechanism will be used along with existing licensing method. Those customers who want to be billed based on the usage of the API features can use the metered licensing.

## Metered Licensing

Aspose.CAD for .Net provides the functionality to use metered licensing mechanism. We have introduced Metered class in API to accomplish this job. The following sample code will demonstrate, how to calculate the consumed CAD API requests.

```
 // Create an instance of CAD Metered class
Aspose.CAD.Metered metered = new Aspose.CAD.Metered();

// Access the setMeteredKey property and pass public and private keys as parameters
metered.SetMeteredKey("*****", "*****");

// Get metered data amount before calling API
decimal amountbefore = Aspose.CAD.Metered.GetConsumptionQuantity();

// Display information
Console.WriteLine("Amount Consumed Before: " + amountbefore.ToString());


// Do processing
//Aspose.CAD.FileFormats.Cad.CadImage image = (Aspose.CAD.FileFormats.Cad.CadImage)Aspose.CAD.Image.load("BlockRefDgn.dwg");


// Get metered data amount After calling API
decimal amountafter = Aspose.CAD.Metered.GetConsumptionQuantity();

// Display information
Console.WriteLine("Amount Consumed After: " + amountafter.ToString()); 
```

## Enhancements

Following enhancements have been introduced in this release.

*   Process of converting DWG to PDF format has been improved.
    
*   Process of converting DWG to PNG format in multithreading has been improved.
    

To view a complete list of new features and to download the latest release, please visit [Aspose.CAD for .NET 16.12.1 page in downloads section][1].

## Aspose.CAD for .NET Resources

The resources, you may need to accomplish your tasks:

*   [Homepage for Aspose.CAD for .NET API][2]
*   [Download Aspose.CAD for .NET][3]
*   [Aspose.CAD for .NET Wiki Docs][4] – Help documentation
*   [API Reference Documents][5]
*   [Aspose.CAD Product Family Forum][6] – Post your technical questions and queries, or any other problem you faced while running Aspose.CAD APIs.
*   [Enable Email Subscription][7] – Don’t limit yourself, you can keep yourself updated with the latest news on Aspose.CAD APIs and new features, fixes, plus other API related topics by subscribing to Aspose.CAD blog.
*   [Aspose.CAD for .NET Examples][8] – We have published our code examples on the social coding website GitHub.com. Anyone can explore the code examples for learning purposes.




[1]: http://www.aspose.com/downloads/cad-family/net
[2]: https://www.aspose.com/products/cad/net
[3]: https://downloads.aspose.com/cad/net
[4]: https://docs.aspose.com/display/cadnet/Home
[5]: https://apireference.aspose.com/net/cad
[6]: https://www.aspose.com/community/forums/aspose.cad-product-family/540/showforum.aspx
[7]: https://blog.aspose.com/category/aspose-products/aspose.cad-product-family/
[8]: https://github.com/aspose-cad/Aspose.CAD-for-.NET





---
title: 'Programmatically loop through PSD layers and Render User-Defined Images using Aspose.PSD API'
date: Fri, 03 May 2019 14:34:06 +0000
draft: false
url: /2019/05/03/rendering-user-defined-images-using-psd-api/
author: Liam Dowen-gould
summary: ''
tags: ['Aspose.Psd', 'Programatically process PSD layers', 'Programmatically loop through PSD layers', 'Success Stories']
categories: ['Aspose.PSD Product Family']
---

## About REGENCY HAMPERS



{{< figure align=center src="images/12240081_824587927658109_4745425038443600458_n.png" alt="">}}


[Regency Hampers][1] is a premium supplier of gift hampers with a large offering of different variants including classic fruit baskets, baby hampers, and fully-fitted picnic hampers. We have a bespoke system built on ASP.NET for both the front-end customer-facing website and back-end management interface. All system changes are developed in house which allows quick and easy adaptation to the changing market, and demands of the business

## Problem

In order to broaden our product offerings, a decision was taken to allow users to personalize their purchases. Some products have wood cases or glassware that allow personalized wording, which can then be engraved, embroidered, thermal transferred, etc. on to their chosen product. Whilst analyzing the problem, we found that the best solution would be to allow our designers to create the initial design in Photoshop, with all its intricacies, and then programmatically alter the text fields to the values entered by the customer stored in our database, thus allowing autonomous creation of personalized design files. This approach was thought to give the designers ultimate control over the final product as all text/image placement would be easily editable for them via the original Photoshop design file.



{{< figure align=center src="images/regency-hampers-aspose.psd-case-study-1-1024x504.png" alt="Personalise Gift preview" caption="Image 1:- Personalize your gift preview">}}


## Solution

The main challenge was in the most imperative part of the solution, altering the text field’s values. After careful research using the internet, [Aspose.PSD for .NET][2] seemed to be a solution. At first glance, it looked suitable, allowing programmatic looping through all layers of a .PSD file, checking for their type (_Only Text Layers were of interest, as images part of the design were needed to stay as they were_) and then checking their name for the relevant flag to say that they were editable fields. Upon identification of an editable field, the text value could be changed with ease. All these changes to the PSD file could then be exported to the raster image type of our choice (_In this case BMP_), without affecting the original design file allowing easy, repeat use.



{{< figure align=center src="images/regency-hampers-aspose.psd-case-study-2.png" alt="Preview of Altered image using Aspose.PSD for .NET" caption="Image 2:- Original Design File (Left) and Altered Design using [Aspose.PSD for .NET](https://products.aspose.com/psd/net) (Right)">}}


Other approaches were considered for this task, such as drawing elements using inbuilt libraries for .NET, but that would have created a large amount of work not only on the development side but also for our designers when it comes to setting up new designs.

## Experience

While looking at [Aspose.PSD for .NET][3], we also looked at other products but after using the [free trial][4], it was clear that [Aspose.PSD for .NET][5] can meet our needs and was quick and easy to implement, having a working prototype ready within a day. This would have not been possible in the other approaches we considered, and the expediency of the project was greatly helped by the [documentation][6] provided (_with examples on use_). However, it was rarely needed as the library was easy and intuitive to use.

We ran into one issue during development, where changing the font of a text field resulted in rendering issues (_The element moved location and rendered in a low resolution_). We figured out a workaround by having multiple text elements and turning them on and off depending upon the required font. Hopefully, this issue will be resolved in the future.

## Next Steps

At this time, we have managed to achieve everything we set out to. Therefore, we currently do not have any plans to expand our offering using [Aspose.PSD for .NET][7] in the future but, it will be kept well in-mind for any future projects.

## Summary

All in all, [Aspose.PSD for .NET][8] helped us achieve our goal of editing and rendering photoshop documents. While currently limited in its image manipulation capabilities (_Transformations and warping are either limited or non-existent at this time_), we do hope they will be added in the future as it will help us to further bolster our product offering.

**Liam Dowen-Gould,  
**Regency Hampers Ltd




[1]: https://www.regencyhampers.com/
[2]: https://products.aspose.com/psd/net
[3]: https://products.aspose.com/psd/net
[4]: https://downloads.aspose.com/psd/net
[5]: https://products.aspose.com/psd/net
[6]: https://docs.aspose.com/display/psdnet/Home
[7]: https://products.aspose.com/psd/net
[8]: https://products.aspose.com/psd/net





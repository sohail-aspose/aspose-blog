---
title: 'Get Hyperlinks from Images in PDF using Java'
date: Tue, 15 Aug 2017 19:18:45 +0000
draft: false
url: /2017/08/15/get-hyperlink-associated-image-file/
author: Codewarior
summary: ''
tags: ['Nayyer Shahbaz']
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/aspose-Pdf-for-Java.png" alt="">}}


A new release version [Aspose.PDF for Java 17.7][1] has been added to the portfolio of Aspose.PDF product family. This release offers a feature to **Get hyperlink associated with the image file**, perform PDF file creation and manipulation with great stability. In this release, we have also improved the PDF form manipulation and the Flatten form fields feature is specifically improved. Furthermore, as a regular monthly release process, this version also includes fixes for issues reported in earlier release versions.

## Get Hyperlink Associated with Image in PDF

Aspose.PDF for Java supports the feature to [Add Image in existing PDF document][2] and also the feature to [Add Hyperlink to PDF document][3]. However, there can be a scenario where an image already presents inside PDF document points to a web URL and you may have a requirement to get hyperlink associated with the image. Please note that links are represented as annotations in a PDF file and they can be added, updated, or deleted. Furthermore, Aspose.PDF for Java also supports getting the destination (URL) of the hyperlink in a PDF file so in order to accomplish above-mentioned requirement, we need to first search the images inside PDF document using following code snippet and then use the extracted rectangular coordinates to get the URL of LinkAnnotation from a specific region.

```
// Open document
 Document doc = new Document("D:\\Tests\\input.pdf");
 // Create ImagePlacementAbsorber object to perform image placement search
 ImagePlacementAbsorber abs = new ImagePlacementAbsorber();
 // Accept the absorber for first page
 doc.getPages().get_Item(1).accept(abs);
 // Display image placement properties for all placements
 for (ImagePlacement imagePlacement : (Iterable)abs.getImagePlacements())
 {     
     System.out.println("image width:" + imagePlacement.getRectangle().getWidth());
     System.out.println("image height:" + imagePlacement.getRectangle().getHeight());
     System.out.println("image LLX:" + imagePlacement.getRectangle().getLLX());
     System.out.println("image LLY:" + imagePlacement.getRectangle().getLLY());
     System.out.println("image horizontal resolution:" + imagePlacement.getResolution().getX());
     System.out.println("image vertical resolution:" + imagePlacement.getResolution().getY());
 }
```

## Stable Inter-File Format Conversion

In this release, we have specifically improved the interfile format conversion features, so PDF to DOC, PDF to PPTX, PDF to HTML and PDF to PDF/A have become more stable and robust as compared to earlier release versions. Some customers also reported incorrect rendering of Chinese text/content when the PDF file is converted to HTML format. In some scenarios, the colors of images are also lost during PDF to HTML conversion and these scenarios are also fixed.

## Miscellaneous fixes

As mentioned above, the tabular text alignment in resultant PPTX, missing notes in rendered PPTX, overlapping of text on table border during PDF to HTML conversion, splitting of text to multiple lines during PDF to PPTX conversion are also resolved. As it is always recommended to use the latest release of our API's, so we suggest you please download the latest release of Aspose.PDF for Java 17.7 and check Release Notes section regarding the list of issues fixed in [Aspose.PDF for Java 17.7][4]

*   [Home page for Aspose.PDF for Java][5]
*   [Download Aspose.PDF for Java][6]
*   [Aspose.PDF product family forum][7] – Post your technical questions and queries, or any other problem you faced while running Aspose.PDF APIs.
*   [Aspose.PDF for Java online documentation][8] – Help documentation and API reference documents.
*   [Enable Blog Subscription][9] – Do not limit yourself, you can keep yourself updated with the latest news on Aspose.PDF APIs, new features, fixes, and other API related topics by subscribing to Aspose.PDF blog.
*   [Aspose.PDF for Java Examples][10] – We have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: https://downloads.aspose.com/pdf/java/new-releases/aspose.pdf-for-java-17.7/
[2]: https://docs.aspose.com/display/pdfnet/Manipulate+Images#ManipulateImages-AddImagetoExistingPDFFile
[3]: https://docs.aspose.com/display/pdfnet/Add+and+Get+Hyperlink#AddandGetHyperlink-AddHyperlinkinaPDFFile
[4]: https://docs.aspose.com/display/pdfjava/Aspose.Pdf+for+Java+17.7+Release+Notes
[5]: https://www.aspose.com/products/pdf/java
[6]: https://downloads.aspose.com/pdf/java
[7]: https://forum.aspose.com/c/pdf
[8]: https://docs.aspose.com/display/pdfjava/Home
[9]: https://blog.aspose.com/category/aspose-products/aspose-pdf-product-family/
[10]: https://github.com/aspose-pdf/Aspose.Pdf-for-Java





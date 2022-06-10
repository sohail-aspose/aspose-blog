---
title: 'Manipulate the Resolution of OMR Image using Java'
date: Tue, 07 Jul 2015 13:59:50 +0000
draft: false
url: /2015/07/07/manipulate-the-resolution-of-omr-image-using-java/
author: Babar Raza
summary: ''
tags: ['Babar Raza']
categories: ['Aspose.OCR Product Family']
---



{{< figure align=center src="images/aspose-OCR-for-Java_100.png" alt="Aspose.OCR for Java logo">}}


We're pleased to announce July's release of Aspose.OCR for Java. Please review the release notes of [Aspose.OCR for Java 2.6.0][1] for a complete list of enhancements. If you are planning to upgrade the API from any previous revision, we strongly recommend you to check the Public API Changes section to know what has been changed since your current version of the API.

## Set the Resolution of OMR Image in Java

[Aspose.OCR for Java][2] requires OMR sheets to be scanned using an image scanner at a resolution that is acceptable to capture the OMR data accurately. Once fed to the Aspose.OCR for Java API, the API recognizes the filled-in elements by comparing the number of black pixels against the number of white pixels in each element. It is important for the API to first determine the resolution of the image before initiating the recognition process.

The resolution of the image is set by the scanner and the Aspose.OCR APIs read this information from the image's metadata. It is also possible that images are preprocessed before feeding them to the Aspose.OCR APIs for data extraction and such manipulation may corrupt or remove the metadata that identifies the image's resolution. In order to handle situation as discussed above, the Aspose.OCR for Java has exposed the OmrImage.Resolution property, allowing the developers to set the resolution information of the image before performing the marker recognition operation.

The following code snippet demonstrates the usage of OmrImage.Resolution property to manipulate the image's resolution.

```
//Load the image to be analyzed
OmrImage image = OmrImage.load("D:/sample.png");

//Define new value of image resolution in double format
image.setResolution(300.0); //overwrites the old DPI value

//Do processing
```

## Aspose.OCR for Java Resources

The resources, you may need to accomplish your tasks:

*   [Home page for Aspose.OCR for Java API][3].
*   [Download Aspose.OCR for Java][4].
*   [Aspose.OCR for Java online documentation][5] – help documentation and API reference documents.
*   [Aspose.OCR Product Family Forum][6] – post your technical questions and queries, or any other problem you are facing while working with Aspose.OCR APIs.
*   [Enable blog Subscription][7] – Do not limit yourself, you can keep yourself updated with the latest news on Aspose.OCR APIs, new features, fixes and other API related topics by subscribing to Aspose.OCR blog.
*   [Aspose.OCR for Java Examples][8] – We have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.

As always, we appreciate your feedback so if you ever have anything to tell us about this release or anything else, please head to the [Aspose.OCR forum][9] for a chat.




[1]: https://products.aspose.com/ocr
[2]: https://products.aspose.com/ocr/java
[3]: https://products.aspose.com/ocr/java
[4]: https://downloads.aspose.com/ocr/java
[5]: https://docs.aspose.com/ocr/java/
[6]: http://forum.aspose.com
[7]: https://blog.aspose.com/
[8]: https://github.com/asposeocr/Aspose_OCR_Java
[9]: http://forum.aspose.com





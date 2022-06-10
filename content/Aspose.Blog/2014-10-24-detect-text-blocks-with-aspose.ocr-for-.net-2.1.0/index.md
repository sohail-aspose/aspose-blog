---
title: 'Detect Text Blocks in Images using C# or VB.NET'
date: Fri, 24 Oct 2014 17:17:09 +0000
draft: false
url: /2014/10/24/detect-text-blocks-with-aspose.ocr-for-.net-2.1.0/
author: Babar Raza
summary: ''
tags: ['Babar Raza']
categories: ['Aspose.OCR Product Family']
---



{{< figure align=center src="images/aspose-OCR-for-net_100.png" alt="Aspose.OCR for .NET logo">}}


We are pleased to announce that the Aspose.OCR for .NET 2.1.0 is now available for public use. While you are [downloading][1] the latest build, here is a look at the most worth mentioning features in this month’s release. For a full list of bug fixes and improvements please refer to the release notes of [Aspose.OCR for .NET 2.1.0][2], and if you are planning to upgrade the API from any previous version, we would suggest you to check the Public API Changes section.

## Detect Text Blocks in Image using C#

Recognized Text blocks can be retrieved using the OcrEngine.Text property only after performing the OCR operation. These blocks are stored as an array of IRecognizedPartInfo and contains information as discussed above along with the position and size of the block on the image. The IRecognizedPartInfo.Box property can be used to get the rectangular area where the detected block (with text or picture) is shown on the image. The Box property returns the coordinates starting from the upper left corner of the image.

Below provided code snippet demonstrates the usage of Aspose.OCR for .NET API to retrieve the additional information from each recognized block.

```
// Initialize OcrEngine
OcrEngine engine = new OcrEngine();

// Load Image
engine.Image = ImageStream.FromFile(imageFile);

// Remove non-textual blocks
engine.Config.RemoveNonText = true;

// Load the resource file
using (engine.Resource = new FileStream(resourceFileName, FileMode.Open))
{
    try
    {
        // Process the whole image
        if (engine.Process())
        {
            //Display text block locations
            Console.WriteLine(engine.Text.PartsInfo[0].Box);
            Console.WriteLine(engine.Text.PartsInfo[1].Box);
        }
    }
    catch (Exception ex)
    {
        Console.WriteLine("Exception: " + ex.Message);
    }
}
```

## Introduction to IRecognizedPartInfo

Aspose.OCR for .NET API has exposed IRecognizedPartInfo to keep track of all the recognized blocks on the image that could be text or detected picture block. Textual blocks are represented by IRecognizedTextPartInfo holding useful information about the recognized text part. Each part has its own style, font, text size, color, language and other attributes. If the text consists of several parts that are written in different font styles or even in different languages then IRecognizedTextPartInfo will hold an item representing an individual element.

## Enhancements to the OcrEngine

Last but not the least, we have made some improvements to the OcrEngine for performance considerations and accuracy. Moreover, we have fixed a few problem regarding the recognition of numbers, and cases that may cause OutOfMemory & IndexOutOfRange exceptions.

As always we appreciate your feedback so if you ever have anything to tell us about this release or anything else, please head to the [Aspose.OCR forum][3] for a chat.




[1]: https://downloads.aspose.com/ocr/net
[2]: https://downloads.aspose.com/ocr/net
[3]: http://forum.aspose.com





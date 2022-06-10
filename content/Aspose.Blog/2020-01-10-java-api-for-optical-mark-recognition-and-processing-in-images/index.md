---
title: 'Java API for Optical Mark Recognition and Processing in Images'
seoTitle: "Java OMR Library | Optical Mark Recognition and Image Processing | Java"
description: "Java OMR library for optical mark recognition and processing in images using Java. Generate OMR template and perform OMR operations on images using Java."
date: Fri, 10 Jan 2020 16:55:09 +0000
draft: false
url: /2020/01/10/java-api-for-optical-mark-recognition-and-processing-in-images/
author: Usman Aziz
summary: "Do you need a simple yet feature-rich **Java OMR library**? Do you want to recognize optical marks in scanned images? Try **Aspose.OMR for Java** - A Java class library to perform the **Optical Mark Recognition** (OMR) operations in Java-based applications. Let's have a quick walk through the features of the said **Java API** to see how to **recognize optical marks** in a variety of image formats and capture **human-marked data** from surveys, questionnaires or tests containing MCQs."
tags: ['Aspose.OMR', 'OMR Recognition and Processing', 'java omr library', 'omr in images', 'omr reader', 'optical mark reader', 'optical mark recognition java']
categories: ['Aspose.OMR Product Family']
---



{{< figure align=center src="images/aspose_omr-for-java-128.png" alt="Java OMR Library">}}


Do you need a simple yet feature-rich **Java OMR library**? Do you want to recognize optical marks in scanned images? Try **[Aspose.OMR for Java][1]** - A Java class library to perform the **Optical Mark Recognition** (OMR) operations in Java-based applications. Let's have a quick walk through the features of the said **Java API** to see how to **recognize optical marks** in a variety of image formats and capture **human-marked data** from surveys, questionnaires or tests containing MCQs.

## Dynamically Create OMR Template using Java OMR Library

_Aspose.OMR for Java_ provides a complete set of features from creating the OMR template to recognizing the optical marks to capture the data. The API supports generating the OMR template file or the image from simple text markups. You can simply pass the template's text markup to the API and it will generate the template for you. The following is a sample text markup for an OMR template.

```
?text=Name__________________________________ Date____________

?grid=ID
sections_count=8
#What is Aspose.OMR main function?
() OCR () Capture human-marked data
() There is no main function () Enhance images
#Can Aspose.OMR process photos as well?
() Yes, indeed! () No
#Aspose.OMR is available on any platform, because it is:
() Cross-platform code () Cloud service
#Aspose.OMR works with any kind of OMR forms: tests, exams, questionnaires, surveys, etc.
() Yes, indeed! () No
#Excellent recognition results can be achieved only for filled bubbles at least for:
() 40% () 60% () 75% () 98%
#Do you have to mark up every question on the page?
(Yes) Yes, that will help a lot! (No) No
#Rate your preference from 0 to 9 with "0" being preference towards performance
and "9" being preference towards flexibility.
(0) (1) (2) (3) (4) (5) (6) (7) (8) (9)
#I found aspose omr to be a useful tool. (5 - strongly agree, 1 - strongly disagree)
(5) (4) (3) (2) (1)

?text= Answer sheet section
?answer_sheet=MainQuestions
elements_count=10
columns_count=5

?text=Sign________________________________
```

You can simply save the text markup in a text file with .txt extension. Once done, you can generate the template using the following steps:

*   Create an [OmrEngine][2] object.
*   Call [OmrEngine.generateTemplate()][3] method that accepts the markup text file's path.
*   Save the template using [GenerationResult.save][4] method.

The following code sample shows how to generate the OMR template from text markup using Java.

{{< gist aspose-com-gists 5dfadede6434f4d17847b621a18cbdee "Generate-OMR-Template-Java.java" >}}

### Output



{{< figure align=center src="images/OMR-Template-725x1024.png" alt="Java OMR Library">}}


## Optical Mark Recognition (OMR) in Images using Java

In order to perform OMR in images, you just need two things - the prepared OMR template (.omr) and the images (user-filled forms/sheets) to perform OMR on. The API supports the OMR for the following image formats:

*   [JPEG][5]
*   [PNG][6]
*   [GIF][7]
*   [TIFF][8]
*   [BMP][9]

The following are the steps to perform OMR in images:

*   Create [OmrEngine][10] object.
*   Create [TemplateProcessor][11] object and initialize it with the OMR template's path.
*   Recognize images using [TemplateProcessor.recognizeImage()][12] method and get results in CSV or JSON format.

The following code sample shows how to recognize optical marks in images using Java.

{{< gist aspose-com-gists 5dfadede6434f4d17847b621a18cbdee "OMR-in-Images-using-Java.java" >}}

## Using a Custom Recognition Threshold for OMR

You can also fine-tune the OMR results by defining a custom threshold between 0 to 100. Increasing the threshold makes the API more strict in recognizing the answers. The threshold values can be set in [TemplateProcessor.recognizeImage()][13] method as the second parameter as shown in the following Java code sample.

{{< gist aspose-com-gists 5dfadede6434f4d17847b621a18cbdee "OMR-in-Images-Threshold-using-Java.java" >}}

## Recalculating the OMR Results

In some cases, you may want to recalculate the OMR results with different threshold values. Instead of calling [TemplateProcessor.recognizeImage()][14] again and again in such cases, you can configure the API for automatic recalculation using [TemplateProcessor.recalculate()][15] method to improve image processing efficiency. The following code sample shows how to implement the recalculation of the OMR results.

{{< gist aspose-com-gists 5dfadede6434f4d17847b621a18cbdee "OMR-in-Images-Recalculation-using-Java.java" >}}

In case you would have any questions or queries related to our Java OMR library, contact us via our [forum][16] for any questions or queries.

## See also

*   [PHP Barcode Generator and Reader API][17]




[1]: https://products.aspose.com/omr/java
[2]: https://apireference.aspose.com/java/omr/com.aspose.omr/OmrEngine
[3]: https://apireference.aspose.com/java/omr/com.aspose.omr/OmrEngine#generateTemplate-java.lang.String-
[4]: https://apireference.aspose.com/java/omr/com.aspose.omr/GenerationResult#save-java.lang.String-java.lang.String-
[5]: https://wiki.fileformat.com/image/jpeg/
[6]: https://wiki.fileformat.com/image/png/
[7]: https://wiki.fileformat.com/image/gif/
[8]: https://wiki.fileformat.com/image/tiff/
[9]: https://wiki.fileformat.com/image/bmp/
[10]: https://apireference.aspose.com/java/omr/com.aspose.omr/OmrEngine
[11]: https://apireference.aspose.com/java/omr/com.aspose.omr/TemplateProcessor
[12]: https://apireference.aspose.com/java/omr/com.aspose.omr/TemplateProcessor#recognizeImage-java.lang.String-
[13]: https://apireference.aspose.com/java/omr/com.aspose.omr/TemplateProcessor#recognizeImage-java.lang.String-int-
[14]: https://apireference.aspose.com/java/omr/com.aspose.omr/TemplateProcessor#recognizeImage-java.lang.String-
[15]: https://apireference.aspose.com/java/omr/com.aspose.omr/TemplateProcessor#recalculate-com.aspose.omr.RecognitionResult-int-
[16]: https://forum.aspose.com/c/omr
[17]: https://blog.aspose.com/2020/01/29/php-barcode-generator-reader-and-scanner-api/






---
title: 'Recognize Text by Performing OCR on Image from URL with Java'
seoTitle: "Recognize Text by Performing OCR on Image from URL with Java"
description: "You can recognize text with OCR on image from URL. It can be a JPEG, PNG, TIFF, BMP, or GIFF image. API can read text from tilted or skewed images in Java."
date: Thu, 27 May 2021 23:16:00 +0000
draft: false
url: /2021/05/27/recognize-text-by-performing-ocr-on-image-from-url-with-java/
author: Farhan Raza
summary: 'You can convert a text from the image to an editable format with Optical Character Recognition (OCR). Images like JPG, PNG, TIFF, BMP, GIF, etc. are used everywhere on the internet and you may need to recognize text from an online image. You can easily use the URL link to that image to perform the OCR on it, instead of saving or downloading the file. The following headings discuss the details further.'
tags: ['OCR Image Text in Java', 'Read Image Text in Java', 'Recognize Text from Skewed Image', 'Recognize Text from Tilted Image', 'Recognize image text in Java']
categories: ['Aspose.OCR Product Family']
---



{{< figure align=center src="images/Perform-OCR-using-Java.jpg" alt="Recognize-Text-OCR-Image-using-Java">}}


You can convert a text from the image to an editable format with Optical Character Recognition (OCR). Images like [JPG][1], [PNG][2], [TIFF][3], [BMP][4], [GIF][5], etc. are used everywhere on the internet and you may need to recognize text from an online image. You can easily use the URL link to that image to perform the OCR on it, instead of saving or downloading the file. The following headings discuss the details further:

*   [Java OCR API – Installation][6]
*   [Recognize Text by Performing OCR on Image from URL with Java][7]
*   [Recognize Text from Skewed or Tilted Image with OCR using Java][8]

## Java OCR API – Installation {#section1}

[Aspose.OCR for Java][9] API can be used to perform Optical Character Recognition operations on images. It can recognize text and convert the image to editable text. Please download the JAR file of API from the [Downloads][10] section or specify the following Maven configurations in pom.xml file of your project:

### Repository```
<repository>
    <id>AsposeJavaAPI</id>
    <name>Aspose Java API</name>
    <url>http://repository.aspose.com/repo/</url>
</repository>
```

### Dependency```
<dependency>
    <groupId>com.aspose</groupId>
    <artifactId>aspose-ocr</artifactId>
    <version>20.5</version>
</dependency>
```

## Recognize Text by Performing OCR on Image from URL with Java {#section2}

You can perform Optical Character Recognition on an image from URL with the following steps:

1.  Create API instance with [AsposeOCR][11] class.
2.  Specify image URI.
3.  Set recognition options with [RecognitionSettings][12] class.
4.  Get result object.
5.  Print result.

The following code explains how to recognize text by performing OCR on image from URL programmatically using Java:

{{< gist aspose-com-gists e74d058177ae660b2e875ee69d6c4ab7 "Recognize-URI-Image.java" >}}

## Recognize Text from Skewed or Tilted Image with OCR using Java {#section3}

Sometimes an image can be tilted or skewed for some reason. For instance, an image created by a camera or scanner can be a little skewed, then you can get the skew angle of the input image. You can improve the accuracy of text recognition by knowing and correcting the skew angle. You need to follow the following steps:

*   Create API Instance using [AsposeOCR][13] object.
*   Set recognition options.
*   Calculate and set skew angle.
*   Get the result with the [RecognitionResult][14] object and print it.

The code below shows how to recognize text from a skewed image with OCR programmatically in Java:

{{< gist aspose-com-gists e74d058177ae660b2e875ee69d6c4ab7 "Get-skew-angle-OCR.java" >}}

## Get Free API License

You can request a [Free Temporary License][15] to evaluate the API in its full capacity.

## Conclusion

In conclusion, you have learned how to recognize text by performing OCR operations on an image from any URL address. Moreover, you have explored how to correct the skew angle for the image to improve the accuracy and efficiency of the API. You can take a look at several other features of the API by visiting the [Documentation][16], or please feel free to contact us via [Free Support Forum][17] in case of any queries.

## See Also

*   [Convert Image to Word Document (DOCX) with OCR using C#][18]
*   [Convert Scanned PDF to Searchable PDF with OCR in Java][19]




[1]: https://docs.fileformat.com/image/jpeg/
[2]: https://docs.fileformat.com/image/png/
[3]: https://docs.fileformat.com/image/tiff/
[4]: https://docs.fileformat.com/image/bmp/
[5]: https://docs.fileformat.com/image/gif/
[6]: #section1
[7]: #section2
[8]: #section3
[9]: https://products.aspose.com/ocr/java
[10]: https://downloads.aspose.com/ocr/java
[11]: https://apireference.aspose.com/ocr/java/com.aspose.ocr/AsposeOCR
[12]: https://apireference.aspose.com/ocr/java/com.aspose.ocr/RecognitionSettings
[13]: https://apireference.aspose.com/ocr/java/com.aspose.ocr/AsposeOCR
[14]: https://apireference.aspose.com/ocr/java/com.aspose.ocr/RecognitionResult
[15]: https://purchase.aspose.com/temporary-license
[16]: https://docs.aspose.com/ocr/java/
[17]: https://forum.aspose.com/c/ocr
[18]: https://blog.aspose.com/2021/05/19/image-to-word-docx-ocr-csharp/
[19]: https://blog.aspose.com/2021/12/13/convert-scanned-pdf-searchable-ocr-java/






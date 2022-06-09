---
title: 'Convert DICOM to JPEG, GIF, PNG, BMP and PDF in Java'
seoTitle: ""
description: ""
date: Fri, 20 Nov 2020 07:44:26 +0000
draft: false
url: /2020/11/20/convert-dicom-to-jpeg-gif-png-bmp-images-in-java/
author: Muhammad Sohail
summary: 'In order to view a DICOM file, you need a dedicated software and you cannot simply embed them in presentations or webpages. To tackle this limitation, you can convert a DICOM file to raster image formats such as JPEG, GIF, PNG, and BMP. In this article, you will learn how to **convert a DICOM** file **programmatically** in **Java**.'
tags: []
categories: ['Aspose.Imaging Product Family']
---



{{< figure align=center src="images/DICOM-to-Image.png" alt="Convert DICOM to Image Java">}}


**Digital Imaging and Communications in Medicine ([DICOM][1]** is the standard for the communication and management of medical imaging information and related data. But you need a dedicated software to view a DICOM file and you cannot simply embed them in presentations or webpages. To tackle this limitation, you can convert a DICOM file to raster image formats such as [JPEG][2], [GIF][3], [PNG][4], and [BMP][5]. In this article, you will learn how to **convert a DICOM** file **programmatically** in **Java**.

*   [Java DICOM Converter API][6]
*   [DICOM to JPEG in Java][7]
*   [DICOM to GIF in Java][8]
*   [Convert DICOM to PNG in Java][9]
*   [DICOM to BMP in Java][10]
*   [DICOM to PDF in Java][11]

## Java DICOM Converter API {#Java-DICOM-Converter-API}

[Aspose.Imaging for Java][12] is a powerful image creation and manipulation API that lets you convert DICOM file to JPEG, GIF, PNG, BMP and [PDF][13] with high fidelity. You can either [download][14] the API’s [JAR][15] or install it within your Maven-based applications using the following configurations.

```
<repository>
    <id>AsposeJavaAPI</id>
    <name>Aspose Java API</name>
    <url>https://repository.aspose.com/repo/</url>
</repository>
```
```
<dependency>
    <groupId>com.aspose</groupId>
    <artifactId>aspose-imaging</artifactId>
    <version>20.10</version>
    <classifier>jdk16</classifier>
</dependency>
```

## DICOM to JPEG in Java {#Convert-DICOM-to-JPEG-in-Java}

The following are the steps to convert DICOM to JPEG in Java:

*   Load the DICOM file into a [DicomImage][16] object from the specified file path.
*   Select the active page in DICOM that you want to convert to JPEG (if it is not set, the default active page will be converted).
*   Save the converted JPEG image using [DicomImage.save(String filePath, ImageOptionsBase options)][17] method.

The following code sample converts a page in DICOM to JPEG in Java.

{{< gist aspose-com-gists cd3cc2832c75fd30fb41106f0ad79a7b "DICOMtoJPEG.java" >}}

**Input DICOM**



{{< figure align=center src="images/DICOM-to-JPG.png" alt="Input DICOM file">}}


**DICOM to JPEG**



{{< figure align=center src="images/DICOM-to-JPG-Converted.png" alt="DICOM to JPG Converted">}}


## DICOM to GIF in Java {#Convert-DICOM-to-GIF-in-Java}

The steps to convert DICOM to GIF are same as we used above to convert DICOM to JPEG. Just access the DICOM file and save it with **.gif** extension. The following are the steps to convert DICOM to animated GIF in Java:

*   Load the DICOM file into a [DicomImage][18] object from the specified file path.
*   Save the converted GIF image using [DicomImage.save(String filePath, ImageOptionsBase options)][19] method.

The following code sample shows how to convert DICOM to GIF in Java.

{{< gist aspose-com-gists b11b576c9b691959cec402b2141bd6ea "DICOMToGIF.java" >}}

## DICOM to PNG in Java {#Convert-DICOM-to-PNG-in-Java}

As you may have guessed already, the steps to convert DICOM to PNG are same as used above to perform other conversions. Simply access the DICOM file using [DicomImage][20] class and save it with **.png** extension. If it is required to convert each page in a DICOM file to PNG, simply call [DicomImage.getDicomPages()][21] function to get **DicomPage\[\]** array and iterate over it as shown below.

The following code example shows how to convert a DICOM to PNG in Java.

{{< gist aspose-com-gists 2ebeba39050b823febf99d277bf5805d "DICOMToPNG.java" >}}

## DICOM to BMP in Java {#Convert-DICOM-to-BMP-in-Java}

Converting DICOM to BMP is as simple as pie. Access the DICOM file using the [DicomImage][22] class and use [DicomImage.save(String filePath, ImageOptionsBase options)][23] method to save DICOM as BMP. The following code sample shows how to convert DICOM to BMP in Java.

{{< gist aspose-com-gists 510622a7ac9ecc1d520561229fafaae5 "DICOMToBMP.java" >}}

## DICOM to PDF in Java {#DICOM-to-PDF-in-Java}

PDF is one of the most popular file formats. So, it is important to know how to transform a DICOM file to PDF in Java. The following code sample explains how to make this conversion.

{{< gist aspose-com-gists 6834d532dabcadaf5eea271dd4c09ee0 "DICOMToPDF.java" >}}

## Conclusion

In this article, you have learned how to convert DICOM file to JPEG, GIF, PNG, BMP and PDF in Java. You have also seen how to set an active page and convert all pages of a DICOM file. Please check the [documentation][24] to learn more about **Aspose.Imaging** API.

## See also

*   [Access and Export Pages in Multipage TIFF, GIF, and Other Multipage Images using Aspose.Imaging][25]




[1]: https://docs.fileformat.com/image/dicom/)
[2]: https://docs.fileformat.com/image/jpeg/
[3]: https://docs.fileformat.com/image/gif/
[4]: https://docs.fileformat.com/image/png/
[5]: https://docs.fileformat.com/image/bmp/
[6]: #Java-DICOM-Converter-API
[7]: #Convert-DICOM-to-JPEG-in-Java
[8]: #Convert-DICOM-to-GIF-in-Java
[9]: #Convert-DICOM-to-PNG-in-Java
[10]: #Convert-DICOM-to-BMP-in-Java
[11]: #DICOM-to-PDF-in-Java
[12]: https://products.aspose.com/imaging/java
[13]: https://docs.fileformat.com/pdf/
[14]: https://downloads.aspose.com/imaging/java
[15]: https://docs.fileformat.com/programming/jar/
[16]: https://apireference.aspose.com/imaging/java/com.aspose.imaging.fileformats.dicom/DicomImage
[17]: https://apireference.aspose.com/imaging/java/com.aspose.imaging/Image#save-java.lang.String-com.aspose.imaging.ImageOptionsBase-
[18]: https://apireference.aspose.com/imaging/java/com.aspose.imaging.fileformats.dicom/DicomImage
[19]: https://apireference.aspose.com/imaging/java/com.aspose.imaging/Image#save-java.lang.String-com.aspose.imaging.ImageOptionsBase-
[20]: https://apireference.aspose.com/imaging/java/com.aspose.imaging.fileformats.dicom/DicomImage
[21]: https://apireference.aspose.com/imaging/java/com.aspose.imaging.fileformats.dicom/DicomImage#getDicomPages--
[22]: https://apireference.aspose.com/imaging/java/com.aspose.imaging.fileformats.dicom/DicomImage
[23]: https://apireference.aspose.com/imaging/java/com.aspose.imaging/Image#save-java.lang.String-com.aspose.imaging.ImageOptionsBase-
[24]: https://docs.aspose.com/imaging/java/developer-guide/
[25]: https://blog.aspose.com/2020/03/03/access-and-export-pages-in-multipage-images-in-csharp-java/






---
title: 'Convert GIF Images to PDF using Java'
seoTitle: "Convert GIF to PDF in Java | GIF Frames to PDF Conversion"
description: "Use Java image processing API to convert GIF images to PDF using Java. Convert all or the seletced frames in GIF to PDF using Java."
date: Tue, 09 Feb 2021 10:02:16 +0000
draft: false
url: /2021/02/09/convert-gif-images-to-pdf-using-java/
author: Usman Aziz
summary: 'Being the software and hardware-independent format, PDF gives an outstanding user experience as compared to other document formats. The consistent layout of PDF makes it a universal format. Therefore, in various scenarios, the documents or images are converted to PDF before they are shared or exchanged. In this article, you will learn **how to convert animated GIF images to PDF using Java**. Particularly, we will convert each frame in a GIF to an image in a PDF file.'
tags: ['GIF frame to PDF in Java', 'Java GIF to PDF', 'convert gif images to pdf java']
categories: ['Aspose.Imaging Product Family']
---



{{< figure align=center src="images/gif-to-pdf-icon.jpg" alt="gif to pdf java">}}


Being the software and hardware-independent format, [PDF][1] gives an outstanding user experience as compared to other document formats. The consistent layout of PDF makes it a universal format. Therefore, in various scenarios, the documents or images are converted to PDF before they are shared or exchanged. In this article, you will learn **how to convert animated GIF images to PDF using Java**. Particularly, we will convert each frame in a [GIF][2] to an image in a PDF file.

*   [Java GIF to PDF Converter API][3]
*   [Convert GIF to PDF using Java][4]
*   [Convert Particular GIF Frame to PDF][5]
*   [Set Page Size in GIF to PDF Conversion][6]
*   [Set PDF Document Info in GIF to PDF Conversion][7]
*   [Get a Free API License][8]

**Info**: You may want to check out the FREE [Text to GIF Converter][9] Aspose recently developed.

## Java GIF to PDF Converter API {#Java-GIF-to-PDF-Converter-API}

[Aspose.Imaging for Java][10] is designed to perform image processing operations from within your Java applications. The API lets you manipulate popular image formats seamlessly. Furthermore, its built-in converter API allows you to convert images from one format to another. Aspose.Imaging for Java can be downloaded as [JAR][11] or installed using the following Maven configurations.

```
<repository>
    <id>AsposeJavaAPI</id>
    <name>Aspose Java API</name>
    <url>http://repository.aspose.com/repo/</url>
</repository>
```
```
<dependency>
    <groupId>com.aspose</groupId>
    <artifactId>aspose-imaging-java</artifactId>
    <version>20.12</version>
    <classifier>jdk16</classifier>
</dependency>
```

## Convert GIF to PDF using Java {#Convert-GIF-to-PDF-using-Java}

The following are the steps to convert a GIF image to PDF using Aspose.Imaging.

*   Load the GIF image using the [Image][12] class.
*   Create an instance of [PdfOptions][13] class.
*   Convert GIF to PDF using [Image.save(String, PdfOptions)][14] method.

The following code sample shows how to convert a GIF to PDF using Java.

{{< gist aspose-com-gists 032de2b87650c56a000bbcc55535f8e5 "gif-to-pdf.java" >}}

### Animated GIF



{{< figure align=center src="images/gif.gif" alt="">}}


### Converted PDF



{{< figure align=center src="images/gif-to-pdf.jpg" alt="gif to pdf java">}}


## Convert Particular GIF Frame to PDF {#Convert-Particular-GIF-Frame-to-PDF-in-Java}

You can also convert a particular frame or a range of frames in GIF to PDF. The following are the steps to perform this operation.

*   Load the GIF image using the [Image][15] class.
*   Create an instance of [PdfOptions][16] class.
*   Specify the frame(s) you want to convert using [PdfOptions.setMultiPageOptions(MultiPageOptions)][17] method.
*   Save the converted PDF using [Image.save(String, PdfOptions)][18] method.

The following code sample shows how to convert particular frame(s) of a GIF to PDF using Java.

{{< gist aspose-com-gists 032de2b87650c56a000bbcc55535f8e5 "gif-frame-to-pdf.java" >}}

## Set Page Size in GIF to PDF Conversion {#Set-Page-Size-in-GIF-to-PDF-Conversion}

Aspose.Imaging for Java also lets you specify the dimensions of the pages in the converted PDF document. The following are the steps to set the height and width of the pages in GIF to PDF conversion.

*   Load the GIF image using the [Image][19] class.
*   Create an instance of [PdfOptions][20] class.
*   Set height and width of the pages using [PdfOptions.setPageSize(new SizeF(float, float))][21] method.
*   Convert GIF to PDF using [Image.save(String, PdfOptions)][22] method.

The following code sample shows how to set the page size in Java GIF to PDF conversion.

{{< gist aspose-com-gists 032de2b87650c56a000bbcc55535f8e5 "gif-to-pdf-pagesize.java" >}}

## Java GIF to PDF - Set Document Info {#Set-PDF-Document-Info-in-GIF-to-PDF}

The PDF format allows you to set the additional information about the document including author, subject, title, and keywords. You can also set these properties for the converted PDF document in GIF to PDF conversion. The following are the steps to set the document information of the PDF.

*   Load the GIF image using the [Image][23] class.
*   Create an instance of [PdfOptions][24] class.
*   Create an instance of [PdfDocumentInfo][25] class.
*   Set properties of the document such as author.
*   Set document info of the PDF using [PdfOptions.setPdfDocumentInfo(DocumentInfo)][26] method.
*   Convert GIF to PDF using [Image.save(String, PdfOptions)][27] method.

The following code sample shows how to set PDF document info in GIF to PDF conversion.

{{< gist aspose-com-gists 032de2b87650c56a000bbcc55535f8e5 "gif-to-pdf-docinfo.java" >}}

## Get a Free API License {#Get-a-Free-API-License}

In case you want to try the API without evaluation limitations, you can [get a free temporary license][28].

## Conclusion

In this article, you have learned how to convert GIF images to PDF using Java. Furthermore, different options have been discussed to customize GIF to PDF conversion. You can explore more about the Java image processing API using [documentation][29].

## See Also

*   [Add Watermark to Images using Java][30]




[1]: https://docs.fileformat.com/pdf/
[2]: https://docs.fileformat.com/image/gif/
[3]: #Java-GIF-to-PDF-Converter-API
[4]: #Convert-GIF-to-PDF-using-Java
[5]: #Convert-Particular-GIF-Frame-to-PDF-in-Java
[6]: #Set-Page-Size-in-GIF-to-PDF-Conversion
[7]: #Set-PDF-Document-Info-in-GIF-to-PDF
[8]: #Get-a-Free-API-License
[9]: https://products.aspose.app/slides/text-to-gif
[10]: https://products.aspose.com/imaging/java
[11]: https://downloads.aspose.com/imaging/java
[12]: https://apireference.aspose.com/imaging/java/com.aspose.imaging/Image
[13]: https://apireference.aspose.com/imaging/java/com.aspose.imaging.imageoptions/PdfOptions
[14]: https://apireference.aspose.com/imaging/java/com.aspose.imaging/Image#save-java.lang.String-com.aspose.imaging.ImageOptionsBase-
[15]: https://apireference.aspose.com/imaging/java/com.aspose.imaging/Image
[16]: https://apireference.aspose.com/imaging/java/com.aspose.imaging.imageoptions/PdfOptions
[17]: https://apireference.aspose.com/imaging/java/com.aspose.imaging/ImageOptionsBase#setMultiPageOptions-com.aspose.imaging.imageoptions.MultiPageOptions-
[18]: https://apireference.aspose.com/imaging/java/com.aspose.imaging/Image#save-java.lang.String-com.aspose.imaging.ImageOptionsBase-
[19]: https://apireference.aspose.com/imaging/java/com.aspose.imaging/Image
[20]: https://apireference.aspose.com/imaging/java/com.aspose.imaging.imageoptions/PdfOptions
[21]: https://apireference.aspose.com/imaging/java/com.aspose.imaging.imageoptions/PdfOptions#setPageSize-com.aspose.imaging.SizeF-
[22]: https://apireference.aspose.com/imaging/java/com.aspose.imaging/Image#save-java.lang.String-com.aspose.imaging.ImageOptionsBase-
[23]: https://apireference.aspose.com/imaging/java/com.aspose.imaging/Image
[24]: https://apireference.aspose.com/imaging/java/com.aspose.imaging.imageoptions/PdfOptions
[25]: https://apireference.aspose.com/imaging/java/com.aspose.imaging.fileformats.pdf/PdfDocumentInfo
[26]: https://apireference.aspose.com/imaging/java/com.aspose.imaging.imageoptions/PdfOptions#setPdfDocumentInfo-com.aspose.imaging.fileformats.pdf.PdfDocumentInfo-
[27]: https://apireference.aspose.com/imaging/java/com.aspose.imaging/Image#save-java.lang.String-com.aspose.imaging.ImageOptionsBase-
[28]: https://purchase.aspose.com/temporary-license
[29]: https://docs.aspose.com/imaging/java
[30]: https://blog.aspose.com/2021/01/27/Add-Watermark-to-Images-using-Java/






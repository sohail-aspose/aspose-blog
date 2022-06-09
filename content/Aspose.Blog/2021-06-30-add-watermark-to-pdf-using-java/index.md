---
title: 'Add Watermark to PDF using Java'
seoTitle: "Add Watermark to PDF using Java | Java PDF API | Java Source Code"
description: "Use Java PDF API to add watermark to the PDF documents in Java. Insert text or image watermark and set its position, font size, color, opacity, etc."
date: Wed, 30 Jun 2021 10:29:00 +0000
draft: false
url: /2021/06/30/add-watermark-to-pdf-using-java/
author: Usman Aziz
summary: '[Watermarks][1] are used to protect PDF documents or claim their ownership. Also, in various cases, watermarks are added to display the status of a PDF document such as draft, manuscript, etc. In order to automate watermarking, this article covers **how to add a text or image watermark to the PDF using Java**.'
tags: ['Add Image Watermark to PDF Java', 'Add Text Watermark to PDF Java', 'Add Watermark to a PDF in Java', 'Java API to Add Watermark to PDF', 'Watermark PDF File in Java']
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/Add-Watermark-to-PDF-Logo.jpg" alt="Add Watermark to PDF Java Logo">}}


[Watermarks][2] are used to protect PDF documents or claim their ownership. Also, in various cases, watermarks are added to display the status of a PDF document such as draft, manuscript, etc. In order to automate watermarking, this article covers **how to add a text or image watermark to the PDF using Java**.

*   [API to Add Watermark to PDF][3]
*   [Add Text Watermark to a PDF Document][4]
*   [Add Image Watermark to PDF Document][5]

## Java API to Add Watermark to PDF {#Java-API-to-Add-Watermark-to-PDF}

In order to add a watermark to PDF documents, we will use [Aspose.PDF for Java][6]. It is a feature-rich API to create, process, and convert PDF files from within the Java applications. You can either [download][7] the API's JAR or install it using the following Maven configurations.

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
    <artifactId>aspose-pdf</artifactId>
    <version>21.6</version>
</dependency>
```

## Add Text Watermark to PDF in Java {#Add-Watermark-to-PDF-in-Java}

The following are the steps to add a text watermark to PDF using Java.

*   Load the PDF using [Document][8] class.
*   Create an instance of [FormattedText][9] class and set watermark text and its properties.
*   Create an instance of [WatermarkArtifact][10] class.
*   Add text to the artifact and set properties such as alignment, rotation angle, opacity, background, etc.
*   Add text watermark to the desired page of PDF using [Document.getPages().get\_Item(index).getArtifacts().add(WatermarkArtifact)][11] method.
*   Save the updated PDF document using [Document.save(String)][12] method.

The following code sample shows how to add a text watermark to a PDF document.

{{< gist aspose-com-gists b5f7f2262b678f17cf0d7b1e318d092e "add-text-watermark-to-pdf.java" >}}

### Output

The following is the screenshot of the watermarked PDF.



{{< figure align=center src="images/Add-Watermark-to-PDF.jpg" alt="adding watermark to pdf in java">}}


## Add Image Watermark to PDF in Java {#Add-Image-Watermark-to-PDF-Document}

The following are the steps to add an image watermark to PDF using Java.

*   Load the PDF using [Document][13] class.
*   Create an instance of [BackgroundArtifact][14] class and set its background image and other properties.
*   Add image watermark to the desired page of PDF using [Document.getPages().get\_Item(index).getArtifacts().add(BackgroundArtifact)][15] method.
*   Save the updated PDF document using [Document.save(String)][16] method.

The following code sample shows how to add an image watermark to a PDF document.

{{< gist aspose-com-gists b5f7f2262b678f17cf0d7b1e318d092e "add-image-watermark-to-pdf.java" >}}

### Output

The following is the screenshot of the watermarked PDF.



{{< figure align=center src="images/Add-Image-Watermark-to-PDF.jpg.png" alt="Image watermark in PDF using Java">}}


## Get a Free API License {#Get-a-Free-API-License}

You can [get a temporary license][17] in order to use the API without evaluation limitations.

## Conclusion

In this article, you have learned how to add a text or image watermark to a PDF using Java. Also, you have seen how to customize the appearance of the watermark using different properties. You can learn more about the Java PDF API using the [documentation][18]. In case you would have any questions, let us know via our [forum][19].

## See Also

*   [Create PDF Files using Java][20]




[1]: https://en.wikipedia.org/wiki/Watermark
[2]: https://en.wikipedia.org/wiki/Watermark
[3]: #Java-API-to-Add-Watermark-to-PDF
[4]: #Add-Watermark-to-PDF-in-Java
[5]: #Add-Image-Watermark-to-PDF-Document
[6]: https://products.aspose.com/pdf/java
[7]: https://downloads.aspose.com/pdf/java
[8]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/Document
[9]: https://apireference.aspose.com/pdf/java/com.aspose.pdf.facades/FormattedText
[10]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/WatermarkArtifact
[11]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/ArtifactCollection#add-com.aspose.pdf.Artifact-
[12]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/Document#save-java.lang.String-
[13]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/Document
[14]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/BackgroundArtifact
[15]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/ArtifactCollection#add-com.aspose.pdf.Artifact-
[16]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/Document#save-java.lang.String-
[17]: https://purchase.aspose.com/temporary-license
[18]: https://docs.aspose.com/pdf/java
[19]: https://forum.aspose.com/
[20]: https://blog.aspose.com/2020/12/31/create-pdf-files-in-java/






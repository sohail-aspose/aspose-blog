---
title: 'Convert PDF to PowerPoint PPT/PPTX using Java'
seoTitle: ""
description: ""
date: Thu, 23 Jul 2020 04:36:53 +0000
draft: false
url: /2020/07/23/convert-pdf-to-powerpoint-ppt-pptx-using-java/
author: Usman Aziz
summary: ''
tags: ['pdf to powerpoint using java', 'pdf to ppt using java', 'pdf to pptx using java']
categories: ['Aspose.PDF Product Family']
---

In this article, I'll show you how to convert **PDF to PowerPoint PPT/PPTX programmatically using Java**.



{{< figure align=center src="images/Convert-PDF-to-PPT-C.png" alt="Convert PDF to PPT PPTX in Java">}}


The [PDF][1] has become one of the most widely used document formats because of its supported features as well as stability and consistency across all the platforms. In various scenarios, you opt to save or share a document in the PDF format. However, in some cases, you may need to export the content of a PDF to a PowerPoint ([PPT][2]/[PPTX][3] presentation. In such a situation, you can avoid manual copy/paste by automating PDF to PowerPoint conversion. In order to deal with such a case, we'll learn how to:

*   [Convert PDF to PowerPoint PPT or PPTX using Java][4]
*   [Convert PDF to PPT/PPTX having slides as images][5]
*   [Track PDF to PPT/PPTX conversion progress][6]

**TIP**: You may want to try Aspose [PDF to PowerPoint Converter][7], which is a live implementation of the process described in this article.

## Java PDF to PPT/PPTX Converter API

[Aspose.PDF for Java][8] is a well-known PDF API with an amazing set of PDF manipulation features. Along with PDF manipulation, the API also provides a powerful PDF to PowerPoint converter that lets you convert each page in the PDF document to a slide in the PPT/PPTX presentation. You can [download][9] the API's JAR or install it within your Maven-based application using the following configurations.

### Repository```
<repository>
    <id>AsposeJavaAPI</id>
    <name>Aspose Java API</name>
    <url>https://repository.aspose.com/repo/</url>
</repository>
```

### Dependency```
<dependency>
    <groupId>com.aspose</groupId>
    <artifactId>aspose-pdf</artifactId>
    <version>20.7</version>
    <classifier>jdk17</classifier>
</dependency>
```

## Convert PDF to PowerPoint PPT/PPTX using Java {#Convert-PDF-to-PowerPoint-PPT-or-PPTX-using-Java}

The following are the steps as well as API references to convert a PDF document to PPTX presentation using Aspose.PDF for Java.

*   Create an instance of the [Document][10] class.
*   Create an object of the [PptxSaveOptions][11] class.
*   Convert PDF to PPTX using [Document.save(String)][12] method.

The following code sample shows how to convert a PDF to PPTX using Java.

{{< gist aspose-com-gists 32bd89909f83834c357a6024cc2fc7f8 "pdf-to-pptx.java" >}}

### PDF Document



{{< figure align=center src="images/PDF-Document.png" alt="PDF to PPTX using Java">}}


### PPTX Presentation



{{< figure align=center src="images/Convert-PDF-to-PPT-in-C.png" alt="PDF to PPT using Java">}}


## Convert PDF to PPTX with Slides as Images using Java {#Convert-PDF-to-PPT/PPTX-with-slides-as-images-using-Java}

You can also convert each page of the PDF to an image within the presentation's slides. This feature is useful when you want to avoid having the selectable text in the presentation. The following are the steps to convert a PDF to PPTX having images in the slides.

*   Initialize the [Document][13] class.
*   Create an instance of the [PptxSaveOptions][14] class.
*   Set [PptxSaveOptions.setSlidesAsImages(true)][15].
*   Save PDF as PPTX using [Document.save(String)][16] method.

The following code sample shows how to convert PDF to PPTX having slides as images.

{{< gist aspose-com-gists 32bd89909f83834c357a6024cc2fc7f8 "pdf-to-pptx-images.java" >}}

## Track PDF to PowerPoint PPTX Conversion Progress {#Track-PDF-to-PowerPoint-PPTX-Conversion-Progress}

You can also track the PDF to PPTX conversion progress by defining a custom progress handler using [PptxSaveOptions.setCustomProgressHandler()][17] method. This feature can be used to show the progress bar or details about how many pages are processed. The following code sample shows how to implement the feature of tracking conversion progress.

{{< gist aspose-com-gists 32bd89909f83834c357a6024cc2fc7f8 "pdf-to-pptx-track-progress.java" >}}

### Output```
SourcePageAnalysed	1 from: 	10
TotalProgress	2 from: 	100
SourcePageAnalysed	2 from: 	10
TotalProgress	5 from: 	100
SourcePageAnalysed	3 from: 	10
TotalProgress	7 from: 	100
SourcePageAnalysed	4 from: 	10
TotalProgress	9 from: 	100
SourcePageAnalysed	5 from: 	10
TotalProgress	12 from: 	100
SourcePageAnalysed	6 from: 	10
TotalProgress	14 from: 	100
SourcePageAnalysed	7 from: 	10
TotalProgress	16 from: 	100
SourcePageAnalysed	8 from: 	10
TotalProgress	18 from: 	100
SourcePageAnalysed	9 from: 	10
TotalProgress	21 from: 	100
SourcePageAnalysed	10 from: 	10
TotalProgress	23 from: 	100
ResultPageCreated	1 from: 	10
TotalProgress	28 from: 	100
ResultPageCreated	2 from: 	10
TotalProgress	32 from: 	100
ResultPageCreated	3 from: 	10
TotalProgress	37 from: 	100
ResultPageCreated	4 from: 	10
TotalProgress	42 from: 	100
ResultPageCreated	5 from: 	10
TotalProgress	46 from: 	100
ResultPageCreated	6 from: 	10
TotalProgress	51 from: 	100
ResultPageCreated	7 from: 	10
TotalProgress	56 from: 	100
ResultPageCreated	8 from: 	10
TotalProgress	61 from: 	100
ResultPageCreated	9 from: 	10
TotalProgress	65 from: 	100
ResultPageCreated	10 from: 	10
TotalProgress	70 from: 	100
ResultPageSaved	1 from: 	10
TotalProgress	73 from: 	100
ResultPageSaved	2 from: 	10
TotalProgress	76 from: 	100
ResultPageSaved	3 from: 	10
TotalProgress	79 from: 	100
ResultPageSaved	4 from: 	10
TotalProgress	82 from: 	100
ResultPageSaved	5 from: 	10
TotalProgress	85 from: 	100
ResultPageSaved	6 from: 	10
TotalProgress	88 from: 	100
ResultPageSaved	7 from: 	10
TotalProgress	91 from: 	100
ResultPageSaved	8 from: 	10
TotalProgress	94 from: 	100
ResultPageSaved	9 from: 	10
TotalProgress	97 from: 	100
ResultPageSaved	10 from: 	10
TotalProgress	100 from: 	100
```

## Conclusion

In this article, you have learned how to programmatically convert PDF to PowerPoint PPT/PPTX using Java. You can implement this feature in Java Swing or any other Java-based applications. In case you may want to learn more about our Java PDF API, consult the [documentation][18].

## See Also

*   [Convert PDF File to PowerPoint Presentation in C#][19]




[1]: https://docs.fileformat.com/pdf/
[2]: https://docs.fileformat.com/presentation/ppt/
[3]: https://docs.fileformat.com/presentation/pptx/)
[4]: #Convert-PDF-to-PowerPoint-PPT-or-PPTX-using-Java
[5]: #Convert-PDF-to-PPT/PPTX-with-slides-as-images-using-Java
[6]: #Track-PDF-to-PowerPoint-PPTX-Conversion-Progress
[7]: https://products.aspose.app/slides/import/pdf-to-powerpoint
[8]: https://products.aspose.com/pdf/java
[9]: https://downloads.aspose.com/pdf/java
[10]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/Document
[11]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/PptxSaveOptions
[12]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/Document#save-java.lang.String-
[13]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/Document
[14]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/PptxSaveOptions
[15]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/PptxSaveOptions#setSlidesAsImages-boolean-
[16]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/Document#save-java.lang.String-
[17]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/PptxSaveOptions#setCustomProgressHandler-com.aspose.pdf.UnifiedSaveOptions.ConversionProgressEventHandler-
[18]: https://docs.aspose.com/
[19]: https://blog.aspose.com/2020/03/18/convert-pdf-to-powerpoint-ppt-pptx-in-csharp-net/






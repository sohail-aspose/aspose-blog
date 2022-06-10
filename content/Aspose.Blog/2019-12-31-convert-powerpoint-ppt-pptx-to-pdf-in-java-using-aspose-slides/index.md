---
title: 'Convert PowerPoint to PDF using Java - PPT to PDF or PPTX to PDF Conversion'
date: Tue, 31 Dec 2019 04:47:10 +0000
draft: false
url: /2019/12/31/convert-powerpoint-ppt-pptx-to-pdf-in-java-using-aspose-slides/
author: Usman Aziz
summary: ''
tags: ['Aspose.Slides for Java', 'Java API', 'convert powerpoint to pdf in java', 'convert ppt to pdf', 'convert pptx to pdf', 'convert pptx to pdf in java', 'convert presentation to pdf in java', 'convert slides to pdf', 'powerpoint to pdf', 'powerpoint to pdf java', 'ppt to pdf', 'pptx to pdf']
categories: ['Aspose.Slides Product Family']
---



{{< figure align=center src="images/Convert-PPT-PPTX-to-PDF-1.png" alt="Java PowerPoint PPT PPTX to PDF">}}


[**PDF**][1] (Portable Document Format) has become the most widely and commonly used digital document format. Since PDF format owns the fixed layout, most of the documents are converted to PDF before they are shared. Among the various document conversions to PDF format, **PowerPoint to PDF** conversion is a popular use case and there should be an automated and time-saving solution to avoid manual conversions specifically when you have to convert a bunch of PowerPoint presentations to PDF. Keeping this in mind, I'll show you how to convert **PowerPoint PPT or PPTX to PDF** **programmatically** in **Java** with various options provided by [**Aspose.Slides for Java**][2] API.

TIP: Check out a live implementation of the [PowerPoint to PDF][3] or [PPT to PDF][4] conversion process.

## PowerPoint to PDF Conversions in Java

In this article, we will cover the following conversion scenarios using Aspose.Slides for Java:

*   Convert PowerPoint PPT or PPTX to PDF in Java
*   Convert PPT or PPTX to PDF with custom options
*   Convert PPT or PPTX to PDF including hidden slides
*   Convert PPT or PPTX to password-protected PDF
*   Convert specific slide(s) of PPT or PPTX to PDF
*   Convert PPT or PPTX to PDF with access permissions

## Installing Aspose.Slides for Java

You can either [download][5] Aspose.Slides for Java JAR or add it in your maven-based project using the following repository and dependency information.

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
    <artifactId>aspose-slides</artifactId>
    <version>19.12</version>
    <classifier>jdk16</classifier>
</dependency>
```

## Convert PowerPoint PPT or PPTX to PDF in Java

The following are the simple steps to convert your PowerPoint presentation to PDF with default options provided by Aspose.Slides for Java.

*   Load PowerPoint PPT or PPTX file using [Presentation][6] object.
*   Call [save()][7] method passing the output PDF file name and the output format.

The following code sample shows how to convert a PowerPoint PPTX to PDF in Java with default options.

{{< gist aspose-com-gists bcc4f993d6b75479636e621002468f35 "Convert-PowerPoint-to-PDF-Java.java" >}}

## Convert PowerPoint PPT or PPTX to PDF with Custom Options

Aspose.Slides for Java provides the [PdfOptions][8] class to let you customize the PowerPoint to PDF conversion. PdfOptions class lets you specify the JPEG quality, define the behavior of metafiles, set text compression level, PDF compliance level, and other options. The following are the steps to convert a PPT or PPTX file to PDF with customized options.

*   Load PowerPoint PPT or PPTX using [Presentation][9] object.
*   Create the object of _PdfOptions_ class.
*   Set/specify the options exposed by the _PdfOptions_ class.
*   Call [save()][10] method.

The following code sample shows how to convert PowerPoint PPTX to PDF in Java with customized options.

{{< gist aspose-com-gists bcc4f993d6b75479636e621002468f35 "Convert-PowerPoint-to-PDF-Java-Custom.java" >}}

## Convert PowerPoint PPT or PPTX to PDF Including Hidden Slides

There could be the case when the PowerPoint presentation contains the hidden slides. In the default PowerPoint to PDF conversion, Aspose.Slides for Java ignores the hidden slides. However, if you want to include the hidden slides in the converted PDF, you can use [PdfOptions.setShowHiddenSlides(true)][11] option.

The following code sample shows how to convert PowerPoint PPTX to PDF including hidden slides in Java.

{{< gist aspose-com-gists bcc4f993d6b75479636e621002468f35 "Convert-PowerPoint-to-PDF-Java-Hidden-Slides.java" >}}

## Convert Specific Slide(s) of PowerPoint Presentation to PDF

Aspose.Slides for Java also allows selecting the slides that you want to include in the resultant PDF document. You can create an array to specify the slides numbers that you want to include in PowerPoint to PDF conversion and pass that to [save()][12] method.

The following code sample shows how to convert specific slides of PowerPoint PPTX to PDF in Java.

{{< gist aspose-com-gists bcc4f993d6b75479636e621002468f35 "Convert-Specific-Slides-PowerPoint-to-PDF-Java.java" >}}

## Convert PowerPoint PPT or PPTX to Password-Protected PDF

You can also convert the PowerPoint presentation to a password-protected PDF to secure your document. You can set the password using[PdfOptions.setPassword("password")][13] and pass _PdfOptions_ object to _save()_ method.

The following code sample shows how to convert PowerPoint PPTX to a password-protected PDF in Java.

{{< gist aspose-com-gists bcc4f993d6b75479636e621002468f35 "Convert-PowerPoint-to-password-protected-PDF-Java.java" >}}

## Convert PowerPoint PPT or PPTX to PDF with Access Permissions

The PDF format allows you to specify different access permissions such as print permission, permission to add or modify text annotations or form fields and so on. In accordance with this feature, Aspose.Slides for Java provides the feature of setting permissions for the PDF document which is converted from the PowerPoint presentation. The [PdfAccessPermissions][14] class contains the set of flags for different permission types you can apply in PowerPoint presentation to PDF conversion.

The following Java code sample shows how to convert PowerPoint presentations to PDF with access permissions.

{{< gist aspose-com-gists bcc4f993d6b75479636e621002468f35 "Convert-PowerPoint-to-PDF-Java-Access-Permissions.java" >}}

You can download the complete set of source code examples in Java from the [GitHub repository][15]. Visit the [documentation][16] for more details on the features exposed by Aspose.Slides for Java. In case you would find an issue or have any questions, feel free to let us know via our [forum][17].




[1]: https://wiki.fileformat.com/view/pdf/
[2]: https://products.aspose.com/slides/java
[3]: https://products.aspose.app/slides/conversion/powerpoint-to-pdf
[4]: https://products.aspose.app/slides/conversion/ppt-to-pdf
[5]: https://downloads.aspose.com/slides/java
[6]: https://apireference.aspose.com/java/slides/com.aspose.slides/Presentation
[7]: https://apireference.aspose.com/java/slides/com.aspose.slides/Presentation#save-java.lang.String-int-
[8]: https://apireference.aspose.com/java/slides/com.aspose.slides/PdfOptions
[9]: http://www.aspose.com/api/java/slides/com.aspose.slides/classes/Presentation
[10]: https://apireference.aspose.com/java/slides/com.aspose.slides/Presentation#save-java.lang.String-int-com.aspose.slides.ISaveOptions-
[11]: https://apireference.aspose.com/java/slides/com.aspose.slides/PdfOptions#setShowHiddenSlides-boolean-
[12]: https://apireference.aspose.com/java/slides/com.aspose.slides/Presentation#save-java.lang.String-int:A-int-
[13]: https://apireference.aspose.com/java/slides/com.aspose.slides/PdfOptions#setPassword-java.lang.String-
[14]: https://apireference.aspose.com/java/slides/com.aspose.slides/PdfAccessPermissions
[15]: https://github.com/aspose-slides/Aspose.Slides-for-Java
[16]: https://docs.aspose.com/display/slidesjava/Getting+Started
[17]: https://forum.aspose.com/c/slides





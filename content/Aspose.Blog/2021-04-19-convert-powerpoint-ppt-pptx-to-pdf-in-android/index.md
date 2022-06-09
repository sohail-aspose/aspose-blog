---
title: 'Convert PowerPoint PPTX or PPT to PDF using Android API'
seoTitle: "Android API: Convert PowerPoint to PDF | PPTX or PPT to PDF in Android"
description: "Use Android PowerPoint API to convert PPTX or PPT presentations to PDF. Use different options to customize PPTX to PDF conversion in Android apps."
date: Mon, 19 Apr 2021 17:24:02 +0000
draft: false
url: /2021/04/19/convert-powerpoint-ppt-pptx-to-pdf-in-android/
author: Usman Aziz
summary: '[PDF][1] has become a standard format for sharing documents over the internet, therefore, files of various formats are converted to PDF. PowerPoint [PPTX][2] or [PPT][3] to PDF is a popular conversion scenario in which slides in a PowerPoint presentation are converted to pages in a PDF. In this article, you will learn **how to perform PowerPoint PPTX/PPT to PDF conversion from within your Android apps**.'
tags: ['Convert PPT to PDF in Android', 'Convert PPTX to PDF in Android', 'Convert PowerPoint to PDF in Android']
categories: ['Aspose.Slides Product Family']
---



{{< figure align=center src="images/Convert-PPT-PPTX-to-PDF-1.png" alt="PowerPoint to PDF Android">}}


[PDF][4] has become a standard format for sharing documents over the internet, therefore, files of various formats are converted to PDF. PowerPoint [PPTX][5] or [PPT][6] to PDF is a popular conversion scenario in which slides in a PowerPoint presentation are converted to pages in a PDF. In this article, you will learn **how to perform PowerPoint PPTX/PPT to PDF conversion from within your Android apps**.

*   [Android API for PowerPoint to PDF Conversion][7]
*   [Convert PPTX to PDF in Android][8]
*   [Additional Options for PPTX to PDF Conversion][9]
*   [Get a Free API License][10]

**TIP**: You may try to check out Aspose [PowerPoint to PDF][11] or [PPT to PDF][12] Converter.

## Android API for PPTX to PDF Conversion {#Android-API-for-PowerPoint-to-PDF-Conversion}

For converting the PowerPoint presentations to PDF in Android apps, we'll use [Aspose.Slides for Android via Java][13]. It is a feature-rich Android API that lets you create, modify and convert presentations seamlessly. You can either download the API from the [downloads section][14] or install it by adding the following configurations in build.gradle.

```
maven {
    url "http://repository.aspose.com/repo/" }
```
```
compile (
        group: 'com.aspose',
        name: 'aspose-slides',
        version: '21.3',
        classifier: 'android.via.java')
```

## Convert PowerPoint PPTX to PDF in Android {#Convert-PPTX-to-PDF-in-Android}

The following are the steps to convert a PowerPoint presentation to PDF in Android.

*   Load PowerPoint PPT or PPTX file using [Presentation][15] class.
*   Call [Presentation.save(String, SaveFormat)][16] method by providing the PDF file's name and the output format.

The following code sample shows how to convert a PPTX file to PDF in Android apps.

{{< gist aspose-com-gists bcc4f993d6b75479636e621002468f35 "Convert-PowerPoint-to-PDF-Java.java" >}}

## Additional Options for PPTX to PDF Conversion {#Additional-Options-for-PPTX-to-PDF-Conversion}

Aspose.Slides also allows you to customize PPTX to PDF conversion using different options. For example, you can set text compression, image quality, PDF compliance, the option to include or exclude hidden slides, etc. To achieve this, the API provides [PdfOptions][17] class.

The following are the steps to customize the PPTX/PPT to PDF conversion.

*   Load PowerPoint PPTX or PPT file using [Presentation][18] class.
*   Create an object of [PdfOptions][19] class and set the desired options.
*   Call [Presentation.save(String, SaveFormat, ISaveOptions)][20] method to save PPTX/PPT as PDF.

The following code sample shows how to customize PPTX to PDF conversion.

{{< gist aspose-com-gists bcc4f993d6b75479636e621002468f35 "Convert-PowerPoint-to-PDF-Java-Custom.java" >}}

## Get a Free API License {#Get-a-Free-API-License}

You can [get a free temporary license][21] in order to use the API without evaluation limitations.

## Conclusion

In this article, you have learned how to convert PowerPoint PPTX/PPT presentations to PDF in Android apps. Furthermore, you have seen how to customize the PPTX to PDF conversion using different options. You can explore more about the API using [documentation][22]. In addition, you can share your queries with us via our [forum][23].

## See Also

*   [Create PowerPoint Presentations using Java][24]




[1]: https://docs.fileformat.com/pdf/
[2]: https://docs.fileformat.com/presentation/pptx/
[3]: https://docs.fileformat.com/presentation/ppt/
[4]: https://docs.fileformat.com/pdf/
[5]: https://docs.fileformat.com/presentation/pptx/
[6]: https://docs.fileformat.com/presentation/ppt/
[7]: #Android-API-for-PowerPoint-to-PDF-Conversion
[8]: #Convert-PPTX-to-PDF-in-Android
[9]: #Additional-Options-for-PPTX-to-PDF-Conversion
[10]: #Get-a-Free-API-License
[11]: https://products.aspose.app/slides/conversion/ppt-to-pdf
[12]: https://products.aspose.app/slides/conversion/ppt-to-pdf
[13]: https://products.aspose.com/slides/android-java
[14]: https://downloads.aspose.com/slides/androidjava
[15]: https://apireference.aspose.com/java/slides/com.aspose.slides/Presentation
[16]: https://apireference.aspose.com/java/slides/com.aspose.slides/Presentation#save-java.lang.String-int-
[17]: https://apireference.aspose.com/java/slides/com.aspose.slides/PdfOptions
[18]: https://apireference.aspose.com/java/slides/com.aspose.slides/Presentation
[19]: https://apireference.aspose.com/java/slides/com.aspose.slides/PdfOptions
[20]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation#save-java.lang.String-int-com.aspose.slides.ISaveOptions-
[21]: https://purchase.aspose.com/temporary-license
[22]: https://docs.aspose.com/slides/androidjava/
[23]: https://forum.aspose.com/
[24]: https://blog.aspose.com/2021/01/18/Create-PowerPoint-Presentations-using-Java/






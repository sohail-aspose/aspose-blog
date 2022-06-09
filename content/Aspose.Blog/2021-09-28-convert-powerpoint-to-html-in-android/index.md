---
title: 'Convert PowerPoint PPTX/PPT to HTML in Android'
seoTitle: "Convert PowerPoint to HTML in Android | PPT to HTML | PPTX to HTML"
description: "Convert PowerPoint PPTX or PPT presentations to HTML in Android. Include or exclude hidden slides in PPTX/PPT to HTML conversion."
date: Tue, 28 Sep 2021 14:56:57 +0000
draft: false
url: /2021/09/28/convert-powerpoint-to-html-in-android/
author: Usman Aziz
summary: 'PowerPoint to HTML conversion could be useful when you need to embed the presentations within your Android applications. You can convert each slide in the presentation into an HTML page. Accordingly, this article covers **how to convert slides in PowerPoint PPTX or PPT to HTML in Android**.'
tags: ['Android PowerPoint to HTML Converter API', 'Convert PowerPoint PPTX to HTML in Android', 'PPT to HTML Android', 'PPTX to HTML Android']
categories: ['Aspose.Slides Product Family']
---



{{< figure align=center src="images/PPTX-to-HTML-1.jpg" alt="PowerPoint PPTX to HTML Android">}}


PowerPoint to HTML conversion could be useful when you need to embed the presentations within your Android applications. You can convert each slide in the presentation into an HTML page. Accordingly, this article covers **how to convert slides in PowerPoint PPTX or PPT to HTML in Android**.

*   [PowerPoint to HTML Converter API][1]
*   [Convert PowerPoint PPTX to HTML in Android][2]
*   [PPT/PPTX to HTML Conversion with Hidden Slides][3]

## Android PowerPoint to HTML Converter API {#Java-PowerPoint-to-HTML-Converter-API}

For PowerPoint to HTML conversion, we will use [Aspose.Slides for Android via Java][4]. It is a feature-rich Android API for creating, modifying and converting presentation documents. You can either [download][5] the API or install it by adding the following configurations in build.gradle.

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

## Convert PowerPoint PPTX to HTML in Android {#Convert-PowerPoint-PPTX-to-HTML-in-Java}

The following are the steps to convert PowerPoint PPTX or PPT files to HTML in Android.

*   First, load the PowerPoint presentation you want to convert using the [Presentation][6] class.
*   Create an object of [HtmlOptions][7] class.
*   Convert PPTX to HTML using [Presentation.save(String,][8] i[nt, HtmlOptions)][9] method.

The following code sample shows how to convert a PowerPoint presentation to HTML.

{{< gist aspose-com-gists 1aa7b2386c8905d53478b28926a1b7e6 "pptx-to-html.java" >}}

## Android: PPTX to HTML Conversion with Hidden Slides {#PPT-PPTX-to-HTML-Conversion-with-Hidden-Slides}

PowerPoint also allows you to hide the slides within a presentation. By default, Aspose.Slides do not include hidden slides in the PowerPoint to HTML conversion. However, you can convert the hidden slides as well by following the steps below.

*   Load the PPTX/PPT presentation you want to convert using the [Presentation][10] class.
*   Create an object of [HtmlOptions][11] class.
*   Include hidden slides using [HtmlOptions.setShowHiddenSlides(true)][12] method.
*   Convert PPTX to HTML using [Presentation.save(String, int, HtmlOptions)][13] method.

The following code sample shows how to include hidden slides in PowerPoint to HTML conversion in Android.

{{< gist aspose-com-gists 1aa7b2386c8905d53478b28926a1b7e6 "pptx-to-html-hidden-slides.java" >}}

## Get a Free API License {#Get-a-Free-API-License}

Get [a free temporary license][14] to use Aspose.Slides for Android via Java without evaluation limitations.

## Online Demo

You can also try the [online PowerPoint to HTML converter][15], which is based on Aspose.Slides.

## Conclusion

In this article, you have learned how to convert PowerPoint PPTX or PPT presentations to HTML in Android. Furthermore, you have seen how to include hidden slides in PowerPoint to HTML conversion. You can learn more about the Android presentation manipulation API using [documentation][16]. Also, you can ask your questions via our [forum][17].

## See Also

*   [Convert PowerPoint PPTX/PPT to SVG in Android][18]




[1]: #Java-PowerPoint-to-HTML-Converter-API
[2]: #Convert-PowerPoint-PPTX-to-HTML-in-Java
[3]: #PPT-PPTX-to-HTML-Conversion-with-Hidden-Slides
[4]: https://products.aspose.com/slides/android-java/
[5]: https://downloads.aspose.com/slides/androidjava
[6]: https://apireference.aspose.com/slides/androidjava/com.aspose.slides/Presentation
[7]: https://apireference.aspose.com/slides/androidjava/com.aspose.slides/HtmlOptions
[8]: https://apireference.aspose.com/slides/androidjava/com.aspose.slides/Presentation#save-java.lang.String-int-
[9]: https://apireference.aspose.com/slides/androidjava/com.aspose.slides/Presentation#save-java.lang.String-int-
[10]: https://apireference.aspose.com/slides/androidjava/com.aspose.slides/Presentation
[11]: https://apireference.aspose.com/slides/androidjava/com.aspose.slides/HtmlOptions
[12]: https://apireference.aspose.com/slides/androidjava/com.aspose.slides/HtmlOptions#setShowHiddenSlides-boolean-
[13]: https://apireference.aspose.com/slides/androidjava/com.aspose.slides/Presentation#save-java.lang.String-int-
[14]: https://purchase.aspose.com/temporary-license
[15]: https://products.aspose.app/slides/conversion
[16]: https://docs.aspose.com/slides/androidjava/
[17]: https://forum.aspose.com/
[18]: https://blog.aspose.com/2021/09/27/convert-powerpoint-to-svg-in-android/





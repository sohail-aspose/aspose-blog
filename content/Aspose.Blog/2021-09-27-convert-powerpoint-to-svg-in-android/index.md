---
title: 'Convert PowerPoint PPTX/PPT to SVG in Android'
seoTitle: "PowerPoint to SVG in Android | PPTX to SVG, PPT to SVG | Source Code"
description: "Use Android PowerPoint API to convert PowerPoint presentations to SVG in Android. Convert PPTX to SVG and PPT to SVG in Android apps."
date: Mon, 27 Sep 2021 14:25:05 +0000
draft: false
url: /2021/09/27/convert-powerpoint-to-svg-in-android/
author: Usman Aziz
summary: 'PowerPoint to [SVG][1] conversion is often performed to display the presentations in Android applications. Various PowerPoint viewers also convert the presentations to SVG for slideshow. Accordingly, this article covers **how to convert PowerPoint PPTX or PPT presentations to SVG files using Android**.'
tags: ['Android PowerPoint to SVG Converter', 'PPT to SVG in Android', 'PPTX to SVG Android', 'PowerPoint to SVG Android']
categories: ['Aspose.Slides Product Family']
---



{{< figure align=center src="images/PowerPoint-to-SVG.jpg" alt="PowerPoint to SVG Android">}}


PowerPoint to [SVG][2] conversion is often performed to display the presentations in Android applications. Various PowerPoint viewers also convert the presentations to SVG for slideshow. Accordingly, this article covers **how to convert PowerPoint PPTX or PPT presentations to SVG files in Android**.

*   [PowerPoint to SVG Converter][3]
*   [Convert PPTX/PPT to SVG in Android][4]

## Android PowerPoint to SVG Converter {#PowerPoint-Presentation-to-SVG-Converter}

In order to convert PPTX or PPT presentations to SVG, we will use [Aspose.Slides for Android via Java][5]. It is a feature-rich Android API that lets you create, modify and convert presentations seamlessly. You can either download the API from the [downloads section][6] or install it by adding the following configurations in build.gradle.

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

## Convert PPTX or PPT Presentations to SVG in Android {#Convert-PPTX-PPT-to-SVG}

The following are the steps to convert a PowerPoint PPTX/PPT presentation to SVG in Android.

*   First, create an instance of [Presentation][7] class to load the presentation.
*   Loop through the slides in presentation and get reference of each slide in [ISlide][8] object.
*   Create a [FileOutputStream][9] object for the output SVG file.
*   Write slide data to the _FileOutputStream_ object using [ISlide.writeAsSvg()][10] method.
*   Finally, close the stream.

The following code sample shows how to convert PowerPoint PPTX/PPT to SVG.

{{< gist aspose-com-gists 7f1775b584fd0f5a3750b72916531f63 "powerpoint-to-svg.java" >}}

## Get a Free API License {#Get-a-Free-API-License}

You can use Aspose.Slides for Android via Java without evaluation limitations by requesting a [temporary license][11].

## Online Demo

Try the [online PowerPoint to SVG converter][12], which is based on Aspose.Slides.

## Conclusion

The PowerPoint presentations are often converted to SVG to embed their content in the applications. For such cases, this article covered PowerPoint to SVG conversion in Android apps. You can visit the [documentation][13] to explore other features of Aspose.Slides for Android via Java. Furthermore, you can feel free to let us know about your queries via our [forum][14].

## See Also

*   [Convert PowerPoint PPTX or PPT to PDF using Android API][15]




[1]: https://docs.fileformat.com/page-description-language/svg/
[2]: https://docs.fileformat.com/page-description-language/svg/
[3]: #PowerPoint-Presentation-to-SVG-Converter
[4]: #Convert-PPTX-PPT-to-SVG
[5]: https://products.aspose.com/slides/android-java/
[6]: https://downloads.aspose.com/slides/androidjava
[7]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation
[8]: https://apireference.aspose.com/slides/java/com.aspose.slides/ISlide
[9]: https://docs.oracle.com/javase/7/docs/api/java/io/FileOutputStream.html
[10]: https://apireference.aspose.com/slides/java/com.aspose.slides/ISlide#writeAsSvg-java.io.OutputStream-
[11]: https://purchase.aspose.com/temporary-license
[12]: https://products.aspose.app/slides/conversion/pptx-to-svg
[13]: https://docs.aspose.com/slides/androidjava
[14]: https://forum.aspose.com/
[15]: https://blog.aspose.com/2021/04/19/convert-powerpoint-ppt-pptx-to-pdf-in-android/





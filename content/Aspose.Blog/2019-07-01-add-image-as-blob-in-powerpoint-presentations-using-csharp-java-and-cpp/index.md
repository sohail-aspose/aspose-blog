---
title: 'Add Image as Blob in PowerPoint Presentations using C#, Java and C++'
date: Mon, 01 Jul 2019 18:59:02 +0000
draft: false
url: /2019/07/01/add-image-as-blob-in-powerpoint-presentations-using-csharp-java-and-cpp/
author: Mudassir
summary: ''
tags: []
categories: ['Aspose.Slides Product Family']
---

[![][1]](https://blog.aspose.com/wp-content/uploads/sites/2/2013/08/aspose-Slides-for-net_100.png) Hi guys! In today's blog, I would like to share my experience after using the latest Aspose.Slides 19.6 which has been enriched with improved image management support features. The best thing about Aspose.Slides is that it has a monthly release where .NET, Java, Android via Java, and C++ based APIs are published together. So, what's available in .NET based API is also available for Java, Android via Java and C++ based APIs. This way the users feel comfortable with API they are using and with the same features available across the board.

In the following sections, I am going to give you a walk through of what new features have been included and what improvements have been carried in API.

## Add Image as a BLOB in Presentation using C#

When dealing with PowerPoint presentation working with images in presentation play a pivotal role. Some times there is a requirement of adding huge images in the presentation. MS PowerPoint include such images as blobs. We have included a new method to **IImageCollection** interface and **ImageCollection** class to support adding large image as streams to treat them as BLOBs.

This example demonstrates how to include the large BLOB (image) and prevent a high memory consumption.

{{< gist aspose-com-gists a56eda38c01ad33dc653116c7bae4293 "Examples-CSharp-Presentations-Saving-AddBlobImageToPresentation-AddBlobImageToPresentation.cs" >}}

The similar Java-based example for this is:

{{< gist aspose-com-gists 1f55f0222bc39a382d831900e8de7400 "Examples-src-main-java-com-aspose-slides-examples-Presentation-Saving-AddBlobImageToPresentation-AddBlobImageToPresentation.java" >}}

The similar C++ based example for this is:

{{< gist aspose-com-gists 81aeb05e6d3a070aa76fdea22ed53bc7 "Examples-SlidesCPP-AddBlobImageToPresentation-AddBlobImageToPresentation.cpp" >}}

## Get Effective Background Values Of Slide

Now, Aspose.Slides provides support to represent the effective background of slide which contains information about effective fill format and effective effect format. To achieve this, **IBackgroundEffectiveData** interface and its implementation by **BackgroundEffectiveData** class have been added.

**CreateBackgroundEffective** method has been added to **IBaseSlide** interface and **BaseSlide** class. This method allows to get effective values for slides background. The following example shows how to get effective background values of slide.

{{< gist aspose-com-gists a56eda38c01ad33dc653116c7bae4293 "Examples-CSharp-Slides-Background-GetBackgroundEffectiveValues-GetBackgroundEffectiveValues.cs" >}}

The similar Java-based example for this is:

{{< gist aspose-com-gists 1f55f0222bc39a382d831900e8de7400 "Examples-src-main-java-com-aspose-slides-examples-Slides-Background-GetBackgroundEffectiveValues-GetBackgroundEffectiveValues.java" >}}

The similar C++ based example for this is:

{{< gist aspose-com-gists 81aeb05e6d3a070aa76fdea22ed53bc7 "Examples-SlidesCPP-GetBackgroundEffectiveValues-GetBackgroundEffectiveValues.cpp" >}}

## Saving Progress Updates in Percentage during rendering {#mce_24}

When using, Aspose.Slides some times one needs to save huge presentation files or convert huge presentation files to PDF. In such a situation, the API user may experience wait conditions till the time the saving or rendering process is completed and such a situation is sometimes annoying. In order to mitigate this, a new **IProgressCallback** interface has been added to **ISaveOptions** interface and **SaveOptions** abstract class.**IProgressCallback** interface represents a callback object for saving progress updates in percentage.

The following example exhibit the use of new future while exporting to PDF.

{{< gist aspose-com-gists a56eda38c01ad33dc653116c7bae4293 "Examples-CSharp-Presentations-Conversion-CovertToPDFWithProgressUpdate-CovertToPDFWithProgressUpdate.cs" >}} {{< gist aspose-com-gists a56eda38c01ad33dc653116c7bae4293 "Examples-CSharp-Presentations-Conversion-CovertToPDFWithProgressUpdate-ExportProgressHandler.cs" >}}

The similar Java-based example for this is:

{{< gist aspose-com-gists 1f55f0222bc39a382d831900e8de7400 "Examples-src-main-java-com-aspose-slides-examples-Presentation-Conversion-CovertToPDFWithProgressUpdate-CovertToPDFWithProgressUpdate.java" >}} {{< gist aspose-com-gists 1f55f0222bc39a382d831900e8de7400 "Examples-src-main-java-com-aspose-slides-examples-Presentation-Conversion-CovertToPDFWithProgressUpdate-ExportProgressHandler.java" >}}

The similar C++ based example for this is:

{{< gist aspose-com-gists 81aeb05e6d3a070aa76fdea22ed53bc7 "Examples-SlidesCPP-CovertToPDFWithProgressUpdate-CovertToPDFWithProgressUpdate.cpp" >}} {{< gist aspose-com-gists 81aeb05e6d3a070aa76fdea22ed53bc7 "Examples-SlidesCPP-CovertToPDFWithProgressUpdate-ExportProgressHandler.cpp" >}}

Wait, there's many other features, enhancement, and bug fixes included in this release. [Here you can get the detail!][2]

When time allows you can check out API [examples at Github][3], talk about this release and other API related issues in our [forum][4].




[1]: https://blog.aspose.com/wp-content/uploads/sites/2/2013/08/aspose-Slides-for-net_100.png "Aspose.Slides or .NET logo"
[2]: https://docs.aspose.com/display/slidesnet/Aspose.Slides+for+.NET+19.6+Release+Notes
[3]: https://github.com/aspose-slides/
[4]: https://forum.aspose.com/c/slides





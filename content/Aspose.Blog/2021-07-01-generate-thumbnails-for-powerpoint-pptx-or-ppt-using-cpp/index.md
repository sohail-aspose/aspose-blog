---
title: 'Generate Thumbnails for PowerPoint PPTX or PPT using C++'
seoTitle: "Generate Thumbnails for PowerPoint PPTX or PPT using C++"
description: "Generate thumbnails for PowerPoint PPTX/PPT files using C++. Use the C++ PowerPoint API to generate thumbnails with custom dimensions."
date: Thu, 01 Jul 2021 16:19:00 +0000
draft: false
url: /2021/07/01/generate-thumbnails-for-powerpoint-pptx-or-ppt-using-cpp/
author: Muhammad Ahmad
summary: 'Thumbnails are usually small-sized images that show the content of the files and make it easier to scroll through them. Microsoft PowerPoint shows the thumbnails for the slides that make it easy to scroll and open the desired slide. There might be situations where you want to make your own PowerPoint viewer application and want to generate the slide thumbnails dynamically. For such cases, this article will teach you **how to generate thumbnails of PowerPoint PPTX or PPT presentations programmatically using C++**.'
tags: ['Generate PPT Thumbnails C++', 'Generate PPTX Thumbnails C++', 'Generate PowerPoint Thumbnails C++']
categories: ['Aspose.Slides Product Family']
---



{{< figure align=center src="images/Generate-PPTX-Thumbnails.jpg" alt="Generate Thumbnails for PowerPoint PPTX or PPT using C++">}}


Thumbnails are usually small-sized images that show the content of the files and make it easier to scroll through them. Microsoft PowerPoint shows the thumbnails for the slides that make it easy to scroll and open the desired slide. There might be situations where you want to make your own PowerPoint viewer application and want to generate the slide thumbnails dynamically. For such cases, this article will teach you **how to generate thumbnails of PowerPoint PPTX or PPT presentations programmatically using C++**.

*   [C++ API for Generating Thumbnails for PowerPoint PPTX/PPT Files][1]
*   [Generate Thumbnails for PowerPoint PPTX/PPT Files using C++][2]
*   [Generate Thumbnails with User-Defined Dimensions][3]

## C++ API for Generating Thumbnails for PowerPoint PPTX/PPT Files {#CPP-API-for-Generating-Thumbnails-for-PowerPoint-PPTX-PPT-Files}

For generating thumbnails of PowerPoint files, we will use the simple and easy-to-use [Aspose.Slides for C++][4] API. It is a robust API that provides many features that help you create, read, and modify PowerPoint files. The API also provides the ability to generate thumbnails of the PowerPoint files. To begin, you can either install the API through [NuGet][5] or download it directly from the [Downloads][6] section.

```
PM> Install-Package Aspose.Slides.Cpp
```

## Generate Thumbnails for PowerPoint PPTX/PPT Files using C++ {#Generate-Thumbnails-for-PowerPoint-PPTX-PPT-Files-using-CPP}

The following are the steps to generate thumbnails of PowerPoint files using C++.

*   Load the PowerPoint file using the [Presentation][7] class.
*   Loop through the slides of the presentation.
*   Generate the thumbnail of each slide using the [ISlide->GetThumbnail(float scaleX, float scaleY)][8] method.
*   Save the thumbnail image using the [Bitmap->Save(const String & filename, const Imaging::ImageFormatPtr & format)][9] method.

The following sample code shows how to generate thumbnails of PowerPoint files using C++.

{{< gist aspose-com-gists b454f7366c0bdbe377d79ce2dd32a858 "Generate_Thumbnail.cpp" >}}

## Generate Thumbnails with User-Defined Dimensions {#Generate-Thumbnails-with-User-Defined-Dimensions}

While generating thumbnails of PowerPoint files, you can also specify the dimensions of the thumbnails according to your requirements. To specify custom dimensions while generating thumbnails, please follow the steps given below.

*   Load the PowerPoint file using the [Presentation][10] class.
*   Set the desired dimensions for the thumbnails.
*   Loop through the slides of the presentation.
*   Generate the thumbnail of each slide using the [ISlide->GetThumbnail(float scaleX, float scaleY)][11] method.
*   Save the thumbnail image using the [Bitmap->Save(const String & filename, const Imaging::ImageFormatPtr & format)][12] method.

The following sample code shows how to generate thumbnails with custom dimensions using C++.

{{< gist aspose-com-gists b454f7366c0bdbe377d79ce2dd32a858 "Generate_Thumbnail_With_Custom_Dimension.cpp" >}}

## Get a Free License

In order to try the API without evaluation limitations, you can request [a free temporary license][13].

## Conclusion

In this article, you have learned how to generate thumbnails for PowerPoint PPTX/PPT files using C++. Furthermore, you have seen how to generate thumbnails with custom dimensions. To learn more about the features provided by the Aspose.Slides for C++ API, you can visit the [official documentation][14]. In case of any questions, please feel free to reach us at our [free support forum][15].

## See Also

*   [Convert PowerPoint to JPG using C++][16]
*   [Convert PowerPoint Presentation to Word Document using C++][17]




[1]: #CPP-API-for-Generating-Thumbnails-for-PowerPoint-PPTX-PPT-Files
[2]: #Generate-Thumbnails-for-PowerPoint-PPTX-PPT-Files-using-CPP
[3]: #Generate-Thumbnails-with-User-Defined-Dimensions
[4]: https://products.aspose.com/slides/cpp
[5]: https://www.nuget.org/packages/Aspose.Slides.Cpp
[6]: https://downloads.aspose.com/slides/cpp
[7]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.presentation
[8]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.i_slide#a7bd377d403ff886232df21351c1fe783
[9]: https://apireference.aspose.com/slides/cpp/class/system.drawing.image#a4db9d0686ee892f6fb8fd6aebb4beb69
[10]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.presentation
[11]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.i_slide#a7bd377d403ff886232df21351c1fe783
[12]: https://apireference.aspose.com/slides/cpp/class/system.drawing.image#a4db9d0686ee892f6fb8fd6aebb4beb69
[13]: https://purchase.aspose.com/temporary-license
[14]: https://docs.aspose.com/slides/cpp/
[15]: https://forum.aspose.com/c/slides/11
[16]: https://blog.aspose.com/2021/03/06/convert-powerpoint-to-jpg-using-cpp/
[17]: https://blog.aspose.com/2021/09/10/convert-powerpoint-presentation-to-word-document-using-cpp/






---
title: 'Convert PowerPoint to JPG using C++'
seoTitle: "Convert PowerPoint to JPG using C++ | PPTX to JPG C++"
description: "Convert PowerPoint Slides to JPG images using C++. Convert PPTX slides to JPG images from within your C++ applications using Aspose.Slides for C++ API."
date: Sat, 06 Mar 2021 19:48:18 +0000
draft: false
url: /2021/03/06/convert-powerpoint-to-jpg-using-cpp/
author: Muhammad Ahmad
summary: 'Microsoft PowerPoint is a powerful and feature-rich software that allows you to create beautiful slides to use in your meetings. Even though PowerPoint is great for presentation purposes, it is not ideal for displaying content on the web, especially if the content is for information purposes only. For this, the better option would be to convert the [PPTX][1] files to images such as [JPEG][2] or [PNG][3]. In this article, you will learn **how to convert PowerPoint to JPG programmatically using C++**.'
tags: ['C++ Convert PowerPoint to JPG', 'Convert PPTX to JPG C++', 'Convert PowerPoint to JPG using C++']
categories: ['Aspose.Slides Product Family']
---



{{< figure align=center src="images/PowerPoint-to-Image-in-C.png" alt="Convert PowerPoint to JPG using C++">}}


Microsoft PowerPoint is a powerful and feature-rich software that allows you to create beautiful slides to use in your meetings. Even though PowerPoint is great for presentation purposes, it is not ideal for displaying content on the web, especially if the content is for information purposes only. For this, the better option would be to convert the [PPTX][4] files to images such as [JPEG][5] or [PNG][6]. In this article, you will learn **how to convert PowerPoint to JPG programmatically using C++**.

*   [C++ API for Converting PowerPoint to JPG][7]
*   [Convert PowerPoint to JPG with Custom Image Dimensions][8]
*   [Get a Free License][9]

**TIP:**

Aspose online [PowerPoint to JPG converter][10] is a live implementation of the PowerPoint to JPG conversion process, so you will do well to check it out.

## C++ API for Converting PowerPoint to JPG {#CPP-API-for-Converting-PowerPoint-to-JPG}

[Aspose.Slides for C++][11] is a feature-rich API that allows you to create and change PowerPoint files without requiring Microsoft PowerPoint. Furthermore, the API supports converting PowerPoint slides to JPG images. You can either install the API through [NuGet][12] or download it directly from the [Downloads][13] section.

```
PM> Install-Package Aspose.Slides.Cpp
```

## Convert PPTX to JPG using C++

The following are the steps to convert PowerPoint files to JPG images.

*   Load the PPTX file using the [Presentation][14] class.
*   Retrieve the slides using the [Presentation->get\_Slides()][15] method and iterate over them.
*   Get the slide's image using the [ISlide->GetThumbnail (float _scaleX_, float _scaleY_)][16] method and assign it to a [Bitmap][17] object.
*   Save the image using the [Bitmap->Save (const String & filename, const Imaging::ImageFormatPtr & format)][18] method.

The following is the sample code to convert PPTX files to JPG images using C++

{{< gist aspose-com-gists ad5a53560fc1c9bb203cb45d1fe3c2ff "Convert-Slides-To-JPG.cpp" >}}

### Source PowerPoint File



{{< figure align=center src="images/SourceSlides.png" alt="PowerPoint Source File Image">}}


### Converted JPG Images



{{< figure align=center src="images/ConvertedJPGImages-1024x320.png" alt="Converted JPG Images">}}


## Convert PowerPoint to JPG with Custom Image Dimensions {#Convert-PowerPoint-to-JPG-with-Custom-Image-Dimensions}

With Aspose.Slides for C++, you can customize the dimensions of the generated images according to your requirements. The following are the steps to convert PowerPoint slides to JPG images with custom dimensions.

*   Load the PPTX file using the [Presentation][19] class.
*   Specify the scaling values for the x-axis and y-axis using the slide's width and height, respectively.
*   Retrieve the slides using the [Presentation->get\_Slides()][20] method and iterate over them.
*   Get the slide's image using the [ISlide->GetThumbnail (float _scaleX_, float _scaleY_)][21] method and assign it to a [Bitmap][22] object.
*   Save the image using the [Bitmap->Save (const String & filename, const Imaging::ImageFormatPtr & format)][23] method.

The following is the sample code for converting PowerPoint presentations to JPG images with custom dimensions.

{{< gist aspose-com-gists ad5a53560fc1c9bb203cb45d1fe3c2ff "Convert-Slides-To-JPG-With-Custom-Dimensions.cpp" >}}

## Get a Free License {#Get-a-Free-License}

You can try the API without evaluation limitations by requesting [a free temporary license][24].

## Conclusion

In this article, you have learned how to convert PowerPoint slides to JPG images using C++. Furthermore, you saw how to provide custom dimensions for the generated images. Aspose.Slides for C++ offers many other features for working with PowerPoint files. You can explore the API in detail by using the [official documentation][25]. If you have any questions, please feel free to contact us on the [forum][26].

## See Also

*   [Convert PowerPoint to PDF using C++][27]




[1]: https://docs.fileformat.com/presentation/pptx/
[2]: https://docs.fileformat.com/image/jpeg/
[3]: https://docs.fileformat.com/image/png/
[4]: https://docs.fileformat.com/presentation/pptx/
[5]: https://docs.fileformat.com/image/jpeg/
[6]: https://docs.fileformat.com/image/png/
[7]: #CPP-API-for-Converting-PowerPoint-to-JPG
[8]: #Convert-PowerPoint-to-JPG-with-Custom-Image-Dimensions
[9]: #Get-a-Free-License
[10]: https://products.aspose.app/slides/conversion/ppt-to-jpg
[11]: https://products.aspose.com/slides/cpp
[12]: https://www.nuget.org/packages/Aspose.Slides.Cpp
[13]: https://downloads.aspose.com/slides/cpp
[14]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.presentation
[15]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.presentation#a9981b38f5a01d9fa5482f05b0a75974c
[16]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.i_slide#a7bd377d403ff886232df21351c1fe783
[17]: https://apireference.aspose.com/slides/cpp/class/system.drawing.bitmap
[18]: https://apireference.aspose.com/slides/cpp/class/system.drawing.image#a4db9d0686ee892f6fb8fd6aebb4beb69
[19]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.presentation
[20]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.presentation#a9981b38f5a01d9fa5482f05b0a75974c
[21]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.i_slide#a7bd377d403ff886232df21351c1fe783
[22]: https://apireference.aspose.com/slides/cpp/class/system.drawing.bitmap
[23]: https://apireference.aspose.com/slides/cpp/class/system.drawing.image#a4db9d0686ee892f6fb8fd6aebb4beb69
[24]: https://purchase.aspose.com/temporary-license
[25]: https://docs.aspose.com/slides/cpp/
[26]: https://forum.aspose.com/c/slides/11
[27]: https://blog.aspose.com/2021/03/03/convert-powerpoint-to-pdf-using-cpp/






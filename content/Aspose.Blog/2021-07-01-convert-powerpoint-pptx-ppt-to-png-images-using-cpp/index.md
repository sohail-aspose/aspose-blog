---
title: 'Convert PowerPoint PPTX/PPT to PNG Images using C++'
seoTitle: "Convert PowerPoint PPTX/PPT to PNG Images using C++"
description: "Convert PowerPoint PPTX/PPT files to PNG images using C++. Use the C++ PowerPoint API to convert presentation slides to PNG images."
date: Thu, 01 Jul 2021 17:02:00 +0000
draft: false
url: /2021/07/01/convert-powerpoint-pptx-ppt-to-png-images-using-cpp/
author: Muhammad Ahmad
summary: 'There might be situations where you need to convert your PowerPoint files to images. For example, to generate thumbnails or to add images of the slides to a document. For such cases, converting PowerPoint files to PNG format will prove to be helpful as [PNG][1] is a popular raster graphics format that supports lossless compression. To that end, this article will teach you **how to convert your PowerPoint presentations to PNG images using C++**.'
tags: ['Convert PPT to PNG C++', 'Convert PPTX to PNG C++', 'Convert PowerPoint to PNG C++']
categories: ['Aspose.Slides Product Family']
---



{{< figure align=center src="images/PowerPoint-to-PNG-Image.jpg" alt="PPT to PNG Images using C++">}}


There might be situations where you need to convert your PowerPoint files to images. For example, to generate thumbnails or to add images of the slides to a document. For such cases, converting PowerPoint files to PNG format will prove to be helpful as [PNG][2] is a popular raster graphics format that supports lossless compression. To that end, this article will teach you **how to convert your PowerPoint presentations to PNG images using C++**.

*   [C++ API for Converting PowerPoint PPTX/PPT Files to PNG Format][3]
*   [Converting PowerPoint PPTX/PPT Files to PNG Images using C++][4]

## C++ API for Converting PowerPoint PPTX/PPT Files to PNG Format {#CPP-API-for-Converting-PowerPoint-PPTX-PPT-Files-to-PNG-Format}

[Aspose.Slides for C++][5] is a robust and feature-rich API that allows you to create, read, and update PowerPoint files without requiring Microsoft PowerPoint to be installed. Furthermore, the API supports converting PowerPoint presentations to PNG images. You can either install the API through [NuGet][6] or download it directly from the [Downloads][7] section.

```
PM> Install-Package Aspose.Slides.Cpp
```

## Convert PowerPoint PPTX/PPT Files to PNG Images using C++ {#Convert-PowerPoint-PPTX-PPT-Files-to-PNG-Images-using-CPP}

The following are the steps to convert PowerPoint files to PNG images using C++.

*   Load the PowerPoint file using the [Presentation][8] class.
*   Set the desired dimensions for the images to be generated.
*   Loop through the slides of the presentation.
*   Generate the image of each slide using the [ISlide->GetThumbnail(float scaleX, float scaleY)][9] method.
*   Save the PNG image using the [Bitmap->Save(const String & filename, const Imaging::ImageFormatPtr & format)][10] method.

The following sample code shows how to convert PowerPoint files to PNG images using C++.

{{< gist aspose-com-gists 0046740d3d811e40fa9a6566be50c906 "Convert_PowerPoint_To_PNG.cpp" >}}

## Get a Free License

In order to try the API without evaluation limitations, you can request [a free temporary license][11].

## Conclusion

In this article, you have learned how to convert PowerPoint files to PNG images using C++. We used the Aspose.Slides for C++ API to achieve this. It is a powerful API that provides a bunch of additional features for working with PowerPoint files. You can explore the API in detail by visiting the [official documentation][12]. In case of any queries, please feel free to reach us at our [free support forum][13].

## See Also

*   [Convert PowerPoint Presentations to SVG using C++][14]
*   [Convert PowerPoint to JPG using C++][15]




[1]: https://docs.fileformat.com/image/png/
[2]: https://docs.fileformat.com/image/png/
[3]: #CPP-API-for-Converting-PowerPoint-PPTX-PPT-Files-to-PNG-Format
[4]: #Convert-PowerPoint-PPTX-PPT-Files-to-PNG-Images-using-CPP
[5]: https://products.aspose.com/slides/cpp
[6]: https://www.nuget.org/packages/Aspose.Slides.Cpp
[7]: https://downloads.aspose.com/slides/cpp
[8]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.presentation
[9]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.i_slide#a7bd377d403ff886232df21351c1fe783
[10]: https://apireference.aspose.com/slides/cpp/class/system.drawing.image#a4db9d0686ee892f6fb8fd6aebb4beb69
[11]: https://purchase.aspose.com/temporary-license
[12]: https://docs.aspose.com/slides/cpp/
[13]: https://forum.aspose.com/c/slides/11
[14]: https://blog.aspose.com/2021/09/16/convert-powerpoint-presentations-to-svg-using-cpp/
[15]: https://blog.aspose.com/2021/03/06/convert-powerpoint-to-jpg-using-cpp/






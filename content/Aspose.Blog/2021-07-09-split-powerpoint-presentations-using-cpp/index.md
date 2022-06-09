---
title: 'Split PowerPoint Presentations using C++'
seoTitle: "Split PowerPoint Presentations using C++ | C++ PowerPoint API"
description: "Split PowerPoint presentations using C++. Use the C++ PowerPoint API to split each slide of a presentation and save it as a separate file."
date: Fri, 09 Jul 2021 14:08:00 +0000
draft: false
url: /2021/07/09/split-powerpoint-presentations-using-cpp/
author: Muhammad Ahmad
summary: 'There might be scenarios where you need to split PowerPoint presentations into multiple files. For example, your presentation may have various sections, and you want each section to be in a separate file. To that end, this article will teach you **how to split PowerPoint PPTX/PPT presentations using C++**.'
tags: ['Split PPT Presentation C++', 'Split PPTX Presentation C++', 'Split PowerPoint Presentation C++']
categories: ['Aspose.Slides Product Family']
---



{{< figure align=center src="images/Split-PowerPoint-Presentation.jpg" alt="Split PowerPoint Presentations using C++">}}


There might be scenarios where you need to split PowerPoint presentations into multiple files. For example, your presentation may have various sections, and you want each section to be in a separate file. To that end, this article will teach you **how to split PowerPoint PPTX/PPT presentations using C++**.

*   [C++ API for Splitting PowerPoint Presentations][1]
*   [Split a PowerPoint Presentation using C++][2]

## C++ API for Splitting PowerPoint Presentations {#CPP-API-for-Splitting-PowerPoint-Presentations}

[Aspose.Slides for C++][3] is a powerful and feature-rich API that allows you to create, read and modify PowerPoint files without requiring Microsoft PowerPoint to be installed. Furthermore, the API supports splitting PowerPoint presentations. You can either install the API through [NuGet][4] or download it directly from the [Downloads][5] section.

```
PM> Install-Package Aspose.Slides.Cpp
```

## Split a PowerPoint Presentation using C++ {#Split-a-PowerPoint-Presentation-using-CPP}

The following are the steps to split a PowerPoint presentation using C++.

*   Load the PowerPoint file using the [Presentation][6] class.
*   Iterate through the slides of the presentation.
*   Within the loop, create an instance of the [Presentation][7] class to represent a new PowerPoint file.
*   Remove the default slide.
*   Add the slide using the [Presentation->get\_Slides()->AddClone(System::SharedPtr<ISlide> sourceSlide)][8] method.
*   Save the presentation using the [Presentation->Save(System::String fname, Export::SaveFormat format)][9] method.

The following sample code shows how to split a PowerPoint presentation using C++.

{{< gist aspose-com-gists 77104b44d5371e3944d2f7d2e9b3a6de "Split_Presentation.cpp" >}}

## Get a Free License

In order to try the API without evaluation limitations, you can request [a free temporary license][10].

## Conclusion

In this article, you have learned how to split PowerPoint presentations using C++. The shared code snippet shows how to split PowerPoint files with just a few lines of code. Aspose.Slides for C++ API provides a bunch of additional features for working with PowerPoint files. You can explore the API in detail by visiting the [official documentation][11]. In case of any queries, please feel free to reach us at our [free support forum][12].

## See Also

*   [Generate Thumbnails for PowerPoint PPTX or PPT using C++][13]
*   [Convert PowerPoint to XAML using C++][14]
*   [Convert PowerPoint PPTX/PPT to TIFF using C++][15]




[1]: #CPP-API-for-Splitting-PowerPoint-Presentations
[2]: #Split-a-PowerPoint-Presentation-using-CPP
[3]: https://products.aspose.com/slides/cpp
[4]: https://www.nuget.org/packages/Aspose.Slides.Cpp
[5]: https://downloads.aspose.com/slides/cpp
[6]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.presentation
[7]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.presentation
[8]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.i_slide_collection#a0c84ed19c8b1730eb8010613a1c229ee
[9]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.presentation#afcd59ec697bf05c10f78c3869de2ec9e
[10]: https://purchase.aspose.com/temporary-license
[11]: https://docs.aspose.com/slides/cpp/
[12]: https://forum.aspose.com/c/slides/11
[13]: https://blog.aspose.com/2021/07/01/generate-thumbnails-for-powerpoint-pptx-or-ppt-using-cpp/
[14]: https://blog.aspose.com/2021/09/13/convert-powerpoint-to-xaml-using-cpp/
[15]: https://blog.aspose.com/2021/09/08/convert-powerpoint-pptx-ppt-to-tiff-using-cpp/






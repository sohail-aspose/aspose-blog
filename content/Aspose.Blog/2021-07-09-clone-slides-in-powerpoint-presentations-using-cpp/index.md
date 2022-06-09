---
title: 'Clone Slides in PowerPoint Presentations using C++'
seoTitle: "Clone Slides in PowerPoint Presentations using C++"
description: "Clone a slide in PowerPoint files using C++. Clone a slide to the end or at a specified position within the same file or in another file."
date: Fri, 09 Jul 2021 18:11:00 +0000
draft: false
url: /2021/07/09/clone-slides-in-powerpoint-presentations-using-cpp/
author: Muhammad Ahmad
summary: 'There might be situations where you need to create a copy of a slide. For example, you need to create a new slide that is similar to an existing slide. In such cases, you can clone the slide in the same presentation or another presentation and modify it according to your requirements. To that end, this article will teach you **how to clone slides within the same PowerPoint presentation or to another PowerPoint presentation using C++**.'
tags: ['Clone Slide in PPT C++', 'Clone Slide in PPTX C++', 'Clone Slide in PowerPoint C++']
categories: ['Aspose.Slides Product Family']
---



{{< figure align=center src="images/Clone-Slides-in-PowerPoint.jpg" alt="Clone Slides in PowerPoint Presentations using C++">}}


There might be situations where you need to create a copy of a slide. For example, you need to create a new slide that is similar to an existing slide. In such cases, you can clone the slide in the same presentation or another presentation and modify it according to your requirements. To that end, this article will teach you **how to clone slides within the same PowerPoint presentation or to another PowerPoint presentation using C++**.

*   [C++ API for Cloning PowerPoint Slides][1]
*   [Cloning a Slide within a PowerPoint Presentation][2]
    *   [Clone a Slide to the End of the PowerPoint Presentation using C++][3]
    *   [Clone a Slide to a Specific Position using C++][4]
*   [Cloning a Slide to Another PowerPoint Presentation][5]
    *   [Clone a Slide to the End of Another PowerPoint Presentation using C++][6]
    *   [Clone a Slide to a Specific Position in Another PowerPoint Presentation using C++][7]

## C++ API for Cloning PowerPoint Slides {#CPP-API-for-Cloning-PowerPoint-Slides}

[Aspose.Slides for C++][8] is a C++ API for working with PowerPoint presentations. It enables you to create, read and modify PowerPoint files without needing additional software. Furthermore, the API supports cloning PowerPoint slides. You can either install the API through [NuGet][9] or download it directly from the [Downloads][10] section.

## Cloning a Slide within a PowerPoint Presentation {#Cloning-a-Slide-within-a-PowerPoint-Presentation}

You can clone a slide to the end of the presentation or at a specific position. In the following sections, we will explore both of these scenarios with code samples.

### Clone a Slide to the End of the PowerPoint Presentation using C++ {#Clone-a-Slide-to-the-End-of-the-PowerPoint-Presentation-using-CPP}

The following are the steps to clone a slide to the end of a PowerPoint presentation.

*   Load the PowerPoint file using the [](https://apireference.aspose.com/slides/cpp/class/aspose.slides.presentation)[Presentation][11] class.
*   Retrieve the slides using the [Presentation->get\_Slides()][12] method.
*   Clone the slide using the [ISlideCollection->AddClone(System::SharedPtr<ISlide> sourceSlide)][13] method.
*   Save the presentation using the [Presentation->Save(System::String fname, Export::SaveFormat format)][14] method.

The following sample code shows how to clone a slide to the end of a PowerPoint presentation using C++.

{{< gist aspose-com-gists 724b75c8a9bfaec816cedc23d3db0768 "Clone_Slide_At_End.cpp" >}}

### Clone a Slide to a Specific Position using C++ {#Clone-a-Slide-to-a-Specific-Position-using-CPP}

The following are the steps to clone a slide to a specific position using C++.

*   Load the PowerPoint file using the [Presentation][15] class.
*   Retrieve the slides using the [Presentation->get\_Slides()][16] method.
*   Insert the slide clone at the desired position using the [ISlideCollection->InsertClone(int32\_t index,System::SharedPtr<ISlide> sourceSlide)][17] method.
*   Save the presentation using the [Presentation->Save(System::String fname, Export::SaveFormat format)][18] method.

The following sample code shows how to clone a slide to a specific position using C++.

{{< gist aspose-com-gists 724b75c8a9bfaec816cedc23d3db0768 "Clone_Slide_At_Specific_Position.cpp" >}}

## Cloning a Slide to Another PowerPoint Presentation {#Cloning-a-Slide-to-Another-PowerPoint-Presentation}

You can clone a slide to the end or at a specific position of another presentation. In the following sections, we will explore both of these scenarios with code samples.

### Clone a Slide to the End of Another PowerPoint Presentation using C++ {#Clone-a-Slide-to-the-End-of-Another-PowerPoint-Presentation-using-CPP}

The following are the steps to clone a slide to the end of another PowerPoint presentation.

*   Load the source PowerPoint file using the [Presentation][19] class.
*   Load the destination PowerPoint file using the [Presentation][20] class.
*   Retrieve the slides of the destination file using the [Presentation->get\_Slides()][21] method.
*   Add the slide clone to the destination presentation using the [](https://apireference.aspose.com/slides/cpp/class/aspose.slides.i_slide_collection#a92e77e45347cf5351817a98ac1051b5f)[ISlideCollection->AddClone(System::SharedPtr<ISlide> sourceSlide)][22] method.
*   Save the destination presentation using the [Presentation->Save(System::String fname, Export::SaveFormat format)][23] method.

The following sample code shows how to clone a slide to the end of another PowerPoint presentation using C++.

{{< gist aspose-com-gists 724b75c8a9bfaec816cedc23d3db0768 "Clone_Slide_At_End_Of_Another_Presentation.cpp" >}}

### Clone a Slide to a Specific Position in Another PowerPoint Presentation using C++ {#Clone-a-Slide-to-a-Specific-Position-in-Another-PowerPoint-Presentation-using-CPP}

The following are the steps to clone a slide to a specific position in another PowerPoint presentation.

*   Load the source PowerPoint file using the [Presentation][24] class.
*   Load the destination PowerPoint file using the [Presentation][25] class.
*   Retrieve the slides of the destination file using the [Presentation->get\_Slides()][26] method.
*   Insert the slide clone at the specificed position in the destination presentation using the [](https://apireference.aspose.com/slides/cpp/class/aspose.slides.i_slide_collection#a0c84ed19c8b1730eb8010613a1c229ee)[ISlideCollection->InsertClone(int32\_t index,System::SharedPtr<ISlide> sourceSlide)][27] method.
*   Save the destination presentation using the [Presentation->Save(System::String fname, Export::SaveFormat format)][28] method.

The following sample code shows how to clone a slide to a specific position in another PowerPoint presentation using C++.

{{< gist aspose-com-gists 724b75c8a9bfaec816cedc23d3db0768 "Clone_Slide_At_Specific_Position_Of_Another_Presentation.cpp" >}}

## Get a Free License

In order to try the API without evaluation limitations, you can request [a free temporary license][29].

## Conclusion

In this article, you have learned how to clone slides in PowerPoint presentations using C++. Specifically, you have learned how to clone a slide to the end or at a specific position of the same presentation or in another presentation. Aspose.Slides for C++ is a robust API that provides many additional features for working with PowerPoint files. You can explore the API in detail by visiting the [official documentation][30]. In case of any queries, please feel free to reach us at our [free support forum][31].

## See Also

*   [Split PowerPoint Presentations using C++][32]
*   [Working with Shapes in PowerPoint presentations using C++][33]




[1]: #CPP-API-for-Cloning-PowerPoint-Slides
[2]: #Cloning-a-Slide-within-a-PowerPoint-Presentation
[3]: #Clone-a-Slide-to-the-End-of-the-PowerPoint-Presentation-using-CPP
[4]: #Clone-a-Slide-to-a-Specific-Position-using-CPP
[5]: #Cloning-a-Slide-to-Another-PowerPoint-Presentation
[6]: #Clone-a-Slide-to-the-End-of-Another-PowerPoint-Presentation-using-CPP
[7]: #Clone-a-Slide-to-a-Specific-Position-in-Another-PowerPoint-Presentation-using-CPP
[8]: https://products.aspose.com/slides/cpp
[9]: https://www.nuget.org/packages/Aspose.Slides.Cpp
[10]: https://downloads.aspose.com/slides/cpp
[11]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.presentation
[12]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.presentation#a9981b38f5a01d9fa5482f05b0a75974c
[13]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.i_slide_collection#a0c84ed19c8b1730eb8010613a1c229ee
[14]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.presentation#afcd59ec697bf05c10f78c3869de2ec9e
[15]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.presentation
[16]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.presentation#a9981b38f5a01d9fa5482f05b0a75974c
[17]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.i_slide_collection#a92e77e45347cf5351817a98ac1051b5f
[18]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.presentation#afcd59ec697bf05c10f78c3869de2ec9e
[19]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.presentation
[20]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.presentation
[21]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.presentation#a9981b38f5a01d9fa5482f05b0a75974c
[22]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.i_slide_collection#a0c84ed19c8b1730eb8010613a1c229ee
[23]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.presentation#afcd59ec697bf05c10f78c3869de2ec9e
[24]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.presentation
[25]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.presentation
[26]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.presentation#a9981b38f5a01d9fa5482f05b0a75974c
[27]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.i_slide_collection#a92e77e45347cf5351817a98ac1051b5f
[28]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.presentation#afcd59ec697bf05c10f78c3869de2ec9e
[29]: https://purchase.aspose.com/temporary-license
[30]: https://docs.aspose.com/slides/cpp/
[31]: https://forum.aspose.com/c/slides/11
[32]: https://blog.aspose.com/2021/07/09/split-powerpoint-presentations-using-cpp/
[33]: https://blog.aspose.com/2021/04/20/working-with-shapes-in-powerpoint-presentations-using-cpp/






---
title: 'Extract Text from PowerPoint Files using C++'
seoTitle: "Extract Text from PowerPoint Files using C++ | Extract Text from Slides"
description: "Extract text from PowerPoint presentations using C++. Extract text from a particular slide or from the entire presentation within your C++ applications."
date: Sat, 10 Apr 2021 09:38:56 +0000
draft: false
url: /2021/04/10/extract-text-from-powerpoint-files-using-cpp/
author: Muhammad Ahmad
summary: 'You may find yourself in scenarios where you have to save the text of the PowerPoint file to a database or some file. Doing this task manually will be time-consuming and less efficient. The better way would be to do the extraction programmatically. To that end, this article will teach you **how to extract text from PowerPoint files using C++**.'
tags: ['Extract Text from PPTX using C++', 'Extract Text from PowerPoint Files C++', 'Extract Text from PowerPoint Slides C++']
categories: ['Aspose.Slides Product Family']
---



{{< figure align=center src="images/Extract-Text-from-PowerPoint.jpg" alt="Extract Text for PowerPoint Files using C++">}}


You may find yourself in scenarios where you have to save the text of PowerPoint files to a database or some file. Doing this task manually will be time-consuming and less efficient. The better way would be to do the extraction programmatically. To that end, this article will teach you **how to extract text from PowerPoint files using C++**.

*   [C++ API to Extract Text from PowerPoint Files][1]
*   [Extracting Text from a PowerPoint Slide using C++][2]
*   [Extracting Text from a PowerPoint Presentation using C++][3]
*   [Get a Free License][4]

## C++ API to Extract Text from PowerPoint Files {#CPP-API-to-Extract-Text-from-PowerPoint-Files}

[Aspose.Slides for C++][5] is a native C++ library that helps you to automate your PowerPoint-related tasks. The API supports creating, reading, and modifying PowerPoint presentations. Furthermore, the API also provides you the ability to extract text from your PowerPoint files. You can either install the API through [NuGet][6] or download it directly from the [Downloads][7] section.

```
PM> Install-Package Aspose.Slides.Cpp
```

## Extracting Text from a PowerPoint Slide using C++ {#Extracting-Text-from-a-PowerPoint-Slide-using-CPP}

The following are the steps to extract text from a PowerPoint slide.

*   Firstly, load the PowerPoint presentation using the [Presentation][8] class.
*   Retrieve the text frames from the slide using [SlideUtil::GetAllTextBoxes (System::SharedPtr<IBaseSlide> slide)][9] method.
*   Loop through the text frames.
*   Within the loop, access the paragraphs using the [ITextFrame->get\_Paragraphs()][10] method.
*   Loop through the paragraphs and access the portions using [IParagraph->get\_Portions()][11] method.
*   Retrieve the text from each portion using [IPortion->get\_Text()][12] method.

The following is the sample code to extract text from a PowerPoint slide using C++.

{{< gist aspose-com-gists c6cba3880eb328b23824b943bc37a45e "Extract-Text-From-Slide.cpp" >}}

## Extracting Text from a PowerPoint Presentation using C++ {#Extracting-Text-from-a-PowerPoint-Presentation-using-CPP}

The following are the steps to extract text from a PowerPoint presentation.

*   Firstly, load the PowerPoint presentation using the [Presentation][13] class.
*   Retrieve the text frames from the entire presentation using [SlideUtil::GetAllTextFrames (System::SharedPtr<IPresentation> pres, bool withMasters)][14] method.
*   Loop through the text frames.
*   Within the loop, access the paragraphs using the [ITextFrame->get\_Paragraphs()][15] method.
*   Loop through the paragraphs and access the portions using [IParagraph->get\_Portions()][16] method.
*   Retrieve the text from each portion using [IPortion->get\_Text()][17] method.

The following is the sample code to extract text from a PowerPoint presentation using C++.

{{< gist aspose-com-gists c6cba3880eb328b23824b943bc37a45e "Extract-Text-From-Presentation.cpp" >}}

## Get a Free License {#Get-a-Free-License}

You can request [a free temporary license][18] to try the API without evaluation limitations.

## Conclusion

In this article, you have learned how to extract text from PowerPoint files using C++. Specifically, you have learned how to extract text from a particular PowerPoint slide or an entire PowerPoint presentation. Aspose.Slides for C++ provides a bunch of additional features for working with presentations. You can explore the API in detail by visiting the [official documentation][19]. In case of any questions, please feel free to contact us on the [free support forum][20].

## See Also

*   [Create Charts in PowerPoint Presentations using C++][21]




[1]: #CPP-API-to-Extract-Text-from-PowerPoint-Files
[2]: #Extracting-Text-from-a-PowerPoint-Slide-using-CPP
[3]: #Extracting-Text-from-a-PowerPoint-Presentation-using-CPP
[4]: #Get-a-Free-License
[5]: https://products.aspose.com/slides/cpp
[6]: https://www.nuget.org/packages/Aspose.Slides.Cpp
[7]: https://downloads.aspose.com/slides/cpp
[8]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.presentation
[9]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.util.slide_util#a97da94e3fc5230cdfc0e30b444c127df
[10]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.i_text_frame#a57d8f1829a8e0c94ca90eddd8c0f2fad
[11]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.i_paragraph#a9a026fad1445f25b3acac30325875286
[12]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.i_portion#a770e826f864a319304dfd1cf21d38485
[13]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.presentation
[14]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.util.slide_util#a5a0aebdc520e5258c8a1f665fdb8be12
[15]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.i_text_frame#a57d8f1829a8e0c94ca90eddd8c0f2fad
[16]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.i_paragraph#a9a026fad1445f25b3acac30325875286
[17]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.i_portion#a770e826f864a319304dfd1cf21d38485
[18]: https://purchase.aspose.com/temporary-license
[19]: https://docs.aspose.com/slides/cpp/
[20]: https://forum.aspose.com/c/slides/11
[21]: https://blog.aspose.com/2021/04/02/create-charts-in-powerpoint-presentations-using-cpp/






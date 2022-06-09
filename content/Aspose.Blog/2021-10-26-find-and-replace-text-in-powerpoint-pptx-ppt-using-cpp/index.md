---
title: 'Find and Replace Text in PowerPoint PPTX/PPT using C++'
seoTitle: "Find and Replace Text in PowerPoint PPTX/PPT using C++"
description: "Find and replace text in PowerPoint presentations using C++. Use the C++ PowerPoint API to find and replace text with just a few lines of code."
date: Tue, 26 Oct 2021 11:19:46 +0000
draft: false
url: /2021/10/26/find-and-replace-text-in-powerpoint-pptx-ppt-using-cpp/
author: Muhammad Ahmad
summary: 'Finding and replacing text is a common task that you may need to do often. In the case of multiple files, doing this programmatically will prove to be more efficient. To that end, this article will teach you **how to find and replace text in PowerPoint files using C++**.'
tags: ['Find and Replace Text in PowerPoint C++', 'Replace Text in PowerPoint Files C++', 'Search and Replace Text in PowerPoint C++']
categories: ['Aspose.Slides Product Family']
---

Finding and replacing text is a common task that you may need to do often. In the case of multiple files, doing this programmatically will prove to be more efficient. To that end, this article will teach you **how to find and replace text in PowerPoint files using C++**.

*   [C++ API for Finding and Replacing Text in PowerPoint Presentations][1]
*   [Find and Replace Text in PowerPoint Files][2]

## C++ API for Finding and Replacing Text in PowerPoint Presentations {#CPP-API-for-Finding-and-Replacing-Text-in-PowerPoint-Presentations}

[Aspose.Slides for C++][3] is a C++ API for working with PowerPoint files. It enables you to create, read and update PowerPoint files without needing Microsoft PowerPoint to be installed. Furthermore, the API allows you to find and replace text in PowerPoint presentations. You can either install the API through [NuGet][4] or download it directly from the [Downloads][5] section.

```
PM> Install-Package Aspose.Slides.Cpp
```

## Find and Replace Text in PowerPoint Files using C++ {#Find-and-Replace-Text-in-PowerPoint-Files-using-CPP}

The following are the steps to find and replace text in PowerPoint files.

*   Firstly, load the PowerPoint file using the [Presentation][6] class.
*   Loop through the slides of the presentation.
*   Within the loop, retrieve the text frames in an [ITextFrame][7] array.
*   Loop through the array of the text frames.
*   Within the loop, iterate through the paragraphs in each [ITextFrame][8].
*   Iterate through the portions in each [IParagraph][9].
*   For each [IPortion][10], check if it contains the desired text. If it exists, then replace the text.
*   Finally, save the presentation using the [Presentation->Save(System::String fname, Export::SaveFormat format)][11] method.

The following sample code shows how to find and replace text in PowerPoint files using C++.



## Get a Free License

In order to try the API without evaluation limitations, you can request [a free temporary license][12].

## Conclusion

In this article, you have learned how to find and replace text in PowerPoint presentations using C++. The shared code snippet shows how to achieve that with just a few lines of code. Aspose.Slides for C++ is a robust and feature-rich API that provides many additional features for automating your PowerPoint workflows. You can explore the API in detail by visiting the [official documentation][13]. In case of any queries, please feel free to reach us at our [free support forum][14].

## See Also

*   [Add Slide Transitions in PowerPoint Presentations using C++][15]
*   [Create and Manipulate Tables in PowerPoint using C++][16]




[1]: #CPP-API-for-Finding-and-Replacing-Text-in-PowerPoint-Presentations
[2]: #Find-and-Replace-Text-in-PowerPoint-Files-using-CPP
[3]: https://products.aspose.com/slides/cpp
[4]: https://www.nuget.org/packages/Aspose.Slides.Cpp
[5]: https://downloads.aspose.com/slides/cpp
[6]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.presentation
[7]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.i_text_frame
[8]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.i_text_frame
[9]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.i_paragraph
[10]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.i_portion
[11]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.presentation#afcd59ec697bf05c10f78c3869de2ec9e
[12]: https://purchase.aspose.com/temporary-license
[13]: https://docs.aspose.com/slides/cpp/
[14]: https://forum.aspose.com/c/slides/11
[15]: https://blog.aspose.com/2021/10/14/add-slide-transitions-in-powerpoint-presentations-using-cpp/
[16]: https://blog.aspose.com/2021/10/22/create-and-manipulate-tables-in-powerpoint-using-cpp/





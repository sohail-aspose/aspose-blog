---
title: 'Merge PowerPoint Presentations using C++'
seoTitle: "Merge PowerPoint Presentations using C++ | Merge PPT/PPTX files C++"
description: "Merge Multiple PowerPoint PPT/PPTX presentations using C++. Merge complete presentations or selected slides using Aspose.Slides for C++ API."
date: Sat, 13 Mar 2021 10:59:00 +0000
draft: false
url: /2021/03/13/merge-powerpoint-presentations-using-cpp/
author: Muhammad Ahmad
summary: 'PowerPoint presentations are used in many scenarios such as meetings, presentations, discussions, etc. There might be situations where you have different presentations created by separate people or have individual presentations used in various meetings. You might need to merge these presentations for sharing or documentation purposes. Doing this task manually would be time-consuming. The efficient way would be to achieve this programmatically. In this article, you will learn **how to merge PowerPoint presentations using C++**.'
tags: ['C++ Merge Multiple PowerPoint Presentations', 'Merge PPT presentations using C++', 'Merge PPTX files using C++', 'Merge PowerPoint Presentation C++']
categories: ['Aspose.Slides Product Family']
---



{{< figure align=center src="images/Merge-PowerPoint-files.jpg" alt="Merge PowerPoint Presentations using C++">}}


PowerPoint presentations are used in many scenarios such as meetings, presentations, discussions, etc. There might be situations where you have different presentations created by separate people or have individual presentations used in various meetings. You might need to merge these presentations for sharing or documentation purposes. Doing this task manually would be time-consuming. The efficient way would be to achieve this programmatically. In this article, you will learn **how to merge PowerPoint presentations using C++**.

*   [C++ API to Merge PowerPoint Presentations][1]
*   [Merge PowerPoint Presentations using C++][2]
*   [Merge Specific PowerPoint Slides using C++][3]
*   [Use Slide Master to Merge PowerPoint Presentations][4]
*   [Get a Free License][5]

## C++ API to Merge PowerPoint Presentations {#CPP-API-to-Merge-PowerPoint-Presentations}

[Aspose.Slides for C++][6] is a C++ library that provides a bunch of features for working with PowerPoint presentations. The API allows you to create, modify and convert PowerPoint presentations without using Microsoft PowerPoint. Furthermore, the API provides the ability to merge different PowerPoint files. You can either install the API through [NuGet][7] or download it directly from the [Downloads][8] section.

```
PM> Install-Package Aspose.Slides.Cpp
```

## Merge PowerPoint Presentations using C++ {#Merge-PowerPoint-Presentations-using-CPP}

The process for merging two presentations using Aspose.Slides for C++ is a breeze. To achieve this, you load both the presentations, loop through the source presentation slides, and add their clone to the target presentation. The following are the steps to merge two PowerPoint presentations.

*   Load the destination PowerPoint file using the [Presentation][9] class.
*   Create another instance of the [Presentation][10] class to represent the source PowerPoint file.
*   Retrieve the slides from the source presentation using the [Presentation->get\_Slides()][11] method and iterate over them.
*   Inside the loop, add each slide to the destination presentation using the [Presentation->get\_Slides()->AddClone (System::SharedPtr<ISlide> sourceSlide)][12] method.
*   Finally, save the merged presentation file using the [Presentation->Save (System::String name, Export::SaveFormat format)][13] method.

The following is the sample code to merge PowerPoint presentations using C++.

{{< gist aspose-com-gists 3fbb5a14be693e49be410ae57cf50d56 "Merge_PowerPoint_Slides.cpp" >}}

The following images show the source, destination and merged presentation files.

### Destination Presentation



{{< figure align=center src="images/MergeSamplePresentation2-1024x515.png" alt="Destination PowerPoint presentation image" caption="Destination PowerPoint presentation image.">}}


### Source Presentation



{{< figure align=center src="images/MergeSamplePresentation3-1024x515.png" alt="Source PowerPoint presentation image." caption="Source PowerPoint presentation image.">}}


### Merged Presentation



{{< figure align=center src="images/MergedPresentationFull-1024x511.png" alt="Merged PowerPoint presentation image" caption="Merged PowerPoint presentation image.">}}


## Merge Specific PowerPoint Slides using C++ {#Merge-Specific-PowerPoint-Slides-using-CPP}

There might be situations where you are not interested in the whole presentation but instead, want to add a subset of slides. To achieve this, you add the necessary condition while looping through the source presentation slides. The following are the steps to merge selected PowerPoint slides.

*   Firstly, load the destination PowerPoint file using the [Presentation][14] class.
*   Create another instance of the [Presentation][15] class to represent the source PowerPoint file.
*   Retrieve the slides from the source presentation using the [Presentation->get\_Slides()][16] method and iterate over them.
*   Inside the loop, add the required slides to the destination presentation using the [Presentation->get\_Slides()->AddClone (System::SharedPtr<ISlide> sourceSlide)][17] method.
*   Finally, save the merged presentation file using the [Presentation->Save (System::String name, Export::SaveFormat format)][18] method.

The following is the sample code to merge selected PowerPoint slides using C++.

{{< gist aspose-com-gists 3fbb5a14be693e49be410ae57cf50d56 "Merge_Selected_PowerPoint_Slides.cpp" >}}

The following image shows the merged presentation file. The source and the destination presentation files are the same as used in the previous example.

### Merged Presentation



{{< figure align=center src="images/MergedPresentationSelected-1024x513.png" alt="Merged PowerPoint presentation with selected slides added" caption="Merged PowerPoint presentation with selected slides added.">}}


## Use Slide Master to Merge PowerPoint Presentations {#Use-Slide-Master-to-Merge-PowerPoint-Presentations}

In the previous two examples, the design of both the source and destination presentations was the same. The following images show the result of merging presentations with different designs.

### Destination Presentation



{{< figure align=center src="images/MergeSamplePresentation1-1024x513.png" alt="Destination PowerPoint presentation image" caption="Destination PowerPoint presentation image.">}}


### Source Presentation



{{< figure align=center src="images/MergeSamplePresentation3-1024x515.png" alt="Source PowerPoint presentation image" caption="Source PowerPoint presentation image.">}}


### Merged Presentation



{{< figure align=center src="images/MergedPresentationSimpleAdd-1024x513.png" alt="Merged PowerPoint presentation with the first slide added" caption="Merged PowerPoint presentation with the first slide added.">}}


You can see in the merged presentation image that the third slide retained its original styling during the merge process. If you want the source slides to use the destination presentation styles, please use the following steps.

*   Load the destination PowerPoint file using the [Presentation][19] class.
*   Create another instance of the [Presentation][20] class to represent the source PowerPoint file.
*   Add the required slides to the destination presentation using the [Presentation->get\_Slides()->AddClone (System::SharedPtr<ISlide> sourceSlide, System::SharedPtr<IMasterSlide> destMaster, bool allowCloneMissingLayout)][21] method.
*   Finally, save the merged presentation file using the [Presentation->Save (System::String name, Export::SaveFormat format)][22] method.

The following is the sample code to merge PowerPoint presentations using slide master.

{{< gist aspose-com-gists 3fbb5a14be693e49be410ae57cf50d56 "Merge_PowerPoint_Slides_Master.cpp" >}}

The following image shows the merged presentation generated by the above sample code.

### Merged Presentation



{{< figure align=center src="images/MergedPresentationMasterAdd-1024x514.png" alt="Merged PowerPoint presentation with the first slide added using the destination presentation styles" caption="Merged PowerPoint presentation with the first slide added using the destination presentation styles.">}}


## Get a Free License {#Get-a-Free-License}

You can try the API without evaluation limitations by requesting [a free temporary license][23].

## Conclusion

In this article, you have learned how to merge multiple PowerPoint presentations using C++. You have seen how to merge complete presentations or selected slides. Furthermore, you have learned how to use the style of the destination presentation for combining the presentations. Aspose.Slides for C++ offers many additional features for working with PowerPoint files. You can explore the API in detail by using the [official documentation][24]. If you have any questions, please feel free to contact us on the [forum][25].

## See Also

*   [Convert PowerPoint to PDF using C++][26]
*   [Convert PowerPoint to JPG using C++][27]




[1]: #CPP-API-to-Merge-PowerPoint-Presentations
[2]: #Merge-PowerPoint-Presentations-using-CPP
[3]: #Merge-Specific-PowerPoint-Slides-using-CPP
[4]: #Use-Slide-Master-to-Merge-PowerPoint-Presentations
[5]: #Get-a-Free-License
[6]: https://products.aspose.com/slides/cpp
[7]: https://www.nuget.org/packages/Aspose.Slides.Cpp
[8]: https://downloads.aspose.com/slides/cpp
[9]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.presentation
[10]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.presentation
[11]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.presentation#a9981b38f5a01d9fa5482f05b0a75974c
[12]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.i_slide_collection#a0c84ed19c8b1730eb8010613a1c229ee
[13]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.presentation#afcd59ec697bf05c10f78c3869de2ec9e
[14]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.presentation
[15]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.presentation
[16]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.presentation#a9981b38f5a01d9fa5482f05b0a75974c
[17]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.i_slide_collection#a0c84ed19c8b1730eb8010613a1c229ee
[18]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.presentation#afcd59ec697bf05c10f78c3869de2ec9e
[19]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.presentation
[20]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.presentation
[21]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.i_slide_collection#a6b040e6b30f52ab4644fafdbc650b640
[22]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.presentation#afcd59ec697bf05c10f78c3869de2ec9e
[23]: https://purchase.aspose.com/temporary-license
[24]: https://docs.aspose.com/slides/cpp/
[25]: https://forum.aspose.com/c/slides/11
[26]: https://blog.aspose.com/2021/03/03/convert-powerpoint-to-pdf-using-cpp/
[27]: https://blog.aspose.com/2021/03/06/convert-powerpoint-to-jpg-using-cpp/






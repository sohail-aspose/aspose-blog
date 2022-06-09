---
title: 'Add Slide Transitions in PowerPoint Presentations using C++'
seoTitle: "Add Slide Transitions in PowerPoint Presentations using C++"
description: "Add slide transitions to PowerPoint presentations using C++. Use the C++ PowerPoint API to set morph transition in PowerPoint files."
date: Thu, 14 Oct 2021 16:04:11 +0000
draft: false
url: /2021/10/14/add-slide-transitions-in-powerpoint-presentations-using-cpp/
author: Muhammad Ahmad
summary: 'Slide transitions are effects shown while navigating from one slide to another. These enhance the look and feel of the presentation and make them more attractive. There might be situations where you need to add slide transitions to PowerPoint files programmatically. To that end, this article will teach you **how to add transitions to PowerPoint slides using C++**.'
tags: ['Add Morph Transition in PowerPoint Slides C++', 'Add Slide Transition in PowerPoint C++', 'Add Slide Transition using C++']
categories: ['Aspose.Slides Product Family']
---

Slide transitions are effects shown while navigating from one slide to another. These enhance the look and feel of the presentation and make them more attractive. There might be situations where you need to add slide transitions to PowerPoint files programmatically. To that end, this article will teach you **how to add transitions to PowerPoint slides using C++**.

*   [C++ API for Adding Transitions in PowerPoint Presentations][1]
*   [Add Slide Transition using C++][2]
*   [Add Advanced Slide Transitions using C++][3]
*   [Setting Morph Transition Type in PowerPoint Presentations][4]
    *   [Set Morph Transition in Microsoft PowerPoint][5]
    *   [Set Morph Transition in PowerPoint Presentations using C++][6]

## C++ API for Adding Transitions in PowerPoint Presentations {#CPP-API-for-Adding-Transitions-in-PowerPoint-Presentations}

[Aspose.Slides for C++][7] is a C++ API for working with PowerPoint files. It enables you to create, read and update PowerPoint files without needing Microsoft PowerPoint to be installed. Furthermore, the API allows you to add slide transitions to PowerPoint presentations. You can either install the API through [NuGet][8] or download it directly from the [Downloads][9] section.

```
PM> Install-Package Aspose.Slides.Cpp
```

## Add Slide Transition using C++ {#Add-Slide-Transition-using-CPP}

The following are the steps to add slide transition in PowerPoint presentations.

*   Firstly, load the PowerPoint file using the [Presentation][10] class.
*   Set the slide transition using the [Presentation->get\_Slides()->idx\_get(0)->get\_SlideShowTransition()->set\_Type (SlideShow::TransitionType value)][11] method.
*   Finally, save the presentation using the [Presentation->Save(System::String fname, Export::SaveFormat format)][12] method.

The following sample code demonstrates how to add transitions to PowerPoint slides using C++.

{{< gist aspose-com-gists 3736d216e71030784785593601cc48fb "Add_Transition.cpp" >}}

## Add Advanced Slide Transitions using C++ {#Add-Advanced-Slide-Transitions-using-CPP}

The following are the steps to add advanced transitions to slides using C++.

*   Firstly, load the PowerPoint file using the [Presentation][13] class.
*   Set the transition type and other transition effects using the [ISlideShowTransition][14] class.
*   Finally, save the presentation using the [Presentation->Save(System::String fname, Export::SaveFormat format)][15] method.

The following sample code shows how to add advanced slide transitions using C++.

{{< gist aspose-com-gists 3736d216e71030784785593601cc48fb "Add_Advanced_Transition.cpp" >}}

## Setting Morph Transition Type in PowerPoint Presentations {#Setting-Morph-Transition-Type-in-PowerPoint-Presentations}

Morph transitions are used in presentations to make smooth transition animation between slides. The following sections cover how to add morph transition in Microsoft PowerPoint and programmatically using C++.

### Set Morph Transition in Microsoft PowerPoint {#Set-Morph-Transition-in-Microsoft-PowerPoint}

The following are the steps to add morph transition in Microsoft PowerPoint.

*   Open the **Transitions** tab.
*   Select the **Morph** transition type.
*   To select the transition effects, select the **Effect Options** in the ****Transitions**** tab.

### Set Morph Transition in PowerPoint Presentations using C++ {#Set-Morph-Transition-in-PowerPoint-Presentations-using-CPP}

Similar to Microsoft PowerPoint, Aspose.Slides for C++ API provides the following morph transition effects.

*   [ByObject][16]: Morph transition will be performed considering shapes as indivisible objects.
*   [ByWord][17]: Morph transition will be performed by transferring text by words where possible.
*   [ByChar][18]: Morph transition will be performed by transferring text by characters where possible.

The following are the steps to set morph transition in PowerPoint presentations using C++.

*   Load the PowerPoint file using the [Presentation][19] class.
*   Set the transition type to [morph][20].
*   Set the morph transition effect using the [IMorphTransition->set\_MorphType(TransitionMorphType value)][21] method.
*   Save the presentation using the [Presentation->Save(System::String fname, Export::SaveFormat format)][22] method.

The following sample code shows how to set morph transitions in PowerPoint presentations using C++.

{{< gist aspose-com-gists 3736d216e71030784785593601cc48fb "Add_Morph_Transition.cpp" >}}

## Get a Free License

In order to try the API without evaluation limitations, you can request [a free temporary license][23].

## Conclusion

In this article, you have learned how to add slide transitions in PowerPoint presentations using C++. Furthermore, you have seen how to add morph transitions to PowerPoint slides using Aspose.Slides for C++ API. It is a robust and feature-rich API that provides a bunch of additional features for working with PowerPoint files. You can explore the API in detail by visiting the [official documentation][24]. In case of any queries, please feel free to reach us at our [free support forum][25].

## See Also

*   [Set Slide Background in PowerPoint Presentations using C++][26]
*   [Apply Theme in PowerPoint Presentations using C++][27]




[1]: #CPP-API-for-Adding-Transitions-in-PowerPoint-Presentations
[2]: #Add-Slide-Transition-using-CPP
[3]: #Add-Advanced-Slide-Transitions-using-CPP
[4]: #Setting-Morph-Transition-Type-in-PowerPoint-Presentations
[5]: #Set-Morph-Transition-in-Microsoft-PowerPoint
[6]: #Set-Morph-Transition-in-PowerPoint-Presentations-using-CPP
[7]: https://products.aspose.com/slides/cpp
[8]: https://www.nuget.org/packages/Aspose.Slides.Cpp
[9]: https://downloads.aspose.com/slides/cpp
[10]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.presentation
[11]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.i_slide_show_transition#aee4641abe6284b222c0d2118be740292
[12]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.presentation#afcd59ec697bf05c10f78c3869de2ec9e
[13]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.presentation
[14]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.i_slide_show_transition
[15]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.presentation#afcd59ec697bf05c10f78c3869de2ec9e
[16]: https://apireference.aspose.com/slides/cpp/namespace/aspose.slides.slide_show#ae8dafb339f33dd662cb316096af73e70
[17]: https://apireference.aspose.com/slides/cpp/namespace/aspose.slides.slide_show#ae8dafb339f33dd662cb316096af73e70
[18]: https://apireference.aspose.com/slides/cpp/namespace/aspose.slides.slide_show#ae8dafb339f33dd662cb316096af73e70
[19]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.presentation
[20]: https://apireference.aspose.com/slides/cpp/namespace/aspose.slides.slide_show#ad9c6c21716b914dcaf27a55f21656e93
[21]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.slide_show.i_morph_transition#a024d3de3698e2dd5a47cacf9bde5a3b5
[22]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.presentation#afcd59ec697bf05c10f78c3869de2ec9e
[23]: https://purchase.aspose.com/temporary-license
[24]: https://docs.aspose.com/slides/cpp/
[25]: https://forum.aspose.com/c/slides/11
[26]: https://blog.aspose.com/2021/10/12/set-slide-background-in-powerpoint-presentations-using-cpp/
[27]: https://blog.aspose.com/2021/10/08/apply-theme-in-powerpoint-presentations-using-cpp/





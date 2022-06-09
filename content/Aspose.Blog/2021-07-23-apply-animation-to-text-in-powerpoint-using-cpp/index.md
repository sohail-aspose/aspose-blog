---
title: 'Apply Animation to Text in PowerPoint using C++'
seoTitle: "Apply Animation to Text in PowerPoint using C++ | Animate Text in Slides"
description: "Apply animation effects to text in PowerPoint presentations using C++. You can also retrieve the animations already applied to the text."
date: Fri, 23 Jul 2021 15:45:00 +0000
draft: false
url: /2021/07/23/apply-animation-to-text-in-powerpoint-using-cpp/
author: Muhammad Ahmad
summary: "Animation is a feature provided by Microsoft PowerPoint that makes presentations more engaging and fun. It can also be used to highlight different elements on the slide to draw the audience's attention. You can add animations to text, shapes, and other elements on the slides. In this article, you will learn **how to apply animation to text in PowerPoint files using C++**."
tags: ['Apply Animation To Text in PowerPoint C++', 'Apply Animation to Text in PPT C++', 'Apply Animation to Text in PPTX C++']
categories: ['Aspose.Slides Product Family']
---

Animation is a feature provided by Microsoft PowerPoint that makes presentations more engaging and fun. It can also be used to highlight different elements on the slide to draw the audience's attention. You can add animations to text, shapes, and other elements on the slides. In this article, you will learn **how to apply animation to text in PowerPoint files using C++**.

*   [C++ API for Applying Animation to Text in PowerPoint Files][1]
*   [Apply Animation to Text in PowerPoint Files using C++][2]
*   [Get Animation Effects from PowerPoint Files using C++][3]

## C++ API for Applying Animation to Text in PowerPoint Files {#CPP-API-for-Applying-Animation-to-Text-in-PowerPoint-Files}

We will use the [Aspose.Slides for C++][4] API to apply text animation in PowerPoint files. It is a robust and feature-rich API for creating, reading, and modifying PowerPoint PPTX/PPT files without requiring Microsoft PowerPoint to be installed. You can either install the API through [NuGet][5] or download it directly from the [Downloads][6] section.

```
PM> Install-Package Aspose.Slides.Cpp
```

## Apply Animation to Text in PowerPoint Files using C++ {#Apply-Animation-to-Text-in-PowerPoint-Files-using-CPP}

Aspose.Slides for C++ supports over 150+ animation effects, such as Expand, Fade, Blink, Zoom, etc. Furthermore, it also provides specific animation effects such as OLEObjectShow and OLEObjectOpen. You can see the complete list of supported animation effects in the [EffectType][7] enumeration.

In order to apply animation to text in PowerPoint presentations, please follow the steps given below.

*   Load the PowerPoint file using the [Presentation][8] class.
*   Select the desired paragraph.
*   Add the animation using the [Presentation->get\_Slides()->idx\_get(int32\_t index)->get\_Timeline()->get\_MainSequence()->AddEffect(System::SharedPtr<IParagraph> paragraph, EffectType effectType, EffectSubtype subtype, EffectTriggerType triggerType)][9] method.
*   Save the presentation using the [Presentation->Save(System::String fname, Export::SaveFormat format)][10] method.

The following sample code shows how to apply an animation effect to text in PowerPoint presentations using C++.

{{< gist aspose-com-gists 92acf66108007302f1a992adc9ae9137 "Apply_Text_Animation.cpp" >}}

## Get Animation Effects from PowerPoint Files using C++ {#Get-Animation-Effects-from-PowerPoint-Files-using-CPP}

You can retrieve the animation effects already applied to a text by following the steps given below.

*   Firstly, load the PowerPoint file using the [Presentation][11] class.
*   Get the sequence of the desired slide in an [ISequence][12] object.
*   Access the shape from the selected slide in an [IAutoShape][13] object.
*   Loop through the paragraphs.
*   Finally, get the effects from the paragraph using the [ISequence->GetEffectsByParagraph(System::SharedPtr<IParagraph> paragraph)][14] method.

The following sample code shows how to get the animation effects from a text in PowerPoint presentations using C++.

{{< gist aspose-com-gists 92acf66108007302f1a992adc9ae9137 "Get_Text_Animation.cpp" >}}

## Get a Free License

In order to try the API without evaluation limitations, you can request [a free temporary license][15].

## Conclusion

In this article, you have learned how to add animation effects to text in PowerPoint presentations using C++. Furthermore, you have seen how to retrieve animation effects from text in PowerPoint presentations. Aspose.Slides for C++ provides many additional features that you can explore in detail by visiting the [official documentation][16]. In case of any questions, please feel free to reach us at our [free support forum][17].

## See Also

*   [Split PowerPoint Presentations using C++][18]
*   [Extract Text from PowerPoint Files using C++][19]




[1]: #CPP-API-for-Applying-Animation-to-Text-in-PowerPoint-Files
[2]: #Apply-Animation-to-Text-in-PowerPoint-Files-using-CPP
[3]: #Get-Animation-Effects-from-PowerPoint-Files-using-CPP
[4]: https://products.aspose.com/slides/cpp
[5]: https://www.nuget.org/packages/Aspose.Slides.Cpp
[6]: https://downloads.aspose.com/slides/cpp
[7]: https://apireference.aspose.com/slides/cpp/namespace/aspose.slides.animation#ae0da11508d382465aa4e7a011df1bf31
[8]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.presentation
[9]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.animation.i_sequence#a5e149e1c5a3c642cf14f8656aae74575
[10]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.presentation#afcd59ec697bf05c10f78c3869de2ec9e
[11]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.presentation
[12]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.animation.i_sequence
[13]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.i_auto_shape
[14]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.animation.i_sequence#a75a56ec1ea4e95b421fbce6dcbcbaf11
[15]: https://purchase.aspose.com/temporary-license
[16]: https://docs.aspose.com/slides/cpp/
[17]: https://forum.aspose.com/c/slides/11
[18]: https://blog.aspose.com/2021/07/09/split-powerpoint-presentations-using-cpp/
[19]: https://blog.aspose.com/2021/04/10/extract-text-from-powerpoint-files-using-cpp/






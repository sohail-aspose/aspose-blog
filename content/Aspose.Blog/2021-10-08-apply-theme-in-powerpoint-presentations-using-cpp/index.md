---
title: 'Apply Theme in PowerPoint Presentations using C++'
seoTitle: "Apply Theme in PowerPoint Presentations using C++"
description: "Apply themes to PowerPoint presentations using C++. Specifically, set the color, font, and backgroud style of PowerPoint presentations."
date: Fri, 08 Oct 2021 16:30:18 +0000
draft: false
url: /2021/10/08/apply-theme-in-powerpoint-presentations-using-cpp/
author: Muhammad Ahmad
summary: 'Microsoft PowerPoint provides a wide variety of themes that you can use in your PowerPoint presentations. These themes improve the look and feel of the presentations and make them perfect for modern and sophisticated pitches. You can also apply themes to PowerPoint files dynamically within your C++ applications. To that end, this article will teach you **how to apply themes in PowerPoint presentations programmatically using C++**.'
tags: ['Apply Theme to a PowerPoint Presentation C++', 'Set Background Style in a PowerPoint Presentation C++', 'Set Theme Color in a PowerPoint Presentation C++', 'Set Theme Font in a PowerPoint Presentation C++']
categories: ['Aspose.Slides Product Family']
---

Microsoft PowerPoint provides a wide variety of themes that you can use in your PowerPoint presentations. These themes improve the look and feel of the presentations and make them perfect for modern and sophisticated pitches. You can also apply themes to PowerPoint files dynamically within your C++ applications. To that end, this article will teach you **how to apply themes in PowerPoint presentations programmatically using C++**.

*   [C++ API for Applying Theme in PowerPoint Presentations][1]
*   [Apply Theme to PowerPoint Presentations using C++][2]
    *   [Set Theme Color in PowerPoint Presentation using C++][3]
    *   [Set Theme Font in PowerPoint Presentation using C++][4]
    *   [Change Theme Background Style in PowerPoint Presentation using C++][5]

## C++ API for Applying Theme in PowerPoint Presentations {#CPP-API-for-Applying-Theme-in-PowerPoint-Presentations}

[Aspose.Slides for C++][6] is a C++ API for working with PowerPoint files. It enables you to create, read and update PPT and PPTX files without needing additional software. Furthermore, the API allows you to apply themes to PowerPoint presentations. You can either install the API through [NuGet][7] or download it directly from the [Downloads][8] section.

```
PM> Install-Package Aspose.Slides.Cpp
```

## Apply Theme to PowerPoint Presentations using C++ {#Apply-Theme-to-PowerPoint-Presentations-using-CPP}

A PowerPoint theme is a set of colors, font family, font size, background style, etc., that can be applied to different elements. In the following sections, we will explore how to set the theme color, font, and background style in PowePoint presentations.

### Set Theme Color in PowerPoint Presentation using C++ {#Set-Theme-Color-in-PowerPoint-Presentation-using-CPP}

The following are the steps to set the theme color for a shape in a PowerPoint presentation.

*   Create an instance of the [Presentation][9] class to represent a new PowerPoint file.
*   Add a shape using the [AddAutoShape(ShapeType shapeType, float x, float y, float width, float height)][10] method.
*   Set the fill type and scheme color.
*   Save the presentation using the [Presentation->Save(System::String fname, Export::SaveFormat format)][11] method.

The following sample code shows how to set the theme color for a shape in a PowerPoint presentation using C++.

{{< gist aspose-com-gists 23dccfc815c10b6ec93a0990dabcc5fe "Set_Theme_Color.cpp" >}}

### Set Theme Font in PowerPoint Presentation using C++ {#Set-Theme-Font-in-PowerPoint-Presentation-using-CPP}

Similar to Microsoft PowerPoint, Aspose.Slides for C++ API provides the following identifiers to set the font from the font scheme.

*   "**+mn-lt**": Body Font Latin (Minor Latin Font)
*   "**+mj-lt**": Heading Font Latin (Major Latin Font)
*   "**+mn-ea**": Body Font East Asian (Minor East Asian Font)
*   "**+mj-ea**": Body Font East Asian (Minor East Asian Font)

The following are the steps to create a text element and assign the Latin font to it.

*   Create an instance of the [Presentation][12] class to represent a new PowerPoint file.
*   Add a shape using the [AddAutoShape(ShapeType shapeType, float x, float y, float width, float height)][13] method.
*   Create a [Paragraph][14] and add a [Portion][15] into it.
*   Set the font using the [Portion->get\_PortionFormat()->set\_LatinFont(System::SharedPtr<IFontData> value)][16] method.
*   Save the presentation using the [Presentation->Save(System::String fname, Export::SaveFormat format)][17] method.

The following sample code shows how to set the theme font in a PowerPoint presentation using C++.

{{< gist aspose-com-gists 23dccfc815c10b6ec93a0990dabcc5fe "Set_Theme_Font.cpp" >}}

### Change Theme Background Style in PowerPoint Presentation using C++ {#Change-Theme-Background-Style-in-PowerPoint-Presentation-using-CPP}

The following are the steps to set the theme background style in a PowerPoint presentation.

*   Create an instance of the [Presentation][18] class to represent a new PowerPoint file.
*   Set the background style using the [Presentation->get\_Masters()->idx\_get(0)->get\_Background()->set\_StyleIndex(uint16\_t value)][19] method.
*   Save the presentation using the [Presentation->Save(System::String fname, Export::SaveFormat format)][20] method.

The following sample code demonstrates how to set the theme background style in a PowerPoint presentation using C++.

{{< gist aspose-com-gists 23dccfc815c10b6ec93a0990dabcc5fe "Set_Theme_Background_Style.cpp" >}}

## Get a Free License

In order to try the API without evaluation limitations, you can request [a free temporary license][21].

## Conclusion

In this article, you have learned how to apply themes in PowerPoint presentations using C++. Specifically, you have learned how to set the theme color, font, and background style of PowerPoint presentations. Aspose.Slides for C++ is a robust API that provides many additional features for working with PPTX/PPT files. You can explore the API in detail by visiting the [official documentation][22]. In case of any queries, please feel free to reach us at our [free support forum][23].

## See Also

*   [Add Watermark to PowerPoint Slides using C++][24]
*   [Apply Animation to Text in PowerPoint using C++][25]




[1]: #CPP-API-for-Applying-Theme-in-PowerPoint-Presentations
[2]: #Apply-Theme-to-PowerPoint-Presentations-using-CPP
[3]: #Set-Theme-Color-in-PowerPoint-Presentation-using-CPP
[4]: #Set-Theme-Font-in-PowerPoint-Presentation-using-CPP
[5]: #Change-Theme-Background-Style-in-PowerPoint-Presentation-using-CPP
[6]: https://products.aspose.com/slides/cpp
[7]: https://www.nuget.org/packages/Aspose.Slides.Cpp
[8]: https://downloads.aspose.com/slides/cpp
[9]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.presentation
[10]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.i_shape_collection#a22cd6252336905ea935496b4b5799ae2
[11]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.presentation#afcd59ec697bf05c10f78c3869de2ec9e
[12]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.presentation
[13]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.i_shape_collection#a22cd6252336905ea935496b4b5799ae2
[14]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.paragraph
[15]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.portion
[16]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.i_base_portion_format#aaa0c944f076af2f5266df244e3046e06
[17]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.presentation#afcd59ec697bf05c10f78c3869de2ec9e
[18]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.presentation
[19]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.i_background#ab4541fcd327796eae1d8772c4aa784ca
[20]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.presentation#afcd59ec697bf05c10f78c3869de2ec9e
[21]: https://purchase.aspose.com/temporary-license
[22]: https://docs.aspose.com/slides/cpp/
[23]: https://forum.aspose.com/c/slides/11
[24]: https://blog.aspose.com/2021/10/07/add-watermark-to-powerpoint-slides-using-cpp/
[25]: https://blog.aspose.com/2021/07/23/apply-animation-to-text-in-powerpoint-using-cpp/





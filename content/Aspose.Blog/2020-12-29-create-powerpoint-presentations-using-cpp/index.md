---
title: 'Create PowerPoint Presentations using C++'
seoTitle: ""
description: ""
date: Tue, 29 Dec 2020 22:32:00 +0000
draft: false
url: /2020/12/29/create-powerpoint-presentations-using-cpp/
author: Usman Aziz
summary: 'MS PowerPoint is a feature-rich application that lets you create attractive presentations having text, graphics, animations, charts, and several other elements. In this post, you will learn how to implement the basic PowerPoint automation features within the C++ applications. Particularly, you will come to know **how to create PowerPoint presentations and add text, images, charts, and tables to the slides using C++**.'
tags: ['add update powerpoint slides in cpp', 'create powerpoint presentation cpp', 'insert charts in powerpoint cpp', 'insert tables in powerpoint cpp', 'insert text in powerpoint cpp']
categories: ['Aspose.Slides Product Family']
---



{{< figure align=center src="images/Create-PowerPoint-Presentation-1.jpg" alt="create powerpoint presentations C++">}}


MS PowerPoint is a feature-rich application that lets you create appealing presentations having text, graphics, animations, charts, and several other elements. In this post, you will learn how to implement the basic PowerPoint automation features within the C++ applications. Particularly, you will come to know **how to create PowerPoint presentations and add text, images, charts, and tables to the slides using C++**.

*   [C++ PowerPoint API][1]
*   [Create a PowerPoint Presentation in C++][2]
*   [Add Slides to a Presentation][3]
*   [Add Text to a PowerPoint Slide][4]
*   [Create a Table in Presentation][5]
*   [Create a Chart in Presentation][6]
*   [Open an Existing PowerPoint Presentation][7]
*   [Get Free License][8]

## C++ PowerPoint API {#C++-PowerPoint-API}

[Aspose.Slides for C++][9] is designed to automate PowerPoint presentation manipulation features within C++ applications. Using the API, you can create, edit, or convert the PowerPoint presentations seamlessly. You can [download][10] the complete package of the API files or get it from [NuGet][11].

## Create a PowerPoint Presentation in C++ {#Create-a-PowerPoint-Presentation-in-C++}

Let's start by creating an empty PowerPoint presentation using Aspose.Slides for C++. The following are the steps to perform this operation.

*   Create an object of the [Presentation][12] class.
*   Save the presentation using [Presentation->Save(String, SaveFormat::Pptx)][13] method.

The following code sample shows how to create a PowerPoint presentation using C++.

{{< gist aspose-slides a690df625dc0b1fff869ab198affe7a4 "Examples-SlidesCPP-CreateNewPresentation-CreateNewPresentation.cpp" >}}

## Add Slide to a Presentation in C++ {#Add-Slide-to-a-Presentation}

Once you have created the PowerPoint presentation, you can insert slides into it. The following are the steps to add slides to a PowerPoint presentation:

*   Create an object of the [Presentation][14] class.
*   Get slides in the [ISlideCollection][15] object using [Presentation->get\_Slides()][16] method.
*   Add slide using [ISlideCollection->AddEmptySlide()][17] method.
*   Save the presentation using [Presentation->Save(String, SaveFormat::Pptx)][18] method.

The following code sample shows how to add slides to a PowerPoint presentation using C++.

{{< gist aspose-slides a690df625dc0b1fff869ab198affe7a4 "Examples-SlidesCPP-AddSlides-AddSlides.cpp" >}}

To learn more about manipulating slides, visit [Adding, Formatting and Manipulating Slides][19].

## Add Text to a PowerPoint Slide using C++ {#Add-Text-to-a-PowerPoint-Slide}

Now, let's add text to a slide in the PowerPoint presentation. For this, you need to insert a textbox to the slide. Below are the steps to perform this operation.

*   Create a new presentation or load an existing one using [Presentation][20] class.
*   Obtain the reference of the slide into [ISlide][21] object using [Presentation->get\_Slides()->idx\_get(int)][22] method.
*   Add a rectangle to the slide using [ISlide->get\_Shapes()->AddAutoShape(ShapeType::Rectangle, int, int, int, int)][23] method and get its reference in [IAutoShape][24] object.
*   Add text frame using [IAutoShape->AddTextFrame(u" ")][25] method.
*   Get the text frame using [IAutoShape->get\_TextFrame()][26] into [ITextFrame][27] object.
*   Get paragraph using [ITextFrame->get\_Paragraphs()->idx\_get(0)][28] into [IParagraph][29] object.
*   Access portion of the paragraph using [IParagraph->get\_Portions()->idx\_get(0)][30] into [IPortion][31] object.
*   Set text using [IPortion->set\_Text(u"Aspose TextBox")][32] method.
*   Save the presentation using [Presentation->Save(String, SaveFormat::Pptx)][33] method.

The following code sample shows how to add text to slides in a PowerPoint presentation using C++.

{{< gist aspose-com-gists 81aeb05e6d3a070aa76fdea22ed53bc7 "Examples-SlidesCPP-TextBoxOnSlideProgram-TextBoxOnSlideProgram.cpp" >}}

To learn more about manipulating text in presentations, visit [Adding, Formatting, and Manipulating Text][34].

## Create a Table in Presentation using C++ {#Create-a-Table-in-Presentation}

The following are the steps to add a table in a PowerPoint presentation's slide using Aspose.Slides for C++.

*   Create an instance of a [Presentation][35] class.
*   Obtain the reference of a slide into an [ISlide][36] object.
*   Define arrays of columns and rows by providing the width.
*   Add a table to the slide using [ISlide->get\_Shapes()->AddTable()][37] method.
*   Iterate through each cell to apply formatting to the top, bottom, right, and left borders.
*   Merge cells if required.
*   Access the text frame of a cell to add some text.
*   Save the presentation as a PPTX file.

The following code sample shows how to create table in PowerPoint presentation using C++.

{{< gist aspose-slides a690df625dc0b1fff869ab198affe7a4 "Examples-SlidesCPP-TableFromScratch-TableFromScratch.cpp" >}}

To learn more about manipulating the tables, visit [Adding, Updating and Manipulating Tables][38].

## Create a Chart in Presentation using C++ {#Create-a-Chart-in-Presentation-using-C++}

Aspose.Slides for C++ supports various types of charts such as scattered, treemap, histogram, and [etc][39]. For the demonstration, let's create a normal chart. Below are the steps to perform this operation.

*   Create an instance of the [Presentation][40] class.
*   Obtain the reference of a slide you want to add the chart on.
*   Add chart with default data along with desired type using [ISlide->get\_Shapes()->AddChart()][41] method.
*   Get the reference of the chart in the [IChart][42] object.
*   Clear the chart data and add new series and categories.
*   Add new chart data for chart series.
*   Set fill color for chart series.
*   Add chart series labels.
*   Save the presentation as a PPTX file.

The following code sample shows how to insert a chart in a PowerPoint presentation using C++.

{{< gist aspose-slides a690df625dc0b1fff869ab198affe7a4 "Examples-SlidesCPP-NormalCharts-NormalCharts.cpp" >}}

Learn more about manipulating charts from [Adding, Formatting, and Manipulating Charts][43].

## Open a PowerPoint Presentation in C++ {#Open-an-Existing-PowerPoint-Presentation}

You can also open an existing PowerPoint presentations in order to edit the content. For this, you can follow the below steps:

*   Load the PPTX file using [Presentation][44] class by providing the file's name.
*   Update the content of the presentation.
*   Save the updated file using the [Presentation->Save(String, SaveFormat)][45] method.

The following code sample shows how to open an existing PowerPoint presentation using C++.

{{< gist aspose-com-gists 81aeb05e6d3a070aa76fdea22ed53bc7 "Examples-SlidesCPP-OpenPresentation-OpenPresentation.cpp" >}}

## Get a Free License {#Get-Free-License}

You can [get a free temporary license][46] in order to try the API without evaluation limitations.

## Conclusion

In this article, you have learned how to create PowerPoint presentations from within the C++ applications. The step-by-step guide and code samples along with API references have shown how to create a presentation from scratch and insert slides, text, tables, and charts into it. You can explore more about the API using the [documentation][47].

## See Also

*   [Convert Presentation to HTML using C++][48]




[1]: #C++-PowerPoint-API
[2]: #Create-a-PowerPoint-Presentation-in-C++
[3]: #Add-Slide-to-a-Presentation
[4]: #Add-Text-to-a-PowerPoint-Slide
[5]: #Create-a-Table-in-Presentation
[6]: #Create-a-Chart-in-Presentation-using-C++
[7]: #Open-an-Existing-PowerPoint-Presentation
[8]: #Get-Free-License
[9]: https://products.aspose.com/slides/cpp
[10]: https://downloads.aspose.com/slides/cpp
[11]: https://www.nuget.org/packages/Aspose.Slides.cpp
[12]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.presentation
[13]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.presentation#afcd59ec697bf05c10f78c3869de2ec9e
[14]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.presentation
[15]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.i_slide_collection
[16]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.presentation#a9981b38f5a01d9fa5482f05b0a75974c
[17]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.i_slide_collection#af2e6ab303a66ec5537765cd99a106823
[18]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.presentation#afcd59ec697bf05c10f78c3869de2ec9e
[19]: https://docs.aspose.com/slides/cpp/adding-formatting-and-manipulating-slides/
[20]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.presentation
[21]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.i_slide
[22]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.i_slide_collection#a640042758d7f73745c4e6a0eceb5524e
[23]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.i_shape_collection#a22cd6252336905ea935496b4b5799ae2
[24]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.i_auto_shape/
[25]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.i_auto_shape#afb267108fea5ee5a213c162c004fcef3
[26]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.i_auto_shape#a61a649d6f83054417f833571d0745512
[27]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.i_text_frame/
[28]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.i_paragraph_collection#ad07debb69ea304f26ff7f94e0f73940b
[29]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.i_paragraph
[30]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.i_portion_collection#a0ec328fe222e4d8a21ababf14e61e11f
[31]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.i_portion
[32]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.i_portion#a77ca201ad712c430fc6180f491c84275
[33]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.presentation#afcd59ec697bf05c10f78c3869de2ec9e
[34]: https://docs.aspose.com/slides/cpp/adding-formatting-and-manipulating-text/
[35]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.presentation
[36]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.i_slide
[37]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.i_shape_collection#a4267156608ecbb1bdeb07b6dd9975aa6
[38]: https://docs.aspose.com/slides/cpp/adding-updating-and-manipulating-tables/
[39]: https://apireference.aspose.com/slides/cpp/namespace/aspose.slides.charts#a23ba9ea390f5be4c8f5ab18baf4f8c05
[40]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.presentation
[41]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.i_shape_collection#a2cd4d47fc5c536012ee15b3a69486374
[42]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.charts.i_chart/
[43]: https://docs.aspose.com/slides/cpp/adding-formatting-and-manipulating-charts/
[44]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.presentation
[45]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.presentation#afcd59ec697bf05c10f78c3869de2ec9e
[46]: https://purchase.aspose.com/temporary-license
[47]: https://docs.aspose.com/slides/cpp/getting-started/
[48]: https://blog.aspose.com/2020/09/04/convert-presentation-to-webpage-html-using-cpp/






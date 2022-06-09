---
title: 'Add Header and Footer in PowerPoint Presentations using C++'
seoTitle: "Add Header and Footer in PowerPoint Presentations using C++"
description: "Add header and footer in PowerPoint presentations using C++. Use the C++ PowerPoint API to manage headers and footers in notes master and notes slides."
date: Wed, 27 Oct 2021 16:41:34 +0000
draft: false
url: /2021/10/27/add-header-and-footer-in-powerpoint-presentations-using-cpp/
author: Muhammad Ahmad
summary: 'You can use header and footer sections in PowerPoint slides to display additional information such as slide number, date, author, etc. You can also manipulate these sections programmatically within your C++ applications. To that end, this article will teach you **how to add header and footer in PowerPoint presentations using C++**.'
tags: ['Add Header and Footer in PowerPoint C++', 'Manage Header and Footer in Notes Master C++', 'Manage Header and Footer in Notes Slide C++', 'Manage Header and Footer in PowerPoint C++']
categories: ['Aspose.Slides Product Family']
---

You can use header and footer sections in PowerPoint slides to display additional information such as slide number, date, author, etc. You can also manipulate these sections programmatically within your C++ applications. To that end, this article will teach you **how to add header and footer in PowerPoint presentations using C++**.

*   [C++ API for Adding Header and Footer in PowerPoint Presentations][1]
*   [Add Header and Footer in PowerPoint Presentations using C++][2]
*   [Manage Header and Footer in Notes Master and Notes Slides using C++][3]
    *   [Change Header and Footer Settings for Notes Master][4]
    *   [Change Header and Footer Settings for Notes Slide][5]

## C++ API for Adding Header and Footer in PowerPoint Presentations {#CPP-API-for-Adding-Header-and-Footer-in-PowerPoint-Presentations}

We will use the [Aspose.Slides for C++][6] API to add header and footer in PowerPoint presentations. It is a robust API providing many features for working with PowerPoint PPTX/PPT files. You can either install the API through [NuGet][7] or download it directly from the [Downloads][8] section.

```
PM> Install-Package Aspose.Slides.Cpp
```

## Add Header and Footer in PowerPoint Presentations using C++ {#Add-Header-and-Footer-in-PowerPoint-Presentations-using-CPP}

The following are the steps for adding header and footer in PowerPoint presentations.

*   Firstly, load the PowerPoint file using the [Presentation][9] class.
*   Set the footer text using the [Presentation->get\_HeaderFooterManager()->SetAllFootersText(System::String text)][10] method.
*   Show the footer by setting its visibility using the [Presentation->get\_HeaderFooterManager()->SetAllFootersVisibility(bool isVisible)][11] method.
*   Access the master notes slide using the [Presentation->get\_MasterNotesSlideManager()->get\_MasterNotesSlide()][12] method.
*   Loop through the shapes of the master notes slide.
*   If the shape is of the type [PlaceholderType::Header][13], set the header text using the [IAutoShape->get\_TextFrame()->set\_Text(System::String value)][14] method.
*   Finally, save the presentation using the [Presentation->Save(System::String fname, Export::SaveFormat format)][15] method.

The following sample code shows how to add a header and footer in a PowerPoint presentation using C++.

{{< gist aspose-com-gists 68cdc7a7f1f25846f76e8941375d05e4 "Add_Header_Footer.cpp" >}}

## Manage Header and Footer in Notes Master and Notes Slides using C++ {#Manage-Header-and-Footer-in-Notes-Master-and-Notes-Slides-using-CPP}

With Aspose.Slides for C++, you can easily manage header and footer for both notes master and notes slides. The following sections cover how to manage header and footer in notes master and notes slides.

### Change Header and Footer Settings for Notes Master {#Change-Header-and-Footer-Settings-for-Notes-Master}

The following are the steps to change the header and footer settings for notes master.

*   Firstly, load the PowerPoint file using the [Presentation][16] class.
*   Access the master notes slide using the [Presentation->get\_MasterNotesSlideManager()->get\_MasterNotesSlide()][17] method.
*   Access the [IMasterNotesSlideHeaderFooterManager][18] using the [IMasterNotesSlide->get\_HeaderFooterManager()][19] method.
*   Use the [IMasterNotesSlideHeaderFooterManager][20] object to update the header and footer.
*   Finally, save the presentation using the [Presentation->Save(System::String fname, Export::SaveFormat format)][21] method.

The following sample code shows how to change the header and footer in notes master using C++.

{{< gist aspose-com-gists 68cdc7a7f1f25846f76e8941375d05e4 "Change_Header_Footer_Notes_Master.cpp" >}}

### Change Header and Footer Settings for Notes Slide {#Change-Header-and-Footer-Settings-for-Notes-Slide}

The following are the steps to change the header and footer settings for notes slides.

*   Firstly, load the PowerPoint file using the [Presentation][22] class.
*   Access the notes slide using the [Presentation->get\_Slides()->idx\_get(0)->get\_NotesSlideManager()->get\_NotesSlide()][23] method.
*   Access the [INotesSlideHeaderFooterManager][24] using the [INotesSlide->get\_HeaderFooterManager()][25] method.
*   Use the [INotesSlideHeaderFooterManager][26] object to update the header and footer.
*   Finally, save the presentation using the [Presentation->Save(System::String fname, Export::SaveFormat format)][27] method.

The following sample code shows how to change the header and footer in the notes slide using C++.

{{< gist aspose-com-gists 68cdc7a7f1f25846f76e8941375d05e4 "Change_Header_Footer_Notes_Slide.cpp" >}}

## Get a Free License

In order to try the API without evaluation limitations, you can request [a free temporary license][28].

## Conclusion

In this article, you have learned how to add header and footer in PowerPoint presentations using C++. Furthermore, you have seen how to change the header and footer in notes master and notes slide using Aspose.Slides for C++ API. It is a powerful API that provides a bunch of additional features for working with PowerPoint PPTX/PPT files. You can explore the API in detail by visiting the [official documentation][29]. In case of any queries, please feel free to reach us at our [free support forum][30].

## See Also

*   [Find and Replace Text in PowerPoint PPTX/PPT using C++][31]
*   [Add Watermark to PowerPoint Slides using C++][32]




[1]: #CPP-API-for-Adding-Header-and-Footer-in-PowerPoint-Presentations
[2]: #Add-Header-and-Footer-in-PowerPoint-Presentations-using-CPP
[3]: #Manage-Header-and-Footer-in-Notes-Master-and-Notes-Slides-using-CPP
[4]: #Change-Header-and-Footer-Settings-for-Notes-Master
[5]: #Change-Header-and-Footer-Settings-for-Notes-Slide
[6]: https://products.aspose.com/slides/cpp
[7]: https://www.nuget.org/packages/Aspose.Slides.Cpp
[8]: https://downloads.aspose.com/slides/cpp
[9]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.presentation
[10]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.i_presentation_header_footer_manager#a8d4783f100b5b5e8c7e4ed04f8baefbb
[11]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.i_presentation_header_footer_manager#a3fdf6f34e04bf56f06b7e43478ff4c6c
[12]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.i_master_notes_slide_manager#abd466e33ff0d398569cdef38db7c7d7d
[13]: https://apireference.aspose.com/slides/cpp/namespace/aspose.slides#a9dee8ab962dcf0c0b507f6acd0f373b9
[14]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.i_text_frame#aa0d44ddd1f1298427a340d03f5c01f5a
[15]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.presentation#afcd59ec697bf05c10f78c3869de2ec9e
[16]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.presentation
[17]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.i_master_notes_slide_manager#abd466e33ff0d398569cdef38db7c7d7d
[18]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.i_master_notes_slide_header_footer_manager
[19]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.i_master_notes_slide#ab377afa733db79517d4ece649f8c9e22
[20]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.i_master_notes_slide_header_footer_manager
[21]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.presentation#afcd59ec697bf05c10f78c3869de2ec9e
[22]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.presentation
[23]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.i_notes_slide_manager#a87185e4cb0a1a3cf7c65e08a97f16024
[24]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.i_notes_slide_header_footer_manager
[25]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.i_notes_slide#a47c31646e5c2916344e1b2385af593af
[26]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.i_notes_slide_header_footer_manager
[27]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.presentation#afcd59ec697bf05c10f78c3869de2ec9e
[28]: https://purchase.aspose.com/temporary-license
[29]: https://docs.aspose.com/slides/cpp/
[30]: https://forum.aspose.com/c/slides/11
[31]: https://blog.aspose.com/2021/10/26/find-and-replace-text-in-powerpoint-pptx-ppt-using-cpp/
[32]: https://blog.aspose.com/2021/10/07/add-watermark-to-powerpoint-slides-using-cpp/





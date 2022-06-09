---
title: 'Working With Notes in PowerPoint Presentations using C++'
seoTitle: "Working With Notes in PowerPoint Presentations using C++"
description: "Mange slide notes in PowerPoint presentations using C++. Read, Add, Update and Remove slide notes in PowerPoint presentations using C++."
date: Thu, 08 Apr 2021 10:40:59 +0000
draft: false
url: /2021/04/08/working-with-notes-in-powerpoint-presentations-using-cpp/
author: Muhammad Ahmad
summary: 'Microsoft PowerPoint provides you with the option to add notes to your slides. These notes can be helpful for the presenter by providing additional information and context. You might find yourself in situations where you have to add or update such notes programmatically in your PowerPoint presentations. In light of that, this article will teach you **how to work with notes in PowerPoint presentations programmatically using C++**.'
tags: ['Add Notes in PowerPoint Slides C++', 'Read Notes from PowerPoint Slides C++', 'Remove Notes from PowerPoint Slides C++', 'Update Notes in PowerPoint Slides C++']
categories: ['Aspose.Slides Product Family']
---



{{< figure align=center src="images/mange-notes-powerpoint.jpg" alt="Mange PowerPoint Slide Notes">}}


Microsoft PowerPoint provides you with the option to add notes to your slides. These notes can be helpful for the presenter by providing additional information and context. You might find yourself in situations where you have to add or update such notes programmatically in your PowerPoint presentations. In light of that, this article will teach you **how to work with notes in PowerPoint presentations programmatically using C++**.

*   [C++ API for Working with Notes in PowerPoint Presentations][1]
*   [Read Notes from a PowerPoint Slide using C++][2]
*   [Add Notes to a PowerPoint Slide using C++][3]
*   [Update Notes of a PowerPoint Slide using C++][4]
*   [Remove Notes from a PowerPoint Slide using C++][5]
*   [Get a Free License][6]

## C++ API for Working with Notes in PowerPoint Presentations {#CPP-API-for-Working-with-Notes-in-PowerPoint-Presentations}

[Aspose.Slides for C++][7] is a native C++ library that supports creating, reading, and manipulating PowerPoint files. The API also supports working with notes in PowerPoint presentations. You can either install the API through [NuGet][8] or download it directly from the [Downloads][9] section.

```
PM> Install-Package Aspose.Slides.Cpp
```

## Read Notes from a PowerPoint Slide using C++ {#Read-Notes-from-a-PowerPoint-Slide-using-CPP}

The following are the steps to read notes from a PowerPoint Slide.

*   Load the PowerPoint presentation using the [Presentation][10] class.
*   Access the [INotesSlideManager][11] for a specific slide using [Presentation->get\_Slides()->idx\_get (int32\_t index)->get\_NotesSlideManager()][12] method.
*   Retrieve the slide notes using the [INotesSlideManager->get\_NotesSlide()][13] method.
*   Read the notes using the [INotesSlide->get\_NotesTextFrame()->get\_Text()][14] method.

The following is the sample code to read notes from a PowerPoint slide using C++.

{{< gist aspose-com-gists 6212a97ef3c254fc335ccc7fe6527376 "Read-Slide-Notes.cpp" >}}

## Add Notes to a PowerPoint Slide using C++ {#Add-Notes-to-a-PowerPoint-Slide-using-CPP}

Aspose.Slides for C++ provides you with the ability to add notes to PowerPoint slides. For that, access the [INotesSlideManager][15] for the required slide and then add the note. The following are the steps to add notes to a specific PowerPoint slide.

*   Firstly, load the PowerPoint presentation using the [Presentation][16] class.
*   Access the [INotesSlideManager][17] for a specific slide using [Presentation->get\_Slides()->idx\_get (int32\_t index)->get\_NotesSlideManager()][18] method.
*   Add new slide notes using the [INotesSlideManager->AddNotesSlide()][19] method.
*   Set the notes text using the [INotesSlide->get\_NotesTextFrame()->set\_Text (System::String value)][20] method.
*   Finally, save the presentation with the note using the [Presentation->Save (System::String name, Export::SaveFormat format)][21] method.

The following is the sample code to add notes to a specific PowerPoint slide using C++.

{{< gist aspose-com-gists 6212a97ef3c254fc335ccc7fe6527376 "Add-Slide-Notes.cpp" >}}

## Update Notes of PowerPoint Slides using C++ {#Update-Notes-of-a-PowerPoint-Slide-using-CPP}

To update the notes, you retrieve the existing note with the [INotesSlideManager][22] and then update the note text. The following are the steps to update the notes of a PowerPoint slide.

*   Firstly, load the PowerPoint presentation using the [Presentation][23] class.
*   Access the [INotesSlideManager][24] for a specific slide using [Presentation->get\_Slides()->idx\_get (int32\_t index)->get\_NotesSlideManager()][25] method.
*   Retrieve the slide notes using the [INotesSlideManager->get\_NotesSlide()][26] method.
*   Update the note text using the [INotesSlide->get\_NotesTextFrame()->set\_Text (System::String value)][27] method.
*   Finally, save the presentation with the updated note using the [Presentation->Save (System::String name, Export::SaveFormat format)][28] method.

The following is the sample code to update the notes of a PowerPoint slide using C++.

{{< gist aspose-com-gists 6212a97ef3c254fc335ccc7fe6527376 "Update-Slide-Notes.cpp" >}}

## Remove Notes from a PowerPoint Slide using C++ {#Remove-Notes-from-a-PowerPoint-Slide-using-CPP}

Remove the notes from a slide by retrieving the [INotesSlideManager][29] for that particular slide and then using the [RemoveNotesSlide()][30] method. The following are the steps to remove notes from a PowerPoint slide.

*   Firstly, load the PowerPoint presentation using the [Presentation][31] class.
*   Access the [INotesSlideManager][32] for a specific slide using [Presentation->get\_Slides()->idx\_get (int32\_t index)->get\_NotesSlideManager()][33] method.
*   Remove the notes using the [INotesSlideManager->RemoveNotesSlide()][34] method.
*   Finally, save the presentation file using the [Presentation->Save (System::String name, Export::SaveFormat format)][35] method.

The following is the sample code to remove notes from a PowerPoint slide using C++.

{{< gist aspose-com-gists 6212a97ef3c254fc335ccc7fe6527376 "Remove-Slide-Notes.cpp" >}}

## Get a Free License {#Get-a-Free-License}

You can request [a free temporary license][36] to try the API without evaluation limitations.

## Conclusion

In this article, you have learned how to manage slide notes in PowerPoint presentations using C++. Specifically, you have learned how to read, add, update and remove notes from PowerPoint slides. Aspose.Slides for C++ also provides many additional features that aid you in your presentation-related tasks. You can explore the API in detail by visiting the [official documentation][37]. In case of any questions, please feel free to reach us on our [free support forum][38].

## See Also

*   [Create Charts in PowerPoint Presentations using C++][39]




[1]: #CPP-API-for-Working-with-Notes-in-PowerPoint-Presentations
[2]: #Read-Notes-from-a-PowerPoint-Slide-using-CPP
[3]: #Add-Notes-to-a-PowerPoint-Slide-using-CPP
[4]: #Update-Notes-of-a-PowerPoint-Slide-using-CPP
[5]: #Remove-Notes-from-a-PowerPoint-Slide-using-CPP
[6]: #Get-a-Free-License
[7]: https://products.aspose.com/slides/cpp
[8]: https://www.nuget.org/packages/Aspose.Slides.Cpp
[9]: https://downloads.aspose.com/slides/cpp
[10]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.presentation
[11]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.i_notes_slide_manager
[12]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.i_slide#ae78a692be68504beadf8c4c0d47c67e1
[13]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.i_notes_slide_manager#a87185e4cb0a1a3cf7c65e08a97f16024
[14]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.i_text_frame#a986842a898d96d8261a6614b537d23d1
[15]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.i_notes_slide_manager
[16]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.presentation
[17]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.i_notes_slide_manager
[18]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.i_slide#ae78a692be68504beadf8c4c0d47c67e1
[19]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.i_notes_slide_manager#a6f9c2a2b96339a66c828fe459b3f09ff
[20]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.i_text_frame#aa0d44ddd1f1298427a340d03f5c01f5a
[21]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.presentation#afcd59ec697bf05c10f78c3869de2ec9e
[22]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.i_notes_slide_manager
[23]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.presentation
[24]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.i_notes_slide_manager
[25]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.i_slide#ae78a692be68504beadf8c4c0d47c67e1
[26]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.i_notes_slide_manager#a87185e4cb0a1a3cf7c65e08a97f16024
[27]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.i_text_frame#aa0d44ddd1f1298427a340d03f5c01f5a
[28]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.presentation#afcd59ec697bf05c10f78c3869de2ec9e
[29]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.i_notes_slide_manager
[30]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.i_notes_slide_manager#a977d6335391b242b807d8cbf1ea9444a
[31]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.presentation
[32]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.i_notes_slide_manager
[33]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.i_slide#ae78a692be68504beadf8c4c0d47c67e1
[34]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.i_notes_slide_manager#a977d6335391b242b807d8cbf1ea9444a
[35]: https://apireference.aspose.com/slides/cpp/class/aspose.slides.presentation#afcd59ec697bf05c10f78c3869de2ec9e
[36]: https://purchase.aspose.com/temporary-license
[37]: https://docs.aspose.com/slides/cpp/
[38]: https://forum.aspose.com/c/slides/11
[39]: https://blog.aspose.com/2021/04/02/create-charts-in-powerpoint-presentations-using-cpp/






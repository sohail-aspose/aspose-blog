---
title: 'Read, Add, Update or Remove Slide Notes in PowerPoint Presentations using C#'
seoTitle: ""
description: ""
date: Tue, 18 Feb 2020 17:16:31 +0000
draft: false
url: /2020/02/18/read-add-update-remove-slide-notes-in-powerpoint-csharp-net/
author: Usman Aziz
summary: ''
tags: ['Add slide notes in PowerPoint', 'Read slide notes in PowerPoint', 'Remove slide notes in PowerPoint', 'Update slide notes in PowerPoint']
categories: ['Aspose.Slides Product Family']
---



{{< figure align=center src="images/aspose-Slides-for-net_100.png" alt="read add update and remove slide notes in PowerPoint using C# .NET">}}


Slide notes in the PowerPoint presentations are used to add references for the presenter to recall the important points during the presentation. These notes can be added to every slide of a PowerPoint presentation. This article also covers some important aspects of dealing with slide notes in presentations programmatically.

After reading this article, you will be able to:

*   [read slide notes in PowerPoint presentation using C#][1],
*   [add slide notes to a PowerPoint presentation in C#][2],
*   [update notes in a particular slide of the PowerPoint presentation in C#][3], and
*   [remove slide notes in a PowerPoint presentation using C#][4].

## Working with Slide Notes using Aspose.Slides for .NET

In order to work with slide notes in PowerPoint, we'll use [Aspose.Slides for .NET][5] - a powerful PowerPoint automation API that supports creating, updating, parsing and converting presentation documents. You can [download][6] the API or install it using the following options:

### Using NuGet Package Manager



{{< figure align=center src="images/Aspose.Slides-NPM.png" alt="read or update slide notes in PowerPoint C# .NET">}}


### Using the Package Manager Console```
PM> Install-Package Aspose.Slides.NET
```

## Read Slide Notes from PowerPoint Presentation in C# {#Read-Slide-Notes-from-PowerPoint-Presentation-in-CSharp}

In order to access the slide notes in PowerPoint, _Aspose.Slides for .NET_ provides [INotesSlideManager][7] interface. _INotesSlideManager_ lets you access, read, add and update the slide notes. The following are the steps to read the slide notes from the PowerPoint presentation.

*   Load the PowerPoint presentation into the [Presentation][8] object.
*   Access the [NotesSlideManager][9] of the particular slide using the [INotesSlideManager][10] interface.
*   Get the slide notes into [INotesSlide][11] interface.
*   Read slide notes using [INotesSlide.NotesTextFrame.Text][12].

The following code sample shows how to read slide notes from a PowerPoint PPTX using C#.

{{< gist aspose-com-gists 01299b860d20eec199d41b1e2c2df93e "read-slide-notes.cs" >}}

## Add Notes to a PowerPoint Slide in C# {#Add-Notes-to-a-PowerPoint-Slide-in-CSharp}

The following are the steps to add notes to a particular slide in a PowerPoint presentation.

*   Load the PowerPoint presentation in the _Presentation_ object.
*   Access the _NotesSlideManager_ of particular slide.
*   Use the _INotesSlide_ interface to add a new note.
*   Save the presentation using [Presentation.Save(String, SaveFormat)][13] method.

The following code sample shows how to add slide notes to a PowerPoint PPTX using C#.

{{< gist aspose-com-gists 01299b860d20eec199d41b1e2c2df93e "add-slide-notes.cs" >}}

## Update Slide Notes in PowerPoint Presentation using C# {#Update-Slide-Notes-in-PowerPoint-Presentation-using-CSharp}

In order to update the notes in a particular presentation slide, you will access the _NotesSlide_ in the same way you have done for reading the notes. Once you have got access to the slide notes, you can simply update the text using [INotesSlide.NotesTextFrame.Text][14] property. Once done, save the presentation file using the _Presentation.Save(String, SaveFormat)_ method.

The following code sample shows how to update slide notes in a PowerPoint presentation using C#.

{{< gist aspose-com-gists 01299b860d20eec199d41b1e2c2df93e "update-slide-notes.cs" >}}

## Remove Slide Notes in PowerPoint Presentation using C# {#Remove-Slide-Notes-in-PowerPoint-Presentation-using-CSharp}

To remove the slide notes from a PowerPoint presentation, simply call [INotesSlideManager.RemoveNotesSlide()][15] method and save the presentation file. The following code sample shows how to remove slide notes from a PowerPoint presentation using C#.

{{< gist aspose-com-gists 01299b860d20eec199d41b1e2c2df93e "remove-slide-notes.cs" >}}

## See also

*   [More options for presentation notes with Aspose.Slides][16]

## Try Aspose.Slides for .NET for Free

You can try _Aspose.Slides for .NET_ using a free [temporary license][17].




[1]: #Read-Slide-Notes-from-PowerPoint-Presentation-in-CSharp
[2]: #Add-Notes-to-a-PowerPoint-Slide-in-CSharp
[3]: #Update-Slide-Notes-in-PowerPoint-Presentation-using-CSharp
[4]: #Remove-Slide-Notes-in-PowerPoint-Presentation-using-CSharp
[5]: https://products.aspose.com/slides/net
[6]: https://downloads.aspose.com/slides/net
[7]: https://apireference.aspose.com/net/slides/aspose.slides/inotesslidemanager
[8]: https://apireference.aspose.com/net/slides/aspose.slides/presentation
[9]: https://apireference.aspose.com/net/slides/aspose.slides/slide/properties/notesslidemanager
[10]: https://apireference.aspose.com/net/slides/aspose.slides/inotesslidemanager
[11]: https://apireference.aspose.com/net/slides/aspose.slides/inotesslide
[12]: https://apireference.aspose.com/net/slides/aspose.slides/inotesslide/properties/notestextframe
[13]: https://apireference.aspose.com/net/slides/aspose.slides.presentation/save/methods/4
[14]: https://apireference.aspose.com/net/slides/aspose.slides/inotesslide/properties/notestextframe
[15]: https://apireference.aspose.com/net/slides/aspose.slides/inotesslidemanager/methods/removenotesslide
[16]: https://docs.aspose.com/display/slidesnet/Presentation+Notes
[17]: https://purchase.aspose.com/temporary-license






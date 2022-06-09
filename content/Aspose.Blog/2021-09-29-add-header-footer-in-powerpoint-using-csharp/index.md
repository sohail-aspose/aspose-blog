---
title: 'Add Header and Footer in PowerPoint Presentations using C#'
seoTitle: "Add Header and Footer in PowerPoint using C# | C# .NET Source Code"
description: "Use .NET PowerPoint API to add header footer in PowerPoint presentation using C# or VB.NET. Manage header and footer in notes slides programmaticaly."
date: Wed, 29 Sep 2021 14:27:33 +0000
draft: false
url: /2021/09/29/add-header-footer-in-powerpoint-using-csharp/
author: Usman Aziz
summary: 'Header and footer in PowerPoint presentations are used to display additional information such as slide number, author, date, etc. In this article, you will learn **how to add and manage the header and footer in PowerPoint PPTX/PPT presentations programmatically using C#**.'
tags: ['API to Manage Header and Footer in PowerPoint', 'Add Header Footer in PowerPoint Presentation Csharp', 'Manage Header Footer in Handout and Notes Slide Csharp']
categories: ['Aspose.Slides Product Family']
---



{{< figure align=center src="images/presentation-2127830_640.png" alt="Add Header and Footer in PowerPoint C#">}}


Header and footer in PowerPoint presentations are used to display additional information such as slide number, author, date, etc. In this article, you will learn **how to add and manage the header and footer in PowerPoint PPTX/PPT presentations programmatically using C#**.

*   [.NET API to Manage Header and Footer in PowerPoint][1]
*   [Add Header and Footer in PowerPoint Presentation][2]
*   [Manage Header and Footer in Handout and Notes Slide][3]
    *   [Change Header and Footer Settings for Notes Master][4]
    *   [Change Header and Footer Settings for Notes Slide][5]

## .NET API to Manage Header and Footer in PowerPoint {#API-to-Manage-Header-and-Footer-in-PowerPoint}

In order to work with header and footer in PowerPoint presentations, we will use [Aspose.Slides for .NET][6]. It is a .NET class library that lets you create and manipulate PowerPoint and OpenOffice documents. You can download the API's DLL from the [downloads][7] section. Also, the API can be installed via [NuGet][8].

```
PM> Install-Package Aspose.Slides.NET
```

## Add Header and Footer in PowerPoint using C# {#Add-Header-Footer-in-PowerPoint-Presentation}

The following are the steps to add header and footer in a PowerPoint presentation using C#.

*   First, create a new presentation or load an existing one using [Presentation][9] class.
*   Then, set footer using [Presentation.HeaderFooterManager.SetAllFootersText(string)][10] method.
*   Access the master notes slide in an [IMasterNotesSlide][11] object using [Presentation.MasterNotesSlideManager.MasterNotesSlide][12] property.
*   Loop through each shape in [IMasterNotesSlide.Shapes][13] collection.
*   If [IShape.Placeholder.Type][14] is [PlaceholderType.Header][15] then set text for header using [((IAutoShape)shape).TextFrame.Text][16] property.
*   Finally, save the presentation using [Presentation.Save(string, SaveFormat)][17] method.

The following code sample shows how to add header and footer in a PowerPoint presentation.

{{< gist aspose-com-gists 09f55917adc4676dd410d7a67e317770 "add-header-footer.cs" >}}

## Manage Header and Footer in Handout and Notes Slide using C# {#Add-Header-Footer-in-Handout-and-Notes-Slide}

Aspose.Slides for .NET also allows you to set the header and footer in handout and notes slides. For this, you can either apply changes in master notes slide or an individual slide. The following sections cover both scenarios.

### Change Header and Footer Settings for Notes Master {#Change-Header-and-Footer-Settings-for-Notes-Master}

*   First, create a new presentation or load an existing one using [Presentation][18] class.
*   Then, access the master notes slide in an [IMasterNotesSlide][19] object using [Presentation.MasterNotesSlideManager.MasterNotesSlide][20] property.
*   Get reference of [IMasterNotesSlideHeaderFooterManager][21] from [IMasterNotesSlide.HeaderFooterManager][22] property.
*   Update the header footer using _IMasterNotesSlideHeaderFooterManager_ object.
*   Finally, save the presentation using [Presentation.Save(string, SaveFormat)][23] method.

The following code sample shows how to change header and footer in notes master using C#.

{{< gist aspose-com-gists 09f55917adc4676dd410d7a67e317770 "change-header-footer-notes-master.cs" >}}

### Change Header and Footer Settings for Notes Slide {#Change-Header-and-Footer-Settings-for-Notes-Slide}

*   First, create a new presentation or load an existing one using [Presentation][24] class.
*   Then, access [INotesSlide][25] object of desired slide using [Presentation.Slides\[index\].NotesSlideManager.NotesSlide][26] property.
*   Get reference of [INotesSlideHeaderFooterManager][27] from [INotesSlide.HeaderFooterManager][28] property.
*   Update the header footer using _INotesSlideHeaderFooterManager_ object.
*   Finally, save the presentation using [Presentation.Save(string, SaveFormat)][29] method.

The following code sample shows how to change header and footer in notes slides using C#.

{{< gist aspose-com-gists 09f55917adc4676dd410d7a67e317770 "change-header-footer-notes-slide.cs" >}}

## Get a Free API License {#Get-a-Free-API-License}

Get a free [temporary license][30] to use Aspose.Slides for .NET without evaluation limitations.

## Conclusion

In this article, you have learned how to add header and footer in PowerPoint presentations using C#. Moreover, you have seen how to change header and footer in notes slides programmatically. Besides, you can explore the [documentation][31] to learn more about Aspose.Slides for .NET. Also, you can ask your questions via our [forum][32].

## See Also

*   [Convert PowerPoint PPTX/PPT to PNG Images in C#][33]
*   [Set Slide Background in PowerPoint Presentations using C#][34]
*   [Generate Thumbnails for PowerPoint PPTX or PPT using C#][35]
*   [Apply Animation to Text in PowerPoint using C#][36]
*   [Split PowerPoint Presentations using C#][37]




[1]: #API-to-Manage-Header-and-Footer-in-PowerPoint
[2]: #Add-Header-Footer-in-PowerPoint-Presentation
[3]: #Add-Header-Footer-in-Handout-and-Notes-Slide
[4]: #Change-Header-and-Footer-Settings-for-Notes-Master
[5]: #Change-Header-and-Footer-Settings-for-Notes-Slide
[6]: https://products.aspose.com/slides/net
[7]: https://downloads.aspose.com/slides/net
[8]: https://www.nuget.org/packages/Aspose.Slides.NET
[9]: https://apireference.aspose.com/slides/net/aspose.slides/presentation
[10]: https://apireference.aspose.com/slides/net/aspose.slides/ipresentationheaderfootermanager/methods/setallfooterstext
[11]: https://apireference.aspose.com/slides/net/aspose.slides/imasternotesslide
[12]: https://apireference.aspose.com/slides/net/aspose.slides/imasternotesslidemanager/properties/masternotesslide
[13]: https://apireference.aspose.com/slides/net/aspose.slides/ibaseslide/properties/shapes
[14]: https://apireference.aspose.com/slides/net/aspose.slides/iplaceholder/properties/type
[15]: https://apireference.aspose.com/slides/net/aspose.slides/placeholdertype
[16]: https://apireference.aspose.com/slides/net/aspose.slides/itextframe/properties/text
[17]: https://apireference.aspose.com/slides/net/aspose.slides.presentation/save/methods/5
[18]: https://apireference.aspose.com/slides/net/aspose.slides/presentation
[19]: https://apireference.aspose.com/slides/net/aspose.slides/imasternotesslide
[20]: https://apireference.aspose.com/slides/net/aspose.slides/imasternotesslidemanager/properties/masternotesslide
[21]: https://apireference.aspose.com/slides/net/aspose.slides/imasternotesslideheaderfootermanager
[22]: https://apireference.aspose.com/slides/net/aspose.slides/imasternotesslide/properties/headerfootermanager
[23]: https://apireference.aspose.com/slides/net/aspose.slides.presentation/save/methods/5
[24]: https://apireference.aspose.com/slides/net/aspose.slides/presentation
[25]: https://apireference.aspose.com/slides/net/aspose.slides/inotesslide
[26]: https://apireference.aspose.com/slides/net/aspose.slides/inotesslidemanager/properties/notesslide
[27]: https://apireference.aspose.com/slides/net/aspose.slides/inotesslideheaderfootermanager
[28]: https://apireference.aspose.com/slides/net/aspose.slides/inotesslide/properties/headerfootermanager
[29]: https://apireference.aspose.com/slides/net/aspose.slides.presentation/save/methods/5
[30]: https://purchase.aspose.com/temporary-license
[31]: https://docs.aspose.com/slides/net/developer-guide/
[32]: https://forum.aspose.com/
[33]: https://blog.aspose.com/2021/09/01/convert-powerpoint-to-png-in-csharp/
[34]: https://blog.aspose.com/2021/08/31/set-background-in-powerpoint-using-csharp/
[35]: https://blog.aspose.com/2021/08/30/generate-pptx-thumbnails-using-csharp/
[36]: https://blog.aspose.com/2021/08/20/apply-animation-to-text-in-powerpoint-using-csharp/
[37]: https://blog.aspose.com/2021/09/03/split-powerpoint-presentations-using-csharp/





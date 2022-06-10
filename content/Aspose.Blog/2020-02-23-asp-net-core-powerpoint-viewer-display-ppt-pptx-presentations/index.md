---
title: 'ASP.NET PowerPoint Viewer - Display PowerPoint Presentations in ASP.NET'
seoTitle: "ASP.NET PowerPoint Viewer | Display PPT/PPTX Files in ASP.NET Core"
description: "ASP.NET Core PowerPoint Viewer. View PowerPoint PPT or PPTX presentaions in ASP.NET web application. Complete open source code and tutorial."
date: Sun, 23 Feb 2020 11:13:40 +0000
draft: false
url: /2020/02/23/asp-net-core-powerpoint-viewer-display-ppt-pptx-presentations/
author: Usman Aziz
summary: ''
tags: ['ASP.NET PowerPoint Viewer', 'Display PowerPoint in ASP.NET Core', 'PowerPoint Viewer in ASP.NET', 'View PowerPoint in ASP.NET Core']
categories: ['Aspose.Slides Product Family']
---



{{< figure align=center src="images/ASP.NET-PowerPoint-Viewer.png" alt="Display PPT PPTX in ASP.NET Core">}}


Are you looking for a **PowerPoint Viewer** to view or embed presentations in your **ASP.NET Core** web application? If yes, continue to read this article and learn how to create a simple **ASP.NET Core PowerPoint Viewer** and **display PPT/PPTX presentations** using **C#**. So let's begin.

## Features of ASP.NET PowerPoint Viewer

Our ASP.NET PowerPoint Viewer will use [Aspose.Slides for .NET][1] API to render the presentation slides as PNG images. Once the slides are rendered, we'll display them using the Bootstrap Carousel. The following will be features of the application:

1.  Browse and view PowerPoint (PPT/PPTX) presentations.
2.  Set the default PowerPoint file to be displayed on page load.
3.  Slider to navigate between slides.

**TIP**: You may want to check out a [live implementation of viewing operations for presentations][2].

## Steps to Create PowerPoint Viewer in ASP.NET Core

The following are some easy steps to create a PowerPoint Viewer in ASP.NET Core.

**1.** Create a new _ASP.NET Core Web Application_ in Visual Studio.



{{< figure align=center src="images/ASP.NET-Core-MVC.png" alt="Create ASP.NET PowerPoint Viewer">}}


**2.** Open _NuGet Package Manager_ and install [Aspose.Slides for .NET][3] package.



{{< figure align=center src="images/Aspose.Slides-NPM.png" alt="ASP.NET PowerPoint Slideshow">}}


**3.** Create _Presentations_ and _Slides_ folders in _wwwroot_ to keep the PowerPoint files and the rendered slides respectively.



{{< figure align=center src="images/wwwroot-folders.png" alt="PowerPoint Slideshow in ASP.NET">}}


**4.** Create a new folder with the name "_Helpers_" in the root folder.

**5.** Create a new class with the name "_Slide_" in the "_Helpers_" folder to store the presentation slides' information.

{{< gist aspose-com-gists b372cb309e92259655e6ed20912ed7f7 "Slide.cs" >}}

**6.** Open the "_HomeController_.cs" and replace its code with the following (_Update the default PowerPoint file's name in Index action_).

{{< gist aspose-com-gists b372cb309e92259655e6ed20912ed7f7 "HomeController.cs" >}}

**7.** Open _Views/Home/index.cshtml_ and replace its content with the following.

{{< gist aspose-com-gists b372cb309e92259655e6ed20912ed7f7 "index.cshtml" >}}

**8.** Build the application and run it in your favorite browser.



{{< figure align=center src="images/PowerPoint-Viewer.png" alt="PowerPoint Viewer in ASP.NET Core">}}


## ASP.NET PowerPoint Viewer - Demo

<figure class="wp-block-embed is-type-video is-provider-youtube wp-block-embed-youtube wp-embed-aspect-4-3 wp-has-aspect-ratio"><div class="wp-block-embed__wrapper">https://youtu.be/DJw7ul1IMBw</div></figure>

## See Also

*   [More options for Presentation Viewer with Aspose.Slides][4]

## Get a Temporary License for Aspose.Slides for .NET

You can get the [temporary license][5] of _Aspose.Slides for .NET_ to avoid trial limitations.




[1]: https://products.aspose.com/slides
[2]: https://products.aspose.app/slides/viewer
[3]: https://products.aspose.com/slides/net
[4]: https://docs.aspose.com/display/slidesnet/Presentation+Viewer
[5]: https://purchase.aspose.com/temporary-license






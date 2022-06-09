---
title: 'Convert PowerPoint to XAML using C#'
seoTitle: "Convert PowerPoint to XAML using C# | PPTX PPT to XAML in C#"
description: "Use .NET PowerPoint API to convert PowerPoint presentations to XAML in C#. Convert PPT to XAML or PPTX to XAML in ASP.NET or other .NET applications."
date: Thu, 05 Aug 2021 23:46:38 +0000
draft: false
url: /2021/08/05/convert-powerpoint-to-xaml-using-csharp/
author: Usman Aziz
summary: '[XAML][1] (eXtensible Application Markup Language) is an [XML][2]\-based descriptive language that is used to design graphical user interfaces. Especially, XAML is used in WPF (Windows Presentation Foundation), UWP (Universal Windows Platform), and Xamarin Forms. In this article, you will learn how to convert the slides in a PowerPoint presentation to the XAML interfaces programmatically. Particularly, the article will cover **PowerPoint PPTX to XAML conversion using C#**.'
tags: ['PPT to XAML Csharp', 'PPTX to XAML Csharp', 'PowerPoint to XAML Csharp']
categories: ['Aspose.Slides Product Family']
---

[XAML][3] (eXtensible Application Markup Language) is an [XML][4]\-based descriptive language that is used to design graphical user interfaces. Especially, XAML is used in WPF (Windows Presentation Foundation), UWP (Universal Windows Platform), and Xamarin Forms. In this article, you will learn how to convert the slides in a PowerPoint presentation to the XAML interfaces programmatically. Particularly, the article will cover **PowerPoint PPTX to XAML conversion using C#**.

*   [API for PPTX to XAML Conversion][5]
*   [Convert PowerPoint PPTX to XAML][6]
*   [PowerPoint to XAML with Custom Options][7]

## C# API for PowerPoint to XAML Conversion {#API-for-PPTX-to-XAML-Conversion}

In order to convert a PowerPoint presentation to XAML, we will use [Aspose.Slides for .NET][8]. It is a presentation manipulation API that lets you create, modify or convert PowerPoint presentations. You can either [download][9] the API or install it using [NuGet][10].

```
PM> Install-Package Aspose.Slides.NET
```

## Convert PowerPoint PPTX to XAML in C# {#Convert-PowerPoint-PPTX-to-XAML}

The following are the steps to convert slides in a PowerPoint presentation to XAML in C#.

*   First, load the PowerPoint presentation using [Presentation][11] class.
*   Convert presentation to XAML files using [Presentation.Save(new XamlOptions())][12] method.

The following code sample shows how to convert a PowerPoint PPTX to XAML.

{{< gist aspose-com-gists 154ccb15bd5aee545b38d8d2db487533 "pptx-to-xaml.cs" >}}

The following is the screenshot of the files we get after performing PPTX to XAML conversion.



{{< figure align=center src="images/PPTX-to-XAML.jpg" alt="PPTX to XAML in C#">}}


## PowerPoint to XAML with Custom Options {#PowerPoint-to-XAML-with-Custom-Options}

You can also customize the PowerPoint to XAML conversion by setting different options. For example, you can define whether to convert hidden slides or not. The following are the steps to convert PowerPoint presentations to XAML with custom options.

*   First, load the PowerPoint presentation using [Presentation][13] class.
*   Create an instance of [XamlOptions][14] class and set [XamlOptions.ExportHiddenSlides][15] to _true_.
*   Convert presentation to XAML files using [Presentation.Save(XamlOptions)][16] method.

The following code sample shows how to customize PowerPoint to XAML conversion in C#.

{{< gist aspose-com-gists 154ccb15bd5aee545b38d8d2db487533 "pptx-to-xaml-custom.cs" >}}

## Get a Free API License {#Get-a-Free-API-License}

You can use Aspose.Slides for .NET without evaluation limitations by requesting a [temporary license][17].

## Conclusion

In this article, you have learned how to convert PowerPoint PPT or PPTX presentations to XAML using C#. You can simply install the API and integrate the provided code in your .NET applications. In addition, you can visit the [documentation][18] to explore other features of Aspose.Slides for .NET. Also, you can feel free to let us know about your queries via our [forum][19].

## See Also

*   [Create MS PowerPoint Presentations in C#][20]




[1]: https://docs.fileformat.com/web/xaml/
[2]: https://docs.fileformat.com/web/xml/
[3]: https://docs.fileformat.com/web/xaml/
[4]: https://docs.fileformat.com/web/xml/
[5]: #API-for-PPTX-to-XAML-Conversion
[6]: #Convert-PowerPoint-PPTX-to-XAML
[7]: #PowerPoint-to-XAML-with-Custom-Options
[8]: https://products.aspose.com/slides/net
[9]: https://downloads.aspose.com/slides/net
[10]: https://www.nuget.org/packages/Aspose.Slides.Net
[11]: https://apireference.aspose.com/slides/net/aspose.slides/presentation
[12]: https://apireference.aspose.com/slides/net/aspose.slides/presentation/methods/save
[13]: https://apireference.aspose.com/slides/net/aspose.slides/presentation
[14]: https://apireference.aspose.com/slides/net/aspose.slides.export.xaml/xamloptions
[15]: https://apireference.aspose.com/slides/net/aspose.slides.export.xaml/xamloptions/properties/exporthiddenslides
[16]: https://apireference.aspose.com/slides/net/aspose.slides/presentation/methods/save
[17]: https://purchase.aspose.com/temporary-license
[18]: https://docs.aspose.com/slides/net/developer-guide/
[19]: https://forum.aspose.com/
[20]: https://blog.aspose.com/2020/12/04/create-powerpoint-presentations-in-csharp/






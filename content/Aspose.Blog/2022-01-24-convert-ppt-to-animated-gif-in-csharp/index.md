---
title: 'Convert PowerPoint PPT to Animated GIF in C#'
date: Mon, 24 Jan 2022 07:48:00 +0000
draft: false
url: /2022/01/24/convert-ppt-to-animated-gif-in-csharp/
author: ''Usman Aziz''
summary: 'PowePoint to GIF conversion is usually performed to avoid the necessity of MS PowerPoint for previewing the presentations. The animated GIF has the ability to contain all the PPT slides in a single file. Therefore, this article covers **how to convert a PowerPoint [PPT][1] or [PPTX][2] presentation to an animated [GIF][3] in C#**. Furthermore, you will learn how to customize frame size, the delay between slides, and frames per second programmatically.'
tags: ['Convert a PowerPoint PPT to GIF in Csharp', 'powerpoint to gif csharp', 'ppt to gif csharp', 'pptx to gif csharp']
categories: ['Aspose.Slides Product Family']
---



{{< figure align=center src="images/Convert-PowerPoint-PPT-to-GIF.png" alt="Convert PowerPoint PPT to Animated GIF in C#">}}


PowePoint to GIF conversion is usually performed to avoid the necessity of MS PowerPoint for previewing the presentations. The animated GIF has the ability to contain all the PPT slides in a single file. Therefore, this article covers **how to convert a PowerPoint [PPT][4] or [PPTX][5] presentation to an animated [GIF][6] in C#**. Furthermore, you will learn how to customize frame size, the delay between slides, and frames per second programmatically.

*   [C# API for PowerPoint to GIF Conversion][7]
*   [Convert a PowerPoint PPT to GIF in C#][8]
*   [Set Additional Options for PPT/PPTX to GIF Conversion][9]

**Info**: Aspose recently developed an online [Text to GIF Converter][10] that allows you to make interesting animations based on simple texts or messages.

## C# .NET API for PowerPoint PPT to GIF Conversion {#Library-for-PowerPoint-to-GIF-Conversion}

To convert PowerPoint PPT/PPTX files to animated GIF, we will use [Aspose.Slides for .NET][11]. It is a feature-rich .NET API for creating and manipulating PowerPoint presentations. Also, it offers high-fidelity conversion of PPT/PPTX files to other formats. You can [download][12] API's DLL or install it using [NuGet][13].

```
PM> Install-Package Aspose.Slides.NET 
```

## Convert a PowerPoint PPT to GIF in C# {#Convert-a-PowerPoint-PPT-to-GIF}

Aspose.Slides for .NET makes it quite easier for you to convert a PPT/PPTX to GIF. Just load the presentation and save it as a GIF. The following are the steps to convert a PPT to GIF in C#.

*   Load the PPT/PPTX presentation using [Presentation][14] class.
*   Save the presentation as GIF using [Presentation.Save(string, SaveFormat.Gif)][15] method.

The following code sample shows how to convert a PowerPoint PPTX file to an animated GIF in C#.

{{< gist aspose-com-gists ba9d2232fc27cb0b4baa4b8e345e5fd1 "ppt-to-gif.cs" >}}

## Set Additional Options - C# PPT to GIF {#Set-Additional-Options-for-PPT-PPTX-to-GIF-Conversion}

You can also customize PPT to GIF conversion using different options such as the delay between slides, frame size of GIF, and the transition in frames per second. The following are the steps to customize PPT to GIF conversion.

*   Load the PPT/PPTX presentation using [Presentation][16] class.
*   Create an instance of [GifOptions][17] class.
*   Set desired options such as frame size.
*   Save the presentation as GIF using [Presentation.Save(string, SaveFormat.Gif, GifOptions)][18] method.

The following code sample shows how to convert a PPT to an animated GIF with customized settings in C#.

{{< gist aspose-com-gists ba9d2232fc27cb0b4baa4b8e345e5fd1 "ppt-to-gif-custom.cs" >}}

## Get a Free License {#Get-a-Free-API-License}

You can [get a free temporary license][19] to use Aspose.Slides for .NET without evaluation limitations.

## Conclusion

In this article, you have learned how to convert PowerPoint PPT/PPTX presentations to animated GIF in C#. Furthermore, you have seen how to customize PowerPoint to GIF conversion using different options. Besides, you can explore more about Aspose.Slides for .NET using the [documentation][20]. Also, you can post your queries to our [forum][21].

## See Also

*   [Create MS PowerPoint Presentations in C#][22]
*   [Add or Remove Shapes in PowerPoint Slides using C#][23]
*   [Extract Images from PowerPoint PPT in C#][24]




[1]: https://docs.fileformat.com/presentation/ppt/
[2]: https://docs.fileformat.com/presentation/pptx/
[3]: https://docs.fileformat.com/image/gif/
[4]: https://docs.fileformat.com/presentation/ppt/
[5]: https://docs.fileformat.com/presentation/pptx/
[6]: https://docs.fileformat.com/image/gif/
[7]: #Library-for-PowerPoint-to-GIF-Conversion
[8]: #Convert-a-PowerPoint-PPT-to-GIF
[9]: #Set-Additional-Options-for-PPT-PPTX-to-GIF-Conversion
[10]: https://products.aspose.app/slides/text-to-gif
[11]: https://products.aspose.com/slides/net
[12]: https://downloads.aspose.com/slides/net
[13]: https://www.nuget.org/packages/Aspose.Slides.Net
[14]: https://apireference.aspose.com/slides/net/aspose.slides/presentation
[15]: https://apireference.aspose.com/slides/net/aspose.slides.presentation/save/methods/5
[16]: https://apireference.aspose.com/slides/net/aspose.slides/presentation
[17]: https://apireference.aspose.com/slides/net/aspose.slides.export/gifoptions
[18]: https://apireference.aspose.com/slides/net/aspose.slides.presentation/save/methods/6
[19]: https://purchase.aspose.com/temporary-license
[20]: https://docs.aspose.com/slides/net/
[21]: https://forum.aspose.com/
[22]: https://blog.aspose.com/2020/12/04/create-powerpoint-presentations-in-csharp/
[23]: https://blog.aspose.com/2020/12/24/add-shapes-to-powerpoint-slides-in-csharp/
[24]: https://blog.aspose.com/2022/01/13/extract-images-from-ppt-in-csharp-net/





---
title: 'Convert PowerPoint PPT or PPTX to PDF using C#'
seoTitle: ""
description: ""
date: Wed, 12 Feb 2020 09:06:52 +0000
draft: false
url: /2020/02/12/convert-powerpoint-ppt-pptx-to-pdf-in-csharp-net/
author: Usman Aziz
summary: ''
tags: ['Convert PPT to PDF in Csharp', 'Convert PPTX to PDF in CSharp', 'Convert PowerPoint to PDF in CSharp']
categories: ['Aspose.Slides Product Family']
---



{{< figure align=center src="images/Convert-PPT-PPTX-to-PDF-1.png" alt="PowerPoint PPT PPTX to PDF">}}


Are you looking for a reliable yet easy solution for converting **PowerPoint PPT or PPTX to PDF**? Do you want to accurately convert PowerPoint presentations to PDF with high quality? If yes then you are at the right place because, in this article, I am going to showcase a bunch of features to seamlessly **convert PowerPoint PPT to PDF or PPTX to PDF programmatically in C#**.

This article is composed of the following PowerPoint to PDF conversion features.

*   [Convert PowerPoint (PPT or PPTX) to PDF in C#][1]
*   [Customized conversion of PPT or PPTX to PDF][2]
*   [Convert hidden slides in PPT or PPTX to PDF][3]
*   [Convert particular slides of PowerPoint presentation to PDF][4]
*   [Convert PowerPoint presentation to a password-protected PDF with desired access permissions][5]

**Note:** Besides PPT to PDF conversion, Aspose.Slides singlehandedly supports conversion of Presentations to many formats: HTML, JPG, TIFF, and others.

To convert PPT to DOC, you have to use Aspose.Slides together with Aspose.Words. You may want to try out our [free PPT to Word converter][6] to see how Aspose APIs handle conversion processes.

## Prerequisite for PowerPoint to PDF Conversion in C#

[Aspose.Slides for .NET][7] is a powerful PowerPoint automation API to create, edit, parse and convert presentation documents and we'll use this API throughout this article. You can install _Aspose.Slides for .NET_ using one of the following ways in Visual Studio.

### Installing via NuGet Package Manager



{{< figure align=center src="images/Aspose.Slides-NPM.png" alt="PPT to PDF">}}


### Installing via Package Manager Console```
PM> Install-Package Aspose.Slides.NET
```

## Convert PPT or PPTX to PDF in C# {#Convert-PPT-or-PPTX-to-PDF-in-CSharp}

The following are the simple steps to convert a PowerPoint presentation to PDF using _Aspose.Slides for .NET_.

*   Create an object of [Presentation][8] class and initialize it with the path of the PowerPoint presentation file.
*   Use [Presentation.Save(string outputFilePath, SaveFormat.Pdf)][9] method to save file as PDF.

The following code sample shows how to convert PPT to PDF in C#.

{{< gist aspose-com-gists d80998365f9fbb69f99b04f642b6caa6 "convert-ppt-to-pdf.cs" >}}

## Convert PPT or PPTX to PDF with Custom Options in C# {#Convert-PPT-or-PPTX-to-PDF-with-Custom-Options-in-CSharp}

You can also customize PowerPoint to PDF conversion by defining different options such as Jpeg quality, text compression level, the behavior of metafiles and etc. You can set these options using the [PdfOptions][10] class.

The following code sample shows how to convert PowerPoint to PDF with custom options in C#.

{{< gist aspose-com-gists d80998365f9fbb69f99b04f642b6caa6 "convert-pptx-to-pdf-custom-options.cs" >}}

## Convert Hidden Slides of PowerPoint Presentation to PDF in C# {#Convert-Hidden-Slides-of-PowerPoint-Presentation-to-PDF-in-CSharp}

The PowerPoint presentations may also contain hidden slides. By default, hidden slides are not included in PPT or PPTX to PDF conversion. In case you want to convert a presentation including hidden slides, you can specify it using [PdfOptions.ShowHiddenSlides][11] property.

The following code sample shows how to convert a PPTX to PDF including hidden slides in C#.

{{< gist aspose-com-gists d80998365f9fbb69f99b04f642b6caa6 "convert-pptx-to-pdf-hidden-slides.cs" >}}

## Convert Selected Slides of PowerPoint PPT or PPTX to PDF in C# {#Convert-Selected-Slides-of-PowerPoint-PPT-or-PPTX-to-PDF-in-CSharp}

Instead of converting the whole presentation, you can also convert the selected slides of the presentation to PDF. For this, you can define the integer array containing the slide numbers and then pass that array to the [Save(String,Int32\[\], SaveFormat.Pdf)][12] method.

The following code sample shows how to convert selected slides of PowerPoint PPT/PPTX to PDF in C#.

{{< gist aspose-com-gists d80998365f9fbb69f99b04f642b6caa6 "convert-pptx-to-pdf-selected-slides.cs" >}}

## Convert PowerPoint Presentation to a Password-protected PDF with Access Permissions {#Convert-PowerPoint-Presentation-to-a-Password-protected-PDF-with-Access-Permissions}

PDF format supports setting the password and access permissions to protect the document. In case you want to apply such a protection mechanism while converting PowerPoint to PDF, you can do it using _PdfOptions_ class.

The following code sample shows how to set a password and specify access permissions while converting PPTX to PDF in C#.

{{< gist aspose-com-gists d80998365f9fbb69f99b04f642b6caa6 "convert-ppt-to-pdf-password-protected.cs" >}}

## Try Aspose.Slides for .NET for Free

You can try and use _Aspose.Slides for .NET_ for free by requesting a [temporary license][13].

## See Also

*   [More Ways to Convert PowerPoint to PDF][14]
*   [Convert PowerPoint to PDF with Notes][15]
*   [Create MS PowerPoint Presentations in C#][16]
*   [Convert PowerPoint PPTX/PPT to PNG Images in C#][17]
*   [Set Slide Background in PowerPoint Presentations using C#][18]
*   [Generate Thumbnails for PowerPoint PPTX or PPT using C#][19]
*   [Apply Animation to Text in PowerPoint using C#][20]
*   [Split PowerPoint Presentations using C#][21]




[1]: #Convert-PPT-or-PPTX-to-PDF-in-CSharp
[2]: #Convert-PPT-or-PPTX-to-PDF-with-Custom-Options-in-CSharp
[3]: #Convert-Hidden-Slides-of-PowerPoint-Presentation-to-PDF-in-CSharp
[4]: #Convert-Selected-Slides-of-PowerPoint-PPT-or-PPTX-to-PDF-in-CSharp
[5]: #Convert-PowerPoint-Presentation-to-a-Password-protected-PDF-with-Access-Permissions
[6]: https://products.aspose.app/slides/conversion/ppt-to-word
[7]: https://products.aspose.com/slides/net
[8]: https://apireference.aspose.com/net/slides/aspose.slides/presentation
[9]: https://apireference.aspose.com/net/slides/aspose.slides.presentation/save/methods/4
[10]: https://apireference.aspose.com/net/slides/aspose.slides.export/pdfoptions
[11]: https://apireference.aspose.com/net/slides/aspose.slides.export/pdfoptions/properties/showhiddenslides
[12]: https://apireference.aspose.com/net/slides/aspose.slides.presentation/save/methods/8
[13]: https://purchase.aspose.com/temporary-license
[14]: https://docs.aspose.com/display/slidesnet/Convert+PowerPoint+PPT+and+PPTX+to+PDF
[15]: https://docs.aspose.com/display/slidesnet/Convert+PowerPoint+PPT+and+PPTX+to+PDF+with+Notes
[16]: https://blog.aspose.com/2020/12/04/create-powerpoint-presentations-in-csharp/
[17]: https://blog.aspose.com/2021/09/01/convert-powerpoint-to-png-in-csharp/
[18]: https://blog.aspose.com/2021/08/31/set-background-in-powerpoint-using-csharp/
[19]: https://blog.aspose.com/2021/08/30/generate-pptx-thumbnails-using-csharp/
[20]: https://blog.aspose.com/2021/08/20/apply-animation-to-text-in-powerpoint-using-csharp/
[21]: https://blog.aspose.com/2021/09/03/split-powerpoint-presentations-using-csharp/






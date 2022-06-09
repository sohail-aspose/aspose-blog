---
title: 'Convert PowerPoint Presentation to Word Document using C#'
seoTitle: "Convert PowerPoint PPTX to Word in C# | PPTX/PPT to DOCX in C#"
description: "Use .NET APIs to convert PowerPoint presentations to Word documents using C#. Perform PPTX or PPT to DOCX conversion in ASP.NET or other .NET applications."
date: Mon, 02 Aug 2021 16:51:00 +0000
draft: false
url: /2021/08/02/convert-powerpoint-to-word-using-csharp/
author: Usman Aziz
summary: 'In certain cases, you may need to convert the PowerPoint presentations to Word documents. In order to automate this process or for batch conversion, this article covers **how to convert PowerPoint PPTX/PPT to Word DOCX using C#**.'
tags: ['powerpoint to word csharp', 'ppt to docx csharp', 'pptx to docx csharp']
categories: ['Aspose.Words Product Family', 'Aspose.Total Product Family', 'Aspose.Slides Product Family']
---



{{< figure align=center src="images/PPTX-to-DOCX.jpg" alt="PPTX to DOCX C#">}}


In certain cases, you may need to convert the PowerPoint presentations to Word documents. In order to automate this process or for batch conversion, this article covers **how to convert PowerPoint PPTX/PPT to Word DOCX using C#**.

*   [APIs for PowerPoint to Word Conversion][1]
*   [Convert PPTX or PPT to DOCX in C#][2]

## APIs for PowerPoint to Word Conversion {#APIs-to-Convert-PowerPoint-Files-to-Word}

In order to convert a PowerPoint presentation to Word document, we'll use [Aspose.Slides for .NET][3] in combination with [Aspose.Words for .NET][4]. The former is a presentation manipulation API that lets you create or modify PowerPoint presentations. Whereas, the latter is a word processing API for generating or processing Word documents. You can either [download][5] the APIs or install them using NuGet. In addition, you can get a complete package of Aspose APIs as [Aspose.Total for .NET][6].

```
PM> Install-Package Aspose.Slides.NET
PM> Install-Package Aspose.Words
```

## Convert PowerPoint PPTX or PPT to DOCX in C# {#Convert-PPTX-or-PPT-to-DOCX}

The following are the steps to convert a PowerPoint presentation to Word document using C#.

*   First, add references of Aspose.Words for .NET and Aspose.Slides for .NET into your project.
*   After that, load the PowerPoint presentation using [Aspose.Slides.Presentation][7] class.
*   Then, save the presentation into a [MemoryStream][8] object.
*   Create an object of [Aspose.Words.Document][9] class and initialize it with _MemoryStream_ object.
*   Finally, save the document using [Aspose.Words.Document.Save(string, Aspose.Words.SaveFormat.Docx)][10] method.

The following code sample shows how to convert a PPTX to DOCX using C#.

{{< gist aspose-com-gists e3fcc8485e0a474ae25de9ce939268aa "pptx-to-docx.cs" >}}

## Get a Free API License {#Get-a-Free-API-License}

You can use the APIs without evaluation limitations by requesting a [temporary license][11].

## Try Online

You can also try the [online PowerPoint to Word converter][12], which is based on the above-mentioned APIs.

## Conclusion

In this article, you have learned how to convert PowerPoint PPT or PPTX to Word DOCX using C#. You can simply install the APIs and integrate the provided code in your .NET applications. In addition, you can consult the documentations listed below to explore other features of the APIs. Furthermore, feel free to let us know about your queries via our [forum][13].

*   [Aspose.Slides for .NET][14]
*   [Aspose.Words for .NET][15]

## See Also

*   [Create MS PowerPoint Presentations in C#][16]




[1]: #APIs-to-Convert-PowerPoint-Files-to-Word
[2]: #Convert-PPTX-or-PPT-to-DOCX
[3]: https://products.aspose.com/slides/net
[4]: https://products.aspose.com/words/net
[5]: https://downloads.aspose.com/
[6]: https://products.aspose.com/total/net/
[7]: https://apireference.aspose.com/slides/net/aspose.slides/presentation
[8]: https://docs.microsoft.com/en-us/dotnet/api/system.io.memorystream
[9]: https://apireference.aspose.com/words/net/aspose.words/document
[10]: https://apireference.aspose.com/words/net/aspose.words.document/save/methods/3
[11]: https://purchase.aspose.com/temporary-license
[12]: https://products.aspose.app/slides/conversion/pptx-to-docx
[13]: https://forum.aspose.com/
[14]: https://docs.aspose.com/slides/net/
[15]: https://docs.aspose.com/words/net/
[16]: https://blog.aspose.com/2020/12/04/create-powerpoint-presentations-in-csharp/






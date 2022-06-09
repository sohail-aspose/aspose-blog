---
title: 'Convert Word Documents to Markdown using C#'
seoTitle: "Convert Word to Markdown (.md) in C# | DOCX, DOC to MD in C# VB.NET"
description: "Use .NET Word API to convert MS Word documents to Markdown (.md) format in C# or VB.NET. Customize DOCX/DOC to MD conversion dynamically."
date: Fri, 12 Nov 2021 06:27:00 +0000
draft: false
url: /2021/11/12/convert-word-to-markdown-using-csharp/
author: Usman Aziz
summary: 'These days, a large number of articles, blogs, and documentation are written in [Markdown][1] ([MD][2] format. However, the Markdown syntax often becomes difficult to remember and write for large-sized documents. To make things easier, you can write content in MS Word and then convert [DOCX][3] or [DOC][4] document to Markdown. To automate Word to Markdown conversion, this article covers **how to convert Word documents to Markdown (.md) files using C#**.'
tags: ['convert doc to markdown in csharp', 'convert word document to markdown in csharp', 'convert word docx to markdown in csharp', 'convert word to md in csharp']
categories: ['Aspose.Words Product Family']
---



{{< figure align=center src="images/Word-to-Markdown.jpg" alt="Convert Word to Markdown in C#">}}


These days, a large number of articles, blogs, and documentation are written in [Markdown][5] ([MD][6] format. However, the Markdown syntax often becomes difficult to remember and write for large-sized documents. To make things easier, you can write content in MS Word and then convert [DOCX][7] or [DOC][8] document to Markdown. To automate Word to Markdown conversion, this article covers **how to convert Word documents to Markdown (.md) files using C#**.

*   [Word to Markdown Converter Library][9]
*   [Convert a Word Document to Markdown][10]
*   [Customize Word to Markdown Conversion][11]

## C# Word to Markdown Converter Library {#Word-to-Markdown-Converter-Library}

[Aspose.Words for .NET][12] is designed to create and manipulate Word documents from within .NET applications. In addition, it provides a built-in converter to convert MS Word documents to other formats. We will use this API to convert Word documents to Markdown format. You can [download][13] the API’s DLL or install it from [NuGet][14] using the package manager console.

```
PM> Install-Package Aspose.Words
```

## Convert a Word Document to Markdown in C# {#Convert-a-Word-Document-to-Markdown}

The following are the steps to convert a Word DOCX file to Markdown format in C#.

*   Load the Word file using [Document][15] class.
*   Convert Word file to Markdown format using [Document.Save(string)][16] method.

The following code sample shows how to convert a DOCX file to Markdown format using C#.

{{< gist aspose-com-gists 25a9ab1cf8da8a1e4c1772a67b52b2ef "word-to-markdown.cs" >}}

## Customize Word to Markdown Conversion {#Customize-Word-to-Markdown-Conversion}

You can also customize the default behavior of Word to Markdown conversion using different options. For example, you can set the alignment of the content in the tables, specify a folder to keep images, and so on. The following are the steps to customize Word to Markdown conversion.

*   Load the Word document using [Document][17] class.
*   Create an object of [MarkdownSaveOptions][18] class.
*   Set desired options such as [MarkdownSaveOptions.ImagesFolder][19].
*   Convert Word document to Markdown using [Document.Save(string, MarkdownSaveOptions)][20] method.

The following code sample shows how to customize DOCX to Markdown conversion using C#.

{{< gist aspose-com-gists 25a9ab1cf8da8a1e4c1772a67b52b2ef "word-to-markdown-custom.cs" >}}

## Get a Free API License {#Get-a-Free-API-License}

You can use Aspose.Words for .NET without evaluation limitations using a [temporary license][21].

## Conclusion

In this article, you have learned how to convert Word DOCX/DOC files to Markdown (.md) in C#. Moreover, you have seen how to customize Word to Markdown conversion using different options. You can also explore other features offered by Aspose.Words for .NET using the [documentation][22]. Also, you can feel free to ask your questions via our [forum][23].

## See Also

*   [Create Word Documents in C# without MS Office][24]
*   [Generate Word Documents from Templates in C# .NET][25]
*   [Convert Word Files to PDF in C#][26]




[1]: https://en.wikipedia.org/wiki/Markdown
[2]: https://docs.fileformat.com/word-processing/md/)
[3]: https://docs.fileformat.com/word-processing/docx/
[4]: https://docs.fileformat.com/word-processing/doc/
[5]: https://en.wikipedia.org/wiki/Markdown
[6]: https://docs.fileformat.com/word-processing/md/)
[7]: https://docs.fileformat.com/word-processing/docx/
[8]: https://docs.fileformat.com/word-processing/doc/
[9]: #Word-to-Markdown-Converter-Library
[10]: #Convert-a-Word-Document-to-Markdown
[11]: #Customize-Word-to-Markdown-Conversion
[12]: https://products.aspose.com/words/net/
[13]: https://downloads.aspose.com/words/net
[14]: https://www.nuget.org/packages/Aspose.Words
[15]: https://apireference.aspose.com/words/net/aspose.words/document
[16]: https://apireference.aspose.com/words/net/aspose.words.document/save/methods/2
[17]: https://apireference.aspose.com/words/net/aspose.words/document
[18]: https://apireference.aspose.com/words/net/aspose.words.saving/markdownsaveoptions
[19]: https://apireference.aspose.com/words/net/aspose.words.saving/markdownsaveoptions/properties/imagesfolder
[20]: https://apireference.aspose.com/words/net/aspose.words.document/save/methods/2
[21]: https://purchase.aspose.com/temporary-license
[22]: https://docs.aspose.com/words/net/
[23]: https://forum.aspose.com/
[24]: https://blog.aspose.com/2020/01/08/csharp-word-automation-create-edit-process-word-documents/
[25]: https://blog.aspose.com/2020/03/05/generate-word-documents-from-templates-in-csharp-net/
[26]: https://blog.aspose.com/2020/01/02/convert-word-doc-docx-to-pdf-in-csharp-net-core/





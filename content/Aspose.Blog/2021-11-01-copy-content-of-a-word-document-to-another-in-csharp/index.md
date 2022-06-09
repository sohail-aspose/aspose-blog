---
title: 'Copy Content from a Word Document to Another in C#'
seoTitle: "C#: Copy Content from a Word Document to Another | Clone Word DOCX"
description: "Use .NET Word library to copy content of a Word document to another in C# or VB.NET. Create a copy of a Word document and save it as a new document."
date: Mon, 01 Nov 2021 13:43:00 +0000
draft: false
url: /2021/11/01/copy-content-of-a-word-document-to-another-in-csharp/
author: Usman Aziz
summary: 'MS Word is a popular and widely used word processing software to create rich text documents. While working with Word documents, you may need to copy the content from one document to another. Moreover, the clones of Word documents are also required in certain cases. To perform these operations programmatically, this article covers **how to copy the content from one Word document to another in C#**. Also, you will learn how to create a copy of a Word document programmatically.'
tags: ['clone word documents in csharp', 'copy content of a word doc to another csharp', 'copy content of a word document to another csharp', 'copy content of a word docx to another csharp']
categories: ['Aspose.Words Product Family']
---



{{< figure align=center src="images/Copy-Word-Documents.jpg" alt="Copy content from one word document to another in C#">}}


MS Word is a popular and widely used word processing software to create rich text documents. While working with Word documents, you may need to copy the content from one document to another. Moreover, the clones of Word documents are also required in certain cases. To perform these operations programmatically, this article covers **how to copy the content from one Word document to another in C#**. Also, you will learn how to create a copy of a Word document programmatically.

*   [C# Library to Copy Content of Word Documents][1]
*   [Copy Content from One Word Document to Another][2]
*   [Create Copy of a Word Document][3]

## C# Library to Copy Content of Word Documents {#Library-to-Copy-Content-from-Word-Documents}

To copy the content from one Word document to another, we will use [Aspose.Words for .NET][4]. It is a feature-rich library to implement word processing features from within .NET applications. You can [download][5] the API’s DLL or install it directly from [NuGet][6] using the package manager console.

```
PM> Install-Package Aspose.Words
```

## Copy Content from a Word Document to Another using C# {#Copy-Content-from-One-Word-Document-to-Another}

The following are the steps to copy the content of a Word document to another using C#.

*   Load the source Word document using [Document][7] class.
*   Similarly, load the destination document using [Document][8] class.
*   Copy the content of source Word document into destination document using [Document.AppendDocument(Document, ImportFormatMode)][9] method.
*   Save the destination document using [Document.Save(string)][10] method.

The following code sample shows how to copy the content of a Word document to another.

{{< gist aspose-com-gists 0b41e0adc9a80929ced47d11d5aca759 "copy-content.cs" >}}

## Create Copy of a Word Document in C# {#Create-Copy-of-a-Word-Document}

You can also copy the content of a Word document into a new document. In other words, you can create clone of a document. The following steps show how to create a copy of the Word document using C#.

*   Load the Word document using [Document][11] class.
*   Create a clone using [Document.Clone()][12] method.
*   Save the cloned document using [Document.Save(string)][13] method.

The following code sample shows how to create a copy of a Word DOCX file in C#.

{{< gist aspose-com-gists 0b41e0adc9a80929ced47d11d5aca759 "clone-document.cs" >}}

## Get a Free API License {#Get-a-Free-API-License}

You can [get a temporary license][14] in order to use Aspose.Words for .NET without evaluation limitations.

## Conclusion

In this article, you have learned how to copy the content from a Word document to another in C#. Moreover, you have seen how to clone a Word document programmatically. Aspose.Words for .NET provides a wide range of other features that you can explore using the [documentation][15]. Also, you can ask your queries via our [forum][16].

## See Also

*   [Create Word Documents in C# without MS Office][17]
*   [Generate Word Documents from Templates in C# .NET][18]




[1]: #Library-to-Copy-Content-from-Word-Documents
[2]: #Copy-Content-from-One-Word-Document-to-Another
[3]: #Create-Copy-of-a-Word-Document
[4]: https://products.aspose.com/words/net/
[5]: https://downloads.aspose.com/words/net
[6]: https://www.nuget.org/packages/Aspose.Words
[7]: https://apireference.aspose.com/words/net/aspose.words/document
[8]: https://apireference.aspose.com/words/net/aspose.words/document
[9]: https://apireference.aspose.com/words/net/aspose.words/document/methods/appenddocument
[10]: https://apireference.aspose.com/words/net/aspose.words.document/save/methods/2
[11]: https://apireference.aspose.com/words/net/aspose.words/document
[12]: https://apireference.aspose.com/words/net/aspose.words/document/methods/clone
[13]: https://apireference.aspose.com/words/net/aspose.words.document/save/methods/2
[14]: https://purchase.aspose.com/temporary-license
[15]: https://docs.aspose.com/words/net/
[16]: https://forum.aspose.com/
[17]: https://blog.aspose.com/2020/01/08/csharp-word-automation-create-edit-process-word-documents/
[18]: https://blog.aspose.com/2020/03/05/generate-word-documents-from-templates-in-csharp-net/





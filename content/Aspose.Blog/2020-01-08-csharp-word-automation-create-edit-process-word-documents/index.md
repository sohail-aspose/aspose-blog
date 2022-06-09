---
title: '.NET Word Automation - Create, Edit or Convert MS Word Documents using C#'
seoTitle: ""
description: ""
date: Wed, 08 Jan 2020 08:42:26 +0000
draft: false
url: /2020/01/08/csharp-word-automation-create-edit-process-word-documents/
author: Usman Aziz
summary: "Are you looking for a .NET Word Automation solution to create and process word processing documents in C#? Do you want to create, edit/modify, and convert Word documents programmatically without requiring MS Office? Let's try out Aspose.Words for .NET API - A complete set of features for creating and processing of MS Word documents (.doc, .docx, etc.) using C# in your .NET or .NET Core based applications."
tags: ['.NET Word API', '.NET Word Library', '.net office library', 'Aspose.Words for .NET', 'C# Word API', 'C# Word Library', 'C# word automation', 'Create Word Document C#', 'Edit Word Document C#', 'Generate Word Document C#', 'Word Processing Library', 'aspose word api', 'ms word library c#', 'word automation api', 'word automation using c#']
categories: ['Aspose.Words Product Family']
---



{{< figure align=center src="images/C-Word-Automation.png" alt="C# .NET Word Automation">}}


Are you looking for a **.NET Word Automation** solution  to create and process word processing documents in **C#**? Do you want to **create**, **edit/modify,** and **convert Word** documents **programmatically** without requiring MS Office? Let's try out **[Aspose.Words for .NET][1]** API which provides a complete set of features to create **MS Word** documents (.doc, .docx, etc.) using **C#** in your **.NET** applications.

MS Word document automation and report generation are in high demand by enterprises. _Aspose.Words for .NET_ is a complete and feature-rich Word automation solution to create, edit, or analyze Word documents in such cases. This article covers all the basic features required for generating and manipulating the Word documents programmatically using C#. Once you read this article, you will be able to:

*   [Create a Word (.doc, .docx) document using C#][2]
*   [Edit or modify a Word document using C#][3]
*   [Convert a Word document using C#][4]
*   [Parse a Word document using C#][5]

## Create Word Documents - C# Word Automation API

_Aspose.Words for .NET_ DLL can be downloaded from [here][6]. Another option is to install it via NuGet Package Manager or Package Manager Console in Visual Studio.

### Using NuGet Package Manager



{{< figure align=center src="images/Aspose.Words-NuGet.png" alt="C# .NET Word Automation Library">}}


### Using Package Manager Console```
PM> Install-Package Aspose.Words
```

## Create a Word Document using C# {#Create-a-Word-doc-docx-document}

Let's start our journey by creating a new Word document using _Aspose.Words for .NET_. The [DocumentBuilder][7] class of the API contains all the methods and properties to create Word documents from scratch. In combination with the [Document][8] class, _DocumentBuilder_ supports inserting elements such as text/paragraphs, checkboxes, tables, lists, images, and the other objects that a Word document can contain. Moreover, you can specify the font and other formatting options using this class.

The following are the steps to create a Word document using _DocumentBuilder_ class.

*   Create a new _Document_ object.
*   Create and new _DocumentBuilder_ object and initialize it with the _Document_ object.
*   Insert/write elements using the _DocumentBuilder_ object.
*   Save the document using [Document.Save][9] method.

The following code sample shows how to create a Word DOCX document with using C#.

{{< gist aspose-com-gists 9d87de8e13e5ad79213ef7e37038e252 "CreateWordDocumentinCSharp.cs" >}}

The following is the document we get after executing the above code.



{{< figure align=center src="images/Creating-a-Word-Document-in-C.png" alt="Create Word document in C# .NET">}}


Visit [these articles][10] to explore more about the elements you can add to a Word document using _Aspose.Words for .NET_.

## Edit a Word Document in C# {#Edit-or-modify-a-Word-document-using-CSharp}

You can also edit or modify the existing Word documents using _Aspose.Words for .NET_. _Aspose.Words_ Document Object Model classes let you access and modify the document's elements as well as their formatting. DOM is actually the in-memory representation of the document. To understand the document representation as DOM, please see the [DOM overview][11].

Let's now check out how to edit an existing element in a Word document. Suppose we need to update the text "This is the first page." in the document that we have recently created. Since this is the first paragraph in the first section of the document, we can access it by specifying the index of the first section and the first paragraph. The following code sample shows how to edit the paragraph in the Word document using C#.

{{< gist aspose-com-gists 9d87de8e13e5ad79213ef7e37038e252 "EditWordDocument.cs" >}}

The following is the updated Word document.



{{< figure align=center src="images/Edit-a-Word-Document-in-C.png" alt="Word Automation in C# .NET">}}


## Convert Word Document to Other Formats in C# {#Convert-a-Word-document-using-CSharp}

Along with creating and manipulating Word documents, Aspose.Words for .NET also allows converting a document to other formats including (but not limited to) PDF, XPS, EPUB, HTML, and image formats such as BMP, PNG or JPEG. The following code sample shows how to convert a Word document to PDF in C#.

{{< gist aspose-com-gists 9d87de8e13e5ad79213ef7e37038e252 "ConvertWordDocumentToPDF.cs" >}}

Visit [this article][12] to see how to convert a Word document to other formats.

## Parse a Word Document in C# {#Parse-a-Word-document-using-CSharp}

You can also parse a Word document by extracting its content as plain text. The following code sample shows how to extract text from a Word document and save it into a _.txt_ file.

{{< gist aspose-com-gists 9d87de8e13e5ad79213ef7e37038e252 "ParseWordDocument.cs" >}}

## Conclusion

In this article, you have seen how to **create or edit MS Word DOC/DOCX documents using C#**. Furthermore, you have learned how to convert or parse MS Word documents programmatically. Visit the documentation of _Aspose.Words for .NET_ for a complete Developer's Guide. In case you would find anything confusing for you, do let us know via our [forum][13].

## Related Article(s)

*   [Convert Word Documents to PDF using C#][14] - A complete guide.




[1]: https://products.aspose.com/words/net
[2]: #Create-a-Word-doc-docx-document
[3]: #Edit-or-modify-a-Word-document-using-CSharp
[4]: #Convert-a-Word-document-using-CSharp
[5]: #Parse-a-Word-document-using-CSharp
[6]: https://downloads.aspose.com/words/net
[7]: https://apireference.aspose.com/net/words/aspose.words/documentbuilder
[8]: https://apireference.aspose.com/net/words/aspose.words/document
[9]: https://apireference.aspose.com/net/words/aspose.words.document/save/methods/2
[10]: https://docs.aspose.com/display/wordsnet/Programming+with+Documents
[11]: https://docs.aspose.com/display/wordsnet/Aspose.Words+Document+Object+Model#Aspose.WordsDocumentObjectModel-ObjectModelOverview
[12]: https://docs.aspose.com/display/wordsnet/Converting+a+Document
[13]: https://forum.aspose.com/c/words
[14]: https://blog.aspose.com/2020/01/02/convert-word-doc-docx-to-pdf-in-csharp-net-core/






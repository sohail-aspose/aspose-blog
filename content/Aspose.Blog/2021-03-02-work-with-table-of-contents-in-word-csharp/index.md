---
title: 'Work with Table of Contents in Word Document using C#'
seoTitle: "Work with Table of Contents in Word Document C# | Add, Update, Remove"
description: "Use .NET Word automation API to work with table of contents (TOC) in Word documents using C#. Add, update, extract, and remove TOC in Word documents."
date: Tue, 02 Mar 2021 10:47:00 +0000
draft: false
url: /2021/03/02/work-with-table-of-contents-in-word-csharp/
author: Usman Aziz
summary: '[Table of Contents][1] (TOC) in a Word document gives you an overview of what a document contains. Furthermore, it lets you navigate to a particular section of the document. In this article, you will learn how to work with a table of contents in Word documents programmatically using C#. Particularly, this article covers how to add, extract, update or remove a table of contents in Word documents.'
tags: ['Add Table of Contents in a Word Document', 'Extract Table of Contents from a Word Document csharp', 'Remove Table of Contents in a Word Document csharp', 'Update Table of Contents in a Word Document csharp', 'Work with TOC in Word Documents Csharp']
categories: ['Aspose.Words Product Family']
---

[Table of Contents][2] (TOC) in a Word document gives you an overview of what a document contains. Furthermore, it lets you navigate to a particular section of the document. In this article, you will learn how to work with a table of contents in Word documents programmatically using C#. Particularly, this article covers how to add, extract, update or remove a table of contents in Word documents.

*   [C# API to Work with TOC in Word Documents][3]
*   [Add Table of Contents in a Word Document][4]
*   [Extract Table of Contents from a Word Document][5]
*   [Update Table of Contents in a Word Document][6]
*   [Remove Table of Contents in a Word Document][7]
*   [Get a Free API License][8]

## C# API to Work with TOC in Word Document {#API-to-Work-with-TOC-in-Word-Document}

In order to work with tables of contents in Word documents, we will use [Aspose.Words for .NET][9]. The said API is designed to perform basic as well as advanced Word automation features from within .NET applications. Furthermore, it gives you a sound grip over the manipulation of table of contents in Word documents. You can either [download][10] the API or install it using [NuGet][11].

```
PM> Install-Package Aspose.Words
```

## Add Table of Contents in a Word Document using C# {#Add-Table-of-Content-in-Word-Document}

The following are the steps to add a table of contents to Word document using Aspose.Words for .NET.

*   Create an instance of the [Document][12] class (in case of loading an existing Word document, provide the file's path in the constructor).
*   Create an instance of [DocumentBuilder][13] class and initialize it with the _Document_ object created earlier.
*   Insert table of contents using [DocumentBuilder.InsertTableOfContents("\\\\o \\"1-3\\" \\\\h \\\\z \\\\u")][14] method.
*   Update the fields using [Document.UpdateFields()][15] method.
*   Save the Word document using [Document.Save(String)][16] method.

The following code sample shows how to add a table of contents in a Word document in C#.

{{< gist aspose-words 9a306a41bb6aea8adfcabf5a575c5718 "Examples-CSharp-Programming-Documents-Document-DocumentBuilderInsertTOC-DocumentBuilderInsertTOC.cs" >}}

## Extract Table of Contents from a Word Document using C# {#Extract-Table-of-Content-in-Word-Document}

The following are the steps to extract fields from a table of contents in a Word document.

*   Load the Word document using the [Document][17] class.
*   Loop through each [Field][18] in the document using [Document.Range.Fields][19] collection.
*   Check if the field type is a hyperlink using [Field.Type][20] property.
*   Check if the field comes under the table of the contents section.
*   Retrieve the information of the field and print it.

The following code sample shows how to extract a table of contents from a Word document using C#.

{{< gist aspose-com-gists 0b968ac8900f80c11e109dffb105f3da "Examples-CSharp-Programming-Documents-Document-ExtractTableOfContents-ExtractTableOfContents.cs" >}}

## Update Table of Contents in Word Document using C# {#Update-Table-of-Content-in-Word-Document}

Whenever you append some content to a Word document, you need to update the table of contents. In order to do it programmatically, you simply need to call [Document.UpdateFields()][21] method before saving the document.

## Remove Table of Contents in Word Document using C# {#Remove-Table-of-Contents-in-Word-Document}

Aspose.Words for .NET also allows you to remove the table of contents from a Word document. The following are the steps to perform this operation.

*   First, load the Word document using the [Document][22] class.
*   Get and store the [FieldStart][23] nodes of each TOC in an array.
*   Loop through the nodes until you get the node of type [FieldEnd][24] (end of the TOC).
*   Remove the nodes using [Node.Remove()][25] method and save the updated document.

The following code sample shows how to remove the table of contents from a Word document in C#.

{{< gist aspose-words 9a306a41bb6aea8adfcabf5a575c5718 "Examples-CSharp-Programming-Documents-Document-RemoveTOCFromDocument-RemoveTOCFromDocument.cs" >}}

## Get a Free API License {#Get-a-Free-API-License}

In case you want to try the API without evaluation limitations, you can [get a free temporary license][26].

## Conclusion

In this article, you have learned how to work with a table of contents in a Word document using C#. The step-by-step guide and code samples have shown how to add, update, extract and remove the table of contents from Word documents. You can explore more about C# Word automation API using [documentation][27]. In case you would have any questions or concerns, please contact us via our [forum][28].

## See Also

*   [Create, Edit or Convert MS Word Documents using C#][29]




[1]: https://en.wikipedia.org/wiki/Table_of_contents
[2]: https://en.wikipedia.org/wiki/Table_of_contents
[3]: #API-to-Work-with-TOC-in-Word-Document
[4]: #Add-Table-of-Content-in-Word-Document
[5]: #Extract-Table-of-Content-in-Word-Document
[6]: #Update-Table-of-Content-in-Word-Document
[7]: #Remove-Table-of-Contents-in-Word-Document
[8]: #Get-a-Free-API-License
[9]: https://products.aspose.com/words/net
[10]: https://downloads.aspose.com/words/net
[11]: https://www.nuget.org/packages/Aspose.Words
[12]: https://apireference.aspose.com/words/net/aspose.words/document
[13]: https://apireference.aspose.com/words/net/aspose.words/documentbuilder
[14]: https://apireference.aspose.com/words/net/aspose.words/documentbuilder/methods/inserttableofcontents
[15]: https://apireference.aspose.com/words/net/aspose.words/document/methods/updatefields
[16]: https://apireference.aspose.com/words/net/aspose.words.document/save/methods/2
[17]: https://apireference.aspose.com/words/net/aspose.words/document
[18]: https://apireference.aspose.com/words/net/aspose.words.fields/field
[19]: https://apireference.aspose.com/words/net/aspose.words/range/properties/fields
[20]: https://apireference.aspose.com/words/net/aspose.words.fields/field/properties/type
[21]: https://apireference.aspose.com/words/net/aspose.words/document/methods/updatefields
[22]: https://apireference.aspose.com/words/net/aspose.words/document
[23]: https://apireference.aspose.com/words/net/aspose.words.fields/fieldstart
[24]: https://apireference.aspose.com/words/net/aspose.words/nodetype
[25]: https://apireference.aspose.com/words/net/aspose.words/node/methods/remove
[26]: https://purchase.aspose.com/temporary-license
[27]: https://docs.aspose.com/words/net/product-overview/
[28]: https://forum.aspose.com/
[29]: https://blog.aspose.com/2020/01/08/csharp-word-automation-create-edit-process-word-documents/






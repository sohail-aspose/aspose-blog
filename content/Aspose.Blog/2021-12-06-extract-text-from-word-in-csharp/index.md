---
title: 'Extract Text from Word Documents in C#'
seoTitle: "Extract Text from Word DOCX DOC in C# | C# Docx Text Extractor"
description: "Use .NET Word library to extract text from MS Word DOCX DOC documents in C# or VB.NET. Extract text between paragraphs, tables, fields, etc. dynamically."
date: Mon, 06 Dec 2021 14:14:58 +0000
draft: false
url: /2021/12/06/extract-text-from-word-in-csharp/
author: Usman Aziz
summary: 'Text extraction from Word documents is often performed in different scenarios. For example, to analyze the text, to extract particular sections of a document and combine them into a single document, and so on. In this article, you will learn **how to extract text from Word documents programmatically in C#**. Moreover, we will cover **how to extract content between specific elements such as paragraphs, tables, etc. dynamically**.'
tags: ['extract text from doc documents in csharp', 'extract text from docx documents in csharp', 'extract text from word documents in csharp', 'ms word text extractor in csharp dotnet']
categories: ['Aspose.Words Product Family']
---



{{< figure align=center src="images/Extract-Text-from-Word-Documents.jpg" alt="Extract Text from MS Word Documents in C#">}}


Text extraction from Word documents is often performed in different scenarios. For example, to analyze the text, to extract particular sections of a document and combine them into a single document, and so on. In this article, you will learn **how to extract text from Word documents programmatically in C#**. Moreover, we will cover **how to extract content between specific elements such as paragraphs, tables, etc. dynamically**.

*   [Library to Extract Text from Word Documents][1]
*   [Text Extraction in Word Documents][2]
*   [Extract Text from a Word Document][3]
    *   [Extract Text between Paragraphs][4]
    *   [Text Extraction between Different Types of Nodes][5]
    *   [Extract Text between Paragraphs based on Styles][6]

**TIP:** You may want to check Aspose [PowerPoint to Word][7] Converter because it demonstrates the popular presentation to Word document conversion process.

## C# Library to Extract Text from Word Documents {#Library-to-Extract-Text-from-Word-Documents}

[Aspose.Words for .NET][8] is a powerful library that allows you to create MS Word documents from scratch. Moreover, it lets you manipulate the existing Word documents for encryption, conversion, text extraction, etc. We will use this library to extract text from the Word DOCX or DOC documents. You can [download][9] the API’s DLL or install it directly from [NuGet][10] using the package manager console.

```
PM> Install-Package Aspose.Words
```

## Text Extraction in Word Documents using C# {#Text-Extraction-in-Word-Documents}

An MS Word document consists of various elements which include paragraphs, tables, images, etc. Therefore, the requirements of text extraction could vary from one scenario to another. For example, you may need to extract text between paragraphs, bookmarks, comments, etc.

Each type of element in a Word document is represented as a node. Therefore, to process a document, you will have to play with the nodes. So let's begin and see how to extract text from Word documents in different scenarios.

## Extract Text from a Word Document in C# {#Extract-Text-from-a-Word-Document}

In this section, we are going to implement a C# text extractor for Word documents and the workflow of text extraction would be as follows:

*   First, we will define the nodes that we want to include in the text extraction process.
*   Then, we will extract the content between the specified nodes (including or excluding the starting and ending nodes).
*   Finally, we will use the clone of extracted nodes, e.g. to create a new Word document consisting of extracted content.

Let's now write a method named **ExtractContent** to which we will pass the nodes and some other parameters to perform the text extraction. This method will parse the document and clone the nodes. The following are the parameters that we will pass to this method.

1.  **StartNode** and **EndNode** as starting and ending points for the extraction of the content, respectively. These can be both block level (**Paragraph** , **Table**) or inline level (e.g **Run**, **FieldStart**, **BookmarkStart** etc.) nodes.
    1.  To pass a field you should pass the corresponding **FieldStart** object.
    2.  To pass bookmarks, the **BookmarkStart** and **BookmarkEnd** nodes should be passed.
    3.  For comments, the **CommentRangeStart** and **CommentRangeEnd** nodes should be used.
2.  **IsInclusive** defines if the markers are included in the extraction or not. If this option is set to false and the same node or consecutive nodes are passed, then an empty list will be returned.

The following is the complete implementation of the **ExtractContent** method that extracts the content between the nodes that are passed.

{{< gist aspose-com-gists 27785844db7029d5d9558f808c89c2b8 "extract-text.cs" >}}

Some helper methods are also required by the **ExtractContent** method to accomplish the text extraction operation, which are given below.

{{< gist aspose-com-gists 27785844db7029d5d9558f808c89c2b8 "text-extraction-helpers.cs" >}}

Now we are ready to utilize these methods and extract text from a Word document.

### Extract Text between Paragraphs in a Word Document {#Extract-Text-between-Paragraphs}

Let's see how to extract content between two paragraphs in a Word DOCX document. The following are the steps to perform this operation in C#.

*   First, load the Word document using **Document** class.
*   Get reference of the starting and ending paragraphs into two objects using **Document.FirstSection.Body.GetChild(NodeType.PARAGRAPH, int, boolean)** method.
*   Call **ExtractContent(startPara, endPara, True)** method to extract the nodes into an object.
*   Call **GenerateDocument(Document, extractedNodes)** helper method to create document consisting of the extracted content.
*   Finally, save the returned document using **Document.Save(string)** method.

The following code sample shows how to extract text between the 7th and 11th paragraphs in a Word document in C#.

{{< gist aspose-com-gists 27785844db7029d5d9558f808c89c2b8 "extract-text-paragraphs.cs" >}}

### Extract Text between Different Types of Nodes in a Word Document {#Text-Extraction-between-DifferentTypes-of-Nodes}

You can also extract content between different types of nodes. For demonstration, let's extract content between a paragraph and a table and save it into a new Word document. The following are the steps to perform this operation.

*   Load the Word document using **Document** class.
*   Get reference of the starting and ending nodes into two objects using **Document.FirstSection.Body.GetChild(NodeType, int, boolean)** method.
*   Call **ExtractContent(startPara, endPara, True)** method to extract the nodes into an object.
*   Call **GenerateDocument(Document, extractedNodes)** helper method to create document consisting of the extracted content.
*   Save the returned document using **Document.Save(string)** method.

The following code sample shows how to extract text between a paragraph and a table in C#.

{{< gist aspose-com-gists 27785844db7029d5d9558f808c89c2b8 "extract-text-nodes.cs" >}}

### Extract Text between Paragraphs based on Styles {#Extract-Text-between-Paragraphs-based-on-Styles}

Let's now check out how to extract content between paragraphs based on styles. For demonstration, we are going to extract content between the first "Heading 1" and the first "Heading 3" in the Word document. The following steps demonstrate how to achieve this in C#.

*   First, load the Word document using **Document** class.
*   Then, extract paragraphs into an object using **ParagraphsByStyleName(Document, "Heading 1")** helper method.
*   Extract paragraphs into another object using **ParagraphsByStyleName(Document, "Heading 3")** helper method.
*   Call **ExtractContent(startPara, endPara, True)** method and pass the first elements in both paragraph arrays as first and second parameters.
*   Call **GenerateDocument(Document, extractedNodes)** helper method to create document consisting of the extracted content.
*   Finally, save the returned document using **Document.Save(string)** method.

The following code sample shows how to extract content between paragraphs based on styles.

{{< gist aspose-com-gists 27785844db7029d5d9558f808c89c2b8 "extract-text-paragraphs-styles.cs" >}}

## Read More

You can explore other scenarios of extracting text from Word documents using [this][11] documentation article.

## Get a Free API License {#Get-a-Free-API-License}

You can get a [temporary license][12] to use Aspose.Words for .NET without evaluation limitations.

## Conclusion

In this article, you have learned how to extract text from MS Word documents using C#. Moreover, you have seen how to extract content between similar or different types of nodes in a Word document programmatically. Thus, you can build your own MS Word text extractor in C#. Besides, you can explore other features of Aspose.Words for .NET using the [documentation][13]. In case you would have any questions, feel free to let us know via our [forum][14].

## See Also

*   [Create Word Documents in C# without MS Office][15]
*   [Generate Word Documents from Templates in C# .NET][16]




[1]: #Library-to-Extract-Text-from-Word-Documents
[2]: #Text-Extraction-in-Word-Documents
[3]: #Extract-Text-from-a-Word-Document
[4]: #Extract-Text-between-Paragraphs
[5]: #Text-Extraction-between-DifferentTypes-of-Nodes
[6]: #Extract-Text-between-Paragraphs-based-on-Styles
[7]: https://products.aspose.app/slides/conversion/ppt-to-wordhttps://products.aspose.app/slides/conversion/ppt-to-word
[8]: https://products.aspose.com/words/net/
[9]: https://downloads.aspose.com/words/net
[10]: https://www.nuget.org/packages/Aspose.Words
[11]: https://docs.aspose.com/words/net/how-to-extract-selected-content-between-nodes-in-a-document/
[12]: https://purchase.aspose.com/temporary-license
[13]: https://docs.aspose.com/words/net/
[14]: https://forum.aspose.com/
[15]: https://blog.aspose.com/2020/01/08/csharp-word-automation-create-edit-process-word-documents/
[16]: https://blog.aspose.com/2020/03/05/generate-word-documents-from-templates-in-csharp-net/





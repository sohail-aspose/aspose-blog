---
title: 'Extract Text from Word Documents in Python'
seoTitle: "Extract Text from Word DOCX DOC in Python | Python Docx Text Extractor"
description: "Use Python Word library to extract text from MS Word DOCX DOC documents. Extract text between paragraphs, tables, fields, etc. dynamically."
date: Thu, 25 Nov 2021 14:58:26 +0000
draft: false
url: /2021/11/25/extract-text-from-word-docx-in-python/
author: Usman Aziz
summary: "Text extraction from Word documents is often performed in different scenarios. For example, to analyze the text, to extract particular sections of a document and combine them into a single document, and so on. In this article, you will learn **how to extract text from Word documents programmatically in Python**. Moreover, we will cover **how to extract content between specific elements such as paragraphs, tables, etc. dynamically**."
tags: ['Python Docx Text Extractor', 'extract content from word document python', 'extract content from word docx python', 'extract text from word document python', 'extract text from word docx python']
categories: ['Aspose.Words Product Family']
---



{{< figure align=center src="images/Extract-Text-in-Word-Documents-in-Python.jpg" alt="Extract Content from Word DOCX documents in Python">}}


Text extraction from Word documents is often performed in different scenarios. For example, to analyze the text, to extract particular sections of a document and combine them into a single document, and so on. In this article, you will learn **how to extract text from Word documents programmatically in Python**. Moreover, we will cover **how to extract content between specific elements such as paragraphs, tables, etc. dynamically**.

*   [Python Library to Extract Text from Word Documents][1]
*   [Text Extraction in Word Documents][2]
*   [Extract Text from a Word Document][3]
    *   [Extract Text between Paragraphs][4]
    *   [Text Extraction between Different Types of Nodes][5]
    *   [Extract Text between Paragraphs based on Styles][6]

**Info**: If you ever need to get a Word document from a PowerPoint presentation, you can use Aspose [Presentation to Word Document][7] converter.

## Python Library to Extract Text from Word Documents {#Python-Library-to-Extract-Text-from-Word-Documents}

[Aspose.Words for Python][8] is a powerful library that allows you to create MS Word documents from scratch. Moreover, it lets you manipulate the existing Word documents for encryption, conversion, text extraction, etc. We will use this library to extract text from the Word DOCX or DOC documents. You can install the library from [PyPI][9] using the following pip command.

```
pip install aspose-words
```

## Text Extraction in Word Documents using Python {#Text-Extraction-in-Word-Documents}

An MS Word document consists of various elements which include paragraphs, tables, images, etc. Therefore, the requirements of text extraction could vary from one scenario to another. For example, you may need to extract text between paragraphs, bookmarks, comments, etc.

Each type of element in a Word document is represented as a node. Therefore, to process a document, you will have to play with the nodes. So let's begin and see how to extract text from Word documents in different scenarios.

## Extract Text from a Word Document in Python {#Extract-Text-from-a-Word-Document}

In this section, we are going to implement a Python text extractor for Word documents and the workflow of text extraction would be as follows:

*   First, we will define the nodes that we want to include in the text extraction process.
*   Then, we will extract the content between the specified nodes (including or excluding the starting and ending nodes).
*   Finally, we will use the clone of extracted nodes, e.g. to create a new Word document consisting of extracted content.

Let's now write a method named **extract\_content** to which we will pass the nodes and some other parameters to perform the text extraction. This method will parse the document and clone the nodes. The following are the parameters that we will pass to this method.

1.  **StartNode** and **EndNode** as starting and ending points for the extraction of the content, respectively. These can be both block level (**Paragraph** , **Table**) or inline level (e.g **Run**, **FieldStart**, **BookmarkStart** etc.) nodes.
    1.  To pass a field you should pass the corresponding **FieldStart** object.
    2.  To pass bookmarks, the **BookmarkStart** and **BookmarkEnd** nodes should be passed.
    3.  For comments, the **CommentRangeStart** and **CommentRangeEnd** nodes should be used.
2.  **IsInclusive** defines if the markers are included in the extraction or not. If this option is set to false and the same node or consecutive nodes are passed, then an empty list will be returned.

The following is the complete implementation of the **extract\_content** method that extracts the content between the nodes that are passed.

{{< gist aspose-com-gists 91bf64bdf5aaea2eac1615bdd85841e1 "extract-text.py" >}}

Some helper methods are also required by **extract\_content** method to accomplish the text extraction operation, which are given below.

{{< gist aspose-com-gists 91bf64bdf5aaea2eac1615bdd85841e1 "text-extraction-helpers.py" >}}

Now we are ready to utilize these methods and extract text from a Word document.

### Extract Text between Paragraphs in a Word Document {#Extract-Text-between-Paragraphs}

Let's see how to extract content between two paragraphs in a Word DOCX document. The following are the steps to perform this operation in Python.

*   First, load the Word document using **Document** class.
*   Get reference of the starting and ending paragraphs into two objects using **Document.first\_section.body.get\_child(NodeType.PARAGRAPH, int, boolean).as\_paragraph()** method.
*   Call **extract\_content(startPara, endPara, True)** method to extract the nodes into an object.
*   Call **generate\_document(Document, extractedNodes)** helper method to create document consisting of the extracted content.
*   Finally, save the returned document using **Document.save(string)** method.

The following code sample shows how to extract text between the 7th and 11th paragraphs in a Word document in Python.

{{< gist aspose-com-gists 91bf64bdf5aaea2eac1615bdd85841e1 "extract-text-paragraphs.py" >}}

### Extract Text between Different Types of Nodes in a Word Document {#Text-Extraction-between-DifferentTypes-of-Nodes}

You can also extract content between different types of nodes. For demonstration, let's extract content between a paragraph and a table and save it into a new Word document. The following are the steps to perform this operation.

*   Load the Word document using **Document** class.
*   Get reference of the starting and ending nodes into two objects using **Document.first\_section.body.get\_child(NodeType, int, boolean)** method.
*   Call **extract\_content(startPara, endPara, True)** method to extract the nodes into an object.
*   Call **generate\_document(Document, extractedNodes)** helper method to create document consisting of the extracted content.
*   Save the returned document using **Document.save(string)** method.

The following code sample shows how to extract text between a paragraph and a table in Python.

{{< gist aspose-com-gists 91bf64bdf5aaea2eac1615bdd85841e1 "extract-text-nodes.py" >}}

### Extract Text between Paragraphs based on Styles {#Extract-Text-between-Paragraphs-based-on-Styles}

Let's now check out how to extract content between paragraphs based on styles. For demonstration, we are going to extract content between the first "Heading 1" and the first "Heading 3" in the Word document. The following steps demonstrate how to achieve this in Python.

*   First, load the Word document using **Document** class.
*   Then, extract paragraphs into an object using **paragraphs\_by\_style\_name(Document, "Heading 1")** helper method.
*   Extract paragraphs into another object using **paragraphs\_by\_style\_name(Document, "Heading 3")** helper method.
*   Call **extract\_content(startPara, endPara, True)** method and pass the first elements in both paragraph arrays as first and second parameters.
*   Call **generate\_document(Document, extractedNodes)** helper method to create document consisting of the extracted content.
*   Finally, save the returned document using **Document.save(string)** method.

The following code sample shows how to extract content between paragraphs based on styles.

{{< gist aspose-com-gists 91bf64bdf5aaea2eac1615bdd85841e1 "extract-text-paragraphs-styles.py" >}}

## Read More

You can explore other scenarios of extracting text from Word documents using [this][10] documentation article.

## Get a Free API License {#Get-a-Free-API-License}

You can get a [temporary license][11] to use Aspose.Words for Python without evaluation limitations.

## Conclusion

In this article, you have learned how to extract text from MS Word documents using Python. Moreover, you have seen how to extract content between similar or different types of nodes in a Word document programmatically. Thus, you can build your own MS Word text extractor in Python. Besides, you can explore other features of Aspose.Words for Python using the [documentation][12]. In case you would have any questions, feel free to let us know via our [forum][13].

## See Also

*   [Create MS Word Documents using Python][14]
*   [Convert Word Document to HTML using Python][15]
*   [Convert Word Documents to PNG, JPEG, or BMP in Python][16]
*   [Word Documents to Markdown using Python][17]
*   [Compare Two Word Documents in Python][18]




[1]: #Python-Library-to-Extract-Text-from-Word-Documents
[2]: #Text-Extraction-in-Word-Documents
[3]: #Extract-Text-from-a-Word-Document
[4]: #Extract-Text-between-Paragraphs
[5]: #Text-Extraction-between-DifferentTypes-of-Nodes
[6]: #Extract-Text-between-Paragraphs-based-on-Styles
[7]: https://products.aspose.app/slides/conversion/ppt-to-word
[8]: https://products.aspose.com/words/python/
[9]: https://pypi.org/project/aspose-words/
[10]: https://docs.aspose.com/words/python/how-to-extract-selected-content-between-nodes-in-a-document/
[11]: https://purchase.aspose.com/temporary-license
[12]: https://docs.aspose.com/words/python/product-overview/
[13]: https://forum.aspose.com/
[14]: https://blog.aspose.com/2021/10/28/create-word-documents-using-python/
[15]: https://blog.aspose.com/2021/11/01/convert-word-to-html-in-python/
[16]: https://blog.aspose.com/2021/11/04/convert-word-to-png-jpg-bmp-in-python/
[17]: https://blog.aspose.com/2021/11/05/convert-word-to-markdown-using-python/
[18]: https://blog.aspose.com/2021/11/11/compare-two-word-documents-in-python/





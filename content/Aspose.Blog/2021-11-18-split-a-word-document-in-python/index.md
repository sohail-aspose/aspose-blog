---
title: 'Split a Word Document into Multiple Files in Python'
seoTitle: "Split a Word DOCX DOC in Python | Python Word Document Splitter"
description: "Use Python Word library to split a Word document into multiple documents using Python. Split the document by sections, pages, or a page range."
date: Thu, 18 Nov 2021 13:13:31 +0000
draft: false
url: /2021/11/18/split-a-word-document-in-python/
author: Usman Aziz
summary: 'In certain cases, you need to split the large Word documents by breaking them down into smaller ones. You can split a Word document by pages, sections, or columns. In this article, you will learn **how to split a Word document into multiple files using Python**. The step-by-step guide and code samples will demonstrate how to split a Word document by sections, pages, or page ranges programmatically.'
tags: ['Python word document splitter', 'split docx in python', 'split word document by page in python', 'split word document by sections in python', 'split word document in python']
categories: ['Aspose.Words Product Family']
---



{{< figure align=center src="images/Split-Word-Documents.jpg" alt="Split Word Documents into Multiple Files in Python">}}


In certain cases, you need to split the large Word documents by breaking them down into smaller ones. You can split a Word document by pages, sections, or columns. In this article, you will learn **how to split a Word document into multiple files using Python**. The step-by-step guide and code samples will demonstrate how to split a Word document by sections, pages, or page ranges programmatically.

*   [Python Library to Split MS Word Documents][1]
*   [Split a Word Document by Sections][2]
*   [Splitting a Word Document by Pages][3]
*   [Split a Word Document by a Page Range][4]

## Python Library to Split MS Word Documents {#Python-Library-to-Split-MS-Word-Documents}

To split a DOCX or DOC document into multiple files, we will use [Aspose.Words for Python][5]. It is a word processing library to create and manipulate Word documents. You can install it in your Python applications from [PyPI][6] using the following pip command.

```
pip install aspose-words 
```

## Split a Word Document by Sections in Python {#Split-a-Word-Document-by-Sections}

In most cases, the Word document is divided into multiple sections using section breaks. To save each section into a separate file, you can split the document by sections. The following steps demonstrate how to split a Word document by sections in Python.

*   Load the Word document using _Document_ class.
*   Loop thourght each section in _Document.sections_ collection.
*   For each section in the collection, perform the following steps:
    *   Create a new object of _Document_ class.
    *   Clear the default sections using _Document.sections.clear()_ method.
    *   Import section into new document using _Document.import\_node(Section, True).as\_section()_ method and get the returned _Section_ in an object.
    *   Add returned _Section_ to the sections collection of new document.
    *   Save the new document as a DOCX file using _Document.save(string)_ method.

The following code sample shows how to split a Word document by sections in Python.

{{< gist aspose-com-gists f528be76773cd3f9b26076b527b0c55b "split-word-document-by-section.py" >}}

## Splitting a Word Document by Pages in Python {#Splitting-a-Word-Document-by-Pages}

Now, let's have a look at how to split each page of the document and save it as a separate DOCX file. The following are the steps to split a Word document by pages.

*   Load the Word document using _Document_ class.
*   Get the page count in the document using _Document.page\_count_ property.
*   Loop through the page count and in each iteration, perform the following steps:
    
    *   Extract the page into an object using _Document.extract\_pages(pageIndex, 1)_ method.
    
    *   Save the extracted page as a DOCX file using _Document.save(string)_ method.

The following code sample shows how to split a Word document by pages.

{{< gist aspose-com-gists f528be76773cd3f9b26076b527b0c55b "split-word-document-by-page.py" >}}

## Split a Word Document by a Page Range in Python {#Split-a-Word-Document-by-a-Page-Range}

You can also split a range of pages in a Word document and save it as a separate file. The following are the steps to achieve this in Python.

*   Load the Word document using _Document_ class.
*   Extract the pages using _Document.extract\_pages(int, int)_ method where first parameter is the starting page's index and the second is number of pages.
*   Save the extracted page range as a DOCX file using _Document.save(string)_ method.

The following code sample shows how to extract a range of pages from a Word document and save it as a DOCX file.

{{< gist aspose-com-gists f528be76773cd3f9b26076b527b0c55b "split-word-document-by-page-range.py" >}}

## Get a Free API License {#Get-a-Free-API-License}

Are you interested in trying Aspose.Words for Python for free? [Get a temporary license][7] to avoid evaluation limitations.

## Conclusion

In this article, you have learned how to split a Word document into multiple documents in Python. The code samples have demonstrated how to split a Word document by sections, pages, or a page range. Aspose.Words for Python also provides a number of exciting features that you can explore using the [documentation][8]. Also, you can post your questions to our [forum][9].

## See Also

*   [Create MS Word Documents using Python][10]
*   [Convert Word Document to HTML using Python][11]
*   [Convert Word Documents to PNG, JPEG, or BMP in Python][12]
*   [Word Documents to Markdown using Python][13]
*   [Compare Two Word Documents in Python][14]




[1]: #Python-Library-to-Split-MS-Word-Documents
[2]: #Split-a-Word-Document-by-Sections
[3]: #Splitting-a-Word-Document-by-Pages
[4]: #Split-a-Word-Document-by-a-Page-Range
[5]: https://products.aspose.com/words/python/
[6]: https://pypi.org/project/aspose-words/
[7]: https://purchase.aspose.com/temporary-license
[8]: https://docs.aspose.com/words/python/product-overview/
[9]: https://forum.aspose.com/
[10]: https://blog.aspose.com/2021/10/28/create-word-documents-using-python/
[11]: https://blog.aspose.com/2021/11/01/convert-word-to-html-in-python/
[12]: https://blog.aspose.com/2021/11/04/convert-word-to-png-jpg-bmp-in-python/
[13]: https://blog.aspose.com/2021/11/05/convert-word-to-markdown-using-python/
[14]: https://blog.aspose.com/2021/11/11/compare-two-word-documents-in-python/





---
title: 'Combine Word Documents using Python'
seoTitle: "Combine Word Documents using Python | Merge DOCX in Python"
description: "Learn how to combine Word documents using Python. Combine two or more DOCX documents into a single one from within your Python applications."
date: Fri, 12 Nov 2021 09:47:55 +0000
draft: false
url: /2021/11/12/combine-word-documents-using-python/
author: Usman Aziz
summary: 'There could be various scenarios when you have to combine multiple Word documents into a single file. For example, when multiple persons are writing different sections of a document and you need to combine the content at the end. On the other hand, you may need to merge all the invoices in one Word document. To perform this merging programmatically, this article covers **how to combine multiple Word DOCX/DOC documents in Python**.'
tags: ['combine docx in python', 'combine word documents using python', 'merge docx files in python', 'merge word documents in python']
categories: ['Aspose.Words Product Family']
---



{{< figure align=center src="images/Merge-Word-Documents.jpg" alt="Combine Word Documents in Python">}}


There could be various scenarios when you have to combine multiple Word documents into a single file. For example, when multiple persons are writing different sections of a document and you need to combine the content at the end. On the other hand, you may need to merge all the invoices in one Word document. To perform this merging programmatically, this article covers **how to combine multiple Word [DOCX][1] or [DOC][2] documents in Python**.

*   [Python Library to Combine Word Documents][3]
*   [Combine Multiple Word Documents in a Single File][4]

## Python Library to Combine Word Documents {#Python-Library-to-Combine-Word-Documents}

To combine the DOCX or DOC files, we will use [Aspose.Words for Python][5], which is a powerful library to create and manipulate MS Word files. It also allows you to split, combine, and convert Word documents seamlessly. You can install the library from [PyPI][6] using the following pip command.

```
pip install aspose-words
```

## Combine Multiple Word DOCX Files in Python {#Combine-Multiple-Word-Documents-in-a-Single-File}

While combining the Word documents, you can specify the formatting you want to apply to the source document. For example, when combining document B with A, you can change the formatting of B as A or keep its original formatting as it is. The following are the steps to combine two Word documents in Python.

*   Load the source Word document using _Document_ class.
*   Load the destination Word document using _Document_ class.
*   Combine documents by appending source document into destination document using _Document.append\_document(Document, aw.ImportFormatMode.KEEP\_SOURCE\_FORMATTING)_ method.
*   Select the _ImportFormatMode_ as per your requirements.
*   Save the destination document using _Document.save(string)_ method.

The following code sample shows how to combine two Word DOCX files in Python.

{{< gist aspose-com-gists b5768be90cce3202f83d485bc2d0db75 "combine-word-documents.py" >}}

### Source Document

The following is the screenshot of the source Word document we have used in this article.



{{< figure align=center src="images/document2.jpg" alt="source word document to combine" caption="Source Word Document">}}


### Destination Document

The following screenshot shows the destination Word document.



{{< figure align=center src="images/document1.jpg" alt="destination word document to combine" caption="Destination Word Document">}}


### Combined Document

The following is the screenshot after combining both Word documents.



{{< figure align=center src="images/combined-word-documents-1024x658.jpg" alt="combined word documents in python" caption="Combined Word Document">}}


## Get a Free API License {#Get-a-Free-API-License}

[Get a temporary license][7] to use Aspose.Words for Python without evaluation limitations.

## Conclusion

In this article, you have learned how to combine two Word documents in a single document using Python. You can install Aspose.Words for Python in your applications and integrate the provided code to merge Word documents. In addition to this, you can explore Aspose.Words for Python using the [documentation][8]. In case you would have any queries, you can ask us via our [forum][9].

## See Also

*   [Convert Word Documents to TIFF using Python][10]
*   [Word Documents to Markdown using Python][11]
*   [Convert Word Document to HTML using Python][12]
*   [Convert PDF Files to Word Document in Python][13]




[1]: https://docs.fileformat.com/word-processing/docx/
[2]: https://docs.fileformat.com/word-processing/doc/
[3]: #Python-Library-to-Combine-Word-Documents
[4]: #Combine-Multiple-Word-Documents-in-a-Single-File
[5]: https://products.aspose.com/words/python/
[6]: https://pypi.org/project/aspose-words/
[7]: https://purchase.aspose.com/temporary-license
[8]: https://docs.aspose.com/words/python/product-overview/
[9]: https://forum.aspose.com/
[10]: https://blog.aspose.com/2021/11/08/convert-word-to-tiff-using-python/
[11]: https://blog.aspose.com/2021/11/05/convert-word-to-markdown-using-python/
[12]: https://blog.aspose.com/2021/11/01/convert-word-to-html-in-python/
[13]: https://blog.aspose.com/2021/10/29/convert-pdf-to-word-in-python/





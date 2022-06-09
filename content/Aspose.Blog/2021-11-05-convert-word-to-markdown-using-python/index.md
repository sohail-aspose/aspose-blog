---
title: 'Convert Word Documents to Markdown using Python'
seoTitle: "Convert Word to Markdown in Python | DOCX, DOC to MD in Python"
description: "Use Python Word library to convert Word documents to Markdown using Python. Control DOCX/DOC to MD conversion dynamically using different options."
date: Fri, 05 Nov 2021 13:31:24 +0000
draft: false
url: /2021/11/05/convert-word-to-markdown-using-python/
author: Usman Aziz
summary: '[Markdown][1] ([MD][2] is a popular format that is used to write articles, blogs, documentation, etc. However, sometimes it becomes difficult to remember and write the Markdown syntax. In such cases, you can simply write content in a Word document and convert it to Markdown. To automate Word to Markdown conversion, this article covers **how to convert Word (.docx or .doc) documents to Markdown (.md) files using Python**.'
tags: ['Convert DOC to Markdown in Python', 'Convert DOCX to MD in Python', 'Convert DOCX to Markdown in Python', 'Convert Word to Markdown in Python']
categories: ['Aspose.Words Product Family']
---



{{< figure align=center src="images/Word-to-Markdown.jpg" alt="Convert Word to Markdown in Python">}}


[Markdown][3] ([MD][4] is a popular format that is used to write articles, blogs, documentation, etc. However, sometimes it becomes difficult to remember and write the Markdown syntax. In such cases, you can simply write content in a Word document and convert it to Markdown. To automate Word to Markdown conversion, this article covers **how to convert Word (.docx or .doc) documents to Markdown (.md) files using Python**.

*   [Python Word to Markdown Converter Library][5]
*   [Convert a Word Document to Markdown][6]
*   [Customize Word to Markdown Conversion][7]

## Python Word to Markdown Converter Library {#Python-Word-to-Markdown-Converter-Library}

In order to convert DOCX or DOC files to Markdown format, we will use [Aspose.Words for Python][8]. The API allows automating the word processing features from within the Python applications. You can create the new Word documents from scratch and manipulate or convert the existing ones seamlessly. Aspose.Words for Python is hosted on [PyPI][9] and can be installed using the following pip command.

```
pip install aspose-words 
```

## Convert Word to Markdown in Python {#Convert-a-Word-Document-to-Markdown}

The following are the steps to convert a Word DOCX to Markdown format.

*   Load the Word document using _Document _class.
*   Convert Word document to Markdown using _Document.save(string)_ method.

The following code sample shows how to convert a DOCX file to Markdown format using Python.

{{< gist aspose-com-gists d2224c7d9075ba15222080d608837b2f "word-to-markdown.py" >}}

## Customize Word to Markdown Conversion {#Customize-Word-to-Markdown-Conversion}

Aspose.Words also allows you to control the Word to Markdown conversion using different options. For example, you can align content in the tables, specify a folder to save images, and so on. The following steps demonstrate how to use these options in Word to Markdown conversion using Python.

*   Load the Word document using _Document _class.
*   Create an object of _MarkdownSaveOptions_ class.
*   Set desired options such as _MarkdownSaveOptions_._images\_folder_.
*   Convert Word document to markdown using _Document.save(string, _MarkdownSaveOptions_)_ method.

The following code sample shows how to set additional options in DOCX to Markdown conversion using Python.

{{< gist aspose-com-gists d2224c7d9075ba15222080d608837b2f "word-to-markdown-custom.py" >}}

## Get a Free API License {#Get-a-Free-API-License}

Use Aspose.Words for Python without evaluation limitations using a [free temporary license][10].

**Info**: You may be interested in another Python API ([Aspose.Slides for Python via NET][11] that allows you to convert presentations (into PDFs, [word documents][12], etc.) and [import images][13] or other documents into presentations.

## Conclusion

In this article, you have learned how to convert Word documents to Markdown (.md) using Python. In addition, you have seen how to control Word to Markdown conversion using different options. Besides, you can visit the [documentation][14] of Aspose.Words for Python to explore other features. You can also ask your questions via our [forum][15].

## See Also

*   [Convert Word Files to PDF using Python][16]
*   [Create Word Documents in Python without MS Office][17]




[1]: https://en.wikipedia.org/wiki/Markdown
[2]: https://docs.fileformat.com/word-processing/md/)
[3]: https://en.wikipedia.org/wiki/Markdown
[4]: https://docs.fileformat.com/word-processing/md/)
[5]: #Python-Word-to-Markdown-Converter-Library
[6]: #Convert-a-Word-Document-to-Markdown
[7]: #Customize-Word-to-Markdown-Conversion
[8]: https://products.aspose.com/words/python/
[9]: https://pypi.org/project/aspose-words/
[10]: https://purchase.aspose.com/temporary-license
[11]: https://products.aspose.com/slides/python-net/)
[12]: https://products.aspose.app/slides/conversion/ppt-to-word
[13]: https://products.aspose.app/slides/import/jpg-to-ppt
[14]: https://docs.aspose.com/words/python/
[15]: https://forum.aspose.com/
[16]: https://blog.aspose.com/2021/10/27/convert-word-to-pdf-in-python/
[17]: https://blog.aspose.com/2021/10/28/create-word-documents-using-python/





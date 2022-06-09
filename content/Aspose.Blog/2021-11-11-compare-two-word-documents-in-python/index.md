---
title: 'Compare Two Word Documents in Python'
seoTitle: "Compare Two Word Documents in Python | Python DOCX Comparison Lib"
description: "Use Python Word library to compare two Word documents using Python. Use additional options to customize Word document comparison dynamically."
date: Thu, 11 Nov 2021 15:50:00 +0000
draft: false
url: /2021/11/11/compare-two-word-documents-in-python/
author: Usman Aziz
summary: 'Comparison of Word documents is performed in various cases to identify the differences. Various online tools allow you to compare Word documents, however, you may need to implement the comparison feature from within your applications. To achieve it, this article shows **how to compare two Word documents in Python**.'
tags: ['check difference in word document in python', 'compare word documents in python', 'python diff checker lib for word documents', 'python difference checker for word documents']
categories: ['Aspose.Words Product Family']
---



{{< figure align=center src="images/Compare-Word-Documents.jpg" alt="Compare Word Documents using Python">}}


Comparison of Word documents is performed in various cases to identify the differences. Various online tools allow you to compare Word documents, however, you may need to implement the comparison feature from within your applications. To achieve it, this article shows **how to compare two Word documents in Python**.

*   [Python Library for Comparing Word Documents][1]
*   [Compare Two Word Documents][2]
*   [Additional Options for Word Document Comparison][3]

## Python Library to Compare Word Documents {#Python-Library-for-Comparing-Word-Documents}

To compare DOCX or DOC documents, we will use [Aspose.Words for Python][4]. The said library allows you to automate word processing features from within your Python applications. You can install the library from [PyPI][5] using the following pip command.

```
pip install aspose-words
```

## Compare Two Word Documents in Python {#Compare-Two-Word-Documents}

Aspose.Words for Python makes it quite easy for you to compare two Word documents. In the comparison process, the changes are posted in the first document as revisions. The following are the steps to compare two Word documents in Python.

*   First, load the first Word document using _Document_ class.
*   Then, load the second document using _Document_ class.
*   Call _compare(Document, string, datetime.today())_ method using the _Document_ object of first document.
*   Check if documents are different using _Document.revisions.count_ property.
*   Finally, save the first document to get the revisions.

The following code sample shows how to compare two Word documents.

{{< gist aspose-com-gists e86343227ed63b2f0739c02b6a8c2f74 "compare-word-document.py" >}}

The following is the screenshot of the comparison result.



{{< figure align=center src="images/Compare-Word-Document-Result.jpg" alt="Compare two Word documents using Python">}}


## Additional Options for Comparing Word Documents {#Additional-Options-for-Word-Comparison}

Aspose.Words also provides some additional options to control the document comparison process. For example, you can ignore specific types of elements such as headers, footers, comments, etc. Also, you can set granularity to specify whether to compare the documents by characters or words. The following are the steps to set these options.

*   First, load the first Word document using _Document_ class.
*   Then, load the second document using _Document_ class.
*   Create an instance of _CompareOptions_ class and set desired options.
*   Call _compare(Document, string, datetime.today(), CompareOptions)_ method using the _Document_ object of first document.
*   Check if documents are different using _Document.revisions.count_ property.
*   Finally, save the first document to get the revisions.

The following code sample shows how to use additional options while comparing two Word documents.

{{< gist aspose-com-gists e86343227ed63b2f0739c02b6a8c2f74 "compare-word-document-custom.py" >}}

## Get a Free API License {#Get-a-Free-API-License}

You can [get a temporary license][6] in order to use Aspose.Words for Python without evaluation limitations.

## Conclusion

In this article, you have learned how to compare two Word documents in Python. Moreover, you have seen how to control the document comparison operation using different options. Besides, you can explore other features of Aspose.Words for Python using the [documentation][7]. In case of any questions, you can ask us via our [forum][8].

## See Also

*   [Convert Word Documents to TIFF using Python][9]
*   [Word Documents to Markdown using Python][10]
*   [Convert Word Document to HTML using Python][11]
*   [Convert PDF Files to Word Document in Python][12]




[1]: #Python-Library-for-Comparing-Word-Documents
[2]: #Compare-Two-Word-Documents
[3]: #Additional-Options-for-Word-Comparison
[4]: https://products.aspose.com/words/python/
[5]: https://pypi.org/project/aspose-words/
[6]: https://purchase.aspose.com/temporary-license
[7]: https://docs.aspose.com/words/python/product-overview/
[8]: https://forum.aspose.com/
[9]: https://blog.aspose.com/2021/11/08/convert-word-to-tiff-using-python/
[10]: https://blog.aspose.com/2021/11/05/convert-word-to-markdown-using-python/
[11]: https://blog.aspose.com/2021/11/01/convert-word-to-html-in-python/
[12]: https://blog.aspose.com/2021/10/29/convert-pdf-to-word-in-python/





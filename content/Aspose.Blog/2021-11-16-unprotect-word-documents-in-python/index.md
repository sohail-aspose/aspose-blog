---
title: 'Unprotect Word Documents in Python'
seoTitle: "Unprotect Word Documents in Python | Python Word DOCX Library"
description: "Use Python Word library to unprotect password-protected Word DOCX or DOC documents programmatically. Remove protection in Word documents dynamically."
date: Tue, 16 Nov 2021 16:22:22 +0000
draft: false
url: /2021/11/16/unprotect-word-documents-in-python/
author: Usman Aziz
summary: 'In various cases, the Word documents are protected with a password before they are shared. On receiving the protected documents, you need to unlock them to access their content. To perform the unlocking programmatically, this article covers **how to unprotect a password-protected Word document using Python**. Moreover, we will cover how to remove restrictions applied to a Word document dynamically.'
tags: ['remove protection from word documents in python', 'remove restrictions from word document in python', 'unprotect word documents in python']
categories: ['Aspose.Words Product Family']
---



{{< figure align=center src="images/Unorotect-Word-Documents.jpg" alt="Unprotect Word Documents using Python">}}


In various cases, the Word documents are protected with a password before they are shared. On receiving the protected documents, you need to unlock them to access their content. To perform the unlocking programmatically, this article covers **how to unprotect a password-protected Word document using Python**. Moreover, we will cover how to remove restrictions applied to a Word document dynamically.

*   [Python Library to Unprotect Word Documents][1]
*   [Unprotect a Word Document][2]
*   [Remove Restrictions in a Word Document][3]

## Python Library to Unprotect Word Documents {#Python-Library-to-Unprotect-Word-Documents}

To unlock the Word documents programmatically, we will use [Aspose.Words for Python][4]. It is a feature-rich library that facilitates you in creating new Word documents from scratch and manipulating the existing ones. You can install the library in your Python applications from [PyPI][5] using the following pip command.

```
pip install aspose-words 
```

## Unprotect a Word Document in Python {#Unprotect-a-Word-Document}

To unprotect a Word document, you would need to provide its password. The following are the steps to unprotect a Word document in Python.

*   Load the password-protected Word document by specifying its path and password in _Document_ constructor.
*   Save the document using _Document.save(string)_ method.

The following code sample shows how to load a password-protected Word document and save it as an unprotected document.

{{< gist aspose-com-gists a4151d5021f76c18f513634e2c90d480 "unprotect-word-documet.py" >}}

## Remove Restrictions in a Word Document using Python {#Remove-Restrictions-in-a-Word-Document}

MS Word also allows you to protect the documents by applying different restrictions. For example, you can make the document read-only, allow comments or revisions only, and so on. The following steps show how to remove restrictions in a Word document using Python.

*   Load the password-protected Word document by specifying its path and password in _Document_ constructor.
*   Call _Document.unprotect()_ method to remove restrictions.
*   Save the updated document using _Document.save(string)_ method.

The following code sample shows how to unprotect a Word document by removing the restrictions.

{{< gist aspose-com-gists a4151d5021f76c18f513634e2c90d480 "remove-restrictions.py" >}}

## Get a Free API License {#Get-a-Free-API-License}

You can get a [temporary license][6] to use Aspose.Words for Python without evaluation limitations.

## Conclusion

In this article, you have learned how to unprotect Word documents in Python. Moreover, you have seen how to remove restrictions applied to a Word document. You can explore more about Aspose.Words for Python using the [documentation][7]. In case you would have any queries, feel free to ask us on our [forum][8].

## See Also

*   [Convert Word Documents to TIFF using Python][9]
*   [Word Documents to Markdown using Python][10]
*   [Convert Word Document to HTML using Python][11]
*   [Convert PDF Files to Word Document in Python][12]




[1]: #Python-Library-to-Unprotect-Word-Documents
[2]: #Unprotect-a-Word-Document
[3]: #Remove-Restrictions-in-a-Word-Document
[4]: https://products.aspose.com/words/python/
[5]: https://pypi.org/project/aspose-words/
[6]: https://purchase.aspose.com/temporary-license
[7]: https://docs.aspose.com/words/python/product-overview/
[8]: https://forum.aspose.com/
[9]: https://blog.aspose.com/2021/11/08/convert-word-to-tiff-using-python/
[10]: https://blog.aspose.com/2021/11/05/convert-word-to-markdown-using-python/
[11]: https://blog.aspose.com/2021/11/01/convert-word-to-html-in-python/
[12]: https://blog.aspose.com/2021/10/29/convert-pdf-to-word-in-python/





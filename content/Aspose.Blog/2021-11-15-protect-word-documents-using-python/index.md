---
title: 'Protect Word Documents using Python'
seoTitle: "Password Protect Word Document in Python | Encrypt DOCX DOC"
description: "Use Python Word library to password protect Word documents in Python. Apply different protection types to resctrict access to Word DOCX DOC in Python."
date: Mon, 15 Nov 2021 14:24:31 +0000
draft: false
url: /2021/11/15/protect-word-documents-using-python/
author: Usman Aziz
summary: 'The information stored in Word documents is always prone to be accessed illegally. To avoid unauthorized access and forging while transmitting the documents, a protection mechanism must be applied. In this article, you will learn **how to protect Word documents with a password in Python**. Moreover, the article will cover how to apply different protection types to a Word document dynamically.'
tags: ['apply restriction to word document in python', 'make word document read only in python', 'protect doc in python', 'protect docx in python', 'protect word document in python']
categories: ['Aspose.Words Product Family']
---



{{< figure align=center src="images/Protect-Unprotect-Word-C.png" alt="Protect Word Documents in Python">}}


The information stored in Word documents is always prone to be accessed illegally. To avoid unauthorized access and forging while transmitting the documents, a protection mechanism must be applied. In this article, you will learn **how to protect Word documents with a password in Python**. Moreover, the article will cover how to apply different protection types to a Word document dynamically.

*   [Python Library to Protect Word Documents][1]
*   [Protect a Word Document with Password][2]
*   [Make a Word Document Read Only][3]
*   [Other Protection Types for Word Documents][4]

## Python Library to Protect Word Documents {#Python-Library-to-Protect-Word-Document}

In order to password protect DOCX, DOC, and other Word formats, we'll use [Aspose.Words for Python][5]. It is a Python library to create and manipulate Word documents dynamically. The said library is hosted on [PyPI][6] and can be installed using the following pip command.

```
pip install aspose-words 
```

## Protect a Word Document with Password in Python {#Protect-a-Word-Document-with-Password}

Aspose.Words makes it quite easier for you to protect a Word document. Simply load the document, set a password, and save the protected document. The following are the steps to password protect a Word DOCX file in Python.

*   First, load the Word document using _Document_ class.
*   Create an object of _OoxmlSaveOptions_ class (to save in DOC format, use _DocSaveOptions_ class instead).
*   Set password using _OoxmlSaveOptions.password_ property.
*   Finally, save the protected Word document using _Document.save(string, _OoxmlSaveOptions_)_ method.

The following code sample shows how to password protect a Word document.

{{< gist aspose-com-gists 56efcbfae80a8c8a93d11d9946aea2b6 "protect-word-document.py" >}}

The following dialogue appears when you open the password-protected Word document.



{{< figure align=center src="images/password-dialogue.jpg" alt="password-protected Word document in Python">}}


## Make a Word Document Read Only in Python {#Make-Word-Document-Read-Only}

In certain cases, you may only need to protect the modification of the content in a Word document. In such cases, you can make the document read-only. The following steps show how to make a Word document read-only in Python.

*   First, load the Word document using _Document_ class.
*   Use _Document.protect(ProtectionType.READ\_ONLY, string)_ method to make the Word document read-only.
*   Finally, save the protected Word document using _Document.save(string)_ method.

The following code sample shows how to protect a Word document and make it read-only.

{{< gist aspose-com-gists 56efcbfae80a8c8a93d11d9946aea2b6 "readonly-word-document.py" >}}

## Other Protection Types for Word Documents {#Other-Protection-Types-for-Word-Document}

Aspose.Words for Python also allows you to use other protection types to protect a Word document. For example, you can allow comments or revisions only. The following is the list of protection types you can apply to a Word document using Aspose.Words for Python.

*   ALLOW\_ONLY\_COMMENTS - To allow adding comments only.
*   ALLOW\_ONLY\_FORM\_FIELDS - To allow accessing form fields only.
*   ALLOW\_ONLY\_REVISIONS - To allow revisions only.
*   READ\_ONLY - To make the document read only.
*   NO\_PROTECTION - No protection.

To learn more about document protection using Aspose.Words for Python, visit [documentation][7].

## Get a Free API License {#Get-a-Free-API-License}

You can use a [free temporary license][8] to avoid evaluation limitations of Aspose.Words for Python.

## Conclusion

In this article, you have learned how to protect Word documents in Python. Moreover, you have seen how to restrict the editing of Word documents using different protection types. Besides, to explore more about Aspose.Words for Python, visit the [documentation][9]. In case you would have any queries, feel free to ask us on our [forum][10].

## See Also

*   [Convert Word Documents to TIFF using Python][11]
*   [Word Documents to Markdown using Python][12]
*   [Convert Word Document to HTML using Python][13]
*   [Convert PDF Files to Word Document in Python][14]




[1]: #Python-Library-to-Protect-Word-Document
[2]: #Protect-a-Word-Document-with-Password
[3]: #Make-Word-Document-Read-Only
[4]: #Other-Protection-Types-for-Word-Document
[5]: https://products.aspose.com/words/python/
[6]: https://pypi.org/project/aspose-words/
[7]: https://docs.aspose.com/words/python/protect-or-encrypt-a-document/
[8]: https://purchase.aspose.com/temporary-license
[9]: https://docs.aspose.com/words/python/product-overview/
[10]: https://forum.aspose.com/
[11]: https://blog.aspose.com/2021/11/08/convert-word-to-tiff-using-python/
[12]: https://blog.aspose.com/2021/11/05/convert-word-to-markdown-using-python/
[13]: https://blog.aspose.com/2021/11/01/convert-word-to-html-in-python/
[14]: https://blog.aspose.com/2021/10/29/convert-pdf-to-word-in-python/





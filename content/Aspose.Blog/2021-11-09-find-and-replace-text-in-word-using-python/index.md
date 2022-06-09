---
title: 'Find and Replace Text in Word Documents using Python'
seoTitle: "Python: Find and Replace Text in Word Documents | Python Word Library"
description: "Use Python Word library to find and replace text in MS Word DOCX/DOC documents. Replace text using RegEx and metacharacters in Word using Python."
date: Tue, 09 Nov 2021 03:00:00 +0000
draft: false
url: /2021/11/09/find-and-replace-text-in-word-using-python/
author: Usman Aziz
summary: 'Quite often, you need to replace a particular text or phrase in the Word documents. MS Word has a built-in feature for such cases and you can replace the desired text with one click. In this article, you will learn **how to programmatically find and replace text in Word documents using Python**. This could be useful when you need to replace text in a bunch of documents. Also, you can embed this feature in your Python applications to censor the Word documents before sharing.'
tags: ['Python Library to Find and Replace Text in Word Documents', 'Replace Text in Word Documents using Metacharacters Python', 'Replace Text in Word Documents using Regular Expression Python', 'Replace Text in a Word Document Python']
categories: ['Aspose.Words Product Family']
---



{{< figure align=center src="images/C-Find-and-Replace-Text.png" alt="Find and replace text in Word using Python">}}


Quite often, you need to replace a particular text or phrase in the Word documents. MS Word has a built-in feature for such cases and you can replace the desired text with one click. In this article, you will learn **how to programmatically find and replace text in Word documents using Python**. This could be useful when you need to replace text in a bunch of documents. Also, you can embed this feature in your Python applications to censor the Word documents before sharing.

*   [Python Library to Find and Replace Text in Word Documents][1]
*   [Find and Replace Text in a Word Document][2]
*   [Replace Text in Word Documents using Regular Expression][3]
*   [Replace Text in Word Documents using Metacharacters][4]

**Info**: Aspose recently developed a free online [Text to GIF][5] service that allows you to animate texts or generate GIFs from simple texts.

## Python Library to Replace Text in Word Documents {#Python-API-to-Find-and-Replace-Text-in-Word-Document}

To find and replace text in DOCX or DOC files, we will use [Aspose.Words for Python][6]. It is a feature-rich Python library that allows you to create and manipulate MS Word documents seamlessly. You can install the library from [PyPI][7] using the following pip command.

```
pip install aspose-words
```

## Find and Replace Text in a Word Document using Python {#Find-and-Replace-Text-in-a-Word-Document}

The following are the steps to find and replace text in a Word document using Python.

*   Load the document using the _Document_ class.
*   Use _Document.range.replace(string, string, aw.replacing.FindReplaceOptions(aw.replacing.FindReplaceDirection.FORWARD))_ method to replace the text.
*   Save the updated document using _Document.save(string)_ method.

The following code sample shows how to replace a particular text in a DOCX document using Python.

{{< gist aspose-com-gists 88b68c48e4cf6a2d3f576c5395b17099 "find-replace-text-word.py" >}}

The following is the input Word document that we used in this example.



{{< figure align=center src="images/Word-Document.png" alt="" caption="Input Word Document">}}


The following is the updated Word document after replacing the text.



{{< figure align=center src="images/Find-And-Replace-Text-In-Document.png" alt="Replace a Text in Word Document using Python" caption="Updated Word Document After Replacing Text">}}


## Replace Text in Word Documents using Regular Expression {#Replace-Text-in-Word-Documents-using-Regular-Expression}

In certain cases, you may want to replace the text that matches a particular pattern. For example, you may want to omit the email addresses written in the documents before sharing them online. For such cases, you can specify a regular expression to replace the matching text occurrences. The following are the steps to replace text in Word documents based on a regular expression.

*   Load the document using the _Document_ class.
*   Create an object of _FindReplaceOptions_ class.
*   Replace text based on regular expression using _Document.range.replace\_regex(string, string, FindReplaceOptions)_ method.
*   Save the updated document using _Document.save(string)_ method.

The following code sample shows how to replace text in a Word document using a regular expression.

{{< gist aspose-com-gists 88b68c48e4cf6a2d3f576c5395b17099 "find-replace-text-word-regex.py" >}}

The following is the screenshot of the Word document after replacing text using a RegEx.



{{< figure align=center src="images/Find-And-Replace-Multiple-Word-In-Document.png" alt="Replace text in Word using Regex">}}


## Python: Replace Text in Word Documents using Metacharacters {#Replace-Text-in-Word-Documents-using-Metacharacters}

In some cases, a piece of text may be composed of different paragraphs, sections, or pages. To replace such phrases, you need to use the following metacharacters.

*   **&p** for a paragraph break
*   **&b** for a section break
*   **&m** for a page break
*   **&l** for a line break

The following code sample shows how to use metacharacters to find and replace text in Word documents.

{{< gist aspose-com-gists 88b68c48e4cf6a2d3f576c5395b17099 "find-replace-text-word-metachar.py" >}}

[Read more][8] about finding and replacing text in Word documents using Python.

## Get a Free API License {#Get-a-Free-API-License}

You can [get a temporary license][9] in order to use Aspose.Words for Python without evaluation limitations.

## Conclusion

In this article, you have learned how to find and replace text in Word documents using Python. In addition to that, you have also seen how to use RegEx and metacharacters to replace text in Word documents. Besides this, you can explore other features offered by Aspose.Words for Python using the [documentation][10]. Also, you can post your questions on our [forum][11].

## See Also

*   [Convert Word Documents to TIFF using Python][12]
*   [Word Documents to Markdown using Python][13]
*   [Convert Word Document to HTML using Python][14]
*   [Convert PDF Files to Word Document in Python][15]




[1]: #Python-API-to-Find-and-Replace-Text-in-Word-Document
[2]: #Find-and-Replace-Text-in-a-Word-Document
[3]: #Replace-Text-in-Word-Documents-using-Regular-Expression
[4]: #Replace-Text-in-Word-Documents-using-Metacharacters
[5]: https://products.aspose.app/slides/text-to-gif
[6]: https://products.aspose.com/words/python/
[7]: https://pypi.org/project/aspose-words/
[8]: https://docs.aspose.com/words/python/find-and-replace/
[9]: https://purchase.aspose.com/temporary-license
[10]: https://docs.aspose.com/words/python/product-overview/
[11]: https://forum.aspose.com/
[12]: https://blog.aspose.com/2021/11/08/convert-word-to-tiff-using-python/
[13]: https://blog.aspose.com/2021/11/05/convert-word-to-markdown-using-python/
[14]: https://blog.aspose.com/2021/11/01/convert-word-to-html-in-python/
[15]: https://blog.aspose.com/2021/10/29/convert-pdf-to-word-in-python/





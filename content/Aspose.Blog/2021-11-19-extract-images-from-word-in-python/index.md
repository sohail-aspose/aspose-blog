---
title: 'Extract Images from Word Documents in Python'
seoTitle: "Extract Images from Word Documents in Python | Python Image Extractor"
description: "Use Python Word library to extract images from Word documents. Extract images from DOCX or DOC files programmatically using Python."
date: Fri, 19 Nov 2021 14:17:01 +0000
draft: false
url: /2021/11/19/extract-images-from-word-in-python/
author: Usman Aziz
summary: 'A picture is worth a thousand words. This is the reason images are an integral part of documents, specifically Word documents. The images are used to make the content more attractive and eye-catching. When parsing Word documents, you may come across the scenario where you need to extract images. To achieve this programmatically, this article covers **how to extract images from Word documents in Python**.'
tags: ['extract images from word document in python', 'fetch images from word documents in python', 'python image extractor for word documents', 'retrieve images from word document python']
categories: ['Aspose.Words Product Family']
---



{{< figure align=center src="images/Extract-Images-from-Word-Document.jpg" alt="extract images from word documents in python">}}


A picture is worth a thousand words. This is the reason images are an integral part of documents, specifically Word documents. The images are used to make the content more attractive and eye-catching. When parsing Word documents, you may come across the scenario where you need to extract images. To achieve this programmatically, this article covers **how to extract images from Word documents in Python**.

*   [Python Library to Extract Images from Word Documents][1]
*   [Extracting Images from Word Documents][2]

**Info**: If you ever need to get a Word document from a PowerPoint presentation, you can use Aspose [Presentation to Word Document][3] converter.

## Python Library to Extract Images from Word Documents {#Python-Library-to-Extract-Images-from-Word-Documents}

[Aspose.Words for Python][4] is a powerful and feature-rich library that is used to create and manipulate Word documents. We will use this library to extract images from DOCX or DOC files. You can install it in your Python applications from [PyPI][5] using the following pip command.

```
pip install aspose-words
```

## Extracting Images from Word Documents in Python {#Extracting-Images-from-Word-Documents}

The images in Word documents are represented by the shape nodes. Therefore, to retrieve images from a document, you will have to parse the shapes. The following steps show how to extract images from a Word document in Python.

*   First, load the Word document using _Document_ class.
*   Then, retrieve all the shapes into an object using _Document.get\_child\_nodes(NodeType.SHAPE, True)_ method.
*   Loop through the shapes and for each shape, perform the following operations:
    *   Cast the shape into _Shape_ type using _as\_shape()_ method.
    *   Check if shape has image using _Shape.has\_image()_ method.
    *   Save the shape as an image using _Shape.image\_data.save(string)_ method.

The following code sample shows how to extract images from a DOCX document in Python.

{{< gist aspose-com-gists 541ef80e756af284d3827cd04466b53f "extract-images-from-word.py" >}}

## Get a Free API License {#Get-a-Free-API-License}

You can get a [temporary license][6] to use Aspose.Words for Python without evaluation limitations.

## Conclusion

Images are commonly used in Word documents to make the content more appealing. In various cases, images are also required to be extracted from the documents along with the text. Therefore, in this article, you have learned how to extract images from Word documents in Python. Besides this, you can explore the [documentation][7] of Aspose.Words for Python. In case you would have any questions, feel free to let us know via our [forum][8].

## See Also

*   [Create MS Word Documents using Python][9]
*   [Convert Word Document to HTML using Python][10]
*   [Convert Word Documents to PNG, JPEG, or BMP in Python][11]
*   [Word Documents to Markdown using Python][12]
*   [Compare Two Word Documents in Python][13]




[1]: #Python-Library-to-Extract-Images-from-Word-Documents
[2]: #Extracting-Images-from-Word-Documents
[3]: https://products.aspose.app/slides/conversion/ppt-to-word
[4]: https://products.aspose.com/words/python/
[5]: https://pypi.org/project/aspose-words/
[6]: https://purchase.aspose.com/temporary-license
[7]: https://docs.aspose.com/words/python/product-overview/
[8]: https://forum.aspose.com/
[9]: https://blog.aspose.com/2021/10/28/create-word-documents-using-python/
[10]: https://blog.aspose.com/2021/11/01/convert-word-to-html-in-python/
[11]: https://blog.aspose.com/2021/11/04/convert-word-to-png-jpg-bmp-in-python/
[12]: https://blog.aspose.com/2021/11/05/convert-word-to-markdown-using-python/
[13]: https://blog.aspose.com/2021/11/11/compare-two-word-documents-in-python/





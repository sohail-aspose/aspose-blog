---
title: 'Convert Word Document to HTML using Python'
seoTitle: "Convert Word to HTML in Python | DOCX to HTML | DOC to HTML"
description: "Use Python Word API to convert Word documents to HTML format in Python. Convert DOCX or DOC to HTML using additional options dynamically."
date: Mon, 01 Nov 2021 23:36:00 +0000
draft: false
url: /2021/11/01/convert-word-to-html-in-python/
author: Usman Aziz
summary: 'Word to [HTML][1] conversion is required in various cases, such as for embedding the content on the web pages. In this article, you will learn **how to convert MS Word [DOCX][2] or [DOC][3] documents to HTML using Python**. Moreover, you will learn how to control the conversion of Word to HTML dynamically using different options.'
tags: ['Python word to html converter', 'doc to html python', 'docx to html python', 'word to html python']
categories: ['Aspose.Words Product Family']
---



{{< figure align=center src="images/Word-to-HTML.jpg" alt="Word to HTML Python">}}


Word to [HTML][4] conversion is required in various cases, such as for embedding the document's content on the web pages. In this article, you will learn **how to convert MS Word [DOCX][5] or [DOC][6] documents to HTML using Python**. Moreover, you will learn how to control the conversion of Word to HTML dynamically using different options.

*   [Python Word to HTML Converter API][7]
*   [Convert a Word Document to HTML][8]
*   [Customize Word to HTML Conversion][9]

## Python Word to HTML Converter API {#Python-Word-to-HTML-Converter-API}

In order to convert Word documents to HTML, we will use [Aspose.Words for Python][10]. It is a powerful and feature-rich API for creating and manipulating Word documents. Also, it provides a high-fidelity conversion of Word documents to other formats. Aspose.Words for Python is available on [PyPI][11] and you can install it using the following pip command.

```
pip install aspose-words 
```

## Convert a Word Document to HTML in Python {#Convert-a-Word-Document-to-HTML-in-Python}

The following are the steps to convert a Word document to an HTML file using Python.

*   Load the Word document using _Document_ class.
*   Create an object of _HtmlSaveOptions_ class.
*   Enable export of font resources using _HtmlSaveOptions.export\_font\_resources_ property.
*   Convert Word document to HTML using _Document.save()_ method.

The following code sample shows how to convert a DOCX file to HTML in Python.

{{< gist aspose-com-gists 1e0865cd17e0d1af503d555c3d3ce497 "word-to-html.py" >}}

## Customize Word to HTML Conversion in Python {#Customize-Word-to-HTML-Conversion}

Aspose.Words for Python also provides different options to customize the Word to HTML conversion. For example, you can convert documents with round-trip information, specify the folder to save the resource files, and so on.

### Convert a Word Document with Round-trip Information

HTML doesn't support all the features provided by MS Word, therefore, to mimic the Word document in HTML we need to save additional information termed as round-trip information. The following are the steps to turn on the export of round-trip information in Word to HTML conversion.

*   Load the Word document using _Document_ class.
*   Create an object of _HtmlSaveOptions_ class and set _HtmlSaveOptions.export\_roundtrip\_information_ property to _true_.
*   Convert Word document to HTML using _Document.save()_ method and pass HTML file's name and _HtmlSaveOptions_ as parameters.

The following code sample shows how to export round-trip information in Word to HTML conversion.

{{< gist aspose-com-gists 1e0865cd17e0d1af503d555c3d3ce497 "word-to-html-roundtrip-info.py" >}}

### Word to HTML: Specify a Folder for Resources

You can also specify a folder where you want to store all the resources such as images, CSS files, and fonts. For this, you can use _HtmlSaveOptions.export\_font\_resources_ property. You can also specify separate folders for fonts and images using _HtmlSaveOptions.fonts\_folder_ and _HtmlSaveOptions.images\_folder_ properties, respectively. The following are the steps to use a separate folder to save resources in Word to HTML conversion.

*   Load the Word document using _Document_ class.
*   Create an object of _HtmlSaveOptions_ class and set _HtmlSaveOptions.export\_font\_resources_ property to _true_.
*   Specify the name of the resource folder using _HtmlSaveOptions.resource\_folder_ property.
*   Convert Word document to HTML using _Document.save()_ method and pass HTML file's name and _HtmlSaveOptions_ as parameters.

The following code sample shows how to specify a resource folder in Word to HTML conversion.

{{< gist aspose-com-gists 1e0865cd17e0d1af503d555c3d3ce497 "word-to-html-resource-folder.py" >}}

## Get a Free API License {#Get-a-Free-API-License}

You can [get a temporary license][12] in order to use Aspose.Words for Python without evaluation limitations.

**Info**: You may be interested in another Python API ([Aspose.Slides for Python via NET][13] that allows you to [convert presentations to images][14] and [import images into presentations][15].

## Conclusion

In this article, you have learned how to convert Word documents to HTML using Python. Moreover, you have seen how to customize the Word to HTML conversion dynamically. Besides, you can explore other features of Aspose.Words for Python using the [documentation][16]. Also, you can ask your questions via our [forum][17].

## See Also

*   [Convert Word Files to PDF using Python][18]
*   [Create Word Documents in Python without MS Office][19]




[1]: https://docs.fileformat.com/web/html/
[2]: https://docs.fileformat.com/word-processing/docx/
[3]: https://docs.fileformat.com/word-processing/doc/
[4]: https://docs.fileformat.com/web/html/
[5]: https://docs.fileformat.com/word-processing/docx/
[6]: https://docs.fileformat.com/word-processing/doc/
[7]: #Python-Word-to-HTML-Converter-API
[8]: #Convert-a-Word-Document-to-HTML-in-Python
[9]: #Customize-Word-to-HTML-Conversion
[10]: https://products.aspose.com/words/python/
[11]: https://pypi.org/project/aspose-words/
[12]: https://purchase.aspose.com/temporary-license
[13]: https://products.aspose.com/slides/python-net/)
[14]: https://products.aspose.app/slides/conversion/ppt-to-jpg
[15]: https://products.aspose.app/slides/import/jpg-to-ppt
[16]: https://docs.aspose.com/words/python/product-overview/
[17]: https://forum.aspose.com/
[18]: https://blog.aspose.com/2021/10/27/convert-word-to-pdf-in-python/
[19]: https://blog.aspose.com/2021/10/28/create-word-documents-using-python/





---
title: 'Create MS Word Documents using Python'
seoTitle: "Create Word Documents in Python | Python Word Library for DOCX DOC"
description: "Use Python library to create MS Word document from scratch in Python. Create DOCX DOC documents and add text, table, image, list, etc. dynamically."
date: Thu, 28 Oct 2021 16:30:52 +0000
draft: false
url: /2021/10/28/create-word-documents-using-python/
author: Usman Aziz
summary: 'MS Word files are immensely used to create various types of documents such as invoices, reports, technical articles, etc. The document automation has facilitated the users to generate Word documents dynamically from within their web or desktop portals. In this article, we will cover **how to generate Word documents in Python without MS Office**. Moreover, you will learn **how to create a [DOCX][1] or [DOC][2] file and add text or other elements into it dynamically using Python**.'
tags: ['create docx in python', 'create word document in python', 'insert image in word document python', 'insert text in word document python', 'modify word document python']
categories: ['Aspose.Words Product Family']
---



{{< figure align=center src="images/C-Word-Automation.png" alt="Word automation in Python ">}}


MS Word files are immensely used to create various types of documents such as invoices, reports, technical articles, etc. The document automation has facilitated the users to generate Word documents dynamically from within their web or desktop portals. Therefore, in this article, we will cover **how to generate Word documents in Python without MS Office**. Moreover, you will learn **how to create a [DOCX][3] or [DOC][4] file and add text or other elements into it dynamically using Python**.

*   [Python API to Create Word Documents][5]
*   [Create a Word DOCX/DOC File in Python][6]
*   [Load an Existing Word Document][7]
*   [Insert Paragraph in a Word Document][8]
*   [Add Table in a Word Document][9]
*   [Add List in a Word DOCX/DOC File][10]
*   [Insert Image in a Word Document][11]
*   [Add Table of Contents in a Word File][12]

**TIP**: Aspose provides a FREE online **[PowerPoint to Word][13]** Converter that allows you to create Word documents from presentations quickly.

## Python API to Create Word Documents {#Python-API-to-Create-Word-Documents}

In order to create Word documents dynamically, we will use [Aspose.Word for Python][14]. It is a powerful Python library that lets you create and manipulate MS Word documents seamlessly. You can install the library in your Python application from [PyPI][15] using the following pip command.

```
pip install aspose-words
```

## Create a Word DOCX or DOC File in Python {#Create-a-Word-File-in-Python}

The following are the steps to create a Word document from scratch in Python.

*   Create an object of _Document_ class.
*   Create an object of _DocumentBuilder_ class.
*   Insert text into document using _DocumentBuilder.write()_ method.
*   Save the Word document using _Document.save()_ method.

The following code sample shows how to create a Word DOCX document.

{{< gist aspose-com-gists 8b57027cc99a09b016a3a9421ccc1f97 "create-document.py" >}}

### Output



{{< figure align=center src="images/create-word-document.jpg" alt="create word document python">}}


## Load an Existing Word Document in Python {#Load-an-Existing-Word-Document-in-Python}

You can also load an existing Word document by providing its path to the _Document_ constructor. The following code sample shows how to load a Word document.

{{< gist aspose-com-gists 8b57027cc99a09b016a3a9421ccc1f97 "load-document.py" >}}

## Insert a Paragraph in Word Document using Python {#Insert-Paragraph-in-a-Word-Document}

The Word documents contain text in the form of paragraphs. Therefore, in this section, we will demonstrate how to insert a paragraph into a Word document using Python.

*   Create an object of _Document_ class.
*   Create an object of _DocumentBuilder_ class.
*   Get reference of font from the _Documentbuilder_ object and set font.
*   Get reference of the paragraph fromat from _Documentbuilder_ object and set indentation, alignment, etc.
*   Insert text into paragraph using _DocumentBuilder.write()_ method.
*   Save the Word document using _Document.save()_ method.

The following code sample shows how to insert a paragraph in a Word document using Python.

{{< gist aspose-com-gists 8b57027cc99a09b016a3a9421ccc1f97 "insert-paragraph.py" >}}

### Output



{{< figure align=center src="images/add-paragraph.jpg" alt="create paragraph in word document python">}}


Learn more about [working with paragraphs][16] in Word documents using Python.

## Add Table in a Word Document using Python {#Add-Table-in-Word-Document}

Tables are an integral part of the documents to display information in the form of rows and columns. Aspose.Words for Python makes it quite easier to work with tables. The following are the steps to add a table in a Word document using Python.

*   Create an object of _Document_ class.
*   Create an object of _DocumentBuilder_ class.
*   **Start a table** using _DocumentBuilder.start\_table()_ method and get reference of the table in an object.
*   **Insert a cell** using _DocumentBuilder.insert\_cell()_ method.
*   Set auto fit using _auto\_fit(aw.tables.AutoFitBehavior.FIXED\_COLUMN\_WIDTHS)_ method.
*   Set alignment of the cell.
*   Insert text into cell using _DocumentBuilder.write()_ method.
*   Repeat inserting cells and text into cells as required.
*   **End a row** when you complete inserting cells.
*   **End table** when you have inserted all the rows.
*   Save the Word document using _Document.save()_ method.

The following code sample shows how to insert a table in a Word document using Python.

{{< gist aspose-com-gists 8b57027cc99a09b016a3a9421ccc1f97 "add-table.py" >}}

### Output



{{< figure align=center src="images/add-table.jpg" alt="create table in word document python">}}


Learn more about how to [work with tables][17] in Word documents using Python.

## Create a List in a Word Document using Python {#Create-a-List-in-a-Word-Document-using-Python}

The following are the steps to create a list in a Word document using Python.

*   Create an object of _Document_ class.
*   Create an object of _DocumentBuilder_ class.
*   Set formatting using _DocumentBuilder.list\_format.apply\_number\_default()_ method.
*   Insert item using _DocumentBuilder.writeln("Item 1")_ method.
*   Insert second item using _DocumentBuilder.writeln("Item 2")_ method.
*   To insert items into next level of the list, call _DcoumentBuilder.list\_format.list\_indent()_ method and insert items.
*   Remove numbers from the list using _DcoumentBuilder.list\_format.remove\_numbers()_ method.
*   Save the Word document using _Document.save()_ method.

The following code sample shows how to create a list in Word documents using Python.

{{< gist aspose-com-gists 8b57027cc99a09b016a3a9421ccc1f97 "add-list.py" >}}

### Output



{{< figure align=center src="images/add-list.jpg" alt="create list in word document python">}}


Read more about [working with lists][18] in Word documents using Python.

## Insert Images in a Word Document using Python {#Insert-Images-in-a-Word-Document}

While working with Word documents, you cannot ignore graphical objects such as images. So let's have a look at how to insert images in a Word document dynamically using Python.

*   Create an object of _Document_ class.
*   Create an object of _DocumentBuilder_ class.
*   Insert image using _DocumentBuilder.insert\_image()_ method and pass image file's path as parameter.
*   Save the Word document using _Document.save()_ method.

The following code sample shows how to insert an image in a Word document using Python.

{{< gist aspose-com-gists 8b57027cc99a09b016a3a9421ccc1f97 "add-image.py" >}}

### Output



{{< figure align=center src="images/add-image.jpg" alt="create image in word document python">}}


## Create Table of Contents in Word Documents using Python {#Create-Table-of-Contents-in-Word-Documents-using-Python}

In various cases, the Word documents contain a table of content (TOC). The TOC gives you an overview of the content of the Word document. The following steps demonstrate how to add a TOC in Word documents using Python.

*   Create an object of _Document_ class.
*   Create an object of _DocumentBuilder_ class.
*   Insert table of contents using _DocumentBuilder.insert\_table\_of\_contents()_ method.
*   Insert a page break after TOC using _DocumentBuilder.insert\_break(aw.BreakType.PAGE\_BREAK)_ method.
*   After adding/updating content of the document, update TOC using _Document.update\_fields()_ method.
*   Save the Word document using _Document.save()_ method.

The following code sample shows how to insert a table of contents in a Word document using Python.

{{< gist aspose-com-gists 8b57027cc99a09b016a3a9421ccc1f97 "add-toc.py" >}}

### Output



{{< figure align=center src="images/add-toc.jpg" alt="create toc in word document python">}}


Read more about [working with the table of contents][19] using Python.

## Read More

This article covered some basic operations of creating Word documents and inserting different elements. Aspose.Words for Python provides a bunch of other features as well that you can explore using the [documentation][20].

## Get a Free API License {#Get-a-Free-API-License}

You can [get a temporary license][21] in order to use Aspose.Words for Python without evaluation limitations.

## Conclusion

In this article, you have learned how to create Word DOCX or DOC files in Python. Moreover, you have seen how to insert text, images, tables, lists, and table of contents in Word documents dynamically. You can try the API and share your feedback or queries via our [forum][22].

## See Also

*   [Convert Word Files to PDF using Python][23]




[1]: https://docs.fileformat.com/word-processing/docx/
[2]: https://docs.fileformat.com/word-processing/doc/
[3]: https://docs.fileformat.com/word-processing/docx/
[4]: https://docs.fileformat.com/word-processing/doc/
[5]: #Python-API-to-Create-Word-Documents
[6]: #Create-a-Word-File-in-Python
[7]: #Load-an-Existing-Word-Document-in-Python
[8]: #Insert-Paragraph-in-a-Word-Document
[9]: #Add-Table-in-Word-Document
[10]: #Create-a-List-in-a-Word-Document-using-Python
[11]: #Insert-Images-in-a-Word-Document
[12]: #Create-Table-of-Contents-in-Word-Documents-using-Python
[13]: https://products.aspose.app/slides/conversion/ppt-to-word
[14]: https://products.aspose.com/words/python/
[15]: https://pypi.org/project/aspose-words/
[16]: https://docs.aspose.com/words/python/working-with-paragraphs/
[17]: https://docs.aspose.com/words/python/working-with-tables/
[18]: https://docs.aspose.com/words/python/working-with-lists/
[19]: https://docs.aspose.com/words/python/working-with-table-of-contents/
[20]: https://docs.aspose.com/words/python/product-overview/
[21]: https://purchase.aspose.com/temporary-license
[22]: https://forum.aspose.com/
[23]: https://blog.aspose.com/2021/10/27/convert-word-to-pdf-in-python/





---
title: 'Create Table in Word Documents using Python'
seoTitle: "Create Table in Word DOCX in Python | Create Nested Tables in Python"
description: "Use Python Word library to create a table in Word DOCX documents in Python. Create nested tables or clone existing tables programmatically."
date: Mon, 22 Nov 2021 17:46:00 +0000
draft: false
url: /2021/11/22/create-table-in-word-using-python/
author: Usman Aziz
summary: 'Tables are commonly used in Word documents to organize information in a grid-like structure. They allow you to summarize the information in the form of rows and columns. In this article, you will learn **how to create a** **table in Word documents programmatically using Python**. Moreover, the article will cover how to create nested tables or clone an existing table in Word documents.'
tags: ['clone table in word document using python', 'create nested table in word document using python', 'create table in docx document using python', 'create table in word document using python']
categories: ['Aspose.Words Product Family']
---



{{< figure align=center src="images/create-tables-in-Word-documents.jpg" alt="create tables in word documents using python">}}


Tables are commonly used in Word documents to organize information in a grid-like structure. They allow you to summarize the information in the form of rows and columns. In this article, you will learn **how to create a** **table in Word documents programmatically using Python**. Moreover, the article will cover how to create nested tables or clone an existing table in Word documents.

*   [Python Library to Create Tables in Word Documents][1]
*   [Create a Table in a Word Document][2]
*   [Create a Nested Table in a Word Document][3]
*   [Clone an Existing Table in a Word Document][4]

**Info**: If you ever need to get a Word document from a PowerPoint presentation, you can use Aspose [Presentation to Word Document][5] converter.

## Python Library to Create Tables in Word Documents {#Python-Library-to-Create-Tables-in-Word-Documents}

To work with tables in Word documents, we will use [Aspose.Words for Python][6]. The library is designed to create and manipulate Word documents dynamically from within the Python applications. You can install the library from [PyPI][7] using the following pip command.

```
pip install aspose-words
```

## Create a Table in a Word Document in Python {#Create-a-Table-in-a-Word-Document}

The following are the steps to create a table in a Word DOCX document using Python.

*   Create an object of _Document _class.
*   Create an object of _DocumentBuilder _class.
*   **Start a table** using _DocumentBuilder.start\_table()_ method and get reference of the table in an object.
*   **Insert a cell** using _DocumentBuilder.insert\_cell()_ method.
*   Set formatting of the cell using _DocumentBuilder.cell\_format_ property.
*   Set auto fit using _auto\_fit(aw.tables.AutoFitBehavior.FIXED\_COLUMN\_WIDTHS)_ method.
*   Set alignment of the cell.
*   Insert text into cell using _DocumentBuilder.write()_ method.
*   Repeat inserting cells and text into cells as required.
*   **End a row** when you complete inserting cells.
*   **End table** when you have inserted all the rows.
*   Save the Word document using _Document.save()_ method.

The following code sample shows how to create a table in DOCX documents using Python.

{{< gist aspose-com-gists baa8cef19a815ab614b1ac489791b7f1 "create-table.py" >}}

The following is the screenshot of the table we have created using the code sample above.



{{< figure align=center src="images/Create-Table-in-Word-Document-1024x267.jpg" alt="" caption="Table in a Word DOCX Document">}}


## Create a Nested Table in a Word Document in Python {#Create-a-Nested-Table-in-a-Word-Document}

Aspose.Words for Python also allows you to create a nested table seamlessly. In other words, you can create a new table within a cell of the table. The following are the steps to create a nested table in a Word DOCX file.

*   Create an object of _Document _class.
*   Create an object of _DocumentBuilder _class.
*   **Start a table** using _DocumentBuilder.start\_table()_ method and get reference of the table in an object.
*   **Insert a cell** using _DocumentBuilder.insert\_cell()_ method and get reference of the cell in a object.
*   Insert text into cell using _DocumentBuilder.write()_ method.
*   Repeat inserting cells and text into cells as required.
*   **End table** when you have inserted all the rows.
*   Move control inside the desired cell usng _DocumentBuilder.move\_to(Cell.first\_paragraph)_ method.
*   Create another table by inserting cells and end the table when done.
*   Save the Word document using _Document.save()_ method.

The following code sample shows how to create a nested table in a DOCX document using Python.

{{< gist aspose-com-gists baa8cef19a815ab614b1ac489791b7f1 "create-nested-table.py" >}}

The following is the output of the code sample above.



{{< figure align=center src="images/Create-Nested-Table-in-Word-Document-1024x252.jpg" alt="" caption="Nested Table in a Word Document">}}


## Clone an Existing Table in a Word Document in Python {#Clone-an-Existing-Table-in-a-Word-Document}

You can also clone an existing table in a Word document. The following are the steps to perform this operation.

*   Load the document using Document class.
*   Get reference of the table in an object using _Document.get\_child(NodeType.TABLE, int, boolean).as\_table()_ method.
*   Call _clone(True).as\_table()_ method using the table's object and get reference of the cloned table in another object.
*   Insert cloned table using _Table.parent\_node.insert\_after()_ method.
*   Insert an empty paragraph between tables using Table.parent\_node.insert\_after(Paragraph(Document), Table) method.
*   Save the Word document using _Document.save()_ method.

The following code sample shows how to clone a table in a Word DOCX document using Python.

{{< gist aspose-com-gists baa8cef19a815ab614b1ac489791b7f1 "clone-table.py" >}}

The following screenshot shows the cloned table in a Word document.



{{< figure align=center src="images/Clone-Table-in-Word-Document-1024x465.jpg" alt="" caption="Cloned Table in a Word Document">}}


## Get a Free API License {#Get-a-Free-API-License}

You can get a [temporary license][8] to use Aspose.Words for Python without evaluation limitations.

## Conclusion

In this article, you have learned how to create tables in Word documents using Python. Moreover, you have seen how to create nested tables or clone the existing tables in Word documents dynamically. Besides, you can visit the [documentation][9] of Aspose.Words for Python to explore other features. In case of any questions, feel free to let us know via our [forum][10].

## See Also

*   [Create MS Word Documents using Python][11]
*   [Convert Word Document to HTML using Python][12]
*   [Convert Word Documents to PNG, JPEG, or BMP in Python][13]
*   [Word Documents to Markdown using Python][14]
*   [Compare Two Word Documents in Python][15]




[1]: #Python-Library-to-Create-Tables-in-Word-Documents
[2]: #Create-a-Table-in-a-Word-Document
[3]: #Create-a-Nested-Table-in-a-Word-Document
[4]: #Clone-an-Existing-Table-in-a-Word-Document
[5]: https://products.aspose.app/slides/conversion/ppt-to-word
[6]: https://products.aspose.com/words/python/
[7]: https://pypi.org/project/aspose-words/
[8]: https://purchase.aspose.com/temporary-license
[9]: https://docs.aspose.com/words/python/product-overview/
[10]: https://forum.aspose.com/
[11]: https://blog.aspose.com/2021/10/28/create-word-documents-using-python/
[12]: https://blog.aspose.com/2021/11/01/convert-word-to-html-in-python/
[13]: https://blog.aspose.com/2021/11/04/convert-word-to-png-jpg-bmp-in-python/
[14]: https://blog.aspose.com/2021/11/05/convert-word-to-markdown-using-python/
[15]: https://blog.aspose.com/2021/11/11/compare-two-word-documents-in-python/





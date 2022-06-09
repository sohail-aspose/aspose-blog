---
title: 'Create and Manipulate Tables in PowerPoint PPT using Python'
seoTitle: "Python: Create and Manipulate Tables in PowerPoint | Python PPTX"
description: "Use Python library to create and manipulate tables in PowerPoint PPT/PPTX using Python. Change formatting and aspect ratio of tables dynamically."
date: Wed, 02 Mar 2022 15:54:00 +0000
draft: false
url: /2022/03/02/work-with-tables-in-powerpoint-ppt-in-python/
author: Usman Aziz
summary: 'Tables are commonly used to organize the data in the form of rows and columns. They make it quite easier to view, understand and analyze the data. In various cases, you have to insert tables in your PowerPoint presentations. To accomplish that programmatically, this article covers **how to create tables in PowerPoint PPT or PPTX using Python**. Moreover, you will learn how to access, modify, and format the existing PowerPoint tables.'
tags: ['Create a Table in PowerPoint PPT in Python', 'Edit a Table in PowerPoint PPT in Python', 'Format a Table in PowerPoint PPT in Python', 'Python Library to Create PowerPoint Tables']
categories: ['Aspose.Slides Product Family']
---



{{< figure align=center src="images/Create-Table-in-PowerPoint-1.jpg" alt="Create and Manipulate Tables in PowerPoint Python">}}


Tables are commonly used to organize the data in the form of rows and columns. They make it quite easier to view, understand and analyze the data. In various cases, you have to insert tables in your PowerPoint presentations. To accomplish that programmatically, this article covers **how to create tables in PowerPoint PPT or PPTX using Python**. Moreover, you will learn how to access, modify, and format the existing PowerPoint tables.

*   [Python Library to Create and Manipulate PowerPoint Tables][1]
*   [Create a Table in PowerPoint Presentations][2]
*   [Edit a Table in a Presentation][3]
*   [Format Text in PowerPoint Tables][4]
*   [Lock Aspect Ratio of the Tables][5]

## Python Library to Create and Manipulate PowerPoint Tables {#API-to-Create-and-Manipulate-Tables-in-PowerPoint}

[Aspose.Slides for Python][6] provides a bunch of features to create, manipulate and convert PowerPoint and OpenOffice documents. We will use this library to create, edit and manipulate tables in our PowerPoint presentations. You can install the library from [PyPI][7] using the following command.

```
> pip install aspose.slides
```

## Create a Table in PowerPoint PPT using Python {#Create-a-Table-in-PowerPoint-Presentation}

The following are the steps to create a table in a PowerPoint PPT/PPTX in Python.

*   First, use **Presentation **class to load or create a PPT/PPTX presentation.
*   Then, get reference of the desired slide where you want to add the table.
*   After that, create two arrays to define the width and height of columns and rows, respectively.
*   Insert a new table on slide using **ISlide.shapes.add\_table()** method and get its reference.
*   Start a loop to iterate through the rows of the table.
*   Start a nested loop to iterate through the cells of the table and perform the following operations in each iteration.
    *   Set text of the cell using **Table.rows\[row\]\[cell\].text\_frame.text** property.
    *   Set cell's border style, if required.
*   Finally, save the presentation using **Presentation.save(string, SaveFormat)** method.

The following code sample shows how to create a table in a PowerPoint presentation.

{{< gist aspose-com-gists 9c6d62f894135aa1dbc332394953da8f "create-table.py" >}}

The following screenshot shows the table that we have created using the above code.



{{< figure align=center src="images/Create-Tables-in-PowerPoint-PPT.png" alt="Create a Table in PowerPoint PPT using Python">}}


## Edit a Table in a PowerPoint PPT using Python {#Access-a-Table-in-a-Presentation-using-Java}

You can also modify an existing table by accessing it from the presentation slide. This is how you can access a PowerPoint table and edit its content or appearance in Python.

*   First, load an existing PowerPoint PPT/PPTX file using **Presentation** class.
*   Then, get reference of the desired slide into an object.
*   Create an object for table and initialize it with **None**.
*   Iterate through all shapes in slide using **ISlide.shapes** collection.
*   Filter the shapes of type **Table**.
*   Manipulate the table as required.
*   Finally, save the presentation using **Presentation.save(string, SaveFormat)** method.

The following code sample shows how to edit tables in a PowerPoint PPT using Python.

{{< gist aspose-com-gists 9c6d62f894135aa1dbc332394953da8f "edit-table.py" >}}

## Format Text in PowerPoint Tables using Python {#Format-Text-in-PowerPoint-Tables-using-Java}

Aspose.Slides for Python also allows you to apply the formatting to the text inside tables. The following steps show how you can achieve this.

*   First, load an existing presentation using **Presentation** class.
*   Then, get reference of the desired slide into an object.
*   Get the reference of the desired table from slide into an object.
*   Set formatting using **PortionFormat**, **ParagraphFormat**, and **TextFrameFormat** objects.
*   Assign formatting to the table using **Table.set\_text\_format()** method.
*   Finally, save the presentation using **Presentation.save(string, SaveFormat)** method.

The following code sample shows how to set the formatting of the text inside a table in PowerPoint using Python.

{{< gist aspose-com-gists 9c6d62f894135aa1dbc332394953da8f "format-table.py" >}}

## Lock Aspect Ratio of PowerPoint Tables in Python {#Lock-the-Aspect-Ratio-of-the-Tables}

You can also lock the aspect ratio of the tables in PowerPoint presentations using Python, as demonstrated in the following steps.

*   First, load an existing presentation using **Presentation** class.
*   Then, get reference of the desired slide into an object.
*   Create a table or retrieve the reference of an existing table into an object.
*   Lock aspect ratio using **Table.shape\_lock.aspect\_ratio\_locked** property.
*   Finally, save the presentation using **Presentation.save(string, SaveFormat)** method.

The following code sample shows how to lock the aspect ratio of the table in PowerPoint PPTX.

{{< gist aspose-com-gists 9c6d62f894135aa1dbc332394953da8f "lock-aspect-ratio.py" >}}

## Get a Free License {#Get-a-Free-API-License}

You can use Aspose.Slides for Python without evaluation limitations by getting a free [temporary license][8].

**Info**: Using Aspose [JPG to PPT][9] or [PNG to PPT][10] converter, you can generate PowerPoint presentations from simple images.

## Conclusion

Tables are an integral part of the documents, which are used to organize the data. In this article, you have learned how to create tables in a PowerPoint PPT/PPTX in Python. Moreover, you have seen how to access and manipulate existing tables in PowerPoint presentations programmatically. Besides, you can also visit the [documentation][11] to explore more about Aspose.Slides for Python. Also, you can ask your questions via our [forum][12].

## See Also

*   [Create PowerPoint Files in Python][13]
*   [Convert PPTX to PDF in Python][14]
*   [Convert PPT to PNG in Python][15]
*   [Add Watermark in PowerPoint PPT in Python][16]
*   [Apply 3D Effects in PowerPoint PPT using Python][17]




[1]: #API-to-Create-and-Manipulate-Tables-in-PowerPoint
[2]: #Create-a-Table-in-PowerPoint-Presentation
[3]: #Access-a-Table-in-a-Presentation-using-Java
[4]: #Format-Text-in-PowerPoint-Tables-using-Java
[5]: #Lock-the-Aspect-Ratio-of-the-Tables
[6]: https://products.aspose.com/slides/python-net
[7]: https://pypi.org/project/aspose.slides/
[8]: https://purchase.aspose.com/temporary-license
[9]: https://products.aspose.app/slides/import/jpg-to-ppt
[10]: https://products.aspose.app/slides/import/png-to-ppt
[11]: https://docs.aspose.com/slides/python-net
[12]: https://forum.aspose.com/
[13]: https://blog.aspose.com/2021/12/31/create-powerpoint-presentations-in-python/
[14]: https://blog.aspose.com/2021/12/28/convert-pptx-ppt-to-pdf-python/
[15]: https://blog.aspose.com/2021/12/29/convert-ppt-to-png-in-python/
[16]: https://blog.aspose.com/2022/02/09/add-watermark-to-powerpoint-ppt-in-python/
[17]: https://blog.aspose.com/2022/01/08/create-three-d-effects-in-ppt-python/





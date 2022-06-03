---
title: 'Add or Remove Shapes in PowerPoint Slides using Python'
date: Mon, 21 Feb 2022 14:17:22 +0000
draft: false
url: /2022/02/21/work-with-shapes-in-powerpoint-in-python/
author: ''Usman Aziz''
summary: 'Various types of diagrams are used in PowerPoint presentations to make the content more elaborative. These diagrams are comprised of different shapes such as ellipses, lines, rectangles, and connectors. In this article, you will learn **how to add, clone, and remove shapes in PowerPoint slides programmatically in Python**.'
tags: ['Add Connector to Shapes in PowerPoint Python', 'Add Shape to PowerPoint Slides in Python', 'Clone a Shape in PowerPoint Slides in Python', 'Python Library to Work with PowerPoint Shapes', 'Remove Shapes from PowerPoint in Python']
categories: ['Aspose.Slides Product Family']
---



{{< figure align=center src="images/Work-with-Shapes-in-Slides-in-C-1024x578.jpg" alt="Work with Shapes in PowerPoint in Python">}}


Various types of diagrams are used in PowerPoint presentations to make the content more elaborative. These diagrams are comprised of different shapes such as ellipses, lines, rectangles, and connectors. In this article, you will learn **how to add, clone, and remove shapes in PowerPoint slides programmatically in Python**.

*   [Python Library to Work with PowerPoint Shapes][1]
*   [Types of PowerPoint Shapes][2]
*   [Add Shape to PowerPoint Slides][3]
*   [Add Connector to Shapes in PowerPoint][4]
*   [Clone a Shape in PowerPoint Slides][5]
*   [Remove Shapes from PowerPoint Slides][6]

## Python Library to Work with PowerPoint Shapes {#API-to-Create-Shapes-in-PowerPoint-Slides}

[Aspose.Slides for Python via .NET][7] is designed to create and manipulate PowerPoint presentations from within the Python applications. We will use this library to work with shapes in PowerPoint slides. You can install it from [PyPI][8] using the following pip command.

```
> pip install aspose.slides
```

## Types of Shapes in PowerPoint {#Types-of-PowerPoint-Shapes}

You can create a variety of shapes in PowerPoint presentations using Aspose.Slides for Python. The most commonly used shapes include:

*   [](https://docs.aspose.com/slides/net/rectangle/)[Connector][9]
*   [](https://docs.aspose.com/slides/net/rectangle/)[Ellipse][10]
*   [](https://docs.aspose.com/slides/net/rectangle/)[Group][11]
*   [](https://docs.aspose.com/slides/net/rectangle/)[Line][12]
*   [](https://docs.aspose.com/slides/net/rectangle/)[Rectangle][13]
*   [and etc.][14]

## Add a Shape to PowerPoint Slides in Python {#Add-Shape-to-PowerPoint-Slides}

To add any shape including ellipse, line, rectangle, **add\_auto\_shape(ShapeType, Single, Single, Single, Single)** method is used to which you can pass the type of the shape and other necessary parameters. The **ShapeType** enum is used to specify the type of the shape. The following are the steps to add a shape to a PowerPoint slide in Python.

1.  Create a presentation or load an existing one using **Presentation** class.
2.  Obtain the reference of the desired slide from **Presentation.slides** collection.
3.  Add an Ellipse (or any other shape) using **add\_auto\_shape(ShapeType, Single, Single, Single, Single)** method.
4.  Save the presentation using **Presentation.save(String, SaveFormat)** method.

The following code sample shows how to add a shape to a PowerPoint slide in Python.

{{< gist aspose-com-gists 53925cebedbb57b8fd3e405561a70c25 "add-shape.py" >}}

The following is the ellipse that we have added using the code sample above.



{{< figure align=center src="images/add-shape-in-PPT.png" alt="Add a Shape to PowerPoint PPT in Python">}}


## Connect PowerPoint Shapes with a Connector in Python {#Add-Connector-to-Shapes-in-PowerPoint-Slides}

In diagrams, different shapes are connected to each other using a line called a connector. A connector could be a straight or curved line. Let's see how to add a connector between two PowerPoint shapes in Python.

1.  First, create an instance of the **Presentation **class to create or load presentation.
2.  Then, obtain the reference of a slide using **Presentation.slides** collection.
3.  Add two shapes just like you have added in the previous section and get their references.
4.  Create a connector using **add\_connector(ShapeType, Single, Single, Single, Single)** method.
5.  Join the shapes using **Connector.start\_shape\_connected\_to** and **Connector.end\_shape\_connected\_to** properties.
6.  Call **Connector.reroute()** method to create the shortest automatic connection path.
7.  Finally, save the presentation using **Presentation.save(string, SaveFormat)** method.

The following code sample shows how to connect shapes in a PowerPoint slide in Python.

{{< gist aspose-com-gists 53925cebedbb57b8fd3e405561a70c25 "add-connector.py" >}}

The following is the screenshot of the presentation after connecting shapes with a connector.



{{< figure align=center src="images/Connect-PowerPoint-Shapes.jpg" alt="Connect PowerPoint Shapes with a Connector in Python">}}


## Clone PowerPoint Shapes in Python {#Clone-a-Shape-in-PowerPoint-Slides}

Sometimes, you opt to clone shapes instead of creating a new one. To achieve that, Aspose.Slides supports shape cloning. The following are the steps to clone a shape in PowerPoint using Python.

1.  First, use **Presentation **class to load presentation file.
2.  Obtain the reference of a slide from **Presentation.slides** collection.
3.  Access the source and destination slide shapes from **ISlide.shapes** collection.
4.  Clone shapes from the source slide shape collection to destination slide using **add\_clone()** method.
5.  Finally, save the updated presentation file.

The following code sample shows how to clone shapes within PowerPoint slides in Python.

{{< gist aspose-com-gists 53925cebedbb57b8fd3e405561a70c25 "clone-shape.py" >}}

## Remove Shapes from PowerPoint Slides in Python {#Remove-Shape-from-PowerPoint-Slides}

You can also remove shapes from PowerPoint presentations by following the steps below.

1.  Create an instance of the **Presentation** class to load the PPT/PPTX file.
2.  Access the desired slide from **Presentation.slides** collection.
3.  Filter the desired shape with a specific text using **IShape.alternative\_text** property.
4.  Remove the shape using **ISlide.shapes.remove(IShape)** method.
5.  Finally, save the updated presentation file.

The following code sample shows how to remove shapes from a PowerPoint slide in Python.

{{< gist aspose-com-gists 53925cebedbb57b8fd3e405561a70c25 "remove-shape.py" >}}

## Get a Free License {#Get-a-Free-API-License}

You can [get a free temporary license][15] to use Aspose.Slides for Python without evaluation limitations.

## Conclusion

MS PowerPoint supports a range of shapes to create different types of diagrams such as flow charts. In this article, we have covered how to create PowerPoint shapes such as ellipses, rectangles, and connect them using connectors in Python. Moreover, you have learned how to clone and remove shapes in PowerPoint slides programmatically. You can explore more about Aspose.Slides for Python using the [documentation][16]. Also, you can feel free to let us know about your queries via our [forum][17].

## See Also

*   [Create PowerPoint Files in Python][18]
*   [Convert PPTX to PDF in Python][19]
*   [Convert PPT to PNG in Python][20]
*   [PPT/PPTX to HTML in Python][21]
*   [Add Watermark in PowerPoint PPT in Python][22]




[1]: #API-to-Create-Shapes-in-PowerPoint-Slides
[2]: #Types-of-PowerPoint-Shapes
[3]: #Add-Shape-to-PowerPoint-Slides
[4]: #Add-Connector-to-Shapes-in-PowerPoint-Slides
[5]: #Clone-a-Shape-in-PowerPoint-Slides
[6]: #Remove-Shape-from-PowerPoint-Slides
[7]: https://products.aspose.com/slides/python-net
[8]: https://pypi.org/project/aspose.slides/
[9]: https://docs.aspose.com/slides/python-net/connector/
[10]: https://docs.aspose.com/slides/python-net/ellipse/
[11]: https://docs.aspose.com/slides/python-net/group/
[12]: https://docs.aspose.com/slides/python-net/line/
[13]: https://docs.aspose.com/slides/python-net/rectangle/
[14]: https://docs.aspose.com/slides/python-net/shape-types/
[15]: https://purchase.aspose.com/temporary-license
[16]: https://docs.aspose.com/slides/python-net/
[17]: https://forum.aspose.com/
[18]: https://blog.aspose.com/2021/12/31/create-powerpoint-presentations-in-python/
[19]: https://blog.aspose.com/2021/12/28/convert-pptx-ppt-to-pdf-python/
[20]: https://blog.aspose.com/2021/12/29/convert-ppt-to-png-in-python/
[21]: https://blog.aspose.com/2021/12/16/convert-ppt-to-html-in-python/
[22]: https://blog.aspose.com/2022/02/09/add-watermark-to-powerpoint-ppt-in-python/





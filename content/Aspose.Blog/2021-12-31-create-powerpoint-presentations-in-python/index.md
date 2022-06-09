---
title: 'Create MS PowerPoint PPT/PPTX in Python'
seoTitle: "Create PowerPoint PPT PPTX in Python | Add Text, Table, Image, Chart"
description: "Use Python PowerPoint library to create or edit PPT/PPTX presentations in Python. Insert slides, text, tables, and charts in PPT presentations."
date: Fri, 31 Dec 2021 14:54:01 +0000
draft: false
url: /2021/12/31/create-powerpoint-presentations-in-python/
author: Usman Aziz
summary: "MS PowerPoint is a feature-rich application that lets you create interactive presentations using charts, graphics, animations, and other elements. As a programmer, you might need to automate PowerPoint's presentation manipulation features from within the Python applications. In this post, you will learn **how to create PowerPoint PPT or PPTX presentations in Python**. In addition, we will cover how to add slides, text, tables, images, and charts in the presentations programmatically."
tags: ['Add Slide to a Presentation in Python', 'Add an Image in Presentation in Python', 'Create a Chart in Presentation in Python', 'Open an Existing Presentation in Python', 'Python Library to Create PowerPoint Presentations']
categories: ['Aspose.Slides Product Family']
---



{{< figure align=center src="images/Create-PowerPoint-Presentation.jpg" alt="Create and modify PowerPoint ppt pptx in Python">}}


MS PowerPoint is a feature-rich application that lets you create interactive presentations using charts, graphics, animations, and other elements. As a programmer, you might need to automate PowerPoint's presentation manipulation features from within the Python applications. In this post, you will learn **how to create PowerPoint PPT or PPTX presentations in Python**. In addition, we will cover how to add slides, text, tables, images, and charts in the presentations programmatically.

*   [Python Library to Create PowerPoint PPT][1]
*   [Create a PowerPoint PPT][2]
*   [Open an Existing Presentation][3]
*   [Add Slide to a Presentation][4]
*   [Add Text to a Presentation][5]
*   [Create a Table in Presentation][6]
*   [Create a Chart in Presentation][7]
*   [Add an Image in Presentation][8]

## Python Library to Create PowerPoint PPT {#Python-Library-to-Create-PowerPoint-Presentations}

[Aspose.Slides for Python via .NET][9] is a powerful Python library that allows you to create and manipulate PowerPoint PPT/PPTX without MS Office. Moreover, you can update existing presentations and convert them to other formats. You can install the library from [PyPI][10] using the following pip command.

```
> pip install aspose.slides
```

## Create a PowerPoint PPT in Python {#Create-a-PowerPoint-Presentation}

First, let's create a PowerPoint presentation having an empty slide, which is added by default. The following steps show how to create a PowerPoint PPT in Python.

*   First, create an instance of the [Presentation][11] class.
*   Then, save PPT using **Presentation.save(string, export.SaveFormat)** method.

The following code sample shows how to create a PowerPoint PPTX file in Python.

{{< gist aspose-com-gists 51b39b78eacada9c434aebca4afce0d3 "create-presentation.py" >}}

## Open a PowerPoint PPTX File in Python {#Open-an-Existing-PowerPoint-Presentation}

You can also open an existing presentation and update its content. To achieve this, you only need to provide the path of the presentation file in the **Presentation** constructor. The following code sample shows how to open an existing PPT/PPTX file in Python.

{{< gist aspose-com-gists 51b39b78eacada9c434aebca4afce0d3 "open-presentation.py" >}}

## Add a Slide to PowerPoint PPT in Python {#Add-Slide-to-a-Presentation}

Let's now add a new slide in the presentation that we have created before. You can also add slides to an existing presentation in the same way by opening the presentation first (as shown in the [previous section][12]. The following are the steps to add a slide in the PPT/PPTX presentation in Python.

*   First, create a new (or load existing) presentation using [Presentation][13] class.
*   Then, get reference of the slides collection using **Presentation.slides** property.
*   Add slide using **Presentation.slides.add\_empty\_slide(LayoutSlide)** method.
*   Finally, save the presentation using **Presentation.save(string, export.SaveFormat)** method.

The following code sample shows how to add a slide in a PowerPoint presentation in Python.

{{< gist aspose-com-gists 51b39b78eacada9c434aebca4afce0d3 "add-slide.py" >}}

## Add Text to a PowerPoint PPT in Python {#Add-Text-to-Presentation-Slide}

Once we have added a slide, we can proceed to add the content. First, let's see how to add text to the presentation slides in Python.

*   Create a new (or load existing) PPT/PPTX using [Presentation][14] class.
*   Get reference of the slide from **Presentation.slides** collection.
*   Add a new auto shape in slide using **Slide.shapes.add\_auto\_shape(slides.ShapeType.RECTANGLE, int, int, int, int)** method and get shape's reference in an object.
*   Add a text frame to the shape using **add\_text\_frame(string)** method.
*   Access the default paragraph of the text frame.
*   Access the default portion of the paragraph.
*   Add text to the portion and save the presentation using **Presentation.save(string, export.SaveFormat)** method.

The following code sample shows how to add text to the slide in a PPT using Python.

{{< gist aspose-com-gists 51b39b78eacada9c434aebca4afce0d3 "add-text.py" >}}

The following is the screenshot of the slide after adding the text.



{{< figure align=center src="images/add-text-to-presentation.png" alt="add text in powerpoint ppt in python">}}


[Read more][15] about working with text in PowerPoint presentations.

## Create Table in a PowerPoint PPT in Python {#Create-Table-in-Presentation}

Tables are an integral part of the documents and are widely used in PowerPoint presentations as well. Aspose.Slides for Python makes it quite easier for you to create a table in a presentation. So let's see how to create a table in a PPT using Python.

*   Create a new (or load existing) PPT/PPTX using [Presentation][16] class.
*   Get reference of the slide from **Presentation.slides** collection.
*   Define arrays of columns with width and rows with height.
*   Create table using **Slide.shapes.addTable()** and get reference of the table in an object.
*   Loop through the cells to apply the formatting.
*   Add text to the cells using **Table.rows\[\]\[\].text\_frame.text** property.
*   Save the presentation using **Presentation.save(string, export.SaveFormat)** method.

The following code sample shows how to create tables in a PowerPoint presentation using Python.

{{< gist aspose-com-gists 51b39b78eacada9c434aebca4afce0d3 "add-table.py" >}}

The following is the output of the code snippet above.



{{< figure align=center src="images/add-table-in-presentation.png" alt="add table in PowerPoint ppt in Python">}}


Explore other features of [creating and manipulating tables][17].

## Create Chart in a PowerPoint PPT in Python {#Create-Charts-in-Presentation}

The following are the steps to add a chart in a PowerPoint presentation in Python.

*   Create a new (or load existing) presentation using [Presentation][18] class.
*   Get reference of the slide from **Presentation.slides** collection.
*   Add a chart with the desired type using **Slide.shapes.addChart(ChartType, single, single, single, single)** method.
*   Access the chart data worksheet.
*   Clear all the default series and categories.
*   Add new series and categories.
*   Add new chart data for chart series.
*   Set fill color for chart series.
*   Add chart series labels.
*   Save the presentation as a PPTX file.

The following code sample shows how to add a chart in a PPT using Python.

{{< gist aspose-com-gists 51b39b78eacada9c434aebca4afce0d3 "add-chart.py" >}}

The following screenshot shows the chart we have created using the code snippet above.



{{< figure align=center src="images/create-chart-in-presentation.png" alt="add chart in PowerPoint pptx in Python">}}


[Learn more][19] about creating charts in PowerPoint presentations.

## Add an Image in PowerPoint PPTX in Python {#Add-an-Image-in-Presentation}

The following are the steps to add an image in a PowerPoint PPTX in Python.

*   Create a new (or load existing) presentation using [Presentation][20] class.
*   Get reference of the slide from **Presentation.slides** collection.
*   Open an image from file using **open(string, string)** method.
*   Add image into the image collection of presentation using **Presentation.images.add\_image()** method.
*   Add image to the slide using **Slide.shapes.add\_picture\_frame()** method.
*   Save the presentation using **Presentation.save(string, export.SaveFormat)** method.

The following code sample shows how to add an image to a PowerPoint presentation in Python.

{{< gist aspose-com-gists 51b39b78eacada9c434aebca4afce0d3 "add-image.py" >}}

The following is the output of the code sample above.



{{< figure align=center src="images/add-image-in-presentation.png" alt="add images in PowerPoint PPT in Python">}}


Read more about [working with images][21] in PowerPoint presentations.

## Get a Free License

You can use Aspose.Slides for Python via .NET without evaluation limitations by getting a [temporary license][22].

## Conclusion

In this article, you have learned how to create PowerPoint PPT/PPTX from scratch in Python. We have demonstrated how to add slides, text, tables, charts, and images in PowerPoint presentations. Furthermore, you can explore other features of Aspose.Slides for Python using the [documentation][23]. Also, feel free to share your queries with us via our [forum][24].

## See Also

*   [Convert PPTX to PDF in Python][25]
*   [Convert PPT to PNG in Python][26]
*   [PPT/PPTX to HTML in Python][27]




[1]: #Python-Library-to-Create-PowerPoint-Presentations
[2]: #Create-a-PowerPoint-Presentation
[3]: #Open-an-Existing-PowerPoint-Presentation
[4]: #Add-Slide-to-a-Presentation
[5]: #Add-Text-to-Presentation-Slide
[6]: #Create-Table-in-Presentation
[7]: #Create-Charts-in-Presentation
[8]: #Add-an-Image-in-Presentation
[9]: https://products.aspose.com/slides/python-net
[10]: https://pypi.org/project/aspose.slides/
[11]: https://docs.aspose.com/slides/python-net/api-reference/aspose.slides/presentation/
[12]: #Open-an-Existing-PowerPoint-Presentation)
[13]: https://docs.aspose.com/slides/python-net/api-reference/aspose.slides/presentation/
[14]: https://docs.aspose.com/slides/python-net/api-reference/aspose.slides/presentation/
[15]: https://docs.aspose.com/slides/python-net/manage-text/
[16]: https://docs.aspose.com/slides/python-net/api-reference/aspose.slides/presentation/
[17]: https://docs.aspose.com/slides/python-net/powerpoint-table/
[18]: https://docs.aspose.com/slides/python-net/api-reference/aspose.slides/presentation/
[19]: https://docs.aspose.com/slides/python-net/powerpoint-charts/
[20]: https://docs.aspose.com/slides/python-net/api-reference/aspose.slides/presentation/
[21]: https://docs.aspose.com/slides/python-net/image/
[22]: https://purchase.aspose.com/temporary-license
[23]: https://docs.aspose.com/slides/python-net
[24]: https://forum.aspose.com/
[25]: https://blog.aspose.com/2021/12/28/convert-pptx-ppt-to-pdf-python/
[26]: https://blog.aspose.com/2021/12/29/convert-ppt-to-png-in-python/
[27]: https://blog.aspose.com/2021/12/16/convert-ppt-to-html-in-python/





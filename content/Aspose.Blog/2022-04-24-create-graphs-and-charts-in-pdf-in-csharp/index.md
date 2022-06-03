---
title: 'Create Graphs and Charts in PDF in C#'
date: Sun, 24 Apr 2022 07:11:00 +0000
draft: false
url: /2022/04/24/create-graphs-and-charts-in-pdf-in-csharp/
author: 'Usman Aziz'
summary: ''
tags: ['Create an Arc in PDF in Csharp', 'Create an Circle in PDF in Csharp', 'Create an Ellipse in PDF in Csharp', 'Create an Line in PDF in Csharp', 'Create an Rectangle in PDF in Csharp', 'DotNet API to Create Graphs and Charts in PDF']
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/Create-Graphs-and-Charts-in-PDF.png" alt="Create Graphs and Charts in PDF in C#">}}


In a number of [PDF][1] documents, graphs and charts are used to visually represent the data. Some are used to graphically describe the flow of the activities or operations in a system such as flow charts, whereas, some are used to draw the patterns. In this article, you will learn **how to create graphs and charts in PDF files programmatically in C#**. We will explicitly cover how to create different graphical objects in a PDF file.

*   [.NET API to Create Graphs and Charts in PDF][2]
*   [Create an Arc in PDF][3]
*   [Create a Circle in PDF][4]
*   [Add a Curve in PDF][5]
*   [Add a Line in PDF][6]
*   [Create a Rectangle in PDF][7]
*   [Create an Ellipse in PDF][8]

## C# .NET API to Create Graphs and Charts in PDF {#API-to-Create-Graphs-and-Charts-in-PDF}

We will use [Aspose.PDF for .NET][9] to create charts and graphs in PDF files. The API is designed to perform PDF generation and manipulation within the .NET applications. It allows you to create PDF files of simple and complex layouts seamlessly. You can [download][10] the API's binaries or install it using [NuGet][11].

```
PM> Install-Package Aspose.PDF
```

## Create an Arc in a PDF in C# {#Create-an-Arc-in-PDF}

The following are the steps to add an arc in PDF in C#.

1.  Create a new PDF or load an existing one using the **[Document][12]** class.
2.  Create a **[Graph][13]** object with dimensions.
3.  Set **[BorderInfo][14]** for graph object.
4.  Create an instance of **[Arc][15]** class and set its dimensions and other parameters.
5.  Add arc to the shapes collection of _Graph_ using **[Graph.Shapes.Add(Arc)][16]** method.
6.  Add graph to the page using **[Page.Paragraphs.Add(Graph)][17]** method.
7.  Save the PDF file using **[Document.Save(String)][18]** method.

The following code sample shows how to add arcs in a PDF in C#.

{{< gist aspose-com-gists 340243ea16f22cd56afbabc050e5b955 "create-arc-in-pdf.cs" >}}

The following are the arcs that we have generated using the above code sample.



{{< figure align=center src="images/Create-Arc-in-PDF.png" alt="Create an Arc in PDF in C#">}}


## Create a Circle in a PDF in C# {#Create-a-Circle-in-PDF}

The following are the steps to add a circle to a PDF file in C#.

1.  Create a new PDF or load an existing one using **[Document][19]** class.
2.  Create a **[Graph][20]** object with dimensions.
3.  Set ****[BorderInfo][21]**** for graph object.
4.  Create an instance of **[Circle][22]** class and set its dimensions.
5.  Add circle to the shapes collection of _Graph_ using **[Graph.Shapes.Add(Circle)][23]** method.
6.  Add graph to the page using **[Page.Paragraphs.Add(Graph)][24]** method.
7.  Save the PDF file using **[Document.Save(String)][25]** method.

The following code sample shows how to add a circle in PDF in C#.

{{< gist aspose-com-gists 340243ea16f22cd56afbabc050e5b955 "create-circle-in-pdf.cs" >}}

The following is the circle that we have generated using the above code sample.



{{< figure align=center src="images/Create-Circle-in-PDF.png" alt="Create a Circle in PDF in C#">}}


## Add a Curve in a PDF in C# {#Add-a-Curve-in-PDF}

The following are the steps to add a curve in a PDF file in C#.

1.  Create a new PDF or load an existing one using **[Document][26]** class.
2.  Create a **[Graph][27]** object with dimensions.
3.  Set ****[BorderInfo][28]**** for graph object.
4.  Create an instance of **[Curve][29]** class and set its dimensions.
5.  Add curve to the shapes collection of _Graph_ using **[Graph.Shapes.Add(Curve)][30]** method.
6.  Add graph to the page using **[Page.Paragraphs.Add(Graph)][31]** method.
7.  Save the PDF file using **[Document.Save(String)][32]** method.

The following code sample shows how to add curves to a PDF file in C#.

{{< gist aspose-com-gists 340243ea16f22cd56afbabc050e5b955 "create-curve-in-pdf.cs" >}}

The following are the curves that we have generated using the above code sample.



{{< figure align=center src="images/Create-Curves-in-PDF.png" alt="Add a Curve in PDF in C#">}}


## Add a Line in a PDF in C# {#Add-a-Line-in-PDF}

The following are the steps to add a line in a PDF using C#.

1.  Create a new PDF or load an existing one using **[Document][33]** class.
2.  Create a **[Graph][34]** object with dimensions.
3.  Set ****[BorderInfo][35]**** for graph object.
4.  Create an instance of **[Line][36]** class and set its dimensions.
5.  Set other properties of line such as style, width, etc.
6.  Add line to the shapes collection of _Graph_ using **[Graph.Shapes.Add(Line)][37]** method.
7.  Add graph to the page using **[Page.Paragraphs.Add(Graph)][38]** method.
8.  Save the PDF file using **[Document.Save(String)][39]** method.

The following code sample shows how to add lines in PDF in C#.

{{< gist aspose-com-gists 340243ea16f22cd56afbabc050e5b955 "create-line-in-pdf.cs" >}}

The following are the lines that we have created using the above code sample.



{{< figure align=center src="images/Create-Line-in-PDF.png" alt="Add a Line in PDF in C#">}}


## Create a Rectangle in PDF in C# {#Create-a-Rectangle-in-PDF}

Similar to other graphical objects, you can add a rectangle to the PDF. Also, you can fill the rectangle with a certain color, control Z-Order, add gradient color, etc. The following are the steps to create a rectangle in a PDF file in C#.

1.  Create a new PDF or load an existing one using **[Document][40]** class.
2.  Create a **[Graph][41]** object with dimensions.
3.  Set ****[BorderInfo][42]**** for graph object.
4.  Create an instance of **[Rectangle][43]** class and set its dimensions.
5.  Set other properties of the rectangle such as fill color, gradient, etc.
6.  Add rectangle to the shapes collection of _Graph_ using **[Graph.Shapes.Add(Rectangle)][44]** method.
7.  Add graph to the page using **[Page.Paragraphs.Add(Graph)][45]** method.
8.  Save the PDF file using **[Document.Save(String)][46]** method.

The following code sample shows how to add rectangles in PDF in C#.

{{< gist aspose-com-gists 340243ea16f22cd56afbabc050e5b955 "create-rectangle-in-pdf.cs" >}}

The following are the rectangles that we have created using the above code sample.



{{< figure align=center src="images/Create-Rectangle-in-PDF.png" alt="Create a Rectangle in PDF in C#">}}


## Create an Ellipse in PDF in C# {#Create-an-Ellipse-in-PDF}

Last but not the least, let's have a look at how to create an ellipse in PDF in C#.

1.  Create a new PDF or load an existing one using **[Document][47]** class.
2.  Create a **[Graph][48]** object with dimensions.
3.  Set ****[BorderInfo][49]**** for graph object.
4.  Create an instance of **[Ellipse][50]** class and set its dimensions.
5.  Set other properties of ellipse such as fill color, etc.
6.  Add ellipse to the shapes collection of _Graph_ using **[Graph.Shapes.Add(Ellipse)][51]** method.
7.  Add graph to the page using **[Page.Paragraphs.Add(Graph)][52]** method.
8.  Save the PDF file using **[Document.Save(String)][53]** method.

The following code sample shows how to add an ellipse in a PDF file in C#.

{{< gist aspose-com-gists 340243ea16f22cd56afbabc050e5b955 "create-ellipse-in-pdf.cs" >}}

The following are the ellipses that we have created using the above code sample.



{{< figure align=center src="images/Create-Ellipse-in-PDF.png" alt="Create an Ellipse in PDF in C#">}}


## Get a Free License {#Get-a-Free-License}

You can [get a free temporary license][54] in order to use Aspose.PDF for .NET without evaluation limitations.

## Conclusion

In this article, you have learned how to create different objects of charts and graphs in PDF files using C#. You have seen how to add arcs, circles, rectangles, lines, curves, and ellipses in a PDF. Furthermore, you can explore more about .NET PDF API using the [documentation][55]. In case you would have any questions or queries, you can contact us via our [forum][56].

## See Also

*   [Add or Remove Annotations in PDF Files using C#][57]
*   [Extract Images from PDF using C#][58]
*   [Create PDF File from Images using C#][59]




[1]: https://docs.fileformat.com/pdf/
[2]: #API-to-Create-Graphs-and-Charts-in-PDF
[3]: #Create-an-Arc-in-PDF
[4]: #Create-a-Circle-in-PDF
[5]: #Add-a-Curve-in-PDF
[6]: #Add-a-Line-in-PDF
[7]: #Create-a-Rectangle-in-PDF
[8]: #Create-an-Ellipse-in-PDF
[9]: https://products.aspose.com/pdf/net/
[10]: https://downloads.aspose.com/pdf/net/
[11]: http://nuget.org/packages/Aspose.PDF
[12]: https://apireference.aspose.com/pdf/net/aspose.pdf/document
[13]: https://apireference.aspose.com/pdf/net/aspose.pdf.drawing/graph
[14]: https://apireference.aspose.com/pdf/net/aspose.pdf/borderinfo
[15]: https://apireference.aspose.com/pdf/net/aspose.pdf.drawing/arc
[16]: https://apireference.aspose.com/pdf/net/aspose.pdf.drawing/graph/properties/shapes
[17]: https://apireference.aspose.com/pdf/net/aspose.pdf/page/properties/paragraphs
[18]: https://apireference.aspose.com/pdf/net/aspose.pdf.document/save/methods/5
[19]: https://apireference.aspose.com/pdf/net/aspose.pdf/document
[20]: https://apireference.aspose.com/pdf/net/aspose.pdf.drawing/graph
[21]: https://apireference.aspose.com/pdf/net/aspose.pdf/borderinfo
[22]: https://apireference.aspose.com/pdf/net/aspose.pdf.drawing/circle
[23]: https://apireference.aspose.com/pdf/net/aspose.pdf.drawing/graph/properties/shapes
[24]: https://apireference.aspose.com/pdf/net/aspose.pdf/page/properties/paragraphs
[25]: https://apireference.aspose.com/pdf/net/aspose.pdf.document/save/methods/5
[26]: https://apireference.aspose.com/pdf/net/aspose.pdf/document
[27]: https://apireference.aspose.com/pdf/net/aspose.pdf.drawing/graph
[28]: https://apireference.aspose.com/pdf/net/aspose.pdf/borderinfo
[29]: https://apireference.aspose.com/pdf/net/aspose.pdf.drawing/curve
[30]: https://apireference.aspose.com/pdf/net/aspose.pdf.drawing/graph/properties/shapes
[31]: https://apireference.aspose.com/pdf/net/aspose.pdf/page/properties/paragraphs
[32]: https://apireference.aspose.com/pdf/net/aspose.pdf.document/save/methods/5
[33]: https://apireference.aspose.com/pdf/net/aspose.pdf/document
[34]: https://apireference.aspose.com/pdf/net/aspose.pdf.drawing/graph
[35]: https://apireference.aspose.com/pdf/net/aspose.pdf/borderinfo
[36]: https://apireference.aspose.com/pdf/net/aspose.pdf.drawing/line
[37]: https://apireference.aspose.com/pdf/net/aspose.pdf.drawing/graph/properties/shapes
[38]: https://apireference.aspose.com/pdf/net/aspose.pdf/page/properties/paragraphs
[39]: https://apireference.aspose.com/pdf/net/aspose.pdf.document/save/methods/5
[40]: https://apireference.aspose.com/pdf/net/aspose.pdf/document
[41]: https://apireference.aspose.com/pdf/net/aspose.pdf.drawing/graph
[42]: https://apireference.aspose.com/pdf/net/aspose.pdf/borderinfo
[43]: https://apireference.aspose.com/pdf/net/aspose.pdf.drawing/rectangle
[44]: https://apireference.aspose.com/pdf/net/aspose.pdf.drawing/graph/properties/shapes
[45]: https://apireference.aspose.com/pdf/net/aspose.pdf/page/properties/paragraphs
[46]: https://apireference.aspose.com/pdf/net/aspose.pdf.document/save/methods/5
[47]: https://apireference.aspose.com/pdf/net/aspose.pdf/document
[48]: https://apireference.aspose.com/pdf/net/aspose.pdf.drawing/graph
[49]: https://apireference.aspose.com/pdf/net/aspose.pdf/borderinfo
[50]: https://apireference.aspose.com/pdf/net/aspose.pdf.drawing/ellipse
[51]: https://apireference.aspose.com/pdf/net/aspose.pdf.drawing/graph/properties/shapes
[52]: https://apireference.aspose.com/pdf/net/aspose.pdf/page/properties/paragraphs
[53]: https://apireference.aspose.com/pdf/net/aspose.pdf.document/save/methods/5
[54]: https://purchase.aspose.com/temporary-license
[55]: https://docs.aspose.com/pdf/net/
[56]: https://forum.aspose.com/
[57]: https://blog.aspose.com/2021/01/04/add-or-remove-annotations-in-pdf-using-csharp/
[58]: https://blog.aspose.com/2021/06/15/extract-images-from-pdf-in-csharp/
[59]: https://blog.aspose.com/2021/04/20/create-pdf-from-images-using-csharp/





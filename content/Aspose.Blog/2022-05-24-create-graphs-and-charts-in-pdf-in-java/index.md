---
title: 'Create Graphs and Charts in PDF in Java'
date: Tue, 24 May 2022 17:16:56 +0000
draft: false
url: /2022/05/24/create-graphs-and-charts-in-pdf-in-java/
author: ''Usman Aziz''
summary: 'Graphs and charts are used to visually represent the data in [PDF][1] files. Furthermore, you can use them to graphically describe the flow of the activities or operations in a system such as flow charts. In this article, you will learn **how to create graphs and charts in PDF files programmatically in Java**. We will explicitly cover how to create different graphical objects in a PDF file.'
tags: ['Add a Curve in PDF in Java', 'Add a Line in PDF in Java', 'Create a Circle in PDF in Java', 'Create a Rectangle in PDF in Java', 'Create an Arc in PDF in Java', 'Create an Ellipse in PDF in Java']
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/Create-Graphs-and-Charts-in-PDF.png" alt="Create Graphs and Charts in PDF in Java">}}


Graphs and charts are used to visually represent the data in [PDF][2] files. Furthermore, you can use them to graphically describe the flow of the activities or operations in a system such as flow charts. In this article, you will learn **how to create graphs and charts in PDF files programmatically in Java**. We will explicitly cover how to create different graphical objects in a PDF file.

*   [Java API to Create Graphs and Charts in PDF][3]
*   [Create an Arc in PDF][4]
*   [Create a Circle in PDF][5]
*   [Add a Curve in PDF][6]
*   [Add a Line in PDF][7]
*   [Create a Rectangle in PDF][8]
*   [Create an Ellipse in PDF][9]

## Java API to Create Graphs and Charts in PDF {#API-to-Create-Graphs-and-Charts-in-PDF}

[Aspose.PDF for Java][10] is an amazing API that provides a range of features for PDF generation and manipulation. Using the API, you can seamlessly create PDF files of simple and complex layouts. We will use this API to create graphs and charts in PDF files. You can [download][11] the API or install it using the following Maven configurations.

```
**Repository:**
<repository>
    <id>AsposeJavaAPI</id>
    <name>Aspose Java API</name>
    <url>https://repository.aspose.com/repo/</url>
</repository>

**Dependency:**
<dependency>
    <groupId>com.aspose</groupId>
    <artifactId>aspose-pdf</artifactId>
    <version>22.4</version>
</dependency>
```

## Create an Arc in a PDF in Java {#Create-an-Arc-in-PDF}

The following are the steps to add an arc in PDF in Java.

1.  Create a new PDF or load an existing one using [**Document**][12] class.
2.  Create a [**Graph**][13] object with dimensions.
3.  Set [**BorderInfo**][14] for graph object.
4.  Create an instance of [**Arc**][15] class and set its dimensions and other parameters.
5.  Add arc to the shapes collection of _Graph_ using **[Graph.getShapes().add(Arc)][16]** method.
6.  Add graph to the page using **[Page.getParagraphs().add(Graph)][17]** method.
7.  Save the PDF file using [**Document.save(String)**][18] method.

The following code sample shows how to add arcs in a PDF in Java.

{{< gist aspose-com-gists b1d8627fecbb379a492d15292fc9328c "create-arc-in-pdf.java" >}}

The following are the arcs that we have generated using the above code sample.



{{< figure align=center src="images/Create-Arc-in-PDF.png" alt="Create an Arc in PDF in Java">}}


## Create a Circle in a PDF in Java {#Create-a-Circle-in-PDF}

The following are the steps to add a circle to a PDF file in Java.

1.  Create a new PDF or load an existing one using [**Document**][19] class.
2.  Create a [**Graph**][20] object with dimensions.
3.  Set [](https://apireference.aspose.com/pdf/java/com.aspose.pdf.drawing/Graph#setBorder-com.aspose.pdf.BorderInfo-)**[**BorderInfo**][21]** for graph object.
4.  Create an instance of **[Circle][22]** class and set its dimensions.
5.  Add circle to the shapes collection of _Graph_ using **[Graph.getShapes().add(Circle)][23]** method.
6.  Add graph to the page using **[Page.getParagraphs().add(Graph)][24]** method.
7.  Save the PDF file using [**Document.save(String)**][25] method.

The following code sample shows how to add a circle in PDF in Java.

{{< gist aspose-com-gists b1d8627fecbb379a492d15292fc9328c "create-circle-in-pdf.java" >}}

The following is the circle that we have generated using the above code sample.



{{< figure align=center src="images/Create-Circle-in-PDF.png" alt="Create a Circle in PDF in Java">}}


## Add a Curve in a PDF in Java {#Add-a-Curve-in-PDF}

The following are the steps to add a curve in a PDF file in Java.

1.  Create a new PDF or load an existing one using [**Document**][26] class.
2.  Create a [**Graph**][27] object with dimensions.
3.  Set [](https://apireference.aspose.com/pdf/java/com.aspose.pdf.drawing/Graph#setBorder-com.aspose.pdf.BorderInfo-)**[**BorderInfo**][28]** for graph object.
4.  Create an instance of **[Curve][29]** class and set its dimensions.
5.  Add curve to the shapes collection of _Graph_ using **[Graph.getShapes().add(Curve)][30]** method.
6.  Add graph to the page using **[Page.getParagraphs().add(Graph)][31]** method.
7.  Save the PDF file using [**Document.save(String)**][32] method.

The following code sample shows how to add curves to a PDF file in Java.

{{< gist aspose-com-gists b1d8627fecbb379a492d15292fc9328c "create-curve-in-pdf.java" >}}

The following are the curves that we have generated using the above code sample.



{{< figure align=center src="images/Create-Curves-in-PDF.png" alt="Add a Curve in PDF in Java">}}


## Add a Line in a PDF in Java {#Add-a-Line-in-PDF}

The following are the steps to add a line in a PDF using Java.

1.  Create a new PDF or load an existing one using [**Document**][33] class.
2.  Create a [**Graph**][34] object with dimensions.
3.  Set [](https://apireference.aspose.com/pdf/java/com.aspose.pdf.drawing/Graph#setBorder-com.aspose.pdf.BorderInfo-)**[**BorderInfo**][35]** for graph object.
4.  Create an instance of **[Line][36]** class and set its dimensions.
5.  Set other properties of line such as style, width, etc.
6.  Add line to the shapes collection of _Graph_ using **[Graph.getShapes().add(Line)][37]** method.
7.  Add graph to the page using **[Page.getParagraphs().add(Graph)][38]** method.
8.  Save the PDF file using [**Document.save(String)**][39] method.

The following code sample shows how to add lines in PDF in Java.

{{< gist aspose-com-gists b1d8627fecbb379a492d15292fc9328c "create-line-in-pdf.java" >}}

The following are the lines that we have created using the above code sample.



{{< figure align=center src="images/Create-Line-in-PDF.png" alt="Add a Line in PDF in Java">}}


## Create a Rectangle in PDF in Java {#Create-a-Rectangle-in-PDF}

Similar to other graphical objects, you can add a rectangle to the PDF. Also, you can fill the rectangle with a certain color, control Z-Order, add gradient color, etc. The following are the steps to create a rectangle in a PDF file in Java.

1.  Create a new PDF or load an existing one using [**Document**][40] class.
2.  Create a [**Graph**][41] object with dimensions.
3.  Set [](https://apireference.aspose.com/pdf/java/com.aspose.pdf.drawing/Graph#setBorder-com.aspose.pdf.BorderInfo-)**[**BorderInfo**][42]** for graph object.
4.  Create an instance of [**Rectangle**][43] class and set its dimensions.
5.  Set other properties of the rectangle such as fill color, gradient, etc.
6.  Add rectangle to the shapes collection of _Graph_ using **[Graph.getShapes().add(Rectangle)][44]** method.
7.  Add graph to the page using **[Page.getParagraphs().add(Graph)][45]** method.
8.  Save the PDF file using [**Document.save(String)**][46] method.

The following code sample shows how to add rectangles in PDF in Java.

{{< gist aspose-com-gists b1d8627fecbb379a492d15292fc9328c "create-rectangle-in-pdf.java" >}}

The following are the rectangles that we have created using the above code sample.



{{< figure align=center src="images/Create-Rectangle-in-PDF.png" alt="Create a Rectangle in PDF in Java">}}


## Create an Ellipse in PDF in Java {#Create-an-Ellipse-in-PDF}

Last but not the least, let's have a look at how to create an ellipse in PDF in Java.

1.  Create a new PDF or load an existing one using [**Document**][47] class.
2.  Create a [**Graph**][48] object with dimensions.
3.  Set [](https://apireference.aspose.com/pdf/java/com.aspose.pdf.drawing/Graph#setBorder-com.aspose.pdf.BorderInfo-)**[**BorderInfo**][49]** for graph object.
4.  Create an instance of **[Ellipse][50]** class and set its dimensions.
5.  Set other properties of ellipse such as fill color, etc.
6.  Add ellipse to the shapes collection of _Graph_ using **[Graph.getShapes().add(Ellipse)][51]** method.
7.  Add graph to the page using **[Page.getParagraphs().add(Graph)][52]** method.
8.  Save the PDF file using [**Document.save(String)**][53] method.

The following code sample shows how to add an ellipse in a PDF file in Java.

{{< gist aspose-com-gists b1d8627fecbb379a492d15292fc9328c "create-ellipse-in-pdf.java" >}}

The following are the ellipses that we have created using the above code sample.



{{< figure align=center src="images/Create-Ellipse-in-PDF.png" alt="Create an Ellipse in PDF in Java">}}


## Get a Free License {#Get-a-Free-License}

You can [get a free temporary license][54] in order to use Aspose.PDF for Java without evaluation limitations.

## Conclusion

In this article, you have learned how to create different objects of charts and graphs in PDF files using Java. You have seen how to add arcs, circles, rectangles, lines, curves, and ellipses in a PDF. Furthermore, you can explore more about the Java PDF API using the [documentation][55]. In case you would have any questions or queries, you can contact us via our [forum][56].

## See Also

*   [Creating PDF Files from Scratch using Java][57]




[1]: https://docs.fileformat.com/pdf/
[2]: https://docs.fileformat.com/pdf/
[3]: #API-to-Create-Graphs-and-Charts-in-PDF
[4]: #Create-an-Arc-in-PDF
[5]: #Create-a-Circle-in-PDF
[6]: #Add-a-Curve-in-PDF
[7]: #Add-a-Line-in-PDF
[8]: #Create-a-Rectangle-in-PDF
[9]: #Create-an-Ellipse-in-PDF
[10]: https://products.aspose.com/pdf/java/
[11]: https://downloads.aspose.com/pdf/java
[12]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/Document
[13]: https://apireference.aspose.com/pdf/java/com.aspose.pdf.drawing/Graph
[14]: https://apireference.aspose.com/pdf/java/com.aspose.pdf.drawing/Graph#setBorder-com.aspose.pdf.BorderInfo-
[15]: https://apireference.aspose.com/pdf/java/com.aspose.pdf.drawing/Arc
[16]: https://apireference.aspose.com/pdf/java/com.aspose.pdf.drawing/Graph#getShapes--
[17]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/Page#getParagraphs--
[18]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/Document#save-java.lang.String-
[19]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/Document
[20]: https://apireference.aspose.com/pdf/java/com.aspose.pdf.drawing/Graph
[21]: https://apireference.aspose.com/pdf/java/com.aspose.pdf.drawing/Graph#setBorder-com.aspose.pdf.BorderInfo-
[22]: https://apireference.aspose.com/pdf/java/com.aspose.pdf.drawing/Circle
[23]: https://apireference.aspose.com/pdf/java/com.aspose.pdf.drawing/Graph#getShapes--
[24]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/Page#getParagraphs--
[25]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/Document#save-java.lang.String-
[26]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/Document
[27]: https://apireference.aspose.com/pdf/java/com.aspose.pdf.drawing/Graph
[28]: https://apireference.aspose.com/pdf/java/com.aspose.pdf.drawing/Graph#setBorder-com.aspose.pdf.BorderInfo-
[29]: https://apireference.aspose.com/pdf/java/com.aspose.pdf.drawing/Curve
[30]: https://apireference.aspose.com/pdf/java/com.aspose.pdf.drawing/Graph#getShapes--
[31]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/Page#getParagraphs--
[32]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/Document#save-java.lang.String-
[33]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/Document
[34]: https://apireference.aspose.com/pdf/java/com.aspose.pdf.drawing/Graph
[35]: https://apireference.aspose.com/pdf/java/com.aspose.pdf.drawing/Graph#setBorder-com.aspose.pdf.BorderInfo-
[36]: https://apireference.aspose.com/pdf/java/com.aspose.pdf.drawing/Line
[37]: https://apireference.aspose.com/pdf/java/com.aspose.pdf.drawing/Graph#getShapes--
[38]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/Page#getParagraphs--
[39]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/Document#save-java.lang.String-
[40]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/Document
[41]: https://apireference.aspose.com/pdf/java/com.aspose.pdf.drawing/Graph
[42]: https://apireference.aspose.com/pdf/java/com.aspose.pdf.drawing/Graph#setBorder-com.aspose.pdf.BorderInfo-
[43]: https://apireference.aspose.com/pdf/java/com.aspose.pdf.drawing/Rectangle
[44]: https://apireference.aspose.com/pdf/java/com.aspose.pdf.drawing/Graph#getShapes--
[45]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/Page#getParagraphs--
[46]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/Document#save-java.lang.String-
[47]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/Document
[48]: https://apireference.aspose.com/pdf/java/com.aspose.pdf.drawing/Graph
[49]: https://apireference.aspose.com/pdf/java/com.aspose.pdf.drawing/Graph#setBorder-com.aspose.pdf.BorderInfo-
[50]: https://apireference.aspose.com/pdf/java/com.aspose.pdf.drawing/Ellipse
[51]: https://apireference.aspose.com/pdf/java/com.aspose.pdf.drawing/Graph#getShapes--
[52]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/Page#getParagraphs--
[53]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/Document#save-java.lang.String-
[54]: https://purchase.aspose.com/temporary-license
[55]: https://docs.aspose.com/pdf/java/
[56]: https://forum.aspose.com/
[57]: https://blog.aspose.com/2020/12/31/create-pdf-files-in-java/





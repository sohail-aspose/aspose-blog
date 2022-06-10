---
title: 'Control Z-Order of Rectangle and Text with transparency using Aspose.Pdf for Java 11.3.0'
date: Thu, 07 Apr 2016 16:18:46 +0000
draft: false
url: /2016/04/07/controll-z-order-of-rectangle-and-text-with-transparency-using-aspose.pdf-for-java-11.3.0/
author: Codewarior
summary: ''
tags: ['Nayyer Shahbaz', 'Add transparent text to PDF', 'Control Z-Order of Rectangle in PDF']
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/aspose-Pdf-for-Java_100.png" alt="Aspose.Pdf for .NET logo">}}


As a part of our continuous improvement process, a new release of [Aspose.PDF for Java 11.3.0][1] which has same set of features recently introduced in its sibling Aspose.PDF for .NET 11.3.0. As Aspose.Pdf for Java is an auto-ported version of Aspose.PDF for .NET, so we try our best to provide similar features in Aspose.PDF for Java so that our customers using Java platform enjoy same set of features. Among these new features, we also have fixed major issues related to PDF to TIFF, PCL to PDF, PDF to HTML, PDF to PDF/A conversion and general performance improvements.

## Controlling Z-Order of Rectangle

Aspose.Pdf for Java supports the feature to add graph objects (for example graph, line, rectangle etc.) to PDF documents. When adding more than one instance of same object inside PDF file, we can control their rendering by specifying the Z-Order. Z-Order is also used when we need to render objects on top of each other.

```
// instantiate Document class object
Document doc1 = new Document();
/// add page to pages collection of PDF file
com.aspose.pdf.Page page1 = doc1.getPages().add();
// set size of PDF page
page1.setPageSize(375, 300);
// set left margin for page object as 0
page1.getPageInfo().getMargin().setLeft(0);
// set top margin of page object as 0
page1.getPageInfo().getMargin().setTop(0);
// create a new rectangle with Color as Red, Z-Order as 0 and certain dimensions
AddRectangle(page1, 50, 40, 60, 40, com.aspose.pdf.Color.getRed(), 2);
// create a new rectangle with Color as Blue, Z-Order as 0 and certain dimensions
AddRectangle(page1, 20, 20, 30, 30, com.aspose.pdf.Color.getBlue(), 1);
// create a new rectangle with Color as Green, Z-Order as 0 and certain dimensions
AddRectangle(page1, 40, 40, 60, 30, com.aspose.pdf.Color.getGreen(), 0);
// save resultant PDF file
doc1.save("c:/pdftest/Z-Order_Test.pdf");

static void AddRectangle(com.aspose.pdf.Page page, float x, float y, float width, float height, com.aspose.pdf.Color color, int zindex)
{
    // create graph object with dimensions same as specified for Rectangle object
    com.aspose.pdf.drawing.Graph graph = new com.aspose.pdf.drawing.Graph(width, height);
    // can we change the position of graph instance
    graph.setChangePosition(false);
    // set Left coordinate position for Graph instance
    graph.setLeft(x);
    // set Top coordinate position for Graph object
    graph.setTop(y);
    // Add a rectangle inside the "graph"
    com.aspose.pdf.drawing.Rectangle rect = new com.aspose.pdf.drawing.Rectangle(0, 0, width, height);
    // set rectangle fill color
    rect.getGraphInfo().setFillColor(color);
    // color of graph object
    rect.getGraphInfo().setColor(color);
    // add rectangle to shapes collection of graph instance
    graph.getShapes().add(rect);
    // set Z-Index for rectangle object
    graph.setZIndex(zindex);
    // add graph to paragraphs collection of page object
    page.getParagraphs().add(graph);
} 
```

## Add transparent Text in PDF

A PDF file contains Image, Text, Graph, attachment, Annotations objects and while creating TextFragment, you can set foreground, background color information as well as text formatting. Aspose.Pdf for Java supports the feature to add text with Alpha color channel.

```
// instantiate Document class object
Document doc1 = new Document();
/// add page to pages collection of PDF file
com.aspose.pdf.Page page1 = doc1.getPages().add();

// create Graph object
com.aspose.pdf.drawing.Graph canvas = new com.aspose.pdf.drawing.Graph(100, 400);
// create rectangle instance with certain dimensions
com.aspose.pdf.drawing.Rectangle rect = new com.aspose.pdf.drawing.Rectangle(100, 100, 400, 400);
// create color object from Alpha color channel
rect.getGraphInfo().setFillColor(com.aspose.pdf.Color.fromArgb(255,0, 0, 64));

// add rectanlge to shapes collection of Graph object
canvas.getShapes().add(rect);
// add graph object to paragraphs collection of page object
page1.getParagraphs().add(canvas);
// set value to not change position for graph object
canvas.setChangePosition(false);

// create TextFragment instance with sample value
TextFragment text = new TextFragment("transparent text transparent text transparent text transparent text transparent text transparent text transparent text transparent text transparent text transparent text transparent text transparent text transparent text transparent text transparent text transparent text ");
// create color object from Alpha channel
com.aspose.pdf.Color color = com.aspose.pdf.Color.fromArgb(30, 0, 255, 0);
// set color information for text instance
text.getTextState().setForegroundColor(color);
// add text to paragraphs collection of page instance
page1.getParagraphs().add(text);
// save PDF file
doc.save("c:/Transparent_Text.pdf");
```

## Miscellaneous fixes

As well as the enhancements and features discussed above, there have been specific improvements regarding PDF to HTML, HTML to PDF conversion features, multi-threading, PDF to TIFF, TIFF to PDF conversion, conversion of PDF to PDF/A compliant documents, text replacement, rendering PDF files to XPS format, are also improved. Please download and try the latest release of [Aspose.PDF for Java 11.3.0][2].




[1]: https://downloads.aspose.com/pdf/java
[2]: https://downloads.aspose.com/pdf/java





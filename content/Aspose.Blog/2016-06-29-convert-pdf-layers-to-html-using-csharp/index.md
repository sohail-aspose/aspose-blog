---
title: 'Convert PDF Layers to HTML using C#'
date: Wed, 29 Jun 2016 03:04:25 +0000
draft: false
url: /2016/06/29/convert-pdf-layers-to-html-using-csharp/
author: Tilal Ahmad
summary: ''
tags: []
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/aspose-Pdf-for-net.png" alt="">}}


We are pleased to announce new version of Aspose.PDF for .NET. [Aspose.PDF for .NET 11.7.0][1] includes number of new features and improvements. It introduced PDF document layers support in HTML conversion, new dash line style of Graph objects and some other features.  We have also improved the XPS to PDF conversion performance in this release. Along with above stated new features and improvements this release fixes number of issues, reported by our customers in previous releases. Some of these are PDF to HTML, HTML to PDF, rendering of XFA form to Static form, use of OTF fonts in HtmlFragment. Please check release notes of Aspose.Pdf for .NET 11.7.0 for complete list.

The following sections describe some details regarding these newly added features/enhancements.

## Convert PDF Layers to HTML using C#

A PDF document can contain different data layers and can have requirement to render each layer separately in Layer element. We have introduced this feature in new release, now you can use **ConvertMarkedContentToLayers** property to control the layers rendering in PDF to HTML conversion.

```
// Open the PDF file

Document doc = new Document(“input.pdf”);

// Instantiate HTML SaveOptions object

HtmlSaveOptions htmlOptions = new HtmlSaveOptions();

// Specify to render PDF document layers separately in output HTML

htmlOptions.ConvertMarkedContentToLayers = true;

// Save the document

doc.Save(“output.html”, htmlOptions);
```

## AutoFitToWindows Value in ColumnAdjustment Type Enum

We have introduced a new value AutoFitToWindows in ColumnAdjustment Type Enum. It will adjust table columns to fit to windows.

```
//Instntiate the Pdf object by calling its empty constructor

Document doc = new Document();

//Create the section in the Pdf object

Page sec1 = doc.Pages.Add();

//Instantiate a table object

Aspose.Pdf.Table tab1 = new Aspose.Pdf.Table();

//Add the table in paragraphs collection of the desired section

sec1.Paragraphs.Add(tab1);

//Set with column widths of the table

tab1.ColumnWidths = “50 50 50”;

tab1.ColumnAdjustment = ColumnAdjustment.AutoFitToWindow;

//Set default cell border using BorderInfo object

tab1.DefaultCellBorder = new Aspose.Pdf.BorderInfo(Aspose.Pdf.BorderSide.All, 0.1F);

//Set table border using another customized BorderInfo object

tab1.Border = new Aspose.Pdf.BorderInfo(Aspose.Pdf.BorderSide.All, 1F);

//Create MarginInfo object and set its left, bottom, right and top margins

Aspose.Pdf.MarginInfo margin = new Aspose.Pdf.MarginInfo();

margin.Top = 5f;

margin.Left = 5f;

margin.Right = 5f;

margin.Bottom = 5f;

//Set the default cell padding to the MarginInfo object

tab1.DefaultCellPadding = margin;

//Create rows in the table and then cells in the rows

Aspose.Pdf.Row row1 = tab1.Rows.Add();

row1.Cells.Add(“col1”);

row1.Cells.Add(“col2”);

row1.Cells.Add(“col3”);

Aspose.Pdf.Row row2 = tab1.Rows.Add();

row2.Cells.Add(“item1”);

row2.Cells.Add(“item2”);

row2.Cells.Add(“item3”);

//Save the Pdf

doc.Save(“ResultantFile.pdf”);
```

## Dash Line Style of Graph Objects

Sometimes we have requirement to create a Graph Object with dashed line. Now, we can easily achieve the requirement with GraphInfo object, as following.

```
// instantiate Document instance

Document doc = new Document();

// add page to pages collection of Document object

Page page = doc.Pages.Add();

// create Drawing object with certain dimensions

Aspose.Pdf.Drawing.Graph canvas = new Aspose.Pdf.Drawing.Graph(100, 400);

// add drawing object to paragraphs collection of page instance

page.Paragraphs.Add(canvas);

// create Line object

Aspose.Pdf.Drawing.Line line = new Aspose.Pdf.Drawing.Line(new float[] { 100, 100, 200, 100 });

// set color for Line object

line.GraphInfo.Color = Aspose.Pdf.Color.Red;

// specify dash array for line object

line.GraphInfo.DashArray = new int[] { 0, 1, 0 };

// set the dash phase for Line instance

line.GraphInfo.DashPhase = 1;

// add line to shapes collection of drawing object

canvas.Shapes.Add(line);

// save PDF document

doc.Save(“DashLineInBlack.pdf”);
```

## Enhancements

Following is a list of improvements included in this release.

*   Improve XPS to PDF conversion performance
*   Improve quality of image inserted to PDF document

## Aspose.PDF for .NET Resources

The following resources will help you work with Aspose.Pdf for .NET:

*   [Home page for Aspose.PDF for .NET][2]
*   [Download Aspose.PDF for .NET][3]
*   [Aspose.PDF product family forum][4] – Post your technical questions and queries, or any other problem you faced while running Aspose.Pdf APIs.
*   Aspose.PDF for .NET online documentation – help documentation.
*   [Aspose.PDF for .NET online API reference][5] - API reference documents.
*   [Enable Blog Subscription][6] – Do not limit yourself, you can keep yourself updated with the latest news on Aspose.Pdf APIs, new features, fixes and other API related topics by subscribing to Aspose.PDF blog.
*   [Aspose.PDF for .NET Examples][7] – We have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: https://products.aspose.com/pdf/net
[2]: https://products.aspose.com/pdf/net
[3]: https://downloads.aspose.com/pdf/net
[4]: http://forum.aspose.com
[5]: https://apireference.aspose.com/pdf/net
[6]: https://blog.aspose.com/
[7]: https://github.com/aspose-pdf/Aspose.Pdf-for-.NET





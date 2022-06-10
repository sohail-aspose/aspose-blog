---
title: 'Convert an Excel Chart To Image'
date: Thu, 17 May 2007 12:00:00 +0000
draft: false
url: /2007/05/17/convert-an-excel-chart-to-image/
author: Laurence
summary: ''
tags: ['Convert an Excel Chart To Image', 'Export Excel Chart to Image']
categories: ['Aspose.Cells Product Family']
---

## Purpose

This document is designed to provide the developers with a detailed understanding on how an excel chart can be exported as an image.

## Introduction

**Charts** are visually appealing and make it easy for users to see comparisons, patterns, and trends in data. For instance, rather than having to analyze several columns of worksheet numbers, you can see at a glance whether sales are falling or rising over quarterly periods, or how the actual sales compare to the projected sales.

Sometimes, you do need to present the chart in your applications or web pages. You might need to insert it into a Word Document, a PDF file, a Power Point Presentation or in some other scenario. Simply you want the chart should be rendered as an image, so that you may paste it into your applications with ease. A **Picture** is worthwhile. Frequently, in the course of work, one has to present statistical and graphical information in an easy to understand and an easy to maintain manner.

You might try **Office Automation** but Office automation has its own drawbacks. There are several reasons and issues involved: E.g., Security, Stability, Scalability/Speed, Price, Features etc.  In Short, there are many reasons, with the top one being that Microsoft themselves strongly recommends against Office automation from software solutions。

There is another option which you can use to convert an Excel Chart to an image using [Aspose.Cells][1]. This is a brand new feature offered by **Aspose.Cells** which is more advanced and of the essence from many of its [Features List][2].  In this article, we create some console applications in Visual Studio.Net, that will convert the Excel Charts to render the image files with a few and simplest lines of code using [Aspose.Cells API][3]. The conversion is performed with precision and accuracy.

## Aspose.Cells:  The Real Product

I would take this opportunity to introduce the product to you. **Aspose.Cells** is an Excel® spreadsheet reporting component that enables you to read and write Excel® spreadsheets without utilizing Microsoft Excel® installed either on the client or server side. **Aspose.Cells** is a very feature rich component that offers much more than just basic exporting of data. With **Aspose.Cells** developers can export data, format spreadsheets in every detail and at every level, import images, import charts, create charts, manipulate charts, stream Excel® data, save in various formats including XLS, CSV, SpreadsheetML, TabDelimited, TXT, XML ([Aspose.PDF][4] integrated) and many more. All the [Aspose][5] components are totally independent and are not affiliated with, nor authorized, sponsored by **Microsoft Corporation**. To know more about the product information, features and for a programmer’s guide, check [Aspose.Cells Decumentation][6] and online featured demos. You may [download][7] its evaluation version for free.

## Performing the Task

For the demonstration, I choose some common tasks here. I have created two charts (a pie chart and a column chart) in MS Excel and covert these charts to image files using the simplest API of **Aspose.Cells** with a few lines of code. For conversion we shall create two console applications.

Following is the task list:

*   **Converting a Pie Chart to an Image File.**
*   **Converting a Column Chart to an Image File.**

## Converting a Pie Chart to an Image File

First we create a pie chart in MS Excel and next we convert the chart to an image file.

### Creating a Pie Chart in MS Excel

I opened a new workbook in MS Excel and input some sales data of the different regions into a worksheet. I, then, created a pie chart based on the data and save the excel file.

### Converting Chart2Image

Now I convert the chart to an image file.

## Download and Install Aspose.Cells

First, you need to [download][8] **Aspose.Cells** for .Net. Install it on your development computer. All [Aspose][9] components, when installed, work in evaluation mode. The evaluation mode has no time limit and it only injects watermarks into produced documents.

## Create a Project

Start Visual Studio. Net and create a new console application. This example will show a C# console application, but you can use VB.NET too.

## Add References

This project will use **Aspose.Cells**. So, you have to add reference to **Aspose.Cells** component in your project. E.g., add a reference to ….\\Program Files\\Aspose\\Aspose.Cells\\Bin\\Net1.0\\Aspose.Cells.dll.

## Code Snippet

Following is the actual code (Written in C#) used by the component to accomplish the task. You may see that very few lines of code are used to accomplish the task.

```
//Create a new workbook.

Aspose.Cells.Workbook workbook = new Aspose.Cells.Workbook();

//Open the existing excel file which contains the pie chart.

workbook.Open("d:\\piechart.xls");

//Get the designer chart (first chart) in the first worksheet.

//of the workbook.

Chart chart = workbook.Worksheets[0].Charts[0];

//Convert the chart to an image file.

System.Drawing.Bitmap bitmap = chart.ToImage();

//Save the chart image (jpg) file to disk.

bitmap.Save(@"d:\PieChart.jpg",System.Drawing.Imaging.ImageFormat.Jpeg);

Additionally I write its parallel VB.NET code here for your convenience:

'Create a new workbook.

Dim workbook As Aspose.Cells.Workbook = New Aspose.Cells.Workbook()

'Open the existing excel file which contains the pie chart.

workbook.Open("d:\piechart.xls");

'Get the designer chart (first chart) in the first worksheet.

'of the workbook.

Dim chart As Chart = workbook.Worksheets(0).Charts(0)

'Convert the chart to an image file.

Dim bitmap As System.Drawing.Bitmap = chart.ToImage()

'Save the chart image (jpg) file to disk.

bitmap.Save("d:\PieChart.jpg",System.Drawing.Imaging.ImageFormat.Jpeg)
```

After executing the above code, a jpg file is created based on the pie chart in the template excel file. Here is the screenshot of the output file:

## **Converting a Column Chart to an Image File**

First we create a column chart in MS Excel and next we convert the chart to an image file as we did it before.

## Creating a Column Chart in MS Excel

I opened a new workbook in MS Excel and input some marketing costs of the different regions into a worksheet. I, then, created a column chart based on the data and save the excel file. Following is the screenshot of the file created in MS Excel: 

## Converting Chart2Image

Now I convert the chart to an image file. I‘ll skip the conventional steps here like creating a new project in Visual Studio.NET or adding reference to Aspose.Cells.dll file. I already did it in the first task. I only write here the actual code with the presentation of the output image file.

## Code Snippet

Following is the actual code (Written in C#) used by the component to accomplish the task. The code is similar to the previous one:

```
//Create a new workbook.

Aspose.Cells.Workbook workbook = new Aspose.Cells.Workbook();

//Open the existing excel file which contains the column chart.

workbook.Open("d:\\columnchart.xls");

//Get the designer chart (first chart) in the first worksheet.

//of the workbook.

Chart chart = workbook.Worksheets[0].Charts[0];

//Convert the chart to an image file.

System.Drawing.Bitmap bitmap = chart.ToImage();

//Save the chart image (jpg) file to disk.

bitmap.Save(@"d:\ColumnChart.jpg",System.Drawing.Imaging.ImageFormat.Jpeg);

Additionally I write its parallel VB.NET code here for your convenience:

'Create a new workbook.

Dim workbook As Aspose.Cells.Workbook = New Aspose.Cells.Workbook()

'Open the existing excel file which contains the column chart.

workbook.Open("d:\columnchart.xls");

'Get the designer chart (first chart) in the first worksheet.

'of the workbook.

Dim chart As Chart = workbook.Worksheets(0).Charts(0)

'Convert the chart to an image file.

Dim bitmap As System.Drawing.Bitmap = chart.ToImage()

'Save the chart image (jpg) file to disk.

bitmap.Save("d:\ColumnChart.jpg",System.Drawing.Imaging.ImageFormat.Jpeg)
```

After executing the above code, a jpg file is created based on the column chart in the template excel file. Here is the screenshot of the output file:

## Summary

In this article I have presented how can we convert an excel chart to render an image file using **Aspose.Cells** component. Hopefully, it will give you some insight, and you will be able to utilize it some scenarios. Since the Chart2Image feature was really demanding and required by some of [Aspose][10] customers. And this is the result of some workout by [Aspose.Cells Product Team][11]. The feature is still young, so there might be some precision and accuracy issues occurred in some cases. We are working to enhance the conversion to make it more elegant and sophisticated and will mend any deficiency if found to strengthen it more.

**Aspose.Cells** can offer more flexibility than others for solutions and provides outstanding speed, efficiency and reliability to meet specific business application requirements. The results do show that **Aspose.Cells** has benefited from years of research, design and careful tuning.

We heartily welcome your queries, comments and suggestions at [Aspose.Cells Forum][12]. We warranty a prompt reply within minutes or hours, Thank you!

[Aspose -  The .NET & Java component publisher][13]




[1]: https://products.aspose.com/cells
[2]: https://products.aspose.com/cells
[3]: https://products.aspose.com/cells
[4]: https://products.aspose.com/pdf
[5]: https://www.aspose.com/
[6]: https://docs.aspose.com/display/cellsproductfamily
[7]: https://downloads.aspose.com/cells
[8]: https://downloads.aspose.com/cells
[9]: http://www.aspose.com
[10]: http://www.aspose.com
[11]: https://products.aspose.com/cells
[12]: https://forum.aspose.com/
[13]: https://products.aspose.com/





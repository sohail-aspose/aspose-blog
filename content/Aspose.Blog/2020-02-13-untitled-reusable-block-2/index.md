---
title: 'Untitled Reusable Block'
seoTitle: ""
description: ""
date: Thu, 13 Feb 2020 17:12:32 +0000
draft: false
url: /2020/02/13/untitled-reusable-block-2/
author: Usman Aziz
summary: ''
---

//Create a new workbook.  

Aspose.Cells.Workbook workbook = new Aspose.Cells.Workbook();  

//Open the existing excel file which contains the pie chart.  

workbook.Open("d:\\\\piechart.xls");  

//Get the designer chart (first chart) in the first worksheet.  

//of the workbook.  

Chart chart = workbook.Worksheets\[0\].Charts\[0\];  

//Convert the chart to an image file.  

System.Drawing.Bitmap bitmap = chart.ToImage();  

//Save the chart image (jpg) file to disk.  

bitmap.Save(@"d:\\PieChart.jpg",System.Drawing.Imaging.ImageFormat.Jpeg);  

Additionally I write its parallel VB.NET code here for your convenience:  

'Create a new workbook.  

Dim workbook As Aspose.Cells.Workbook = New Aspose.Cells.Workbook()  

'Open the existing excel file which contains the pie chart.  

workbook.Open("d:\\piechart.xls");  

'Get the designer chart (first chart) in the first worksheet.  

'of the workbook.  

Dim chart As Chart = workbook.Worksheets(0).Charts(0)  

'Convert the chart to an image file.  

Dim bitmap As System.Drawing.Bitmap = chart.ToImage()  

'Save the chart image (jpg) file to disk.

bitmap.Save("d:\\PieChart.jpg",System.Drawing.Imaging.ImageFormat.Jpeg)








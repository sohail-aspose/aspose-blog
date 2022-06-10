---
title: '12th Wonder Uses Aspose.Cells to Extract PDF from Excel File'
date: Thu, 06 Sep 2018 04:16:45 +0000
draft: false
url: /2018/09/06/12th-wonder-uses-aspose.cells-to-extract-pdf-from-excel-file/
author: Sabrinatran
summary: ''
tags: []
categories: ['Aspose.Cells Product Family']
---

12th Wonder specializes in creating solutions to solve complex business problems. We had to provide a solution for displaying complex excel documents within an ASP.Net MVC application. We tried many solutions including writing custom code to convert excel to pdf, but we figured out the effort to maintain custom code is very high. So we decided to do a POC using Aspose.Cells product.

The formatting and layout of the excel file that we wanted to display as a PDF document within our MVC application were really complex and immutable. The excel sheet has multiple worksheets and each sheet contains 5 or more pages laid out side by side.  While displaying the excel sheet as pdf, we converted each worksheet into a separate document, with each document having a variable number of pages. The Excel also contains plain text, images, text boxes, custom formats such as double borders, strikeout cells, and different font styles. The fidelity of the generated pdf is really critical.

Please see below for a screenshot of a single page from the uploaded excel file.



{{< figure align=center src="images/AsposeExcel.png" alt="">}}


The sample code below is used to read the first page from the first worksheet in the uploaded excel file using the excellent Aspose.Cells library.

The first step is to initialize the Aspose.Cells object using the code below

```
//Load your Excel file

Aspose.Cells.Workbook wb = new Aspose.Cells.Workbook(“<Specify your file path>”);
```

The library has multiple overloaded methods that make it easy to read a specific worksheet.  The worksheet can be read either with the index of the worksheet or by the name of the worksheet.

```
//Access the worksheet

Aspose.Cells.Worksheet sourceSheet = wb.Worksheets[“<give the worksheet name>”];

To read the range in the selected worksheet, in my case I am reading from A4 to AE52.

//Read the range from Cell A4 to Cell AE 52

sourceSheet.PageSetup.PrintArea = “A4:AE52”;
```

After setting all the custom properties Aspose.Cells product will do the job and covert the specified range spreadsheet into PDF file.  Use the following code to generate the pdf file

```
//Save to Pdf – one page per sheet true

Aspose.Cells.PdfSaveOptions pdfSaveOptions = new Aspose.Cells.PdfSaveOptions();

pdfSaveOptions.OnePagePerSheet = true;

pdfSaveOptions.PageIndex = sourceSheet.Index;

pdfSaveOptions.PageCount = 1;

wb.Save(destFilePath + “_” + DateTime.Now.ToShortDateString() + “.pdf”, pdfSaveOptions);
```

Here is my output file, after generating PDF file.



{{< figure align=center src="images/AsposePdf.png" alt="">}}


Visually, there is no difference between the uploaded excel and the generated PDF page.

Please see below for the complete source code



{{< figure align=center src="images/AsposePdfCode.png" alt="">}}


Aspose.Cells is an excellent library to convert excel to pdf. We had no problems in completing the POC in less than a day.









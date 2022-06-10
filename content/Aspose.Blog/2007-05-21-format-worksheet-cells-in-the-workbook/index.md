---
title: 'Format Worksheet Cells in the Workbook'
date: Mon, 21 May 2007 00:16:00 +0000
draft: false
url: /2007/05/21/format-worksheet-cells-in-the-workbook/
author: Laurence
summary: ''
tags: ['Format Cells in Excel Worksheet', 'Format Cells in Excel in .NET']
categories: ['Aspose.Cells Product Family']
---

**Purpose**

This article is designed to provide the developers with a detailed perceptive on how to create a workbook to input data into a worksheet and apply some formatting to the cells in the rows and columns of the worksheet using [Aspose.Cells][1] component.

**In this Article**

Here is a quick look what the article is all about:

Working with Worksheet Formatting

*   Using Styles to quickly Format data

*   Formatting Cells in Rows and Columns

*   Using Borders and Colors to emphasize data

*   Applying Number Formats to carry more weight to data

*   Using Fonts and Attributes to bring data to light

*   Formatting data in a named Range of Cells

*   Changing the Alignment Setting and Orientation of data

*   Setting Row height and Column width to adjust the contents

**Data Formatting**

To distinguish between different types of information on a worksheet, for the optimal display of the data on your worksheet and to make a worksheet easier to scan, you do format the worksheet. A **Format** represents a style and is defined as a set of characteristics, such as fonts and font sizes, number formats, cell borders, cell shading with solid background color or a specific color pattern, indentation, alignment and text orientation in the cells.  

For enhanced visibility to draw attention to specific data and to give your worksheet a professional look you should choose the right combination of fonts, font styles, size, color and other attributes which can make your data or numbers in the cells jump right off the worksheet. Similarly, borders provide you further ways to highlight information in the cells in a Worksheet. A **Border** is a line drawn around a cell or a group of cells. There is another way called Number Formats, which is also used to make your data more meaningful. By applying different Number Formats, you can change the appearance of numbers without changing the number behind the appearance.  

You might try **Office Automation** for itbut Office automation has its own drawbacks. There are several reasons and issues involved: E.g., Security, Stability, Scalability/Speed, Price, Features etc. In Short, there are many reasons, with the top one being that Microsoft themselves strongly recommends against Office automation from software solutions. You come across different solutions / components in the market with the assertion of performing the tasks. But the question is whether the component (you choose) can really perform the tasks with excellence. You might be looking at the component’s speed to perform the tasks, performance in the diverse environment, and quality of the results and more importantly reliability related your scenarios.

I use [Aspose.Cells][2] for the tasks mentioned above. **Aspose.Cells** provides you the flexibility and feasibility to draw borders around cells and range of cells with ease. Moreover the component is well versed to apply fonts with attributes and shade the cells. The component is efficient enough that you can format a complete row or column, set alignments, wrap and rotate the text in the cells. **Aspose.Cells** supports to apply all types of Number Formats including General format, numbers in Decimal notations, numbers with Currency symbols, numbers as a Percentage of 100, numbers in Scientific format, numbers in DateTime values and Custom Number format.

In this article, we create a console application in Visual Studio.NET that will generate the annual **Sales** **Report**. We create a workbook from the scratch; insert data into cells in a worksheet first related the report and finally format the worksheet in it using [Aspose.Cells API][3].

**Aspose.Cells :  The Real Product**

I would take this opportunity to introduce the product to you. **Aspose.Cells** is an Excel® spreadsheet reporting component that enables you to read and write Excel® spreadsheets without utilizing Microsoft Excel® to be installed either on the client or server side. **Aspose.Cells** is a very feature rich component that offers much more than just basic exporting of data. With **Aspose.Cells** developers can export data, format spreadsheets in every detail and at every level, import images, import charts, create charts, manipulate charts, stream Excel® data, save in various formats including XLS, CSV, SpreadsheetML, TabDelimited, TXT, XML ([Aspose.Pdf][4] integrated) and many more. All the [Aspose][5] components are totally independent and are not affiliated with, nor authorized, sponsored by **Microsoft Corporation**. **Aspose.Cells** has a huge list of features. To know more about the product information, features and for a programmer’s guide, please check its summary of [Features List][6] , [Aspose.Cells Decumentation][7] and online featured [demos][8].  So I strongly recommend you and invite you to try the component one time at least and see the difference. You can try its evaluation version; it is totally free without any time limitation what so ever. You may [download][9] its evaluation version for free.

**Performing the Tasks**

For demonstration, I develop a simple console application which creates an excel workbook from the scratch (you may utilize template file and format its data too.), insert sales data into the first worksheet in the excel book, format data into the cells and save the excel report file. I exhibit all the underlying formatting tasks using the simplest **API** of **Aspose.Cells**.

**Format Cells in Rows and Columns**

Below are the steps involved how to create a spreadsheet and format different cells in different rows and columns of a worksheet.

##### Download and Install Aspose.Cells

First of all, you need to [download][10] **Aspose.Cells** for .Net. Install it on your development computer. All [Aspose][11] components, when installed, work in the evaluation mode. The evaluation mode has no time limit and it only injects watermarks into produced documents.

##### Create a Project

Start Visual Studio. Net and create a new console application. This example will show a **C#** console application, but you can use **VB.NET** too.

##### Add References

This project will use **Aspose.Cells**. So, you have to add reference to **Aspose.Cells** component in your project. E.g., add a reference to ….\\Program Files\\Aspose\\Aspose.Cells\\Bin\\Net1.0\\Aspose.Cells.dll

**Code Snippet**

Following is the actual code (Written in **C#**) used by the component to accomplish the tasks. You may see how **Aspose.Cells** feature rich **API** can be used to accomplish the underlying tasks. To understand you in a better way, comments are embedded with each line of code.

```
//——————————————————————–

//— AsposeFormatWorksheet

//— A Console Application which describes how to format a worksheet.

//—

//— The Application creates a workbook from the scratch, input some

//— data into a worksheet and apply formatting to the cells in the

//— rows and columns of the worksheet.

//—

//— © Aspose 2007. All rights reserved.

//— Support: http://www.aspose.com/Community/forums/

//—

//——————————————————————–

using System;

using System.Drawing;

using Aspose.Cells;

 

namespace AsposeFormatWorksheet

{

    /// <summary>

    /// AsposeFormatWorksheet

    /// Use Aspose.Cells to perform the task

    /// </summary>

    class Class1

    {

       /// <summary>

       /// The main entry point for the application.

       /// </summary>

       [STAThread]

       static void Main(string[] args)

       {

           string fileName = @”D:\FormatWorksheet.xls”;

           CreateSalesReport(fileName);

          

       }

      

       private static void CreateSalesReport(string fileName)

       {

       // Uncomment the code below when you have purchased license

       // for Aspose.Cells. You need to deploy the license in the

       // same folder as your executable, alternatively you can add

       // the license file as an embedded resource to your project.

       //

       // // Set license for Aspose.Cells

       // Aspose.Cells.License cellsLicense = new

       // Aspose.Cells.License();

       // cellsLicense.SetLicense(“Aspose.Cells.lic”);

          

 

      //Create a new Workbook.

       Workbook workbook = new Workbook();

//Open a template file with data

       Workbook.Open(fileName);

       //Note: Since Excel color palette has 56 colors on it.

       //The colors are indexed 0-55.

       //Please check: http://www.aspose.com/Products/Aspose.Cells/Api/Aspose.Cells.Workbook.ChangePalette.html

       //If a color is not present on the palette, we have to add it

       //to the palette, so that we may use.

       //Add a few custom colors to the palette.

       workbook.ChangePalette(Color.FromArgb(155,204,255),55);

       workbook.ChangePalette(Color.FromArgb(0,51,105),54); 

       workbook.ChangePalette(Color.FromArgb(250,250,200),53);

       workbook.ChangePalette(Color.FromArgb(124,199,72),52);

          

       CreateCellsFormatting(workbook);

          

       //Get the first worksheet in the book.

       Worksheet worksheet = workbook.Worksheets[0];

       //Name the worksheet.

       worksheet.Name = “Sales Report”;

       //Save the excel file.

       workbook.Save(fileName);

            

      

       }

   

   

       private static void CreateCellsFormatting(Workbook workbook)

       {

          

           //Define a style object adding a new style

           //to the collection list.

           Style stl0 = workbook.Styles[workbook.Styles.Add()];

           //Set a custom shading color of the cells.

           stl0.ForegroundColor = Color.FromArgb(155,204,255);

           //Set the solid background fillment.

           stl0.Pattern = BackgroundType.Solid;

           //Set a font.

           stl0.Font.Name = “Trebuchet MS”;

           //Set the size.

           stl0.Font.Size = 18; 

           //Set the font text color.

           stl0.Font.Color = Color.Maroon;

           //Set it bold

           stl0.Font.IsBold = true;

           //Set it italic.

           stl0.Font.IsItalic = true;

           //Define a style flag struct.

           StyleFlag flag = new StyleFlag();

           //Apply cell shading.

           flag.CellShading = true;

           //Apply font.

           flag.FontName = true;

           //Apply font size.

           flag.FontSize = true;

           //Apply font color.

           flag.FontColor = true;

           //Apply bold font.

           flag.FontBold = true;

           //Apply italic attribute.

           flag.FontItalic = true;

           //Get the first row in the first worksheet. 

           Row row = workbook.Worksheets[0].Cells.Rows[0];

           //Apply the style to it.

           row.ApplyStyle(stl0,flag);

 

           //Obtain the cells of the first worksheet.

           Cells cells = workbook.Worksheets[0].Cells;

           //Set the height of the first row.

           cells.SetRowHeight(0,30); 

 

           //Define a style object adding a new style

           //to the collection list.

           Style stl1 = workbook.Styles[workbook.Styles.Add()];

           //Set the rotation angle of the text.

           stl1.Rotation = 45;

           //Set the custom fill color of the cells.

           stl1.ForegroundColor = Color.FromArgb(0,51,105);

           //Set the solid background pattern for fillment.

           stl1.Pattern = BackgroundType.Solid;

           //Set the left border line style.

           stl1.Borders[BorderType.LeftBorder].LineStyle = CellBorderType.Thin;

           //Set the left border line color.

           stl1.Borders[BorderType.LeftBorder].Color = Color.White;  

           //Set the horizontal alignment to center aligned.

           stl1.HorizontalAlignment = TextAlignmentType.Center;

           //Set the vertical alignment to center aligned.

           stl1.VerticalAlignment = TextAlignmentType.Center;

           //Set the font.

           stl1.Font.Name = “Times New Roman”;

           //Set the font size.

           stl1.Font.Size = 10; 

           //Set the font color.

           stl1.Font.Color = Color.White;

           //Set the bold attribute.

           stl1.Font.IsBold = true;

           //Set the style flag struct. 

           flag = new StyleFlag();

           //Apply the left border.

           flag.LeftBorder = true;

           //Apply text rotation orientation.

           flag.Rotation  = true;

           //Apply fill color of cells.

           flag.CellShading = true;

           //Apply horizontal alignment.

           flag.HorizontalAlignment = true;

           //Apply vertical alignment.

           flag.VerticalAlignment = true;

           //Apply the font.

           flag.FontName = true;

           //Apply the font size.

           flag.FontSize = true;

           //Apply the font color.

           flag.FontColor = true;

           //Apply the bold attribute.

           flag.FontBold = true;

           //Get the second row of the first worksheet.

           row = workbook.Worksheets[0].Cells.Rows[1];

           //Apply the style to it.

           row.ApplyStyle(stl1,flag);

 

           //Set the height of the second row.

           cells.SetRowHeight(1,48);

 

           //Define a style object adding a new style

           //to the collection list.

           Style stl2 = workbook.Styles[workbook.Styles.Add()];

           //Set the custom cell shading color.

           stl2.ForegroundColor = Color.FromArgb(155,204,255);

           //Set the solid background pattern for fillment color.

           stl2.Pattern = BackgroundType.Solid;

           //Set the font.

           stl2.Font.Name = “Trebuchet MS”;

           //Set the font color.

           stl2.Font.Color = Color.Maroon;

           //Set the font size.

           stl2.Font.Size = 10;

           //Set the style flag struct.

           flag = new StyleFlag();

           //Apply cell shading.

           flag.CellShading = true;

           //Apply the font.

           flag.FontName = true;

           //Apply the font color.

           flag.FontColor = true;

           //Apply the font size.

           flag.FontSize = true;

           //Get the first column in the first worksheet.

           Column col = workbook.Worksheets[0].Cells.Columns[0];

           //Apply the style to it.

           col.ApplyStyle(stl2,flag);

          

           //Define a style object adding a new style

           //to the collection list.

           Style stl3 = workbook.Styles[workbook.Styles.Add()];  

           //Set the custom cell filling color.

           stl3.ForegroundColor  = Color.FromArgb(124,199,72);

           //Set the solid background pattern for fillment color.

           stl3.Pattern = BackgroundType.Solid;

           //Apply the style to A2 cell.

           cells[“A2”].Style = stl3;  

      

           //Define a style object adding a new style

           //to the collection list.

           Style stl4 = workbook.Styles[workbook.Styles.Add()];

           //Set the custom font text color.

           stl4.Font.Color=  Color.FromArgb(0,51,105);

           //Set the bottom border line style.

           stl4.Borders[BorderType.BottomBorder].LineStyle = CellBorderType.Thin;

           //Set the bottom border line color to custom color.

           stl4.Borders[BorderType.BottomBorder].Color  = Color.FromArgb(124,199,72);

           //Set the background fill color of the cells.

           stl4.ForegroundColor = Color.White;

           //Set the solid fillcolor pattern.

           stl4.Pattern = BackgroundType.Solid;

           //Set custom number format.

           stl4.Custom = “$#,##0.0”;

           //Set a style flag struct.

           flag = new StyleFlag();

           //Apply font color.

           flag.FontColor = true;

           //Apply cell shading color.

           flag.CellShading = true;

           //Apply custom number format.

           flag.NumberFormat = true;

           //Apply bottom border.

           flag.BottomBorder = true;

          

           //Define a style object adding a new style

           //to the collection list.

           Style stl5 = workbook.Styles[workbook.Styles.Add()];

           //Set the bottom borde line style.

           stl5.Borders[BorderType.BottomBorder].LineStyle = CellBorderType.Thin;

           //Set the bottom border line color.

           stl5.Borders[BorderType.BottomBorder].Color  = Color.FromArgb(124,199,72);

           //Set the custom shading color of the cells.

           stl5.ForegroundColor = Color.FromArgb(250,250,200);

           //Set the solid background pattern for fillment color.

           stl5.Pattern = BackgroundType.Solid;

           //Set custom number format.

           stl5.Custom = “$#,##0.0”;

           //Set font text color.

           stl5.Font.Color= Color.Maroon;  

                           

           //Create a named range of cells (B3:M25)in the first worksheet.

           Range range = workbook.Worksheets[0].Cells.CreateRange(“B3″,”M25”);

           //Name the range.

           range.Name = “MyRange”;

           //Apply the style to cells in the named range.

           range.ApplyStyle(stl4,flag);

 

           //Apply different style to alternative rows

           //in the range.

           for (int i = 0;i<=22;i++)

           {

              for (int j=0;j<12;j++)

              {

                  if(i%2==0)

                  {

                     range[i,j].Style = stl5;

                 

                  }

             

              }

           }

          

           //Define a style object adding a new style

           //to the collection list.   

           Style stl6 = workbook.Styles[workbook.Styles.Add()];

           //Set the custom fill color of the cells.

           stl6.ForegroundColor = Color.FromArgb(0,51,105);

           //Set the background pattern for fillment color.

           stl6.Pattern = BackgroundType.Solid;

           //Set the font.

           stl6.Font.Name = “Arial”;

           //Set the font size.

           stl6.Font.Size = 10; 

           //Set the font color

           stl6.Font.Color = Color.White;

           //Set the text bold.

           stl6.Font.IsBold = true;

           //Set the custom number format.

           stl6.Custom = “$#,##0.0”; 

           //Set the style flag struct.

           flag = new StyleFlag();

           //Apply cell shading.

           flag.CellShading = true;

           //Apply the arial font.

           flag.FontName = true;

           //Apply the font size.

           flag.FontSize = true;

           //Apply the font color.

           flag.FontColor = true;

           //Apply the bold attribute.

           flag.FontBold = true;

           //Apply the number format.

           flag.NumberFormat = true;

           //Get the 26th row in the first worksheet which produces totals.

           row = workbook.Worksheets[0].Cells.Rows[25];

           //Apply the style to it.

           row.ApplyStyle(stl6,flag);

           //Now apply this style to those cells (N3:N25) which

           //has productwise sales totals.

           for (int i = 2;i<25;i++)

           {

              cells[i,13].Style = stl6;

          

           }

           //Set N column’s width to fit the contents.

           workbook.Worksheets[0].Cells.SetColumnWidth(13,9.33);   

      

       }

   

    }

}

 

 

Additionally I write its parallel VB.NET code here for your convenience:

‘——————————————————————–

‘— AsposeFormatWorksheet

‘— A Console Application which describes how to format a worksheet.

‘—

‘— The Application creates a workbook from the scratch, input some

‘— data into a worksheet and apply formatting to the cells in the

‘— rows and columns of the worksheet.

‘—

‘— © Aspose 2007. All rights reserved.

‘— Support: http://www.aspose.com/Community/forums/

‘—

‘——————————————————————–

 

Imports System

Imports System.Drawing

Imports Aspose.Cells

 

‘AsposeFormatWorksheet

‘Use Aspose.Cells to perform the task

 

Module Module1

 

    Sub Main()

        Dim fileName As String = “D:\FormatWorksheet.xls”

        CreateSalesReport(filename)

    End Sub

 

    Private Sub CreateSalesReport(ByVal fileName As String)

 

        ‘ Uncomment the code below when you have purchased license for

        ‘ Aspose.Cells. You need to deploy the license in the same folder

        ‘ as your executable, alternatively you can add the license file

        ‘ as an embedded resource to your project.

        ‘

        ‘ ‘ Set license for Aspose.Cells

        ‘ Dim cellsLicense As Aspose.Cells.License = New

        ‘ Aspose.Cells.License()

      ‘ cellsLicense.SetLicense(“Aspose.Cells.lic”)  

 

        ‘Create a new Workbook.

        Dim workbook As Workbook = New Workbook()

      ‘Open a template file with data

      workbook.Open(fileName)

        ‘Note: Since Excel color palette has 56 colors on it.

        ‘The colors are indexed 0-55.

        ‘Please check: http://www.aspose.com/Products/Aspose.Cells/Api/Aspose.Cells.Workbook.ChangePalette.html

        ‘If a color is not present on the palette, we have to add it

        ‘to the palette, so that we may use.

        ‘Add a few custom colors to the palette.

        workbook.ChangePalette(Color.FromArgb(155, 204, 255), 55)

        workbook.ChangePalette(Color.FromArgb(0, 51, 105), 54)

        workbook.ChangePalette(Color.FromArgb(250, 250, 200), 53)

        workbook.ChangePalette(Color.FromArgb(124, 199, 72), 52)

 

        CreateCellsFormatting(workbook)

 

        ‘Get the first worksheet in the book.

        Dim worksheet As Worksheet = workbook.Worksheets(0)

        ‘Name the worksheet.

        worksheet.Name = “Sales Report”

        ‘Save the excel file.

        workbook.Save(fileName)

 

    End Sub

 

 

    Private Sub CreateCellsFormatting(ByVal workbook As Workbook)

 

 

        ‘Define a style object adding a new style

        ‘to the collection list.

        Dim stl0 As Style = workbook.Styles(workbook.Styles.Add())

        ‘Set a custom shading color of the cells.

        stl0.ForegroundColor = Color.FromArgb(155, 204, 255)

        ‘Set the solid background fillment.

        stl0.Pattern = BackgroundType.Solid

        ‘Set a font.

        stl0.Font.Name = “Trebuchet MS”

        ‘Set the size.

        stl0.Font.Size = 18

        ‘Set the font text color.

        stl0.Font.Color = Color.Maroon

        ‘Set it bold

        stl0.Font.IsBold = True

        ‘Set it italic.

        stl0.Font.IsItalic = True

        ‘Define a style flag struct.

        Dim flag As StyleFlag = New StyleFlag()

        ‘Apply cell shading.

        flag.CellShading = True

        ‘Apply font.

        flag.FontName = True

        ‘Apply font size.

        flag.FontSize = True

        ‘Apply font color.

        flag.FontColor = True

        ‘Apply bold font.

        flag.FontBold = True

        ‘Apply italic attribute.

        flag.FontItalic = True

        ‘Get the first row in the first worksheet. 

        Dim row As Row = workbook.Worksheets(0).Cells.Rows(0)

        ‘Apply the style to it.

        row.ApplyStyle(stl0, flag)

 

        ‘Obtain the cells of the first worksheet.

        Dim cells As Cells = workbook.Worksheets(0).Cells

        ‘Set the height of the first row.

        cells.SetRowHeight(0, 30)

 

        ‘Define a style object adding a new style

        ‘to the collection list.

        Dim stl1 As Style = workbook.Styles(workbook.Styles.Add())

        ‘Set the rotation angle of the text.

        stl1.Rotation = 45

        ‘Set the custom fill color of the cells.

        stl1.ForegroundColor = Color.FromArgb(0, 51, 105)

        ‘Set the solid background pattern for fillment.

        stl1.Pattern = BackgroundType.Solid

        ‘Set the left border line style.

        stl1.Borders(BorderType.LeftBorder).LineStyle = CellBorderType.Thin

        ‘Set the left border line color.

        stl1.Borders(BorderType.LeftBorder).Color = Color.White

        ‘Set the horizontal alignment to center aligned.

        stl1.HorizontalAlignment = TextAlignmentType.Center

        ‘Set the vertical alignment to center aligned.

        stl1.VerticalAlignment = TextAlignmentType.Center

        ‘Set the font.

        stl1.Font.Name = “Times New Roman”

        ‘Set the font size.

        stl1.Font.Size = 10

        ‘Set the font color.

        stl1.Font.Color = Color.White

        ‘Set the bold attribute.

        stl1.Font.IsBold = True

        ‘Set the style flag struct. 

        flag = New StyleFlag()

        ‘Apply the left border.

        flag.LeftBorder = True

        ‘Apply text rotation orientation.

        flag.Rotation = True

        ‘Apply fill color of cells.

        flag.CellShading = True

        ‘Apply horizontal alignment.

        flag.HorizontalAlignment = True

        ‘Apply vertical alignment.

        flag.VerticalAlignment = True

        ‘Apply the font.

        flag.FontName = True

        ‘Apply the font size.

        flag.FontSize = True

        ‘Apply the font color.

        flag.FontColor = True

        ‘Apply the bold attribute.

        flag.FontBold = True

        ‘Get the second row of the first worksheet.

        row = workbook.Worksheets(0).Cells.Rows(1)

        ‘Apply the style to it.

        row.ApplyStyle(stl1, flag)

 

        ‘Set the height of the second row.

        cells.SetRowHeight(1, 48)

 

        ‘Define a style object adding a new style

        ‘to the collection list.

        Dim stl2 As Style = workbook.Styles(workbook.Styles.Add())

        ‘Set the custom cell shading color.

        stl2.ForegroundColor = Color.FromArgb(155, 204, 255)

        ‘Set the solid background pattern for fillment color.

        stl2.Pattern = BackgroundType.Solid

        ‘Set the font.

        stl2.Font.Name = “Trebuchet MS”

        ‘Set the font color.

        stl2.Font.Color = Color.Maroon

        ‘Set the font size.

        stl2.Font.Size = 10

        ‘Set the style flag struct.

        flag = New StyleFlag()

        ‘Apply cell shading.

        flag.CellShading = True

        ‘Apply the font.

        flag.FontName = True

        ‘Apply the font color.

        flag.FontColor = True

        ‘Apply the font size.

        flag.FontSize = True

        ‘Get the first column in the first worksheet.

        Dim col As Column = workbook.Worksheets(0).Cells.Columns(0)

        ‘Apply the style to it.

        col.ApplyStyle(stl2, flag)

 

        ‘Define a style object adding a new style

        ‘to the collection list.

        Dim stl3 As Style = workbook.Styles(workbook.Styles.Add())

        ‘Set the custom cell filling color.

        stl3.ForegroundColor = Color.FromArgb(124, 199, 72)

        ‘Set the solid background pattern for fillment color.

        stl3.Pattern = BackgroundType.Solid

        ‘Apply the style to A2 cell.

        cells(“A2”).Style = stl3

 

        ‘Define a style object adding a new style

        ‘to the collection list.

        Dim stl4 As Style = workbook.Styles(workbook.Styles.Add())

        ‘Set the custom font text color.

        stl4.Font.Color = Color.FromArgb(0, 51, 105)

        ‘Set the bottom border line style.

        stl4.Borders(BorderType.BottomBorder).LineStyle = CellBorderType.Thin

        ‘Set the bottom border line color to custom color.

        stl4.Borders(BorderType.BottomBorder).Color = Color.FromArgb(124, 199, 72)

        ‘Set the background fill color of the cells.

        stl4.ForegroundColor = Color.White

        ‘Set the solid fillcolor pattern.

        stl4.Pattern = BackgroundType.Solid

        ‘Set custom number format.

        stl4.Custom = “$#,##0.0”

        ‘Set a style flag struct.

        flag = New StyleFlag()

        ‘Apply font color.

        flag.FontColor = True

        ‘Apply cell shading color.

        flag.CellShading = True

        ‘Apply custom number format.

        flag.NumberFormat = True

        ‘Apply bottom border.

        flag.BottomBorder = True

 

        ‘Define a style object adding a new style

        ‘to the collection list.

        Dim stl5 As Style = workbook.Styles(workbook.Styles.Add())

        ‘Set the bottom borde line style.

        stl5.Borders(BorderType.BottomBorder).LineStyle = CellBorderType.Thin

        ‘Set the bottom border line color.

        stl5.Borders(BorderType.BottomBorder).Color = Color.FromArgb(124, 199, 72)

        ‘Set the custom shading color of the cells.

        stl5.ForegroundColor = Color.FromArgb(250, 250, 200)

        ‘Set the solid background pattern for fillment color.

        stl5.Pattern = BackgroundType.Solid

        ‘Set custom number format.

        stl5.Custom = “$#,##0.0”

        ‘Set font text color.

        stl5.Font.Color = Color.Maroon

 

        ‘Create a named range of cells (B3:M25)in the first worksheet.

        Dim range As Range = workbook.Worksheets(0).Cells.CreateRange(“B3”, “M25”)

        ‘Name the range.

        range.Name = “MyRange”

        ‘Apply the style to cells in the named range.

        range.ApplyStyle(stl4, flag)

 

        ‘Apply different style to alternative rows

        ‘in the range.

        Dim i As Integer

        Dim j As Integer

        For i = 0 To 22 Step 1

 

            For j = 0 To 11 Step 1

 

                If i Mod 2 = 0 Then

 

                    range(i, j).Style = stl5

 

                End If

 

            Next

 

        Next

 

        ‘Define a style object adding a new style

        ‘to the collection list.     

        Dim stl6 As Style = workbook.Styles(workbook.Styles.Add())

        ‘Set the custom fill color of the cells.

        stl6.ForegroundColor = Color.FromArgb(0, 51, 105)

        ‘Set the background pattern for fillment color.

        stl6.Pattern = BackgroundType.Solid

        ‘Set the font.

        stl6.Font.Name = “Arial”

        ‘Set the font size.

        stl6.Font.Size = 10

        ‘Set the font color

        stl6.Font.Color = Color.White

        ‘Set the text bold.

        stl6.Font.IsBold = True

        ‘Set the custom number format.

        stl6.Custom = “$#,##0.0”

        ‘Set the style flag struct.

        flag = New StyleFlag()

        ‘Apply cell shading.

        flag.CellShading = True

        ‘Apply the arial font.

        flag.FontName = True

        ‘Apply the font size.

        flag.FontSize = True

        ‘Apply the font color.

        flag.FontColor = True

        ‘Apply the bold attribute.

        flag.FontBold = True

        ‘Apply the number format.

        flag.NumberFormat = True

        ‘Get the 26th row in the first worksheet which produces totals.

        row = workbook.Worksheets(0).Cells.Rows(25)

        ‘Apply the style to it.

        row.ApplyStyle(stl6, flag)

        ‘Now apply this style to those cells (N3:N25) which

        ‘has productwise sales totals.

        For i = 2 To 24 Step 1

 

            cells(i, 13).Style = stl6

 

        Next

        ‘Set N column’s width to fit the contents.

        workbook.Worksheets(0).Cells.SetColumnWidth(13, 9.33)

 

    End Sub

 

End Module
```

After executing the above code, an excel file is generated with a formatted worksheet “Sales Report”. Here is the screenshot of the output file:

**Summary**

Worksheet Data formatting is in many ways more significant because it can change the meaning of your data. If you plan to print your worksheet, email it to your clients, or show it off to your boss, you need to think about whether your worksheet is formatted and furnished in a viewer-friendly way. A careful use of color, shading, borders, fonts, number formatting, alignment, indentation and orientation can make the difference between a messy glob of data and a worksheet that’s easy to work with and understand.

In this article I have presented how can we format data occupied into the different cells in a worksheet using **Aspose.Cells** component. Hopefully, it will give you some insight, and you will be able to utilize it some scenarios. **Aspose.Cells** can offer more flexibility than others for solutions and provides outstanding speed, efficiency and reliability to meet specific business application requirements. The results do show that **Aspose.Cells** has benefited from years of research, design and careful tuning.  

Feel free to contact [Aspose.Cells Product Team][12] which is always working to enhance the product all the time to make it more stable and sophisticated and will resolve any issue or complication if found on the spot within no time. We heartily welcome your queries, comments and suggestions at [Aspose.Cells Forum][13]. We warranty a prompt reply within minutes or hours, Thank you!




[1]: /Products/Aspose.Cells/
[2]: https://products.aspose.com/cells
[3]: https://products.aspose.com/cells
[4]: https://products.aspose.com/pdf
[5]: /
[6]: https://products.aspose.com/cells
[7]: https://docs.aspose.com/display/cellsproductfamily
[8]: https://products.aspose.com/cells
[9]: https://downloads.aspose.com/cells
[10]: https://downloads.aspose.com/cells
[11]: http://aspose.com
[12]: https://products.aspose.com/cells
[13]: http://forum.aspose.com





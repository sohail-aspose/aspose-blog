---
title: 'Aspose Customer Newsletter, December 2007'
date: Tue, 04 Dec 2007 13:48:00 +0000
draft: false
url: /2007/12/04/aspose-customer-newsletter-december-2007/
author: Salman Sarfraz
summary: ''
tags: ['Customer Newsletters']
---

**In This Issue**

*   **Welcome!**
*   **Product Spotlight – [Aspose.Pdf][1]**
*   **Aspose.BarCode makes headway**
*   **A more optimized Aspose.Slides for Java**
*   **Import and export Excel 2007 XLSX file with Aspose.Cells for Java**
*   **Aspose.Words for .NET 4.4.2.0 Released**
*   **Technical Tip – Quick migration to the latest Aspose.Slides with new tables engine**
*   **Aspose.Total for Reporting Services Mega Release**

**Welcome**

Welcome to the December 2007 issue of the Aspose Newsletter! In this month’s newsletter, we will provide some introductory information about our spotlight product: Aspose.Pdf. We will also look at the new and exciting features offered in the recent releases of Aspose.Total for Reporting Services, Aspose.Words, Aspose.Cells, Aspose.Slides and Aspose.BarCode. You will learn about the latest news from Aspose along with the monthly Tech-Tip, which demonstrates how you can quickly migrate to the latest Aspose.Slides with new tables engine.

**Product Spotlight**

[**Aspose.Pdf**][2] is a non-graphical PDF® document reporting component that enables either .NET or Java applications to create PDF documents without utilizing Adobe Acrobat®.  Aspose.Pdf is very affordably priced and offers a wealth of strong features including: compression, tables, graphs, images, hyperlinks, security and custom fonts.  Aspose.Pdf supports creation of PDF files through both an API and from XML templates and XSL-FO files.  Aspose.Pdf is very easy to use and is provided with 14 fully featured demos written in both C# and Visual Basic. Please [**download**][3] the free evaluation version of Aspose.Pdf to see how it fulfills your business needs.

**Aspose.BarCode makes headway**

The [**Aspose.BarCode**][4] line of products has made quite a few improvements. The Aspose.BarCode documentation has recently gotten a makeover. For details please visit the official **release page**. A new version of Aspose.BarCode for .NET has also been released (**details**). You can download it from [**here**][5]. A few enhancements were also made in [**Aspose.BarCode for Reporting Services**][6] which lead to the release of v1.2.0.0 (**details**). This is available for download [**here**][7].

**A more optimized Aspose.Slides for Java**

The latest version 1.8.0.0 of [**Aspose.Slides**][8] for Java has been released. The new release includes a new and optimized tables engine along with significant memory and speed optimizations for reading and writing PPT files. Among the many other new features, this release also provides the possibility to read file name of OLE1 objects and improved text rendering on slides. Also included are numerous bug fixes. The latest version can be downloaded from [**here**][9]. For more details, please visit its official **release page**.  

**Import and export Excel 2007 XLSX file with Aspose.Cells for Java**

The latest release of [**Aspose.Cells**][10] for Java v1.9.1 now supports the import and export of Excel 2007 XLSX files. Also included in this release is the support for sorting data of ranges and the ability to be used with PHP. Numerous bug fixes and improvements are also included. The latest version can be downloaded from [**here**][11]. For more information about this release please consult the official **release page**.

**Aspose.Words for .NET 4.4.2.0 Released**

[**Aspose.Words**][12] for .NET v4.4.2.0 has been released. This is a maintenance release of Aspose.Words which contains improvements and fixes to DOCX import as well as many other improvements and fixes. Please download this latest release from [**here**][13]. Form more information about this release please consult the official **release page**.  

**Technical Tip –  
    Quick migration to the latest Aspose.Slides with new tables engine**

Latest [**Aspose.Slides**][14] for .NET 2.7.0 (and for Java 1.8.0) introduced a new tables engine and a new public API which is not fully compatible with the previous versions. The most important difference is the processing of borders of a cell. In the past to change the border style we could write something like this:  
  
  
\[C#\]  
  
// Accessing the cell in first row and first column  
Cell cell = table.GetCell(0,0);  
// Accessing the top border of the cell  
CellBorder border = cell.TopBorder;  
// Setting the color of the top border  
border.LineFormat.ForeColor = Color.Red;  
// Setting the width of the top border  
border.LineFormat.Width = 3;  
  
\[VB\]  
  
' Accessing the cell in first row and first column  
Dim cell As Cell =  table.GetCell(0,0)  
' Accessing the top border of the cell  
Dim border As CellBorder =  cell.TopBorder  
' Setting the color of the top border  
border.LineFormat.ForeColor = Color.Red  
' Setting the width of the top border  
border.LineFormat.Width = 3  
  
\[Java\]  
  
// Accessing the cell in first row and first column  
Cell cell = table.getCell(0,0);  
// Accessing the top border of the cell  
CellBorder border = cell.getTopBorder();  
// Setting the color of the top border  
border.getLineFormat().setForeColor(Color.RED);  
// Setting the width of the top border  
border.getLineFormat().setWidth(3);  
  
Actually, border of a merged cell can have several lines which wasn't processed. New tables engine provides very simple mechanism for that. Each CellBorder has iterator to lines. So to migrate to the new versions you should rewrite code in the following way:  
  
\[C#\]  
  
// Accessing the cell in first row and first column  
Cell cell = table.GetCell(0,0);  
// Accessing the top border of the cell  
CellBorder border = cell.TopBorder;  
// Accessing the iterator of the lines in top border of the cell  
IEnumerator iter = border.GetEnumerator();  
// Loop through all the lines  
while (iter.MoveNext())  
{  
    Line line = (Line) iter.Current;  
    // Setting the color of the top border  
    line.LineFormat.ForeColor = Color.Red;  
    // Setting the width of the top border  
    line.LineFormat.Width = 3;  
}  
  
\[VB\]  
  
' Accessing the cell in first row and first column  
Dim cell As Cell =  table.GetCell(0,0)  
' Accessing the top border of the cell  
Dim border As CellBorder =  cell.TopBorder  
' Accessing the iterator of the lines in top border of the cell  
Dim iter As IEnumerator =  border.GetEnumerator()  
' Loop through all the lines  
While iter.MoveNext()  
    Dim line As Line = CType(iter.Current, Line)  
    ' Setting the color of the top border  
    line.LineFormat.ForeColor = Color.Red  
    ' Setting the width of the top border  
    line.LineFormat.Width = 3  
End While  
  
\[Java\]  
  
// Accessing the cell in first row and first column  
Cell cell = table.getCell(0,0);  
// Accessing the top border of the cell  
CellBorder border = cell.getTopBorder();  
// Accessing the iterator of the lines in top border of the cell  
Iterator iter = border.iterator();  
// Loop through all the lines  
while (iter.hasNext())  
{  
    Line line = (Line) iter.next();  
    // Setting the color of the top border  
    line.getLineFormat().setForeColor(Color.RED);  
    // Setting the width of the top border  
    line.getLineFormat().setWidth(3);  
}  

**Aspose.Total for Reporting Services Mega Release**

Aspose is pleased to announce the release of their third major product suite, [**Aspose.Total for Reporting Services**][15].  The “Aspose.Total for Reporting Services” suite is comprised of five different rendering extensions which extend SQL Reporting, allowing reports to be exported to a variety of new formats. Since their inception in 2002, Aspose’s core focus has centered on file management.  Their new line of products for SQL Reporting Services is a continuation of that effort, providing database experts with a powerful new set of tools to accommodate the growing needs of their audience. An evaluation version of the suite can be downloaded from [**here**][16]. For more information, please visit the official **release page**.




[1]: http://www.aspose.com/Products/Aspose.Pdf/Default.aspx
[2]: http://www.aspose.com/Products/Aspose.Pdf/Default.aspx
[3]: http://www.aspose.com/Community/Files/51/aspose.pdf/default.aspx
[4]: http://www.aspose.com/Products/Aspose.Barcode/
[5]: http://www.aspose.com/Community/Files/53/aspose.barcode/category1082.aspx
[6]: http://www.aspose.com/Products/Aspose.BarCode.Reporting.Services/
[7]: http://www.aspose.com/Community/Files/52/aspose.barcode.reporting.services/category1217.aspx
[8]: http://www.aspose.com/Products/Aspose.Slides/
[9]: http://www.aspose.com/Community/Files/51/aspose.slides/category1199.aspx
[10]: http://www.aspose.com/Products/Aspose.Cells/
[11]: http://www.aspose.com/Community/Files/51/aspose.cells/entry102877.aspx
[12]: http://www.aspose.com/Products/Aspose.Words/
[13]: http://www.aspose.com/Community/Files/51/aspose.words/entry103596.aspx
[14]: http://www.aspose.com/Products/Aspose.Slides/
[15]: http://www.aspose.com/Products/Aspose.Total/
[16]: http://www.aspose.com/Community/Files/50/aspose.total.for.reporting.services/default.aspx




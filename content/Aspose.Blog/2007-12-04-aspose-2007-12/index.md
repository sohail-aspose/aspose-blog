---
title: 'Aspose 顾客时事通讯, 2007 年12月'
date: Tue, 04 Dec 2007 13:06:00 +0000
draft: false
url: /2007/12/04/aspose-2007-12/
author: Salman Sarfraz
summary: ''
tags: ['Aspose China']
---

**In This Issue**

*   **欢迎!**
*   **亮点产品– [Aspose.Pdf][1]**
*   **Aspose.BarCode取得进展**
*   **优化了的 Aspose.Slides for Java**
*   **使用Aspose.Cells for Java输入和输出****Excel 2007 XLSX文件**
*   **Aspose.Words for .NET 4.4.2.0 已发布**
*   **技术小技巧 – 快速转换到拥有新表格引擎的Aspose.Slides新版本中**
*   **Aspose.Total for Reporting Services 发布**

**欢迎**

欢迎阅读Aspose2007年11月份的时事快报！在本期快报中，我们将对我们的亮点产品Aspose.Pdf作出相关介绍。我们还将介绍新进发布的Aspose.Total for Reporting Services, Aspose.Words, Aspose.Cells, Aspose.Slides and Aspose.BarCode中令人兴奋的新功能. 通过本月的技术小技巧，您还将会了解到来自Aspose的最新信息——how you can quickly migrate to the latest Aspose.Slides with new tables engine.

**   亮点产品**

[**Aspose.Pdf**][2]是一个不用非图形PDF®文档报表组件，可以让您在.NET或Java应用程序中不使用Adobe Acrobat®便可创建PDF文档。Aspose.Pdf 拥有很好的性价比及强大的功能，包括：压缩、表格、图表、图像、超链接、安全以及自定义字体。Aspose.Pdf 支持通过API以及从XML模板和XSL-FO文件创建PDF。Aspose.Pdf使用非常简单，提供了14个用C#和Visual Basic写的功能demo。请 **[下载][3]**Aspose.Pdf 的免费试用版，看其是否满足您的业务需求。

**Aspose.BarCode取得进展**

[**Aspose.BarCode**][4]做了相当大的改进。Aspose.BarCode 文档已做了翻新。更多细节请访问官方**发布网页**.。Aspose.BarCode for .NET的新版本也以发布(**细节**)。可在**[这里][5]**下载[**Aspose.BarCode for Reporting Services**][6] 也做了一些改进，新版本为 v1.2.0.0 (**细节**).。可在**[这里][7]**下载。

**优化了的Aspose.Slides for Java**

 [**Aspose.Slides**][8] for Java的新版本1.8.0.0 已发布。新版本中包括一个新的、得到优化的表格引擎，并且在读写PPT文件的速度上得到了优化。其它一些新功能，如可以读取OLE1对象的文件名、改良的幻灯片文本呈现。新版本还解决了一些bug。新版本可在**[这里][9]**下载。更多细节可以浏览官方**发布网页**。  

**使用Aspose.Cells for Java输入和输出export Excel 2007 XLSX 文件**

新近发布的[**Aspose.Cells**][10] for Java v1.9.1目前支持输入和输出Excel 2007 XLSX文件。还支持数据排序并可使用PHP。数个bug也得到了解决。最新版本可在**[这里][11]**下载。更多详细信息请访问官方**发布网页**。

**Aspose.Words for .NET 4.4.2.0 已发布**

[**Aspose.Words**][12] for .NET v4.4.2.0 已发布。这是Aspose.Words的维护版本，包括一些改进和对输入DOCX文件bug的解决。还包括其他一些改进和bug的解决。可在**[这里][13]**下载最新版本。更多详细信息可访问官方**发布网页**。  

**技术小技巧–  
    Quick migration to the latest Aspose.Slides with new tables engine**

新近发布的 [**Aspose.Slides**][14] for .NET 2.7.0 (以及for Java 1.8.0)引进了一种新的表格引擎和尚未与先前版本完全兼容的公用API 。最重要的不同之处在于处理单元边框。过去在改变边框风格时，我们可以这样写：  
  
  
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
  
事实上，合并单元的边框有些未被处理的线条。新的表格引擎为此提供了一种及其简单的新机制。每个单元边框对线条拥有iterator。因此您可以通过以下方式重写代码来转换到新版本中：  
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

**Aspose.Total for Reporting Services 发布**

Aspose非常高兴地宣布他们的第三方产品包[**Aspose.Total for Reporting Services**][15].已发布。该 “Aspose.Total for Reporting Services” 包由5个不同的扩充编译而成，包括SQL报表、允许报表以多种新格式输出。早在2002年，Aspose’的中心焦点便放在文件管理上。他们的新产品SQL Reporting Services便是该努力的结果，提供了拥有强大工具集的数据专家来满足他们客户需求。该包的试用版可在**[这里][16]**下载。更多详情可浏览官方**发布网页**。




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




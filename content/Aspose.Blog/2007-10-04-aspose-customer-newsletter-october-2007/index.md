---
title: 'Aspose 顾客时事通讯, 2007 年10月'
date: Thu, 04 Oct 2007 15:04:00 +0000
draft: false
url: /2007/10/04/aspose-customer-newsletter-october-2007/
author: Salman Sarfraz
summary: ''
tags: ['Aspose China']
---

*   **欢迎！**
*   **产品推荐 – [Aspose.Pdf for Reporting Services][1]**
*   **使用 Aspose.Cells for Java将Excel文件输出为PDF**
*   **Aspose.BarCode for .NET 现在支持MacroPDF417 条码**
*   **使用Aspose.Cells for .NET创建加密的Excel文件**
*   **使用Aspose.Words for Reporting Services将HTML格式报表输出至Word格式**
*   **Aspose.Network v3.6.0.0的最新更新**
*   **技术小技巧 – 加载Web图片(从URL)至Excel工作表**
*   **Aspose.Pdf for .NET v3.6.0.0 补丁  
    **

**欢迎**

欢迎阅读Aspose2007年10月份时事快报! 在本月的时事快报中，我们将对推荐产品：Aspose.Pdf for Reporting Services做出相关性的介绍。我们还会介绍Aspose.Words for Reporting Services, Aspose.Network, Aspose.Pdf, Aspose.BarCode 以及Aspose.Cells这些产品在最新版本中新增的一些另人兴奋的功能。通过本月的技术小技巧，您将会了解到来自Aspose的最新信息—— 使用Aspose.Cells for .NET如何将Web图片（来自URL）加载到Excel的工作表中去。

**   产品推荐**

[**Aspose.Pdf for Reporting Services**][2] 是一个允许您在Microsoft SQL Server 2000 和 2005 Reporting Services中生成PDF报表的灵活的.NET解决方案。几乎支持所有的RDL报表特性，并允许您生成具备表格，图表，矩阵，页眉和页脚，节，列表，文本框，矩形，线条以及图片等的高质量PDF。得益于Aspose.Pdf组件技术，Aspose.Pdf for Reporting Services是一个在Microsoft SQL Server Reporting Services中生成PDF报表的理想产品。请**[下载][3]** Aspose.Pdf for Reporting Services 的免费试用版，看其是否满足您的商业需求。  

**使用 Aspose.Cells for Java将Excel文件输出为PDF**

The most important feature added in the recent release of 最新版本[**Aspose.Cells**][4] for Java v1.9.0.0中新增的一个最重要的功能就是支持输出Excel文件为Aspose.Pdf的xml格式，该格式可以使用Aspose.Pdf转换为PDF文档。当然也添加了一些其它功能：像在拷贝工作表时支持注释拷贝和内容选定，支持追踪引用单元和依赖单元等。此外，支持公式计算，带有智能标记的POJO和POJOs 也得到改良。一些重要的bug如范围指定，交叉表和公式计算等也得到了解决。更多细节，请阅读完**全手册**。  

**Aspose.BarCode for .NET现在支持MacroPDF417条码**

[**Aspose.BarCode**][5] for .NET v2.3.2.0中, 新增了对MacroPDF417条码(PDF417)的支持，从而使用户可以将大量数据编码为条码。一些与QR条码以及PDF417数字模式编码相关的bug也得到解决。获取更多有关Aspose.BarCode for .NET v2.3.2.0的更新，请点**击****。**  

**使用Aspose.Cells for .NET创建加密的Excel文件**

[**Aspose.Cells**][6] for .NET v4.4.0.0新增的一个重要的功能是开发者可以很容易地使用Aspose.Cells创建加密的Excel文件。在将图表转换为图片，XLS文件转换为PDF方面也做了改进。此外，一些bug也得到了解决。了解更多详情，请访**问** 其官方发布网页。

**使用Aspose.Words for Reporting Services将HTML格式报表转换为Word文档**

在[**Aspose.Words for Reporting Services**][7] v1.4.1.0最新版本中介绍了一个非常引人注意的功能。现在，您可以在Microsoft SQL Server Reporting Services 中使用一种特殊的模式，将HTML文本显示在文本框内，并可在同个文本框内允许使用不同的内嵌格式，如粗体，斜体等。此外，您可以插入任意HTML。如果您想输出多格式的报表至IMicrosoft Word文档，这项功能将正是您所需要的。更多细节，请点击其**官方发布** 网页。  

**Aspose.Network v3.6.0.0的最新更新**

新增了一些功能和重要改进，[**Aspose.Network**][8] v3.6.0.0 变得更加优秀。新增功能包括在Eml格式中支持多节或混合节，删除Outlook Message File中的附件以及将无法递送的报告信息（Outlook Message files）转换为Eml格式。此外新增了一些功能和改进，一些总共要bug也得到解决。获取 Aspose.Network for .NET v3.6.0.0的更多改进细节，请 **点击。**  
  

**技术小技巧**

****加载 Web 图片 (从 URL) 至 Excel工作表**  
**  
有时，您需要插入一个来自URL的图片到Excel 文件中。您可以很简单地完成。您仅需要将其提取或下载至流。然后，您可以使用**[Aspose.Cells][9]**将图片（流）插入到工作表当中。下面是一个简单的示例：  
  
  
\[C#\]  
  
  
//Define memory stream object  
System.IO.MemoryStream objImage;  
  
//Define web client object  
System.Net.WebClient objwebClient;  
  
//Define a string which will hold the web image url  
string sURL = "http://files.myopera.com/Mickeyjoe\_irl/albums/38458/abc.jpg";  
  
try  
{  
   //Instantiate the web client object  
   objwebClient = new System.Net.WebClient();  
  
   //Now, extract data into memory stream downloading the image data into the array of bytes  
   objImage = new System.IO.MemoryStream(objwebClient.DownloadData(sURL));  
  
   //Create a new workbook  
   Aspose.Cells.Workbook wb = new Aspose.Cells.Workbook();  
  
   //Get the first worksheet in the book  
   Aspose.Cells.Worksheet sheet = wb.Worksheets\[0\];  
  
   //Get the first worksheet pictures collection  
   Aspose.Cells.Pictures pictures = sheet.Pictures;  
  
   //Insert the picture from the stream to B2 cell  
   pictures.Add(1,1,objImage);  
  
   //Save the excel file  
   wb.Save("d:\\\\test\\\\webimagebook.xls");  
}  
catch (Exception ex )  
{  
   //Write the error message on the console  
   Console.WriteLine(ex.Message);  
}  
  
  
\[VB\]  
  
  
'Define memory stream object  
Dim objImage As System.IO.MemoryStream  
  
'Define web client object  
Dim objwebClient As System.Net.WebClient  
  
'Define a string which will hold the web image url  
Dim sURL As String = "http://files.myopera.com/Mickeyjoe\_irl/albums/38458/abc.jpg"  
  
Try  
   'Instantiate the web client object  
   objwebClient = New System.Net.WebClient  
  
   'Now, extract data into memory stream downloading the image data into the array of bytes  
   objImage = New System.IO.MemoryStream(objwebClient.DownloadData(sURL))  
  
   'Create a new workbook  
   Dim wb As Aspose.Cells.Workbook = New Aspose.Cells.Workbook  
    
   'Get the first worksheet in the book  
   Dim sheet As Aspose.Cells.Worksheet = wb.Worksheets(0)  
    
   'Get the first worksheet pictures collection  
   Dim pictures As Aspose.Cells.Pictures = sheet.Pictures  
    
   'Insert the picture from the stream to B2 cell  
   pictures.Add(1, 1, objImage)  
    
   'Save the excel file  
   wb.Save("d:\\test\\webimagebook.xls")  
Catch ex As Exception  
   'Write the error message on the console  
   Console.WriteLine(ex.Message)  
End Try

**Aspose.Pdf for .NET v3.6.0.0 补丁**

在2007年9月份，[**Aspose.Pdf**][10] 团队发布了提供大量更新，改进以及解决bug的补丁。新功能包括支持以XML格式嵌入图片数据，非阻断空间，从DataGrid控件中输出数据，XMP数据元以及多格式列表等。将HTML转换为PDF,Word转换为PDF，目录（TOC），表格，脚注，文本段落等bug均得到改进和解决。详细列表可以浏览 **这里**.。请**[下载][11]**最新版本 (其包含之前发布的补丁) 从而保证您的应用程序使用Aspose.Pdf更好地工作。  
  

隐私保护




[1]: http://www.aspose.com/Products/Aspose.Pdf.Reporting.Services/
[2]: http://www.aspose.com/Products/Aspose.Pdf.Reporting.Services/
[3]: http://www.aspose.com/Community/Files/52/aspose.pdf.reporting.services/default.aspx
[4]: http://www.aspose.com/Community/Files/51/aspose.cells/category1195.aspx
[5]: http://www.aspose.com/Community/Files/53/aspose.barcode/default.aspx
[6]: http://www.aspose.com/Community/Files/51/aspose.cells/category1084.aspx
[7]: http://www.aspose.com/Community/Files/52/aspose.words.reporting.services/default.aspx
[8]: http://www.aspose.com/Community/Files/54/aspose.network/default.aspx
[9]: http://www.aspose.com/Products/Aspose.Cells/
[10]: https://products.aspose.com/pdf
[11]: http://www.aspose.com/Community/Files/51/aspose.pdf/default.aspx




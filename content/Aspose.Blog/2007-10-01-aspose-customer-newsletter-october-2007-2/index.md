---
title: 'Aspose Customer Newsletter, October 2007'
date: Mon, 01 Oct 2007 19:43:00 +0000
draft: false
url: /2007/10/01/aspose-customer-newsletter-october-2007-2/
author: Salman Sarfraz
summary: ''
tags: ['Customer Newsletters']
---

**In This Issue**

*   **Welcome!**
*   **Product Spotlight – [Aspose.Pdf for Reporting Services][1]**
*   **Export Excel files to PDF using Aspose.Cells for Java**
*   **Aspose.BarCode for .NET now supports MacroPDF417 symbology**
*   **Create Encrypted Excel files using Aspose.Cells for .NET**
*   **Export HTML formatted reports to Word documents using Aspose.Words for Reporting Services**
*   **Latest Enhancements in Aspose.Network v3.6.0.0**
*   **Technical Tip – Load a Web Image (from a URL) into an Excel Worksheet**
*   **Aspose.Pdf for .NET v3.6.0.0 Mega Release**

**Welcome**

Welcome to the October 2007 issue of the Aspose Newsletter! In this month’s newsletter, we will provide some introductory information about our spotlight product: Aspose.Pdf for Reporting Services. We will also look at the new and exciting features offered in the recent releases of Aspose.Words for Reporting Services, Aspose.Network, Aspose.Pdf, Aspose.BarCode and Aspose.Cells. You will learn about the latest news from Aspose along with the monthly Tech-Tip, which demonstrates how you can load a web image (from a URL) into an Excel worksheet using Aspose.Cells for .NET.

**Product Spotlight**

[**Aspose.Pdf for Reporting Services**][2] is a robust .NET solution which allows you to produce PDF reports in Microsoft SQL Server 2000 and 2005 Reporting Services. Almost all RDL report features are supported, allowing you to generate high quality PDF reports having tables, charts, matrices, headers & footers, sections, lists, textboxes, rectangles, lines and images etc. Leveraging from the technology of Aspose.Pdf component, Aspose.Pdf for Reporting Services is the ideal product for anyone looking to generate PDF reports in Microsoft SQL Server Reporting Services. Please [**download**][3] the free evaluation version of Aspose.Pdf for Reporting Services to see how it fulfills your business needs.  

**Export Excel files to PDF using Aspose.Cells for Java**

The most important feature added in the recent release of [**Aspose.Cells**][4] for Java v1.9.0.0 is the support of exporting Excel files in Aspose.Pdf xml format, which can be converted to PDF documents using Aspose.Pdf. Few more features are also added to this release like the support of copying comments & named ranges while a worksheet is copied and the support of tracing precedents & dependents of a cell etc. Moreover, the support of formula calculation, POJO and POJOs with smart markers is also improved. Many important bugs related to named ranges, pivot tables and formula calculation etc. are also fixed. For more details, please read the **complete story.**  

**Aspose.BarCode for .NET now supports MacroPDF417 symbology**

In [**Aspose.BarCode**][5] for .NET v2.3.2.0, the support of MacroPDF417 (which is an implementation of PDF417) symbology is also added that will enable our customers to encode very large amount of data into barcodes. Some bugs related to QR barcode and PDF417 numeric mode encodings are also fixed. To get more details about the improvements made in Aspose.BarCode for .NET v2.3.2.0, please **click here.**  

**Create Encrypted Excel files using Aspose.Cells for .NET**

One of the important features added to [**Aspose.Cells**][6] for .NET v4.4.0.0 is that now developers can easily create encrypted Excel files from scratch using Aspose.Cells. There are some improvements made in Chart to Image and XLS to PDF conversions. Moreover, few bugs are also fixed in this release. For more details, please **visit** its official release page.

**Export HTML formatted reports to Word documents using Aspose.Words for Reporting Services**

The latest release of [**Aspose.Words for Reporting Services**][7] v1.4.1.0 introduces a very interesting feature. Now, you can enable a special mode in Microsoft SQL Server Reporting Services that will instruct the renderer to understand HTML text hosted within textboxes. This allows applying different inline formatting such as bold or italic within the same textbox. Moreover, you can insert almost any HTML you wish. If you want to export rich formatted reports to Microsoft Word documents, this new feature is exactly what you need. To get more details, please check its **official release** page.  

**Latest Enhancements in Aspose.Network v3.6.0.0**

With the addition of many new features and important enhancements, [**Aspose.Network**][8] v3.6.0.0 has just got better. New features include the support of rendering multipart/mixed type part in Eml format, deleting attachments in Outlook Message files and converting non-deliverable report message (Outlook Message files) to Eml format. Besides new features and enhancements, some important bugs are also fixed in this release. To get more details about the improvements made in Aspose.Network for .NET v3.6.0.0, please **click here.**  
  

**Technical Tip**

****Load a Web Image (from a URL) into an Excel Worksheet**  
**  
Sometimes, you do require inserting a picture from a URL into an Excel file. You may do it quite easily. You just need to extract & download image data into stream and then you may use [**Aspose.Cells**][9] to insert image (from the stream) into the worksheet. Following is a simple way to achieve this:  
  
  
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

**Aspose.Pdf for .NET v3.6.0.0 Mega Release**

In the month of September, 2007, the [**Aspose.Pdf**][10] team published a Mega Release that provides plenty of new features, improvements and bug fixes. The new features include the support of embedded image data in XML, non-breaking space, importing data from DataGrid control, XMP metadata and rich formatting list labels etc. The improvements and bug fixes are related to HTML to PDF & Word to PDF conversions, table of contents (TOC), tables, footnotes and text paragraphs etc. The complete list of all these improvements can be viewed **here**. Please [**download**][11] this latest release now to make your applications work better using Aspose.Pdf.




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




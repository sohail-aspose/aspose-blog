---
title: 'Aspose Customer Newsletter August, 2007'
date: Wed, 01 Aug 2007 09:42:00 +0000
draft: false
url: /2007/08/01/aspose-customer-newsletter-august-2007/
author: Salman Sarfraz
summary: ''
tags: ['Customer Newsletters']
---

**In This Issue**

*   **Welcome**
*   **Product Spotlight – [Aspose.Slides for Reporting Services][1]**
*   **Generate Excel Reports in MS SQL Server using Aspose.Cells for Reporting Services**
*   **Experience an Improved User Interface in Aspose.Editor v2.1.0**
*   ****New Releases of Aspose.Pdf for Java****
*   **Latest Enhancements in Aspose.Grid v1.9.2**
*   **Aspose.Words for Reporting Services even works on MS SQL Server 2008 "Katmai"**
*   **Technical Tip **–** Parse Microsoft Outlook Message files programmatically**
*   **Aspose.Words for .NET v4.3.0 is Optimized for Windows Vista**
*   **Aspose.Pdf for .NET v3.5.5.0 Mega Hotfix**

**Welcome**

Welcome to the August 2007 issue of the Aspose Newsletter! In this month’s newsletter, we will provide some introductory information about our spotlight product: Aspose.Slides for Reporting Services. We will also look at the new and exciting features offered in the recent releases of Aspose.Cells for Reporting Services, Aspose.Grid, Aspose.Words, Aspose.Pdf, Aspose.Editor and Aspose.Words for Reporting Services. You will learn about the latest news from Aspose along with the monthly Tech-Tip, which demonstrates how you can parse Microsoft Outlook Message files programmatically using Aspose.Network.

**Product Spotlight**

**[Aspose.Slides for Reporting Services][2]** is the only solution in the market that makes possible generating true PPT and PPS reports in Microsoft SQL Server 2005 Reporting Services (x86 and x64). All RDL report features, including tables, matrices, charts and images are converted with the highest degree of precision to Microsoft PowerPoint presentations.  
Microsoft SQL Server Reporting Services does not have built-in abilities to export reports as Microsoft PowerPoint presentations, but after installing Aspose.Slides for Reporting Services on your server, you will get access to two additional export formats:  
  
PPT – PowerPoint Presentation via Aspose.Slides  
PPS – PowerPoint Show via Aspose.Slides  
  
Aspose.Slides for Reporting Services create presentations on the server without utilizing Microsoft PowerPoint. Aspose.Slides for Reporting Services internally uses Aspose.Slides for .NET – the world-class component for server-side presentations processing. Please **[download][3]** the free evaluation version of Aspose.Slides for Reporting Services to see how it fulfills your business needs.  

**Generate Excel Reports in MS SQL Server using Aspose.Cells for Reporting Services**

**[Aspose.Cells for Reporting Services][4]** allows you to deliver native Excel reports in Microsoft SQL Server 2005 Reporting Services. Unlike the built-in renderer for Excel based reports, Aspose.Cells for Reporting Services provides an extended feature set and allow RDL reports to be converted to: Excel 97-2003 binary XLS format, SpreadsheetML or the Excel 2007 XLSX format.  
  
In the recent release of Aspose.Cells for Reporting Services, some other valuable features are also added like the support of background image and exporting data to CSV & Tab Delimited files etc. Moreover, few important bugs are also fixed. To get more details, please **click here**.  

**Experience an Improved User Interface in Aspose.Editor v2.1.0**

Aspose has published a new release of **[Aspose.Editor][5]**. The main goal of this release was to improve user interface and provide standard controls expected from an editor application. Aspose.Editor now features embedded ruler, main menu bar, tool bar and more. Developers can use provided standard controls, customize them or replace with third-party controls. This simplifies creating user-friendly editor applications and reduces development efforts. To get more details about the improvements made in Aspose.Editor for .NET v2.1.0, please **click here**.  

**New Releases of Aspose.Pdf for Java**

With the latest releases of **[Aspose.Pdf][6]**, java developers can enjoy some newly added important features such as JavaScript, annotations and bookmarks. JavaScript provides one of the easiest and most powerful ways to customize PDF files. Using annotation feature, you can easily add comments to the PDF during the creation process. The bookmark feature enables you to create bookmarks automatically from the headings of the document. Some important bugs (related to adding tables in PDF, getting colors information, licensing, controlling image size and setting background picture for PDF section) are also fixed. For more details, please visit the official release pages of **v2.2.0.0** and **v2.2.1.0**.

**Latest Enhancements in Aspose.Grid v1.9.2**

With the addition of many new features and important enhancements, **[Aspose.Grid][7]** v1.9.2 has just got better. New features include the support of XHTML 1.0 based rendering, worksheets serialization, custom and auto-filtering, dragging & scrolling and command bar etc. Moreover, the performance of formula engine, XHTML rendering and other features of Aspose.Grid is highly optimized to increase its efficiency. Besides new features and enhancements, some important bugs are also fixed in this release. To get more details about the improvements made in Aspose.Grid for .NET v1.9.2, please **click here**.  
  

**Aspose.Words for Reporting Services even works on MS SQL Server 2008 "Katmai"**

It is a great pleasure to announce that our Aspose.Words team tested **[Aspose.Words for Reporting Services][8]** on the CTP 3 of Microsoft SQL Server 2008 “Katmai” Reporting Services and it worked great. Moreover, the support for **_WritingMode_** property of textboxes is also added. To get more details about these features and other improvements made in Aspose.Words for Reporting Services, please check the release pages of **v1.3.0** and **v1.3.1**.  
  

**Technical Tip**

****Parse Microsoft Outlook Message files programmatically**  
**  
Did you know that you could parse Microsoft Outlook Message files programmatically by just a few lines of code using **[Aspose.Network][9]**? Here’s how:  
  
\[C#\]  
  
//Loading outlook email message file  
MapiMessage msg = MapiMessage.FromFile(@"C:\\WithAttachment.msg");  
  
//Obtaining subject of the email message  
Console.WriteLine("Subject:" + msg.Subject);  
  
//Obtaining sender name of the email message  
Console.WriteLine("From:" + msg.SenderName);  
  
//Obtaining body of the email message  
Console.WriteLine("Body:" + msg.Body);  
  
//Obtaining information about number of attachments in the email message  
Console.WriteLine("Attachment Count:" + msg.Attachments.Count);  
  
//Iterating through all attachments in the email message  
foreach (MapiAttachment attachment in msg.Attachments)  
{  
//Accessing the file name of the attachment  
Console.WriteLine("Attachment:"+ attachment.FileName);  
  
//Saving attachment  
attachment.Save(attachment.LongFileName);  
}  
  
\[VB\]  
  
'Loading outlook email message file  
Dim msg As MapiMessage = MapiMessage.FromFile("C:\\WithAttachment.msg")  
  
'Obtaining subject of the email message  
Console.WriteLine("Subject:" + msg.Subject)  
  
'Obtaining sender name of the email message  
Console.WriteLine("From:" + msg.SenderName)  
  
'Obtaining body of the email message  
Console.WriteLine("Body:" + msg.Body)  
  
'Obtaining information about number of attachments in the email message  
Console.WriteLine("Attachment Count:" + msg.Attachments.Count)  
  
‘Iterating through all attachments in the email message  
Dim attachment As MapiAttachment  
For Each attachment In msg.Attachments  
Accessing the file name of the attachment  
Console.WriteLine("Attachment:"+ attachment.FileName)  
  
'Saving attachment  
attachment.Save(attachment.LongFileName)  
Next  
  

**Aspose.Words for .NET v4.3.0 is Optimized for Windows Vista**

The recent release of **[Aspose.Words][10]** for .NET v4.3.0 is greatly optimized for 64-bit operating systems including Windows Vista x64 and Windows Server 2003 x64. Aspose.Words is heavily tested under Windows Vista and all installation issues are fixed. Some important bugs regarding WordML export, Word to PDF conversion, bookmarks, fonts, SECTIONPAGES field and HTML stream export are also fixed. For more details, please read the **complete story**.  
  

**Aspose.Pdf for .NET v3.5.5.0 Mega Hotfix**

In the month of July, 2007, the **[Aspose.Pdf][11]** team released 3 Mega Hot fixes that provide about 30 bug fixes related to Word/HTML to PDF conversion, section & page breaks, footnotes, tables, positioning of images, table of contents (TOC), page numbering, columns spanning and tab stops etc. Be sure to check out the full list of these bug fixes through their official release pages (**1st**, **2nd** and **3rd** Mega Hot fixes). Please **[download][12]** the latest release (as it also includes the bug fixes of previous releases) now to make your applications work better using Aspose.Pdf.




[1]: /Products/Aspose.Slides.Reporting.Services/
[2]: /Products/Aspose.Slides.Reporting.Services/
[3]: /Community/Files/52/aspose.slides.reporting.services/default.aspx
[4]: /Community/Files/52/aspose.cells.reporting.services/default.aspx
[5]: /Community/Files/53/aspose.editor/default.aspx
[6]: /Community/Files/51/aspose.pdf/default.aspx
[7]: /Community/Files/53/aspose.grid/default.aspx
[8]: /Community/Files/52/aspose.words.reporting.services/default.aspx
[9]: /Community/Files/54/aspose.network/default.aspx
[10]: /Community/Files/51/aspose.words/default.aspx
[11]: /Products/Aspose.Pdf/
[12]: /Community/Files/51/aspose.pdf/default.aspx




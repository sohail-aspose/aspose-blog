---
title: 'Aspose Customer Newsletter, November 2007'
date: Thu, 01 Nov 2007 17:54:00 +0000
draft: false
url: /2007/11/01/aspose-customer-newsletter-november-2007/
author: Salman Sarfraz
summary: ''
tags: ['Customer Newsletters']
---

**In This Issue**

*   **Welcome!**
*   **Special Announcement – Aspose.Custom for Reporting Services is on its way!**
*   **Product Spotlight – [Aspose.Slides][1]**
*   **Improved Aspose.Total Northwind Demos**
*   **Aspose.Grid supports Microsoft ASP.NET AJAX Extensions for .NET 2.0**
*   **Open, Generate, Save & Convert DOCX using Aspose.Words for .NET**
*   **Aspose.Editor now works on Microsoft Windows Vista**
*   **Aspose.Words for Reporting Services 2.0.0.0 Released**
*   **Technical Tip – Adding multi-line watermark to existing PDF**
*   **Aspose.Pdf for .NET v3.6.1.0 Mega Hotfix**

**Welcome**

Welcome to the November 2007 issue of the Aspose Newsletter! In this month’s newsletter, we will provide some introductory information about our spotlight product: Aspose.Slides. We will also look at the new and exciting features offered in the recent releases of Aspose.Total, Aspose.Words, Aspose.Grid, Aspose.Editor and Aspose.Pdf. You will learn about the latest news from Aspose along with the monthly Tech-Tip, which demonstrates how you can add multi-line watermark to your existing PDF documents using Aspose.Pdf.Kit.

**Special Announcement**

We already offer Aspose.Custom, a flexible solution that allows customers to design their own suites of components according to their needs. Currently, Aspose.Custom allows customers to only add .NET or Java components to their custom suites but we received several requests from customers asking about the support of adding Reporting Services products to Aspose.Custom too. So, it is to inform our valuable customers that we are also going to add Aspose.Custom for Reporting Services section to our [**Aspose.Custom**][2] page in this month. We hope that, this change will be more useful for customers who would like to buy multiple Reporting Services products with a reasonable discount.

**Product Spotlight**

[**Aspose.Slides**][3] is a non-graphical PowerPoint® management component that enables either .NET or Java applications to read and write PowerPoint documents without utilizing Microsoft PowerPoint. Aspose.Slides is the first and only .NET and Java component that provides the functionality to manage PowerPoint documents. As with all Aspose components, Aspose.Slides is written in managed C#, well priced and lightening fast. Please [**download**][4] the free evaluation version of Aspose.Pdf for Reporting Services to see how it fulfills your business needs.

**Improved Aspose.Total Northwind Demos**

The improved demos of [**Aspose.Total**][5] now support Windows Vista. They are offered in both MS Visual Studio 2003 and 2005 formats. It is recommended that the users of Windows Vista use the demos provided in MS Visual Studio 2005 format. You can download the demos from [**here**][6]. For more details, please read the **complete story**.  

**Aspose.Grid supports Microsoft ASP.NET AJAX Extensions for .NET 2.0**

The new release of [**Aspose.Grid**][7] v1.9.3 now contains support for Microsoft ASP.NET AJAX Extensions for .NET 2.0. You may use **Grid.Web** with the AJAX extensions web control, **UpdatePanel**. Among other new features are; the support for TAB, SHIFT-TAB navigation and the addition of some new classes, methods & properties. Some other improvements and bug fixes have also been included in this release. To get more details about the improvements made in Aspose.Grid v1.9.3, please **click here**.  

**Open, Generate, Save & Convert DOCX using Aspose.Words for .NET**

The previous release of [**Aspose.Words**][8] for .NET introduced the ability to save documents in the Microsoft Word 2007 DOCX format. The current release of Aspose.Words for .NET v4.4.1.0 makes it possible to load DOCX files. So, now you can easily open, generate, save and convert DOCX documents using Aspose.Words. This makes Aspose.Words for .NET one of the first document processing components on the market that provides such capabilities. In addition to the support for loading DOCX files, this release also includes numerous bug fixes and improvements. For more details, please **visit** its official release page.

**Aspose.Editor now works on Microsoft Windows Vista**

The latest release of [**Aspose.Editor**][9] v2.2.0 adds support for Windows Vista. Since the control was tested only on 32-bit Vista editions we cannot guarantee it working on 64-bit editions, however it should work. Text drag-and-drop inside document has been implemented in this version. Also included in this release are .NET 2.0 binaries and separate demos for Visual Studio 2005 in addition to various bug fixes since the last release. To get more details, please check its **official release** page.  

**Aspose.Words for Reporting Services 2.0.0.0 Released**

[**Aspose.Words for Reporting Services**][10] v2.0.0.0 has been released. This release finally introduces a feature that has been expected by many users - export to flow layout documents! This means that, now you are able to convert RDL reports to "true", "normal", easy to edit documents as if they were created manually by an office worker! With version 2.0, you can get documents that allow to insert paragraph breaks and contain tables crossing over pages (that grow when adding contents). To get more details about the improvements made in Aspose.Words for Reporting Services v2.0.0.0, please **click here**.  

**Technical Tip – Adding multi-line watermark to existing PDF**

A lot of users want to stamp their PDF documents with multi-line text. They usually try to use “\\n” and “<BR>” but these types of characters are not supported by Aspose.Pdf.Kit. So, to make it possible, we have added another method named AddNewLineText() in FormattedText class of [**Aspose.Pdf.Kit**][11].  
  
Please refer to the following code chunk to add multi-line watermark in existing PDF.  
  
\[C#\]  
  
//Instantiate a stamp object  
Stamp logoStamp = new Stamp();  
  
//Instantiate an object of FormattedText class  
FormattedText formatText = new FormattedText("Hello World!", System.Drawing.Color.FromArgb(180, 0, 0), FontStyle.TimesItalic, EncodingType.Winansi, false, 50);  
  
//Add another line for Stamp  
formatText.AddNewLineText("Good Luck");  
  
//BindLogo to PDF  
logoStamp.BindLogo(formatText);  
  
\[VB\]  
  
'Instantiate a stamp object  
Dim logoStamp As New Stamp()  
  
'Instantiate an object of FormattedText class  
Dim formatText As New FormattedText("Hello World!", System.Drawing.Color.FromArgb(180, 0, 0), FontStyle.TimesItalic, EncodingType.Winansi, False, 50)  
  
'Add another line for Stamp  
formatText.AddNewLineText("Good Luck")  
  
'BindLogo to PDF  
logoStamp.BindLogo(formatText)  

**Aspose.Pdf for .NET v3.6.1.0 Mega Hotfix**

During the month of October 2007, the [**Aspose.Pdf**][12] team published a Mega Hotfix that provides plenty of bug fixes, some new features and improvements. The bug fixes and improvements are related to HTML to PDF & Word to PDF conversions, tables, header & footer, page numbering, ordered list and memory issues etc. The complete list of all these improvements can be viewed **here**. Please [**download**][13] this latest release now to make your applications work better using Aspose.Pdf.




[1]: http://www.aspose.com/Products/Aspose.Slides/
[2]: http://www.aspose.com/PURCHASE/Aspose.Custom.aspx
[3]: http://www.aspose.com/Products/Aspose.Slides/
[4]: http://www.aspose.com/Community/Files/51/aspose.slides/default.aspx
[5]: http://www.aspose.com/Products/Aspose.Total/
[6]: http://www.aspose.com/Community/Files/50/aspose.total/category1173.aspx
[7]: http://www.aspose.com/Products/Aspose.Grid/
[8]: http://www.aspose.com/Products/Aspose.Words/
[9]: http://www.aspose.com/Products/Aspose.Editor/
[10]: http://www.aspose.com/Products/Aspose.Words.Reporting.Services/
[11]: http://www.aspose.com/Products/Aspose.Pdf.Kit/
[12]: https://products.aspose.com/pdf
[13]: http://www.aspose.com/Community/Files/51/aspose.pdf/default.aspx




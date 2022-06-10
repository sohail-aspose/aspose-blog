---
title: 'Aspose Customer Newsletter, February 2008'
date: Fri, 01 Feb 2008 11:48:58 +0000
draft: false
url: /2008/02/01/aspose-customer-newsletter-february-2008/
author: Salman Sarfraz
summary: ''
tags: ['Customer Newsletters']
---

**In This Issue**

*   **Welcome!**
*   **Product Spotlight – [Aspose.Flash][1]**
*   **Aspose.Network supports SSL for IMAP / POP3 / SMTP**
*   **Aspose.Pdf.Kit for .NET 2.7.0.0 released**
*   **Exporting to DOCX with Aspose.Words for Java**
*   **Aspose.Words OOXML import soon to come out of beta**
*   **Aspose.Cells for Reporting Services 1.1.0.0 released  
    **
*   **Technical Tip – Using Aspose.Words with PHP**

Welcome

Welcome to the February 2008 issue of the Aspose Newsletter! In this month’s newsletter, we will provide some introductory information about our spotlight product: Aspose.Flash. We will also look at the new and exciting features offered in the recent releases of Aspose.Network, Aspose.Pdf.Kit, Aspose.Words, and Aspose.Cells for Reporting Services. You will learn about the latest news from Aspose along with the monthly Tech-Tip, which demonstrates how you can use Aspose.Words with PHP.

Product Spotlight

Developers using Flash® content in conjunction with the powerful .NET framework have the ability to produce some of the highest quality, feature rich sites today. [Aspose.Flash][2] helps to extend the potential of that powerful combination even further. Aspose.Flash is a non-graphical, .NET Flash® management component. With Aspose.Flash developers can dynamically manipulate and generate Flash® content directly from their .NET applications. Aspose.Flash is written in native C# and is lightening fast. Take the time to [download][3] the free evaluation version today to see how Aspose.Flash can work for you.

Aspose.Network supports SSL for IMAP / POP3 / SMTP

[Aspose.Network][4] is a complete solution for network programming on the .NET platform. The latest version 3.8.0.0 of Aspose.Network for .NET has been released. This is a major release containing SSL support for IMAP and POP3. SSL support for SMTP was added in the 3.7.0.0 release earlier. Aspose.Network now supports using Secure Sockets Layer (SSL) to encrypt the connection (POP3/IMAP). Aspose.Network.Mail also supports sending email via SSL over SMTP protocol. Implicit / Explicit Security mode is also supported in SSL over SMTP/IMAP/POP3. In addition Aspose.Network.Ftp now supports parsing VAS/VMS format item list and Aspose.Network.Pop3 includes support for 3 types of authentication. Also included in this release are numerous bug fixes and improvements. For more information about the 3.8.0.0 release and to download the latest version please refer to the description found [here][5]. For more information about the 3.7.0.0 release please consult the official release page.

Aspose.Pdf.Kit for .NET 2.7.0.0 released

[Aspose.Pdf.Kit][6] for .NET 2.7.0.0 has been released. This new release supports creating bookmarks for all pages as well as creating nested bookmarks. Support for exchanging bookmarks of XML and extracting bookmarks to HTML has also been added. In addition a new method is added for disposing Form fields more flexibly, and a set of new methods and properties have been added in PdfViewer for printing large PDF files more efficiently. This release also includes many improvements and numerous bug fixes. The latest version can be downloaded from [here][7]. For more details, please visit its official release page.  

Exporting to DOCX with Aspose.Words for Java

The latest version 2.4.0.0 of [Aspose.Words][8] for Java has been released. With this release Aspose.Words for Java now supports exporting to Microsoft Office 2007 Open XML (DOCX) format. The set of DOCX features supported by Aspose.Words is comprehensive. Only a few limitations are applicable in the current version. The latest version can be downloaded from [here][9]. For more information about this release please consult the official release page.

Aspose.Words OOXML import soon to come out of beta

We have been working hard to provide great support for Office Open XML in Aspose.Words. In this regard there have been three major releases which can be considered as milestones. These include Aspose.Words for .NET 4.4.0.0 which included support for exporting to Microsoft Office 2007 Open XML (DOCX), Aspose.Words for .NET 4.4.1.0 with beta support for import of DOCX files and Aspose.Words for Java 2.4.0.0 with support for exporting to DOCX. Import of DOCX files is still in Beta, but we are successfully finalizing it. A production release is planned soon. We have also created a detailed Aspose.Words to OOXML conformance specification which can be found [here][10]. For more information please consult this post.  

Aspose.Cells for Reporting Services 1.1.0.0 released

We have released [Aspose.Cells for Reporting Services][11] version 1.1.0.0. In this release we provide a client add-in tool, Aspose.Cells Report Designer, which allows users to use MS Excel as a report design tool. With Aspose.Cells Report Designer users can design a report template in Excel instead of Visual Studio or other report builder tool. The report template is embedded in Reporting Services RDL file and can be published to Report Server. It makes report design an easy and fast task. Also in this release the Aspose.Cells for Reporting Services server render is greatly enhanced. Working with the report template, users can utilize all advanced Excel features in Reporting Services, including native Excel charts, advanced formulas, pivot tables and more. Numerous other improvements and bug fixes have also been included. Please download this latest release from [here][12].  

Technical Tip – Using Aspose.Words with PHP

Aspose.Words for .NET and Aspose.Words for Java can both be used with PHP. Given below is a code snippet showing how you can use Aspose.Words with PHP. The following example shows how to insert sections using DocumentBuilder, specify page setup for a section and reset page setup to defaults using Aspose.Words for .NET.  
  
**\[PHP using Aspose.Words for .NET\]**  
  
// Load License  
$license = new COM('Aspose.Words.License');  
$license->SetLicense("c:/Aspose.Words.lic");  
  
// Create an object to use.  
$builder = new COM('Aspose.Words.DocumentBuilder');  
  
// Modify the first section in the document.  
$builder->PageSetup->Orientation = 2;  
$builder->PageSetup->VerticalAlignment = 1;  
$builder->Writeln("Section 1, landscape oriented and text vertically centered.");  
  
// Start a new section and reset its formatting to defaults.  
$builder->InsertBreak(5);  
$builder->PageSetup->ClearFormatting();  
$builder->Writeln("Section 2, back to default Letter paper size, portrait orientation and top alignment.");  
  
// Save the document  
$builder->Document->Save("C:/tmp.doc");  
  
The following example shows how to create a simple Hello World document in PHP using Aspose.Words for Java.  
**  
\[PHP using Aspose.Words for Java\]**  
  
$docFileName="c:/java.doc";  
  
// Setting license  
$License = new Java('com.aspose.words.License');  
$License->setLicense('c:/Aspose.Words.Java.lic');  
  
// Creating Aspose.Words Objects  
$Document = new Java('com.aspose.words.Document') or die("Cant load Document");  
$DocumentBuilder = new Java('com.aspose.words.DocumentBuilder',$Document) or die("Cant load DocumentBuilder");  
  
// Do something with document  
$DocumentBuilder->writeln("Hello world from Aspose.Words!!!");  
  
// Saves the document to destination  
$Document->save($docFileName,1);




[1]: http://www.aspose.com/Products/Aspose.Flash/
[2]: http://www.aspose.com/Products/Aspose.Flash/
[3]: http://www.aspose.com/Community/Files/51/aspose.flash/default.aspx
[4]: http://www.aspose.com/Products/Aspose.Network/
[5]: http://www.aspose.com/Community/Files/54/aspose.network/entry110079.aspx
[6]: http://www.aspose.com/Products/Aspose.Pdf.Kit/
[7]: http://www.aspose.com/Community/Files/51/aspose.pdf.kit/entry107457.aspx
[8]: http://www.aspose.com/Products/Aspose.Words/
[9]: http://www.aspose.com/Community/Files/51/aspose.words/entry107226.aspx
[10]: http://www.aspose.com/Community/Files/51/aspose.words/entry107522.aspx
[11]: http://www.aspose.com/Products/Aspose.Cells.Reporting.Services/
[12]: http://www.aspose.com/Community/Files/52/aspose.cells.reporting.services/entry108211.aspx




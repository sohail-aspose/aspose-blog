---
title: 'Aspose Customer Newsletter, September 2007'
date: Sat, 01 Sep 2007 22:07:00 +0000
draft: false
url: /2007/09/01/aspose-customer-newsletter-september-2007-2/
author: Salman Sarfraz
summary: ''
tags: ['Customer Newsletters']
---

**In This Issue**

*   **Welcome!**
*   **Special Announcement – Our address has changed!**
*   **Product Spotlight – **[Aspose.BarCode for Reporting Services][1]****
*   **Convert DOC, RTF, WordML and HTML documents to DOCX**
*   **Secure your PDF documents with Digital Signatures**
*   **Aspose.Words for Java v2.3.0.0 Released**
*   **Latest Enhancements in Aspose.Network v3.5.3.0**
*   **Aspose.Words for Reporting Services now supports DOCX format too**
*   **Technical Tip – Change page orientation in RDL reports exported to Word documents**
*   **Aspose.Pdf for .NET v3.5.8.0 Mega Hotfix  
    **

**Welcome**

Welcome to the September 2007 issue of the Aspose Newsletter! In this month’s newsletter, we will provide some introductory information about our spotlight product: Aspose.BarCode for Reporting Services. We will also look at the new and exciting features offered in the recent releases of Aspose.Words for Reporting Services, Aspose.Network, Aspose.Pdf, Aspose.Words and Aspose.Pdf.Kit. You will learn about the latest news from Aspose along with the monthly Tech-Tip, which demonstrates how you can customize the page orientation in RDL reports that are exported to Microsoft Word documents using Aspose.Words for Reporting Services.

**Special Announcement**

It is to inform our valuable customers that we have recently changed our business address. The new business address is:  
  
Aspose Pty Ltd  
Suite 119, 272 Victoria Avenue  
Chatswood, NSW, 2067  
Australia  
  
All other contact information would remain the same. The customers, who pay by checks, can send their checks at above address in future. We remain thankful for your attention.  

**Product Spotlight**

**[Aspose.BarCode for Reporting Services][2]** is the most comprehensive .NET solution for the rendering of barcode images in Microsoft SQL Server 2000 and 2005 Reporting Services. Following the success of Aspose.BarCode for .NET, Aspose.BarCode for Reporting Services has introduced the support of more than 25 most popular barcode symbologies including Linear (Code128, Code39, Code93, EAN13, EAN14 (SSCC14), EAN8, UPCA, UPCE, BooklandEAN, Interleaved2of5, Standard2of5, MSI, Code11, Codabar, Postnet, Planet and SSCC18 etc.) and 2D (PDF417, QR and DataMatrix etc.) barcodes.  
  
It allows developers to display high quality barcode labels on SQL reports. These barcode labels can be rendered in four image formats i.e. Bmp, Jpg, Gif and Png. Aspose.BarCode for Reporting Services can be used very easily by adding it to the toolbox of Visual Studio IDE and then dropping it on the SQL report just like windows or web controls. Please **[download][3]** the free evaluation version of Aspose.BarCode for Reporting Services to see how it fulfills your business needs.  

**Convert DOC, RTF, WordML and HTML documents to DOCX**

The most important feature added in the recent release of **[Aspose.Words][4]** for .NET v4.4.0.0 is the support of exporting documents to Microsoft Office 2007 Open XML (DOCX) format. It means that now developers can easily convert DOC, RTF, WordML and HTML documents to latest DOCX format using Aspose.Words for .NET. Moreover, now Aspose.Words assemblies and installer are also **_signed_** with Authenticode. Many important bugs regarding Word to PDF conversion, opening & saving documents and custom properties etc. are also fixed. For more details, please read the **complete story**.  

**Secure your PDF documents with Digital Signatures**

In **[Aspose.Pdf.Kit][5]** for .NET v2.6.0.0, the support of Digital Signature is added that can make your PDF documents more secure by authenticating the identity of a user and contents of the document. Few improvements are also made in Form (either AcroForm or XfaForm) related features. Some bugs related to bookmarks, form fields, encryption, links & text extraction, combo box filling and flattening, XFA text fields and PdfViewer etc. are also fixed. To get more details about the improvements made in Aspose.Pdf.Kit for .NET v2.6.0.0, please **click here**.  

**Aspose.Words for Java v2.3.0.0 Released**

Aspose has published a maintenance release of **[Aspose.Words][6]** for Java that includes a Java version of all those bug fixes that were made in the .NET versions (v4.2.2 to v4.3.1) of Aspose.Words. Moreover, many other improvements are also made in this release related to footnotes, file size optimization and the import of DOC & HTML files. For more details, please **visit** its official release page.

**Latest Enhancements in Aspose.Network v3.5.3.0**

With the addition of many new features and important enhancements, [**Aspose.Network**][7] v3.5.3.0 has just got better. New features include the support of saving linked resources of email messages locally, adding performance counters (like number of emails sent or failed etc.) for sending bulk emails, dragging & dropping files from windows explorer and launching Outlook email client with attachments etc. Besides new features and enhancements, some important bugs are also fixed in this release. To get more details about the improvements made in Aspose.Network for .NET v3.5.3.0, please **click here**.

**Aspose.Words for Reporting Services now supports DOCX format too**

It is a great pleasure to announce that **[Aspose.Words for Reporting Services][8]** now also supports exporting RDL reports to Microsoft Office 2007 Open XML format (DOCX). So, developers can generate reports in any of the four Microsoft Word formats: DOC, RTF, WordML and DOCX. To get more details about these features and other improvements made in Aspose.Words for Reporting Services, please check its **official release** page.  
  

**Technical Tip**

****Change page orientation in RDL reports exported to Word documents**  
**  
From time to time, our customers ask us to add certain configuration settings for customizing the export of RDL reports to Microsoft Word documents via **[Aspose.Words for Reporting Services][9]**. So, today we are going to talk about the page orientation setting.  
  
Suppose, you have a report containing a wide table or matrix whose right part goes beyond the edge of the page. Microsoft renderers such as PDF would wrap the table to the next page but we don’t consider this as a neat approach because such report, when printed, might confuse the reader. Basically, this is a signal to the report’s designer that the report should be reworked. But, using Aspose.Words for Reporting Services, you can simply instruct the renderer to change page orientation from portrait to landscape. Unless the table is enormously wide, this trick should remedy the explained problem.  
  
To change page orientation, please add the following lines to the _C:\\Program Files\\Microsoft SQL Server\\<Instance>\\Reporting Services\\ReportServer\\rsreportserver.config_ file (the example is for the DOC renderer):  
  

<Render>  
   …  
        <Extension Name="AWDOC" Type="Aspose.Words.ReportingServices.DocRenderer,Aspose.Words.ReportingServices">  
                <Configuration>  
                        <DeviceInfo>  
**                                <PageOrientation>Landscape</PageOrientation>**  
                        </DeviceInfo>  
                </Configuration>  
        </Extension>  
</Render>  
  

**Aspose.Pdf for .NET v3.5.8.0 Mega Hotfix**

In the month of August, 2007, the **[Aspose.Pdf][10]** team released 3 Mega Hot fixes that provide more than 30 bug fixes related to Word, RTF, HTML & XSL-FO to PDF conversion, margins, sections, underlined tabs, inline HTML, text borders, paragraphs, replaceable symbols, footnotes, text alignment and formatting etc. Be sure to check out the full list of these bug fixes through their official release pages (**1st**, **2nd** and **3rd** Mega Hot fixes). Please **[download][11]** the latest release (as it also includes the bug fixes of previous releases) now to make your applications work better using Aspose.Pdf.




[1]: http://www.aspose.com/Products/Aspose.BarCode.Reporting.Services/
[2]: http://www.aspose.com/Products/Aspose.BarCode.Reporting.Services/
[3]: http://www.aspose.com/Community/Files/52/aspose.barcode.reporting.services/default.aspx
[4]: http://www.aspose.com/Community/Files/51/aspose.words/default.aspx
[5]: http://www.aspose.com/Community/Files/51/aspose.pdf.kit/default.aspx
[6]: http://www.aspose.com/Community/Files/51/aspose.words/default.aspx
[7]: http://www.aspose.com/Community/Files/54/aspose.network/default.aspx
[8]: http://www.aspose.com/Community/Files/52/aspose.words.reporting.services/default.aspx
[9]: http://www.aspose.com/Products/Aspose.Words.Reporting.Services/
[10]: https://products.aspose.com/pdf
[11]: http://www.aspose.com/Community/Files/51/aspose.pdf/default.aspx




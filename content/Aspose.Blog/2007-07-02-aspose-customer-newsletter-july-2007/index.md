---
title: 'Aspose Customer Newsletter, July 2007'
date: Mon, 02 Jul 2007 05:07:00 +0000
draft: false
url: /2007/07/02/aspose-customer-newsletter-july-2007/
author: Salman Ehsan
summary: ''
tags: ['Customer Newsletters']
---

**In This Issue...**

*   **Welcome!**
*   **Product Spotlight –[Aspose.Network][1]**
*   **Aspose.Cells for Java 1.8.2 Released**
*   **Use Aspose.Words for Reporting Services on SQL Server 2000 & 2005**
*   **Aspose.Slides 1.7.4.0 for Java developers**
*   **Export & Import to and from Excel 2007 using Aspose.Cells for .NET**
*   **Technical Tip – Visibility of Headers & Footers on slides after cloning**
*   **Aspose.Pdf for .NET 3.5.1.0 Released**
*   **Aspose.Words for .NET 4.2.6 Mega Hotfix**

**Welcome**

Welcome to the July 2007 issue of the Aspose Newsletter! In this month’s newsletter, we will provide some introductory information about our spotlight product: Aspose.Network. We will also look at the new and exciting features offered in the recent releases of Aspose.Cells, Aspose.Words for Reporting Services, Aspose.Pdf, Aspose.Slides and Aspose.Words. You will learn about the latest news from Aspose along with the monthly Tech-Tip, which demonstrates how you can deal with the visibility issue of headers & footers after cloning slides using Aspose.Slides.

**Product Spotlight**

[Aspose.Network][2] is a suite of flexible and easy to use .NET components combined together to produce a most unique & powerful component ever introduced in the market by any component vendor. Aspose.Network takes you to the depths of complex network programming concepts in an easiest way to save your time and efforts. Aspose.Network implements a long series of network protocols (like **SMTP, MIME, POP3, FTP, WhoIs, DNS, ICMP** & **IMAP** etc.) to allow developers for creating a huge variety of network applications without plunging themselves into the complexities of network protocol details.  
  
Aspose.Network can be used by developers to perform a variety of tasks in their applications. For example, opening or saving emails in the form of EML (.eml) or MHT (.mht) files, parsing Microsoft Outlook Messages (\*.msg), dealing with MIME messages, embedding objects in the email messages, sending bulk emails, creating emails using mail merge feature with different types of data sources like DataTable & DataReader etc., sending iCalendar compliant messages, working in asynchronous mode, receiving and managing emails using POP3, uploading, downloading & managing files on servers using File Transfer Protocol (FTP), retrieving domains information from WhoIs servers, querying domains in synchronous or asynchronous modes using DNS protocol, sending & receiving Pings in synchronous or asynchronous modes, processing ICMP messages, connecting to Microsoft Outlook Express for accessing and managing emails using Internet Message Access Protocol (IMAP), verifying email addresses & penetrating through different types of proxies etc. Please [download][3] the free evaluation version of Aspose.Network to see how it fulfills your business needs.  
 

[![][4]](https://downloads.aspose.com/)[](https://docs.aspose.com/display/diagramjava/How+to+Convert+a+Visio+Diagram)

**Aspose.Cells for Java 1.8.2 Released**

There are many enhancements and bug fixes that are made in the recent release of [Aspose.Cells][5] for Java 1.8.2. These enhancements include the support of linking text box in the chart to the cell, setting scatter x-axis value of the chart, handling the font of comments loaded from a template file and optimization of auto-fit feature. Few bugs are also fixed related to opening files, formula calculation, saving CSV files, copying & removing sheets etc. To get more details about this new release of Aspose.Cells for Java, please [click here][6].  
   

**Use Aspose.Words for Reporting Services on SQL Server 2000 & 2005**

We are happy to announce a new release of [Aspose.Words for Reporting Services][7]. In this release, there are many improved features but the most important feature is the support of Microsoft SQL Server 2000 Reporting Services. In earlier versions, only MS SQL Server 2005 Reporting Services was supported but now developers have full freedom to generate DOC, RTF and WordprocessingML (also known as WordML) reports on both versions of MS SQL Server. For more details, please [visit][8] the official release page of Aspose.Words for Reporting Services 1.2.0.  

[![][9]](https://docs.aspose.com/display/diagramjava/How+to+Convert+a+Visio+Diagram)[](https://downloads.aspose.com/pdf)

**Aspose.Slides 1.7.4.0 for Java developers**

With the addition of few nice features and many important enhancements, [Aspose.Slides][10] for Java 1.7.4.0 has just got better. Now, developers can create and read extended bullets on notes. It is also possible to extract embedded text files (and other _**native**_ documents, which don’t have special OLE server) from PowerPoint presentations. Moreover, almost 10 bugs are also fixed related to notes, PowerPoint 2007 presentations (containing tables), presentations with notes and without paragraphs, SVG export, thumbnails & cloning etc. To get more details about the improvements made in Aspose.Slides for Java 1.7.4.0, please [click here][11].

[![][12]](https://downloads.aspose.com/)[](https://downloads.aspose.com/barcode)

**Export & Import to and from Excel 2007 using Aspose.Cells for .NET**

In [Aspose.Cells][13] for .NET 4.3.0, the support of Excel 2007 is also added. Currently, developers can only export & import their data and formatting to & from Excel 2007 files. However, in coming releases, Aspose.Cells will provide the full support of Excel 2007. There are also some other improvements made in Aspose.Cells like the support of page setup settings of header & footer in Excel to PDF conversion and optimizations in formula calculation engine & chart to image feature. Few bugs related to Excel to PDF conversion, conditional formatting and checkbox are also fixed. To get more details about these improvements, please [click here][14].  
  

[![][15]](https://downloads.aspose.com/cells)[](https://downloads.aspose.com/barcode)

**Technical Tip**

**Visibility of Headers & Footers on slides after cloning  
**  
One of the most common uses of Aspose.Slides is building large multi-slide presentations from separate slides. This operation is also documented in the Programmer's Guide of Aspose.Slides. However, from time to time, slides lose their headers, footers, dates and page numbers. The reason is very simple. The information about the visibility of these fields is stored in the main header of the presentation instead of slide or master slide. So, to clone slides with headers and footers, it's necessary to add one more step. This step is to add a small method (whose code is given below) to your application and call it by providing source and destination slide parameters after the cloning of each slide.  
  
  
  
\[C#\]  
  
  
//Implementation of method (taking source & destination slides as parameters) to control the  
//visibility of headers & footers  
public void InheritHeadersFootersVisibility(Slide srcSlide, Slide dstSlide)  
{  
    //Accessing the headers & footers of source and destination slides  
    HeaderFooter srcHF = srcSlide.HeaderFooter;  
    HeaderFooter dstHF = dstSlide.HeaderFooter;  
  
    //Assigning the visibility information (about header, footer, page number, date/time) of source  
    //slide to destination slide  
    dstHF.IsHeaderVisible = srcHF.IsHeaderVisible;  
    dstHF.IsFooterVisible = srcHF.IsFooterVisible;  
    dstHF.IsPageNumberVisible = srcHF.IsPageNumberVisible;  
    dstHF.IsDateTimeVisible = srcHF.IsDateTimeVisible;  
    dstHF.IsDateTimeFixed = srcHF.IsDateTimeFixed;  
    dstHF.IsShowOnTitleSlide = srcHF.IsShowOnTitleSlide;  
}  

  
  
\[VB\]  
  
  
‘Implementation of method (taking source & destination slides as parameters) to control the  
‘visibility of headers & footers  
Public  Sub InheritHeadersFootersVisibility(ByVal srcSlide As Slide, ByVal dstSlide As Slide)  
  
    ‘Accessing the headers & footers of source and destination slides  
    Dim srcHF As HeaderFooter =  srcSlide.HeaderFooter  
    Dim dstHF As HeaderFooter =  dstSlide.HeaderFooter  
  
    ‘Assigning the visibility information (about header, footer, page number, date/time) of source  
    ‘slide to destination slide  
    dstHF.IsHeaderVisible = srcHF.IsHeaderVisible  
    dstHF.IsFooterVisible = srcHF.IsFooterVisible  
    dstHF.IsPageNumberVisible = srcHF.IsPageNumberVisible  
    dstHF.IsDateTimeVisible = srcHF.IsDateTimeVisible  
    dstHF.IsDateTimeFixed = srcHF.IsDateTimeFixed  
    dstHF.IsShowOnTitleSlide = srcHF.IsShowOnTitleSlide  
End Sub  

  
  
\[JAVA\]  
  
  
//Implementation of method (taking source & destination slides as parameters) to control the  
//visibility of headers & footers  
public void InheritHeadersFootersVisibility(Slide srcSlide, Slide dstSlide)  
{  
    //Accessing the headers & footers of source and destination slides  
    HeaderFooter srcHF = srcSlide.getHeaderFooter();  
    HeaderFooter dstHF = dstSlide.getHeaderFooter();  
  
    //Assigning the visibility information (about header, footer, page number, date/time) of source  
    //slide to destination slide  
    dstHF.setHeaderVisible(srcHF.isHeaderVisible());  
    dstHF.setFooterVisible(srcHF.isFooterVisible());  
    dstHF.setPageNumberVisible(srcHF.isPageNumberVisible());  
    dstHF.setDateTimeVisible(srcHF.isDateTimeVisible());  
    dstHF.setDateTimeFixed(srcHF.isDateTimeFixed());  
    dstHF.setShowOnTitleSlide(srcHF.isShowOnTitleSlide());  
}  
  
After using the above method in your applications, headers and footers in destination slides will have the same visibility properties like on the source slides.

**Aspose.Pdf for .NET 3.5.1.0 Released**

In the recent release of [Aspose.Pdf][16] for .NET 3.5.1.0, Aspose has provided the support of adding ellipse and round rectangles in PDF documents. Moreover, features like applying rich formatting on list labels and adding vertical lines between MS Word columns are also added. Some important bugs regarding Word to PDF conversion and PDF security are also fixed. For more details, please read the [complete story][17]. In June, 2007, there were few more releases of Aspose.Pdf providing more new features and bug fixes. For updates and complete details, please check [Aspose.Pdf Blog][18].

[![][19]](https://downloads.aspose.com/pdf)[](https://downloads.aspose.com/pdf)

**Aspose.Words for .NET 4.2.6 Mega Hotfix**

In the month of June, 2007, the [Aspose.Words][20] team released a Mega Hotfix that provides plenty of bug fixes related to DOC, PDF and Mail Merge. Some new features are also added to Aspose.Words like the extraction of embedded OLE objects, export of inline images (in word documents) as inline to PDF and support of header & footer from Edge setting. Be sure to check out the [full list][21] of these new features and bug fixes through its official release page. Please [download][22] the latest release now to make your applications work better using Aspose.Words.  
  
 

[![][23]](https://downloads.aspose.com/words)




[1]: https://downloads.aspose.com/
[2]: https://downloads.aspose.com/
[3]: https://downloads.aspose.com/
[4]: https://www.aspose.cloud/templates/aspose/App_Themes/V3/images/total/272x272/aspose_total-for-net.png
[5]: https://downloads.aspose.com/cells
[6]: https://blog.aspose.com/
[7]: https://docs.aspose.com/display/diagramjava/How+to+Convert+a+Visio+Diagram
[8]: https://blog.aspose.com/
[9]: https://www.aspose.com/templates/aspose/App_Themes/V3/images/words/272x272/aspose_words-for-net.png
[10]: https://downloads.aspose.com/
[11]: https://blog.aspose.com/
[12]: https://www.aspose.cloud/templates/aspose/App_Themes/V3/images/slides/272x272/aspose_slides-for-net.png
[13]: https://downloads.aspose.com/cells
[14]: https://blog.aspose.com/
[15]: https://www.aspose.cloud/templates/aspose/App_Themes/V3/images/cells/272x272/aspose_cells-for-net.png
[16]: https://downloads.aspose.com/pdf
[17]: https://blog.aspose.com/
[18]: https://blog.aspose.com/
[19]: https://www.aspose.cloud/templates/aspose/App_Themes/V3/images/pdf/272x272/aspose_pdf-for-net.png
[20]: https://downloads.aspose.com/words
[21]: https://blog.aspose.com/
[22]: https://downloads.aspose.com/words
[23]: https://www.aspose.cloud/templates/aspose/App_Themes/V3/images/slides/272x272/aspose_slides-for-net.png




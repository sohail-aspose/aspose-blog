---
title: 'Aspose Customer Newsletter, June 2007'
date: Fri, 01 Jun 2007 20:57:00 +0000
draft: false
url: /2007/06/01/aspose-customer-newsletter-june-2007/
author: Salman Ehsan
summary: ''
tags: ['Customer Newsletters']
---

**In This Issue...**

*   **Welcome!**
*   **Product Spotlight – [Aspose.Chart][1]**
*   **Aspose.BarCode for Java = Aspose.BarCode for .NET**
*   **Aspose.Pdf.Kit for .NET 2.5.1.0 is published with improved features**
*   **Aspose.Network now supports parsing Microsoft Outlook Message documents**
*   **Technical Tip – Speed up Word to PDF conversion**
*   **A powerful release of Aspose.Pdf.Kit 1.8.0.0 for Java developers**
*   **Aspose.Words for .NET 4.2.5 Mega Hotfix**

**Welcome**

  
Welcome to the June 2007 issue of the Aspose Newsletter! In this month’s newsletter, we will provide some introductory information about our spotlight product: Aspose.Chart. We will also look at the new and exciting features offered in the recent releases of Aspose.BarCode, Aspose.Pdf.Kit, Aspose.Network, Aspose.Pdf and Aspose.Words. You will learn about the latest news from Aspose along with the monthly Tech-Tip, which demonstrates how you can speed up the conversion of Word to PDF documents using Aspose.Words and Aspose.Pdf.

**Product Spotlight**

[Aspose.Chart][2] is a practical, no-frills charting component, which enables .NET applications to create great looking charts of 21 most popular types with some stylish effects including 3D rendering, transparency, gradients and anti-aliasing. The chart types supported by Aspose.Chart include Area, Bar, Bubble, Contour, Candlestick, Cube, Curve, Curve Area, Doughnut, Gantt, High Low Close, Line, Open High Low Close, Pareto, Pie, Pyramid, Point, Radar, Scatter, Step and Surface etc.  
  
Using Aspose.Chart, you can create charts via API, XML or both. You can even export charts to SWF (Adobe Flash) with clickability. Please [download][3] the free evaluation version of Aspose.Chart to see how it fulfills your business needs. To learn more about its usage, please [click here][4].

[![][5]](https://www.aspose.cloud/templates/aspose/App_Themes/V3/images/cells/272x272/aspose_cells-for-net.png)[](https://docs.aspose.com/display/diagramjava/How+to+Convert+a+Visio+Diagram)

**Aspose.BarCode for Java = Aspose.BarCode for .NET**

  
With the recent release of [Aspose.BarCode][6] for Java 1.1.0, now Java developers can enjoy all features of Aspose.BarCode that are available in its .NET version. Aspose.BarCode for Java now supports barcode generation & recognition, web rendering with servlet support and various image formats etc.  
  
There are more than 20 barcode symbologies (including 1D and 2D) supported in Aspose.BarCode for Java that include CodaBar, Code11, Code128, Code39, Code93, EAN128, EAN13, EAN14, EAN8, BooklandEAN, MSI, ITF14, Interleaved2Of5, Planet, Postnet, UPCA, SSCC18, QR, PDF417, DataMatrix and Aztec. To get more details about this new release of Aspose.BarCode for Java, please [click here][7].  
  
 

[![][8]](https://downloads.aspose.com/barcode)[](https://downloads.aspose.com/words)

**Aspose.Pdf.Kit for .NET 2.5.1.0 is published with improved features**

We are happy to announce a new release of [Aspose.Pdf.Kit.][9] In this recent release of Aspose.Pdf.Kit, you will find improved support of annotations, text formatting, AcroForms and PDF to images conversion etc. For more details, please [visit][10] the official release page of Aspose.Pdf.Kit for .NET 2.5.1.0. In the month of May 2007, another release of Aspose.Pdf.Kit was also made that had many other improvements too. You may also get the details about those improvements by clicking [here][11].

[![][12]](https://downloads.aspose.com/pdf)[](https://downloads.aspose.com/pdf)

**Aspose.Network now supports parsing Microsoft Outlook Message documents**

In the recent release of [Aspose.Network][13] 3.5.0.0, Aspose has added the support of parsing Microsoft Outlook Message documents. Using this feature, now developers can read message properties by MAPI property tags, access recipient information, read & save attachments and read OLE objects. Moreover, features like multi-language support and RTF body decompression are also added. For more details, please read the [complete story.  
](https://blog.aspose.com/)

[![][14]](https://downloads.aspose.com/)[](https://downloads.aspose.com/barcode)

**Technical Tip**

  
**Speed up Word to PDF conversion**  
  
A lot of customers have experienced that while converting a Word document to PDF, the conversion process takes a considerable amount of time to complete. In order to speed up this process you should add the following lines of code:  
  
\[C#\]  
  
//Enable the caching of True type font map on disk  
pdf.IsTruetypeFontMapCached = true;  
  
//Set the path of True type font map file  
pdf.TruetypeFontMapPath = System.IO.Path.GetTempPath();  
  
\[VB\]  
  
‘Enable the caching of True type font map on disk  
pdf.IsTruetypeFontMapCached = True  
  
‘Set the path of True type font map file  
pdf.TruetypeFontMapPath = System.IO.Path.GetTempPath()  
  
Above lines should be added before the Aspose.Pdf.Save() method is called. For example:  
  
\[C#\]  
  
//Instantiate the Word Document Object  
Aspose.Words.Document doc = new Aspose.Words.Document("WordDocument.doc");  
  
//Save the Word Document in XML Format that can be handled by Aspose.Pdf  
doc.Save("XMLDocument.xml", SaveFormat.FormatAsposePdf);  
  
//Instantiate a Pdf Document Object  
Aspose.Pdf.Pdf pdf = new Aspose.Pdf.Pdf();  
  
//Bind XML document With Aspose.Pdf Object  
pdf.BindXML("XMLDocument.xml", null);  
  
//Add these two lines to Speed up the conversion  
pdf.IsTruetypeFontMapCached = true;  
pdf.TruetypeFontMapPath = System.IO.Path.GetTempPath();  
  
//Save PDF  
pdf.Save("PDFDocument.pdf");  
  
\[VB\]  
  
'Instantiate the Word Document Object  
Dim doc As Aspose.Words.Document = New Aspose.Words.Document("WordDocument.doc")  
  
'Save the Word Document in XML Format that can be handled by Aspose.Pdf  
doc.Save(“XMLDocument.xml”, SaveFormat.FormatAsposePdf)  
  
'Instantiate a Pdf Document Object  
Dim pdf As Aspose.Pdf.Pdf = New Aspose.Pdf.Pdf()  
  
'Bind XML document With Aspose.Pdf Object  
pdf.BindXML(“XMLDocument.xml”, Nothing)  
  
'Added these two lines to Speed up the conversion  
pdf.IsTruetypeFontMapCached = True  
pdf.TruetypeFontMapPath = System.IO.Path.GetTempPath()  
  
'Save PDF  
pdf.Save("PDFDocument.pdf")  

**A powerful release of Aspose.Pdf.Kit 1.8.0.0 for Java developers**

With the addition of some nice features and few important enhancements, [Aspose.Pdf.Kit][15] for Java 1.8.0.0 has just got better. Now, developers can fill XFA fields in PDF templates without losing any action or script information. It is also possible to extract information about bookmarks & links and draw polygons in existing PDF documents. Moreover, few bugs are also fixed. To get more details about the improvements made in Aspose.Pdf.Kit for Java 1.8.0.0, please [click here][16].

[![][17]](https://downloads.aspose.com/pdf)

**Aspose.Words for .NET 4.2.5 Mega Hotfix**

  
In the month of May 2007, the [Aspose.Words][18] team released 3 Mega Hot fixes that provide about 37 bug fixes related to RTF, DOC, WordML, HTML, PDF and Model. Be sure to check out the full list of these bug fixes through their official release pages ([1st][19], [2nd][20] and [3rd][21] Mega Hotfix). Please [download][22] the latest release (as it also includes the bug fixes of previous releases) now to make your applications work better using Aspose.Words.  
 

[![][23]](https://downloads.aspose.com/words)[](https://downloads.aspose.com/cells)




[1]: https://www.aspose.cloud/templates/aspose/App_Themes/V3/images/cells/272x272/aspose_cells-for-net.png
[2]: https://www.aspose.cloud/templates/aspose/App_Themes/V3/images/cells/272x272/aspose_cells-for-net.png
[3]: https://www.aspose.cloud/templates/aspose/App_Themes/V3/images/cells/272x272/aspose_cells-for-net.png
[4]: https://blog.aspose.com/
[5]: https://www.aspose.cloud/templates/aspose/App_Themes/V3/images/cells/272x272/aspose_cells-for-net.png
[6]: https://downloads.aspose.com/barcode
[7]: https://blog.aspose.com/
[8]: https://www.aspose.cloud/templates/aspose/App_Themes/V3/images/barcode/272x272/aspose_barcode-for-net.png
[9]: https://downloads.aspose.com/pdf
[10]: https://blog.aspose.com/
[11]: https://blog.aspose.com/
[12]: https://www.aspose.com/templates/aspose/App_Themes/V3/images/words/272x272/aspose_words-for-net.png
[13]: https://downloads.aspose.com/
[14]: https://www.aspose.com/templates/aspose/App_Themes/V3/images/words/272x272/aspose_words-for-java.png
[15]: https://downloads.aspose.com/pdf
[16]: https://blog.aspose.com/
[17]: https://www.aspose.com/templates/aspose/App_Themes/V3/images/words/272x272/aspose_words-for-net.png
[18]: https://downloads.aspose.com/words
[19]: https://blog.aspose.com/
[20]: https://blog.aspose.com/
[21]: https://blog.aspose.com/
[22]: https://downloads.aspose.com/words
[23]: https://www.aspose.com/templates/aspose/App_Themes/V3/images/words/272x272/aspose_words-for-net.png




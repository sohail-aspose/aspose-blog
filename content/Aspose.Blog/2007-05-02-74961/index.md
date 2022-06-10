---
title: 'Aspose Customer Newsletter, May 2007'
date: Wed, 02 May 2007 00:10:00 +0000
draft: false
url: /2007/05/02/74961/
author: Salman Ehsan
summary: ''
tags: ['Customer Newsletters']
---

**In This Issue...**

*   **Welcome!**
*   **Product Spotlight – [Aspose.Words for Reporting Services][1]**
*   **Aspose.Editor now works on Web Forms too**
*   **Aspose.Pdf for .NET 3.4.0.0 Released!**
*   **Support of new symbologies is added to Aspose.BarCode**
*   **Technical Tip – Convert XLS file (containing images or charts) to PDF**
*   **Aspose.Cells for .NET has just got better**
*   **Manipulate your PDF documents with an improved version of Aspose.Pdf.Kit**
*   **Aspose.Words for .NET 4.2.2 Mega Hotfix**

**Welcome**

Welcome to the May 2007 issue of the Aspose Newsletter! In this month’s newsletter, we will provide some introductory information about our spotlight product: Aspose.Words for Reporting Services. We will also look at the new and exciting features offered in the recent releases of Aspose.Editor, Aspose.Cells, Aspose.Words, Aspose.Pdf and Aspose.Pdf.Kit. You will learn about the latest news from Aspose along with the monthly Tech-Tip, which demonstrates how you can convert your XLS files (containing images or charts) to PDF documents using Aspose.Cells and Aspose.Pdf.

**Product Spotlight**

[Aspose.Words for Reporting Services][2] is the only solution on the market that makes possible generating true DOC, RTF and WordprocessingML reports in Microsoft SQL Server 2005 Reporting Services. All RDL report features, including tables, matrices, charts and images are converted with the highest degree of precision to Microsoft Word documents.  
  
Microsoft SQL Server 2005 Reporting Services does not have built-in abilities to export reports as Microsoft Word documents, but after installing Aspose.Words for Reporting Services on your server, you will get access to three additional export formats:  
  
• DOC – Microsoft Word Document via Aspose.Words  
• RTF – Rich Text Format via Aspose.Words  
• XML – WordprocessingML via Aspose.Words  
  
Aspose.Words for Reporting Services creates documents on the server without utilizing Microsoft Word. Aspose.Words for Reporting Services internally uses Aspose.Words for .NET – the world-class component for server-side document processing and conversions. Please [download][3] the free evaluation version of Aspose.Words for Reporting Services to see how it fulfills your business needs. To learn more about its usage, please [click here][4].  
 

**Aspose.Editor now works on Web Forms too**

In the recent release of [Aspose.Editor][5] 2.0.0, many improvements are made but the most significant improvement is the support of ASP.NET Web Forms, which means that now developers can read & write RTF, DOC, HTML etc. and use other powerful features of Aspose.Editor in both Windows and Web based applications. For more details, please read the [complete story][6].  
  
 

**Aspose.Pdf for .NET 3.4.0.0 Released!**

We are happy to announce a new release of [Aspose.Pdf][7]. With the new and exciting features of Aspose.Pdf 3.4.0.0, you will find it easier to create quality PDF documents according to your requirements without much coding efforts.  
  
In this recent release of Aspose.Pdf for .NET, you will find improved support for Tables, Footnotes, Floating box, Inline HTML, Text formatting, HTML to PDF, Word to PDF and XSL-FO to PDF etc. For more details, please [visit][8] the official release page of Aspose.Pdf for .NET 3.4.0.0.

[![][9]](https://downloads.aspose.com/pdf)

**Support of new symbologies is added to Aspose.BarCode**

In [Aspose.BarCode][10] 2.3.0, the support of three new barcode symbologies is also added. These barcode symbologies include EAN14 (SCC14), SSCC18 and ITF14. Now, Aspose.BarCode supports 25 barcode symbologies. There are also some other improvements made to Aspose.BarCode. To get more details about these improvements, please [click here][11].  
  
 

[![][12]](https://downloads.aspose.com/barcode)

**Technical Tip**

**Convert XLS file (containing images or charts) to PDF  
**  
Now, Aspose.Cells supports converting XLS files (that contain images and charts) to PDF documents. However, since we use Aspose.Pdf xml file as a medium, to preserve those image files, please save your Aspose.Pdf xml file on disk, not in a stream.  
  
\[C#\]  
  
// Saving an XLS file in Aspose.Pdf xml format  
Workbook wb = new Workbook();  
wb.Open("C:\\\\book1.xls);  
wb.Save("C:\\\\xls2pdf.xml", FileFormatType.AsposePdf);  
  
// Converting XLS file to PDF through Aspose.Pdf using Aspose.Pdf xml file as a medium  
Aspose.Pdf.Pdf pdf = new Aspose.Pdf.Pdf();  
pdf.BindXML("c:\\\\xls2pdf.xml", null);  
pdf.Save("C:\\\\xls2pdf.pdf");  
  
\[VB\]  
  
‘ Saving an XLS file in Aspose.Pdf xml format  
Dim wb as Workbook = new Workbook()  
wb.Open("C:\\book1.xls)  
wb.Save("C:\\xls2pdf.xml", FileFormatType.AsposePdf)  
  
‘ Converting XLS file to PDF through Aspose.Pdf using Aspose.Pdf xml file as a medium  
Dim pdf as Aspose.Pdf.Pdf = new Aspose.Pdf.Pdf()  
pdf.BindXML("c:\\\\xls2pdf.xml", null)  
pdf.Save("C:\\xls2pdf.pdf")  
 

**Manipulate your PDF documents with an improved version of Aspose.Pdf.Kit**

Now, developers can manipulate their PDF documents more easily with the latest release of [Aspose.Pdf.Kit][13] for .NET 2.4.1.0. In this release, several new features are added. These new features include the support of Unicode in stamping, importing and exporting form data as XFA, exporting the content of annotation specified types from PDF to XFDF stream, extracting the content of annotation specified types from an existing PDF document etc. In addition to these new features, few bugs are also fixed in Aspose.Pdf.Kit to make it more secure and powerful. You may review the complete list of these newly added features and bug fixes from the online product announcement by clicking [here][14].

[![][15]](https://downloads.aspose.com/pdf)

**Aspose.Cells for .NET has just got better**

With the addition of some nice features and few important enhancements, [Aspose.Cells][16] 4.2 has just got better. Now, developers can manipulate charts, images and other drawing objects in template files. It is also possible to save charts as images. XLS to PDF conversion is more enhanced to produce better results. Moreover, formula calculation engine is optimized to be more efficient and accurate. To get more details about the improvements made in Aspose.Cells 4.2, please [click here][17].  
 

[![][18]](https://downloads.aspose.com/cells)

**Aspose.Words for .NET 4.2.2 Mega Hotfix**

In the month of April, 2007, the Aspose.Words team released a Mega Hotfix [Aspose.Words][19] 4.2.2 that provides about 16 bug fixes related to RTF, DOC, WordML, HTML, PDF and Mail Merge. Be sure to check out the [full list][20] of these bug fixes. Please [download][21] the latest release now to make your applications work better using Aspose.Words.  
  
 

[![][22]](https://downloads.aspose.com/words)




[1]: https://docs.aspose.com/display/diagramjava/How+to+Convert+a+Visio+Diagram
[2]: https://docs.aspose.com/display/diagramjava/How+to+Convert+a+Visio+Diagram
[3]: https://docs.aspose.com/display/diagramjava/How+to+Convert+a+Visio+Diagram
[4]: https://blog.aspose.com/
[5]: https://downloads.aspose.com/words
[6]: https://blog.aspose.com/
[7]: https://downloads.aspose.com/pdf
[8]: https://blog.aspose.com/
[9]: https://www.aspose.cloud/templates/aspose/App_Themes/V3/images/total/272x272/aspose_total-for-net.png
[10]: https://downloads.aspose.com/barcode
[11]: https://blog.aspose.com/
[12]: https://www.aspose.cloud/templates/aspose/App_Themes/V3/images/cells/272x272/aspose_cells-for-net.png
[13]: https://downloads.aspose.com/pdf
[14]: https://blog.aspose.com/
[15]: https://www.aspose.com/templates/aspose/App_Themes/V3/images/words/272x272/aspose_words-for-net.png
[16]: https://downloads.aspose.com/cells
[17]: https://blog.aspose.com/
[18]: https://www.aspose.cloud/templates/aspose/App_Themes/V3/images/pdf/272x272/aspose_pdf-for-net.png
[19]: https://downloads.aspose.com/words
[20]: https://blog.aspose.com/
[21]: https://downloads.aspose.com/words
[22]: https://www.aspose.cloud/templates/aspose/App_Themes/V3/images/slides/272x272/aspose_slides-for-net.png




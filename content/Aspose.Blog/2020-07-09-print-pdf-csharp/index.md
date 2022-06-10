---
title: 'C# Print PDF Documents Programmatically with .NET'
seoTitle: "C# Print PDF Documents Programmatically with .NET | Printer Page Setting"
description: "Using C#, print a PDF, or multiple PDF in your .NET applications. Print secured PDF and to different page sources, tray or bin. Track Print Progress of PDF."
date: Thu, 09 Jul 2020 23:02:37 +0000
draft: false
url: /2020/07/09/print-pdf-csharp/
author: Farhan Raza
summary: ''
tags: ['C# print pdf', 'paper sources pdf', 'paper tray c#', 'print multiple pdf', 'print pdf c#', 'print progress c#', 'print secured pdf', 'print status c#']
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/printPDF-300x300.png" alt="Print PDF files C#">}}


Many companies are lessening the use of paper to a large extent. However, there are some scenarios where printing is important. For instance, a system may contain details of online order in PDF format. They need to print PDF while dispatching an online order for delivery. They process items on a large scale so printing each document manually could be quite a task. [Aspose.PDF for .NET API][1], in addition to many other file manipulation and conversion features, supports the efficient printing of PDF files. Let us explore the following use cases related to printing PDF files in .NET applications using C#:

*   [Print PDF File with C#][2]
*   [Print Multiple PDF Files with C#][3]
*   [Print Specific Pages of PDF with C#][4]
*   [Print Secured PDF file with C#][5]
*   [Print PDF Pages to Different Paper Trays with C#][6]
*   [Printing Different Page Range to Different Paper Source using C#][7]
*   [Check Print Job Status while Printing PDF with C#][8]

## Print PDF File with C# {#section1}

Printing of PDF files can be automated in your .NET applications using C# or VB.net. You can print PDF files by following the simple steps below:

1.  Create an object of [PdfViewer][9] Class
2.  Load input PDF document
3.  Print the PDF file

The code snippet below shows how to print PDF file using C#:

{{< gist aspose-cloud 7b6fd21096e2fbbda3548cdd8c565b96 "PrintPDF.cs" >}}

## Print Multiple PDF Files with C# {#section2}

If you need to print multiple files because of the nature of your business, then the feature is already supported by Aspose.PDF for .NET API. Printing multiple PDF files, one by one with the above code snippet can be a little slow. Therefore, let us take the PDF printing another step further to make the process easier. Here we will be using List while adding the name of each PDF file to that list. Following steps explain how we will be printing multiple PDF files:

1.  Initialize a List of String type
2.  Add PDF files to list
3.  Load input PDF file
4.  Print multiple PDF files

The code snippet shows how to print multiple PDF files using C#:

{{< gist aspose-cloud 7b6fd21096e2fbbda3548cdd8c565b96 "PrintMultiplePDF.cs" >}}

## Print Specific Pages of PDF with C# {#section3}

The feature of printing specific pages of PDF documents is available in the API. We will be considering an example that includes printing multiple page ranges. You need to specify the from and to page numbers as explained in the steps below:

*   Set the file input and output paths
*   Set printing of specific pages by defining a range
*   Specify parameters of printing
*   Print the pages as specified formerly

The code snippet below shows how to print specific pages of the document using C#:

{{< gist aspose-cloud 7b6fd21096e2fbbda3548cdd8c565b96 "PrintSpecificPages.cs" >}}

## Print Secured PDF file with C# {#section4}

A PDF file can be secured and protected by a password. However, the password could be of two types i.e User and Owner password. The PDF files secured with the user password need a password to open and view the encrypted PDF file. On the other hand, the owner password is required to modify the contents of the secured and password protected PDF file. Following steps explain printing of secure PDF:

1.  Load secured PDF with password
2.  Create [PdfViewer][10] object
3.  Print secured PDF file

Following code snippet shows how to print a secured PDF file using C#:

{{< gist aspose-cloud 7b6fd21096e2fbbda3548cdd8c565b96 "PrintSecuredPDF.cs" >}}

## Print PDF to Specific Paper Tray of a Printer with C# {#section5}

You can print a PDF to specific paper tray with Aspose.PDF for .NET API. For instance, you might want to print a PDF with lot of photos to a different paper tray and textual PDF file to a different paper tray. Follow the steps below to set output tray or bin for printing PDF files:

1.  Load input PDF file
2.  Set attributes for printing
3.  Specify [PageSettings][11] and [PaperSource][12]
4.  Call [PrintDocumentWithSettings][13] method

It is noteworthy here that you can change the name of the printer. Here we will be using Microsoft Print to PDF, as an example. Following code snippet follows these steps and shows how to print a document to a specific paper tray or bin of a printer with C#:

{{< gist aspose-cloud 7b6fd21096e2fbbda3548cdd8c565b96 "PrintPDFspecificTray.cs" >}}

## Printing Page Range to Different Paper Sources using C# {#section6}

There could be scenarios where you might need to print different pages of one PDF document to different paper trays or bin. For instance, a different paper source for the cover page and different for the other pages. You can certainly follow the below steps to print page ranges to different paper sources within the same printing job:

1.  Initialize an object of [PdfViewer][14] class
2.  Use [PdfQueryPageSettings][15] event handler delegate
3.  Set page and printer settings
4.  Call [PrintDocumentWithSettings][16] method

Following code snippet shows how to follow these steps and print different page ranges to different paper sources or trays using C#:

{{< gist aspose-cloud 7b6fd21096e2fbbda3548cdd8c565b96 "PrintPageRange.cs" >}}

## Check Print Job Status while Printing PDF with C# {#section7}

You can print PDF files to different printers. For example, Microsoft Print to PDF, Microsoft XPS Document Writer, or any physical printer. However, the printing can take a long time duration for huge PDF documents or the printing can fail for some reason. Therefore, the API offers a feature that lets you check print job status with the following steps:

1.  Load input PDF file
2.  Specify page settings
3.  Set printer name
4.  Print PDF document with [PrintDocumentWithSettings][17]

Below code snippet shows how to check print job status or print progress of PDF using C#:

{{< gist aspose-cloud 7b6fd21096e2fbbda3548cdd8c565b96 "PrintPDFstatus.cs" >}}

Resultantly, this code snippet prints on the .NET application's console about printing status of the PDF file:



{{< figure align=center src="images/PrintStatus.png" alt="C# Print Pdf">}}


## Conclusion

To sum up, we have learned different approaches and use cases of printing password secured and unsecured PDF files with C# or VB NET in your programming applications. Moreover, we have explored the printing of whole PDF documents. Likewise, we have learned printing some page ranges by specific page trays, bins, or paper sources. Furthermore, we have also checked how to monitor the print status or print progress of documents using C#.

## See Also

[Print PDF Files Programmatically using Java][18]




[1]: https://products.aspose.com/pdf/net
[2]: #section1
[3]: #section2
[4]: #section3
[5]: #section4
[6]: #section5
[7]: #section6
[8]: #section7
[9]: https://apireference.aspose.com/pdf/net/aspose.pdf.facades/pdfviewer
[10]: https://apireference.aspose.com/pdf/net/aspose.pdf.facades/pdfviewer
[11]: https://docs.microsoft.com/en-us/dotnet/api/system.drawing.printing.pagesettings?view=dotnet-plat-ext-3.1
[12]: https://docs.microsoft.com/en-us/dotnet/api/system.drawing.printing.printersettings.papersources?view=netframework-4.7.2
[13]: https://apireference.aspose.com/pdf/net/aspose.pdf.facades/pdfviewer/methods/printdocumentwithsettings/index
[14]: https://apireference.aspose.com/pdf/net/aspose.pdf.facades/pdfviewer
[15]: https://apireference.aspose.com/pdf/net/aspose.pdf.facades/pdfquerypagesettingseventhandler
[16]: https://apireference.aspose.com/pdf/net/aspose.pdf.facades/pdfviewer/methods/printdocumentwithsettings/index
[17]: https://apireference.aspose.com/pdf/net/aspose.pdf.facades/pdfviewer/methods/printdocumentwithsettings/index
[18]: https://blog.aspose.com/2020/11/04/print-pdf-files-programmatically-using-java/






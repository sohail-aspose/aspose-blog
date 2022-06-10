---
title: 'Print PDF Files Programmatically using Java'
seoTitle: "Java Print PDF Files Programmatically | PDF Java Printer API"
description: "You can easily print PDF documents in your Java applications programmatically. Print multiple, specific, page range, or batch print the PDF files."
date: Wed, 04 Nov 2020 12:51:54 +0000
draft: false
url: /2020/11/04/print-pdf-files-programmatically-using-java/
author: Farhan Raza
summary: 'Printing PDF documents is often a key function in different companies and organizations. You can easily print a PDF file programmatically using Java language. You can work with Aspose.PDF for Java API by configuring it in your environment. Let us walk through different PDF printing scenarios that are possible in your Java applications.'
tags: ['Java PDF Print', 'Java PDF Printing', 'Print PDF Java', 'Print PDF using Java', 'Printing PDF Java']
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/Print-PDF-Java.png" alt="Print PDF with Java Programmatically">}}


Printing PDF documents is often a key function in different companies and organizations. You can easily print a PDF file programmatically using Java language. You can work with [Aspose.PDF for Java][1] API by [configuring][2] it in your environment. Let us walk through different PDF printing scenarios that are possible in your Java applications:

*   [Print PDF File using Java][3]
*   [Printing Multiple PDF Documents using Java][4]
*   [Print Specific Pages or Range of Pages using Java][5]
*   [Print Secured PDF using Java][6]
*   [Check Status of Print Task while Printing PDF using Java][7]

## Print PDF File using Java {#section1}

You can easily print a PDF file using Java code by following the steps below:

1.  Create [PdfViewer][8] object
2.  Load input PDF file
3.  Print the PDF file

The code snippet below shows how to print PDF files programmatically using Java:

{{< gist aspose-com-gists 1950ab4331c2c33e324754772996eada "PrintPDF.java" >}}

## Printing Multiple PDF Documents using Java {#section2}

Printing multiple files, or batch printing of PDF files is a simple process using Java language. You can print a number of PDF files by following the steps below:

1.  Initialize a list of String type
2.  Add multiple PDF files to Print
3.  Print PDF documents

The following code shows how to print multiple PDF files using Java language:

{{< gist aspose-com-gists 1950ab4331c2c33e324754772996eada "PrintMultiplePDF.java" >}}

## Print Specific Pages or Range of Pages using Java {#section3}

The API gives you a lot of control while printing PDF files. You can work with different fields and methods while printing files, as per your requirements. For example, if you do not want to print all the pages of a PDF file and only a few pages. It could be some continuous page range like from Page Number 3 till Page Number 7, or these could be random pages like Page Number 1,5 and 6. You can cover both of the scenarios with the following steps:

1.  Initialize [PdfViewer][9] object
2.  Set attributes for printing
3.  Create objects for printer and page settings
4.  Specify if you want to print all pages, specific pages, or a continuous page range
5.  Print PDF document using the printer and page settings

The following code shows how to print specific pages or a range of pages in a PDF document with Java:

{{< gist aspose-com-gists 1950ab4331c2c33e324754772996eada "PrintSpecificpages.java" >}}

## Print Secured PDF using Java {#section4}

Sometimes PDF files are secured or encrypted with passwords in order to ensure authorized access to the data. You can easily access and print the secured or encrypted PDF file using Java code and print the file as per your requirements. You need to follow the steps below:

1.  Load password-protected PDF input file with the password
2.  Initialize [PdfViewer][10] object
3.  Print the PDF document

The code below is based on these steps which explains how to print the secured PDF files using Java code:

{{< gist aspose-com-gists 1950ab4331c2c33e324754772996eada "PrintSecuredPDF.java" >}}

## Check Status of Print Task while Printing PDF using Java {#section5}

You can keep an eye on status of print job after the file is sent to printing queue of the printer. This lets your application decide whether the print has been successful or not. PdfViewer class exposes the method getPrintStatus which helps you to check the status of print job. For example, while printing a PDF to XPS format, you can get the status by following the steps below:

1.  Load input PDF file
2.  Set attributes for printing
3.  Create objects for printer and page settings
4.  Set printer name
5.  Print the output to file
6.  Check the print status

The following code shows how to check status of print task during PDF printing using Java code:

{{< gist aspose-com-gists 1950ab4331c2c33e324754772996eada "PrintingStatus.java" >}}

## Conclusion

We have explored different scenarios related to the printing of PDF files in your Java applications. You can easily integrate these features into your web applications, console applications, or any other type of project you are working with, using Java language. You can explore further the API by learning from [API references][11] or [Product Documentation][12]. There are a lot more possible scenarios related to PDF printing and you can freely discuss with us via [Free Support Forum][13]. We will be glad to help!

## See Also

[Print PDF Files using C# or VB.NET][14]




[1]: https://products.aspose.com/pdf/java
[2]: https://docs.aspose.com/pdf/java/installation/
[3]: #section1
[4]: #section2
[5]: #section3
[6]: #section4
[7]: #section5
[8]: https://apireference.aspose.com/pdf/java/com.aspose.pdf.facades/PdfViewer
[9]: https://apireference.aspose.com/pdf/java/com.aspose.pdf.facades/PdfViewer
[10]: https://apireference.aspose.com/pdf/java/com.aspose.pdf.facades/PdfViewer
[11]: https://apireference.aspose.com/pdf/java
[12]: https://docs.aspose.com/pdf/java/
[13]: https://forum.aspose.com/c/pdf
[14]: https://blog.aspose.com/2020/07/09/print-pdf-csharp/






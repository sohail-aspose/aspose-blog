---
title: 'PDF to Excel Conversion, PDF/A-3, Support of Better JavaScript and Layered PDF Files with Aspose.PDF for Java 9.3.0'
date: Mon, 28 Jul 2014 06:23:35 +0000
draft: false
url: /2014/07/28/convert-pdf-to-excel-pdfa-3-in-java-and-create-layered-pdf-files/
author: Codewarior
summary: ''
tags: ['Nayyer Shahbaz', 'PDF optimization', 'PDF to Excel conversion', 'convert pdf to excel', 'convert pdf to pdfa', 'optimize PDF document in Java', 'pdf to excel']
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/aspose-Pdf-for-Java_100.png">}}


Aspose.Pdf for Java is ported from its sibling Aspose.PDF for .NET, so in every new release, we work to support the same set of features in the Java API as are available in the .NET API. The new release of [Aspose.PDF for Java 9.3.0][1] is a better and enhanced version of the API compared to earlier versions. This new release introduces some great new features, enhancements to existing features and fixes for issues in previously released versions. We always recommend using the latest release of our APIs because they include lots of new enhancements and code optimizations.

## Convert PDF to Excel in Java

In this release, we have introduced the feature to convert a PDF file to a Microsoft Excel workbook, where each individual page in the PDF is rendered as a separate worksheet. To accomplish this requirement, a new class named ExcelSaveOptions has been introduced. The following code snippet shows the steps to convert a PDF file to an Excel workbook. For further details, you may consider reading [Convert PDF to Excel workbook.][2]

```
// Load PDF document
com.aspose.pdf.Document pdfDocument = new com.aspose.pdf.Document("c:/input.pdf");
// Instantiate ExcelSave Option object
com.aspose.pdf.ExcelSaveOptions excelsave = new com.aspose.pdf.ExcelSaveOptions();
// Save the output in XLS format
pdfDocument.save("c:/resultant.xls", excelsave); 
```

## Convert PDF to PDF/A\_3B in Java

PDF to PDF/A conversion has been supported in this API for a while already. To further extend this feature, we have introduced the capability to convert PDF documents to PDF/A\_3B format. For this purpose, a new value, PDF\_A\_3B, has been introduced to the PdfFormat class. For more information, read the [Convert PDF File to PDF/A][3] article.

```
// Load source PDF file
Document doc = new Document("inFile.pdf");
// Convert file to PDF/A_3 format
doc.convert("logFile.txt", PdfFormat.PDF_A_3B, ConvertErrorAction.Delete);
// Save resultnat file
doc.save("outFile.pdf");
```

## PDF Expiration feature

JavaScript is one of the great options available in PDF documents as it provides the capability to call certain features/operations at a particular event. Using JavaScript, we can also set PDF expiration. Please visit the following link for further information on how to [set PDF expiration.][4]

## Add Layers to PDF File in Java

Layers can be useful when you have a multi-lingual file that you want to distribute and want text in each language to appear on different layers, with the background design appearing on a separate layer as well. You might also create documents with animation that appears on a separate layer. One example could be to add a license agreement to your file, and you don’t want a user to view the content until they agree to the terms of the agreement. The latest release of Aspose.Pdf for Java supports adding layers to PDF files (either while creating a new document or manipulating an existing file). In order to accomplish this requirement, a class named Layer is introduced. Please visit the following link for further information about [adding layers to a PDF file.][5]

## Un-embed Fonts from PDF

Fonts are embedded inside a PDF file so that text is displayed properly when the document is viewed on a machine that does not have all of the fonts the PDF contains installed. However, when embedding the fonts, the complete font is included in the PDF and the file size increases. To optimize the size of a PDF file, it is possible to un-embed fonts. To accomplish this requirement, the UnembedFonts(..) method has been introduced to the OptimizationOptions class. If true is passed as an argument to this method, the fonts in the PDF file are no longer embedded. Please visit the following link for further details on how to [optimize PDF file size][6].

## Set Privileges on a PDF using DocumentPrivilege

The DocumentPrivilege class has been introduced to allow users to set PDF access privileges. Using this class, you can allow or prevent users from certain operations on a PDF file. Please take a look at the following article for information on how to [set privileges on an existing PDF file.][7]

As well as the new features mentioned above, this version includes fixes related to converting SVG/PCL/HTML/XPS files to PDF and converting PDF files to image format. Better text and image extraction, general performance improvements when generating PDF files and much more. Go ahead, download and start exploring the new release of [Aspose.PDF for Java 9.3.0.][8]




[1]: https://downloads.aspose.com/pdf/java
[2]: https://docs.aspose.com/display/pdfjava/Convert+PDF+to+Excel+XLS+and+XLSX
[3]: https://docs.aspose.com/display/pdfjava/Convert+PDF+to+other+Formats
[4]: https://docs.aspose.com/display/pdfjava/Manipulate+PDF+Document#ManipulatePDFDocument-SetPDFExpiration
[5]: https://docs.aspose.com/display/pdfjava/Manipulate+PDF+Document#ManipulatePDFDocument-AddLayerstoPDFFile
[6]: https://docs.aspose.com/
[7]: https://docs.aspose.com/
[8]: https://downloads.aspose.com/pdf/java





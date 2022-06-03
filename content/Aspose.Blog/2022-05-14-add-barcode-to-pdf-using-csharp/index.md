---
title: 'Add Barcode to PDF using C#'
date: Sat, 14 May 2022 13:58:36 +0000
draft: false
url: /2022/05/14/add-barcode-to-pdf-using-csharp/
author: 'Muzammil Khan'
summary: 'As a C# developer, you can add a machine-readable barcode image to a PDF document programmatically in .NET applications. In this article, you will learn how to add a barcode to PDF documents and read barcode from PDF using C#.'
tags: ['Add Barcode to PDF', 'Add Barcode to PDF in C#', 'Add QR Code to PDF', 'Add QR Code to PDF C#', 'C# API to Add Barcode to PDF', 'C# Barcode API', 'Embed Barcode in PDF C#', 'Read Barcode from PDF', 'Read Barcode from PDF in C#']
categories: ['Aspose.PDF Product Family', 'Aspose.BarCode Product Family']
---



{{< figure align=center src="images/add-barcode-to-pdf-using-csharp.jpg" alt="Add Barcode to PDF using C#">}}


[PDF][1] is the most popular format for sharing and printing documents. Many organizations use PDF as a standard format for generating reports and sharing other official documents. In certain cases, we may need to embed specific data or information about the document, product, or company as a barcode image in PDF documents. We can add a machine-readable barcode image to a PDF document programmatically in .NET applications. In this article, we will learn **how to add a barcode to PDF documents using C#**.

The article shall cover the following topics:

*   [C# API to Add Barcode to PDF][2]
*   [Create PDF Document and Add Barcode][3]
*   [Add Barcode to Existing PDF Document][4]
*   [Add QR Code to PDF Documents][5]
*   [Read Barcode from PDF Document][6]

## C# API to Add Barcode to PDF {#CSharp-API-to-Add-Barcode-to-PDF}

For adding barcodes to PDF documents, we will follow a two-step procedure. Firstly, we will be using the [Aspose.PDF for .NET][7] API to create or load a PDF document, then we will generate and add the barcode image to the PDF using the [Aspose.BarCode for .NET][8] API. Please either [download][9] the DLLs of the APIs or install them using [NuGet][10].

```
PM> Install-Package Aspose.BarCode
PM> Install-Package Aspose.PDF
```

## Create PDF Document and Add Barcode in C# {#Create-PDF-Document-and-Add-Barcode-in-CSharp}

We can create a new PDF document and add a barcode image to the PDF by following the steps given below:

1.  Firstly, create an instance of the **_[BarcodeGenerator][11]_** class with the _**[EncodeType][12]**_ and text to encode as arguments.
2.  Next, create an instance of the memory stream object
3.  Then, call the [**_Save()_**][13] method to save the barcode image to the memory stream.
4.  Next, create an instance of the **_[Document][14]_** class.
5.  Then, add a **_[page][15]_** to the newly created PDF document.
6.  Next, create an instance of the **_[PdfFileMend][16]_** class.
7.  Then, call the **_[BindPdf()][17]_** method with the **_Document_** object to bind it.
8.  Next, call the **_[AddImage()][18]_** method with the stream object and image position coordinates as arguments.
9.  After that, save the PDF using the **_[Save()][19]_** method. It takes the output PDF file path as an argument.
10.  Finally, call the **_[Close()][20]_** method to close the **_PdfFileMend_** object.

The following code example demonstrates **how to create a new PDF document and add a barcode image using C#**.

{{< gist aspose-barcode-gists f4986b73e3e139a5b105a5a1f2adbe4b "Add-Barcode-to-PDF-CSharp_Add.cs" >}}



{{< figure align=center src="images/Create-PDF-Document-and-Add-Barcode-in-CSharp.jpg" alt="Create PDF Document and Add Barcode in C#." caption="Create PDF Document and Add Barcode in C#.">}}


## Add Barcode to Existing PDF Document in C# {#Add-Barcode-to-Existing-PDF-Document-in-CSharp}

We can also add a barcode image to any page of existing PDF documents. The **_AddImage()_** method allows adding an image to the specified page of the PDF document at specified coordinates. We can insert an image into an existing PDF document by following the steps given below:

1.  Firstly, create an instance of the **_[BarcodeGenerator][21]_** class with the _**[EncodeType][22]**_ and text to encode as arguments.
2.  Next, create an instance of the memory stream object
3.  Then, call the [**_Save()_**][23] method to save the barcode image to the memory stream.
4.  Next, load the PDF document using the **_[Document][24]_** class.
5.  Then, create an instance of the **_[PdfFileMend][25]_** class.
6.  Next, call the **_[BindPdf()][26]_** method with the **_Document_** object to bind it.
7.  Then, call the **_[AddImage()][27]_** method with the stream object, page number, and image position coordinates as arguments.
8.  After that, save the PDF using the **_[Save()][28]_** method. It takes the output PDF file path as an argument.
9.  Finally, call the **_[Close()][29]_** method to close the **_PdfFileMend_** object.

The following code example demonstrates **how to add a barcode image to an existing PDF document using C#**.

{{< gist aspose-barcode-gists f4986b73e3e139a5b105a5a1f2adbe4b "Add-Barcode-to-PDF-CSharp_AddToExisting.cs" >}}



{{< figure align=center src="images/Add-Barcode-to-Existing-PDF-Document-in-CSharp-1024x512.jpg" alt="Add Barcode to Existing PDF Document in C#." caption="Add Barcode to Existing PDF Document in C#.">}}


## Add QR Code to PDF Documents in C# {#Add-QR-Code-to-PDF-Documents-in-CSharp}

Similarly, we can also add a QR code to the PDF documents by following the steps mentioned earlier. However, we just need to set the _**[EncodeType][30]**_ as QR in the first step. We may also need to adjust the image position in step # 7.

The following code example demonstrates **how to add a QR code to a PDF document using C#**.

{{< gist aspose-barcode-gists f4986b73e3e139a5b105a5a1f2adbe4b "Add-Barcode-to-PDF-CSharp_AddQR.cs" >}}



{{< figure align=center src="images/Add-QR-Code-to-PDF-Documents-in-CSharp-1024x512.jpg" alt="Add QR Code to PDF Documents in C#." caption="Add QR Code to PDF Documents in C#.">}}


## Read Barcode from PDF Document using C# {#Read-Barcode-from-PDF-Document-using-CSharp}

We can recognize any barcode image embedded on any of the pages of the PDF document using the [PdfExtractor][31] class. It allows extracting images from PDF, and then we will read the barcode information from the extracted image. We can read barcodes from the PDF documents by following the steps given below:

1.  Firstly, create an instance of the **_[PdfExtractor][32]_** class.
2.  Next, bind the input PDF document using the **_[BindPdf()][33]_** method.
3.  Then, set the page range for image extraction.
4.  Next, call the **_[ExtractImage()][34]_** method to extract the images.
5.  Then, save the image to stream in a loop.
6.  Next, create an instance of the **_[BarCodeReader][35]_** class with image stream and **_[DecodeType][36]_** as arguments.
7.  After that, call the **_[ReadBarCodes()][37]_** method to get the **_[BarCodeResult][38]_** object.
8.  Finally, show the barcode information.

The following code example demonstrates **how to read a barcode image from a PDF document using C#**.

{{< gist aspose-barcode-gists f4986b73e3e139a5b105a5a1f2adbe4b "Add-Barcode-to-PDF-CSharp_Read.cs" >}}

```
Codetext found: Code39Standard
Symbology: 1234567
```

## Get a Free License {#Get-a-Free-API-License}

You can [get a free temporary license][39] to try the library without evaluation limitations.

## Conclusion

In this article, we have learned how to:

*   create a PDF document programmatically;
*   generate and add a barcode image to the PDF in C#;
*   extract images from a PDF document using C#;
*   read barcode image from a PDF document.

Besides, you can learn more about Aspose.BarCode for .NET API using the [documentation][40]. In case of any ambiguity, please feel free to contact us on the [forum][41].

## See Also

*   [Generate Barcode with Logo using C#][42]
*   [Generate and Display Barcode Image in ASP.NET MVC][43]




[1]: https://docs.fileformat.com/pdf/
[2]: #CSharp-API-to-Add-Barcode-to-PDF
[3]: #Create-PDF-Document-and-Add-Barcode-in-CSharp
[4]: #Add-Barcode-to-Existing-PDF-Document-in-CSharp
[5]: #Add-QR-Code-to-PDF-Documents-in-CSharp
[6]: #Read-Barcode-from-PDF-Document-using-CSharp
[7]: https://products.aspose.com/finance/net
[8]: https://products.aspose.com/barcode/net/
[9]: https://downloads.aspose.com/barcode/net
[10]: https://www.nuget.org/packages/aspose.barcode
[11]: https://apireference.aspose.com/barcode/net/aspose.barcode.generation/barcodegenerator
[12]: https://apireference.aspose.com/barcode/net/aspose.barcode.generation/encodetypes
[13]: https://apireference.aspose.com/barcode/net/aspose.barcode.generation.barcodegenerator/save/methods/2
[14]: https://apireference.aspose.com/pdf/net/aspose.pdf/document
[15]: https://apireference.aspose.com/pdf/net/aspose.pdf/page
[16]: https://apireference.aspose.com/pdf/net/aspose.pdf.facades/pdffilemend
[17]: https://apireference.aspose.com/pdf/net/aspose.pdf.facades/facade/methods/bindpdf
[18]: https://apireference.aspose.com/pdf/net/aspose.pdf.facades/pdffilemend/methods/addimage
[19]: https://apireference.aspose.com/pdf/net/aspose.pdf.facades.pdffilemend/save/methods/1
[20]: https://apireference.aspose.com/pdf/net/aspose.pdf.facades/pdffilemend/methods/close
[21]: https://apireference.aspose.com/barcode/net/aspose.barcode.generation/barcodegenerator
[22]: https://apireference.aspose.com/barcode/net/aspose.barcode.generation/encodetypes
[23]: https://apireference.aspose.com/barcode/net/aspose.barcode.generation.barcodegenerator/save/methods/2
[24]: https://apireference.aspose.com/pdf/net/aspose.pdf/document
[25]: https://apireference.aspose.com/pdf/net/aspose.pdf.facades/pdffilemend
[26]: https://apireference.aspose.com/pdf/net/aspose.pdf.facades/facade/methods/bindpdf
[27]: https://apireference.aspose.com/pdf/net/aspose.pdf.facades/pdffilemend/methods/addimage
[28]: https://apireference.aspose.com/pdf/net/aspose.pdf.facades.pdffilemend/save/methods/1
[29]: https://apireference.aspose.com/pdf/net/aspose.pdf.facades/pdffilemend/methods/close
[30]: https://apireference.aspose.com/barcode/net/aspose.barcode.generation/encodetypes
[31]: https://apireference.aspose.com/pdf/net/aspose.pdf.facades/pdfextractor
[32]: https://apireference.aspose.com/pdf/net/aspose.pdf.facades/pdfextractor
[33]: https://apireference.aspose.com/pdf/net/aspose.pdf.facades.pdfextractor/bindpdf/methods/1
[34]: https://apireference.aspose.com/pdf/net/aspose.pdf.facades/pdfextractor/methods/extractimage
[35]: https://apireference.aspose.com/barcode/net/aspose.barcode.barcoderecognition/barcodereader
[36]: https://apireference.aspose.com/barcode/net/aspose.barcode.barcoderecognition/barcodereader/constructors/2
[37]: https://apireference.aspose.com/barcode/net/aspose.barcode.barcoderecognition/barcodereader/methods/readbarcodes
[38]: https://apireference.aspose.com/barcode/net/aspose.barcode.barcoderecognition/barcoderesult
[39]: https://purchase.aspose.com/temporary-license
[40]: https://docs.aspose.com/barcode/net/
[41]: https://forum.aspose.com/c/barcode/13
[42]: https://blog.aspose.com/2022/04/23/generate-barcode-with-logo-using-csharp/
[43]: https://blog.aspose.com/2022/04/04/generate-and-display-barcode-image-in-asp-net-mvc/





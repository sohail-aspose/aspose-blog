---
title: 'Create Barcode in Word Documents using C#'
seoTitle: "Create Barcode in Word using C# | Read Barcode from Word in C#"
description: "Programmatically Create Barcode in Word documents using C# with Aspose.BarCode for .NET API. Recognize and read barcodes from Word documents using C#."
date: Tue, 31 May 2022 08:21:13 +0000
draft: false
url: /2022/05/31/create-barcode-in-word-documents-using-csharp/
author: Muzammil Khan
summary: 'As a C# developer, you can easily generate and add barcode or QR code images to Word documents in .NET applications. In this article, you will learn **how to create barcodes in Word documents programmatically using C#**.'
tags: ['Add Barcode to DOCX in C#', 'Add Barcode to Word C#', 'Add QR Code to Word', 'Add QR Code to Word C#', 'Barcode in Word', 'Create Barcode in Word', 'Create Barcode in Word C#', 'Create Word Document C#', 'Generate Barcode in C#', 'Generate Barcodes', 'Generate QR Code in C#', 'Generate QR Codes', 'How to Create Barcode in Word', 'How to Create Barcode in Word using C#', 'Read Barcode from Word', 'Read Barcode from Word in C#']
categories: ['Aspose.Words Product Family', 'Aspose.BarCode Product Family']
---



{{< figure align=center src="images/create-barcode-in-word-documents-using-csharp.jpg" alt="Create Barcode in Word Documents using C#">}}


Barcodes are images in the form of parallel lines, dots, or rectangles with encoded data/information. The industry professionals embed and access product information, track product movement, and keep up with inventory using barcodes. In certain cases, we may need to generate and add barcodes in MS Word documents. MS Word is the most popular and widely used graphical word processing program. It is used to create new documents with text, images, or graphics, write professional-quality write-ups, edit, and format the existing documents, etc. The [DOCX][1] and [DOC][2] are the popular file formats supported by MS Word. In this article, we will learn **how to create a barcode in Word documents programmatically using C#**.

The following topics shall be covered in this article:

*   [C# API to Create Barcode in Word Documents][3]
*   [Generate and Add Barcode to Word Document][4]
*   [Add Barcode to Existing Word Document][5]
*   [Add QR Code to Word Document][6]
*   [Read Barcode from Word Document][7]

## C# API to Create Barcode in Word Documents {#CSharp-API-to-Create-Barcode-in-Word-Documents}

For generating a barcode and adding a barcode image to Word documents, we will follow a two-step procedure. Firstly, we will be using the [Aspose.Words for .NET][8] API to create or load a Word document, then we will generate and add the barcode image to the document using the [Aspose.BarCode for .NET][9] API. The _[Document][10]_ class of the Aspose.Words for .NET API allows creating a new Word document or loading an existing Word file in the application. The _[Save()][11]_ method of this class saves the document on the given file path. The _[DocumentBuilder][12]_ class of the API provides methods for building a document. It provides various overloaded _[InsertImage()][13]_ methods to insert an image in the document.

The Aspose.BarCode for .NET API allows generating various [types of supported barcodes][14]. For this purpose, it provides the _[BarcodeGenerator][15]_ class to generate the barcode of the specified _[EncodeType][16]_. We can save the generated barcode image using the [_Save()_][17] method of this class. The API also provides the _[BarCodeImageFormat][18]_ enumeration to specify the save formats. We can read the barcode from images using the _[BarCodeReader][19]_ class of the API.

Please either [download][20] the DLLs of the APIs or install them using [NuGet][21].

```
PM> Install-Package Aspose.BarCode
PM> Install-Package Aspose.Words
```

## Generate and Add Barcode to Word Document in C# {#Generate-and-Add-Barcode-to-Word-Document-in-CSharp}

We can create a new Word document and add a barcode image to the document by following the steps given below:

1.  Firstly, create an instance of the **_BarcodeGenerator_** class. It takes the _**EncodeType**_ and text to encode as arguments.
2.  Next, create an instance of the memory stream object.
3.  Then, call the **_Save()_** method to save the barcode image to the memory stream.
4.  Next, create an instance of the **_Document_** class.
5.  Then, initialize an instance of the **_DocumentBuilder_** class with the Document object.
6.  After that, insert the barcode image using the **_[InsertImage()][22]_** method with the stream object as an argument.
7.  Finally, call the **_Save()_** method. It takes the output DOCX file path as an argument.

The following code example shows **how to generate and add a barcode to a new Word document using C#**.

{{< gist aspose-barcode-gists 28a680aa9f1add7c9bab0b69b70bb690 "Create-Barcode-in-Word-CSharp_Add.cs" >}}



{{< figure align=center src="images/Generate-and-Add-Barcode-to-Word-Document-in-CSharp.jpg" alt="Generate and add Barcode to a new Word document in C#." caption="Generate and add Barcode to a new Word document in C#.">}}


## Add Barcode to Existing Word Document in C# {#Add-Barcode-to-Existing-Word-Document-in-CSharp}

We can generate and add a barcode image to any existing Word document by following the steps given below:

1.  Firstly, create an instance of the **_BarcodeGenerator_** class with the _**EncodeType**_ and text to encode as arguments.
2.  Next, create an instance of the memory stream object.
3.  Then, call the **_Save()_** method to save the barcode image to the memory stream.
4.  Next, load an existing Word document using the **_Document_** class.
5.  Then, initialize an instance of the **_DocumentBuilder_** class with the Document object.
6.  After that, insert the barcode image using the **_[InsertImage()][23]_** method with the stream object and its position as arguments.
7.  Finally, call the **_Save()_** method. It takes the output DOCX file path as an argument.

The following code example shows **how to generate and add a barcode to an existing Word document using C#**.

{{< gist aspose-barcode-gists 28a680aa9f1add7c9bab0b69b70bb690 "Create-Barcode-in-Word-CSharp_AddToExisting.cs" >}}



{{< figure align=center src="images/Add-Barcode-to-Existing-Word-Document-in-CSharp-1024x564.jpg" alt="Add Barcode to Existing Word Document in C#." caption="Add Barcode to Existing Word Document in C#.">}}


## Add QR Code to Word Document using C# {#Add-QR-Code-to-Word-Document-using-CSharp}

Similarly, we can also generate a QR code image and add it to the Word document by following the steps mentioned earlier. However, we just need to set the _**EncodeType**_ as _**QR **_or **_GS1QR_** in the first step. We may also need to adjust the image position in step 6.

The following code example demonstrates **how to add a QR code to a Word document using C#**.

{{< gist aspose-barcode-gists 28a680aa9f1add7c9bab0b69b70bb690 "Create-Barcode-in-Word-CSharp_AddQR.cs" >}}



{{< figure align=center src="images/Add-QR-Code-to-Word-Document-using-CSharp.jpg" alt="Add QR Code to Word Document using C#." caption="Add QR Code to Word Document using C#.">}}


## Read Barcode from Word Document using C# {#Read-Barcode-from-Word-Document-using-CSharp}

We can recognize any barcode image available on any page of the Word document by following the steps given below:

1.  Firstly, load an existing Word document using the **_Document_** class.
2.  Next, access the **_[NodeCollection][24]_** of _[Shape][25]_ types using the **_[GetChildNodes()][26]_** method.
3.  Then, loop through all the shapes and check if the shape is an image.
4.  Next, save the image to the stream.
5.  Then, create an instance of the **_BarCodeReader_** class with image stream and **_[DecodeType][27]_** as arguments.
6.  After that, call the **_[ReadBarCodes()][28]_** method to get the **_[BarCodeResult][29]_** object.
7.  Finally, show the barcode information.

The following code example shows **how to read a barcode image from a Word document using C#**.

{{< gist aspose-barcode-gists 28a680aa9f1add7c9bab0b69b70bb690 "Create-Barcode-in-Word-CSharp_ReadBarcode.cs" >}}

```
Codetext found: 1234567890, Symbology: Code39Standard
```

## Get a Free License {#Get-a-Free-API-License}

You can [get a free temporary license][30] to try the library without evaluation limitations.

## Conclusion

In this article, we have learned how to:

*   create a Word document programmatically;
*   generate a barcode image and add it to the Word document;
*   create a QR code and insert it into a Word document;
*   read a barcode image from a Word document in C#.

Besides, you can learn more about Aspose.BarCode for .NET API using the [documentation][31]. In case of any ambiguity, please feel free to contact us on the [forum][32].

## See Also

*   [Generate Barcode in Excel using C#][33]
*   [Add Barcode to PDF using C#][34]
*   [Generate Barcode with Logo using C#][35]
*   [Generate and Display Barcode Image in ASP.NET MVC][36]




[1]: https://docs.fileformat.com/word-processing/docx/
[2]: https://docs.fileformat.com/word-processing/doc/
[3]: #CSharp-API-to-Create-Barcode-in-Word-Documents
[4]: #Generate-and-Add-Barcode-to-Word-Document-in-CSharp
[5]: #Add-Barcode-to-Existing-Word-Document-in-CSharp
[6]: #Add-QR-Code-to-Word-Document-using-CSharp
[7]: #Read-Barcode-from-Word-Document-using-CSharp
[8]: https://products.aspose.com/words/net
[9]: https://products.aspose.com/barcode/net/
[10]: https://apireference.aspose.com/words/net/aspose.words/document/
[11]: https://apireference.aspose.com/words/net/aspose.words/document/save
[12]: https://apireference.aspose.com/words/net/aspose.words/documentbuilder/
[13]: https://apireference.aspose.com/words/net/aspose.words/documentbuilder/insertimage/
[14]: https://docs.aspose.com/barcode/net/barcode-types-and-image-formats/
[15]: https://apireference.aspose.com/barcode/net/aspose.barcode.generation/barcodegenerator
[16]: https://apireference.aspose.com/barcode/net/aspose.barcode.generation/encodetypes
[17]: https://apireference.aspose.com/barcode/net/aspose.barcode.generation.barcodegenerator/save/methods/2
[18]: https://apireference.aspose.com/barcode/net/aspose.barcode.generation/barcodeimageformat/
[19]: https://apireference.aspose.com/barcode/net/aspose.barcode.barcoderecognition/barcodereader
[20]: https://downloads.aspose.com/barcode/net
[21]: https://www.nuget.org/packages/aspose.barcode
[22]: https://apireference.aspose.com/words/net/aspose.words/documentbuilder/insertimage
[23]: https://apireference.aspose.com/words/net/aspose.words/documentbuilder/insertimage
[24]: https://apireference.aspose.com/words/net/aspose.words/nodecollection/
[25]: https://apireference.aspose.com/words/net/aspose.words/nodetype/
[26]: https://apireference.aspose.com/words/net/aspose.words/compositenode/getchildnodes
[27]: https://apireference.aspose.com/barcode/net/aspose.barcode.barcoderecognition/barcodereader/constructors/2
[28]: https://apireference.aspose.com/barcode/net/aspose.barcode.barcoderecognition/barcodereader/methods/readbarcodes
[29]: https://apireference.aspose.com/barcode/net/aspose.barcode.barcoderecognition/barcoderesult
[30]: https://purchase.aspose.com/temporary-license
[31]: https://docs.aspose.com/barcode/net/
[32]: https://forum.aspose.com/c/barcode/13
[33]: https://blog.aspose.com/2022/05/26/generate-barcode-in-excel-using-csharp/
[34]: https://blog.aspose.com/2022/05/14/add-barcode-to-pdf-using-csharp/
[35]: https://blog.aspose.com/2022/04/23/generate-barcode-with-logo-using-csharp/
[36]: https://blog.aspose.com/2022/04/04/generate-and-display-barcode-image-in-asp-net-mvc/





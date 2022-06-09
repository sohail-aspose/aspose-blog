---
title: 'Add QR Code to PowerPoint Presentation using C#'
seoTitle: "Add QR Code to PowerPoint Presentation using C#"
description: "Programmatically add QR code to PowerPoint presentation using C# with Aspose.BarCode for .NET API. Recognize and read barcodes from presentation using C#."
date: Thu, 02 Jun 2022 17:28:17 +0000
draft: false
url: /2022/06/02/add-qr-code-to-powerpoint-presentation-using-csharp/
author: Muzammil Khan
summary: 'As a C# developer, you can easily generate QR codes or barcodes and add to PowerPoint presentations programmatically without using MS PowerPoint. In this article, you will learn **how to add QR code to a PowerPoint presentation using C#**.'
tags: ['Add QR Code to Presentation', 'How to Create QR Code for PPT', 'QR Code PPT', 'QR Code PPTX', 'QR Code in C#', 'QR Code to PPTX C#', 'Read QR Code C#', 'Slide QR Code']
categories: ['Aspose.Slides Product Family', 'Aspose.BarCode Product Family']
---



{{< figure align=center src="images/add-qr-code-to-powerpoint-presentation-using-csharp.jpg" alt="Add QR Code to PowerPoint Presentation using C#">}}


PowerPoint is a popular tool used to present information in the form of a slide show. Where each slide contains specific information/ data in the form of text, list, image, video, graphs, etc. In a PowerPoint presentation, we can embed any specific URL, presenter's social media account link, or an email address using a QR code. So that, people with a QR reader on their smartphone can capture the URL without having to write it down. In this article, we will learn **how to add a QR code to a PowerPoint presentation using C#**.

The following topics shall be covered in this article:

*   [What is QR Code][1]
*   [C# API to Add QR Code to PowerPoint Presentation][2]
*   [Generate QR Code and Add to Presentation][3]
*   [Add QR Code to Existing Presentation][4]
*   [Add Barcode to PowerPoint Presentation][5]
*   [Read QR Code from Presentation][6]

## What is QR Code {#What-is-QR-Code}

A (Quick Response) **QR** code is a type of matrix barcode consisting of an array of black and white squares. As the name shows, the QR code allows the users to access information instantly when scanned. It is used to store encoded alphanumeric information that can be decoded by QR code readers available on digital devices, such as cell phones.

## C# API to Add QR Code to PowerPoint Presentation {#CSharp-API-to-Add-QR-Code-to-PowerPoint-Presentation}

For generating a QR code and adding it to [PPT][7] or [PPTX][8] files, we will follow a two-step procedure. Firstly, we will be using the [Aspose.Slides for .NET][9] API to create or load a PowerPoint presentation, then we will generate and add the QR code image to the presentation slides using the [Aspose.BarCode for .NET][10] API.

Aspose.Slides for .NET API enables to read, write, protect, modify and convert presentations of the [supported formats][11] in .NET applications without using MS PowerPoint. It offers various classes to perform different operations. The _[Presentation][12]_ class of the API allows creating a new presentation or loading an existing presentation file in the application. The _[Save()][13]_ method of this class saves the presentation in the provided format on the given file path. The _[ISlide][14]_ interface of the API represents a slide in a presentation.

We will be using the Aspose.BarCode for .NET API to generate a QR code. It allows generating various [types of supported barcodes][15]. For this purpose, it provides the _[BarcodeGenerator][16]_ class to generate the QR code or barcode of the specified _[EncodeType][17]_. We can save the generated QR/barcode image using the [_Save()_][18] method of this class. The API also provides the _[BarCodeImageFormat][19]_ enumeration to specify the save formats. We can read the barcode or QR code from images using the _[BarCodeReader][20]_ class of the API.

Please either [download][21] the DLLs of the APIs or install them using [NuGet][22].

```
PM> Install-Package Aspose.BarCode
PM> Install-Package Aspose.Cells
```

## Generate and Add QR Code to Presentation in C# {#Generate-and-Add-QR-Code-to-Presentation-in-CSharp}

We can create a new presentation and add a QR code image to the presentation slide by following the steps given below:

1.  Firstly, create an empty presentation using the **_Presentation_** class.
2.  Next, create an instance of the **_BarcodeGenerator_** class. It takes the _**Encode Type**_ as an argument.
3.  Then, add text to encode and set other optional barcode properties.
4.  Next, create an instance of the memory stream object.
5.  Then, call the **_**_BarcodeGenerator_**_**.**_Save()_** method to save the QR code image to the memory stream.
6.  Next, call the _[AddImage()][23]_ method to add the image to the presentation's _[image][24]_ collection.
7.  Then, call the _[InsertEmptySlide()][25]_ method to insert an empty slide at the specified index with a title layout.
8.  Next, get the newly inserted slide by its index.
9.  After that, insert the QR code image on the slide using the _[AddPictureFrame()][26]_ method.
10.  Optionally, set the picture frame formatting such as fill type, color, width, rotation, etc.
11.  Finally, call the **_**_Presentation_**_**.**_Save()_** method. It takes the output PPTX file path and the _[SaveFormat][27]_ as arguments.

The following code example shows **how to generate and add a QR to a new presentation slide using C#**.

{{< gist aspose-barcode-gists 2b24e05386bd287ef917e56cbe04b282 "Add-QR-Code-to-Presentation-CSharp_AddQR.cs" >}}



{{< figure align=center src="images/generate-and-add-qr-code-to-presentation-using-csharp-1024x758.jpg" alt="Generate and Add QR Code to Presentation in C#" caption="Generate and Add QR Code to Presentation in C#.">}}


## Add QR Code to Existing Presentation in C# {#Add-QR-Code-to-Existing-Presentation-in-CSharp}

We can load an existing presentation and add a QR code image by following the steps given below:

1.  Firstly, load an existing presentation using the **_Presentation_** class.
2.  Next, create an instance of the **_BarcodeGenerator_** class. It takes the _**Encode Type**_ and text to encode as arguments.
3.  Then, create an instance of the memory stream object.
4.  After that, call the **_**_BarcodeGenerator_**_**.**_Save()_** method to save the QR code image to the memory stream.
5.  Next, call the _[AddImage()][28]_ method to add the image to the presentation's _[image][29]_ collection.
6.  Then, get the specific slide by its index.
7.  After that, insert the QR code image on the slide using the _[AddPictureFrame()][30]_ method.
8.  Finally, call the **_**_Presentation_**_**.**_Save()_** method. It takes the output PPTX file path and the _[SaveFormat][31]_ as arguments.

The following code example shows **how to generate and add a QR to an existing presentation using C#**.

{{< gist aspose-barcode-gists 2b24e05386bd287ef917e56cbe04b282 "Add-QR-Code-to-Presentation-CSharp_AddQRToExisting.cs" >}}



{{< figure align=center src="images/add-qr-code-to-existing-presentation-using-csharp-1024x496.jpg" alt="Add QR Code to Existing Presentation in C#" caption="Add QR Code to Existing Presentation in C#.">}}


## Add Barcode to PowerPoint Presentation in C# {#Add-Barcode-to-PowerPoint-Presentation-in-CSharp}

Similarly, we can also generate a barcode code image and add it to the presentation by following the steps mentioned earlier. However, we just need to set the _**EncodeType**_ other than _**QR **_or **_GS1QR_** in the second step. We may also need to adjust the image position in step 7.

The following code example demonstrates **how to add a barcode to a PowerPoint presentation using C#**.

{{< gist aspose-barcode-gists 2b24e05386bd287ef917e56cbe04b282 "Add-QR-Code-to-Presentation-CSharp_AddBarcode.cs" >}}



{{< figure align=center src="images/add-barcode-to-presentation-using-csharp-1024x832.jpg" alt="Add Barcode to PowerPoint Presentation in C#." caption="Add Barcode to PowerPoint Presentation in C#.">}}


## Read QR Code from Presentation in C# {#Read-QR-Code-from-Presentation-in-CSharp}

We can recognize any barcode or QR code image available on any of the slides in the presentation by following the steps given below:

1.  Firstly, load an existing presentation using the **_Presentation_** class.
2.  Next, loop through all the images in the presentation's image collection.
3.  Then, save the image to the stream.
4.  Next, create an instance of the **_BarCodeReader_** class with image stream and **_[DecodeType][32]_** as arguments.
5.  After that, call the **_[ReadBarCodes()][33]_** method to get the **_[BarCodeResult][34]_** object.
6.  Finally, show the QR code information.

The following code example shows **how to read a QR code image from a presentation using C#**.

{{< gist aspose-barcode-gists 2b24e05386bd287ef917e56cbe04b282 "Add-QR-Code-to-Presentation-CSharp_ReadQRCode.cs" >}}

```
Codetext found: https://www.aspose.com
Symbology: QR
```

## Get a Free License {#Get-a-Free-API-License}

You can [get a free temporary license][35] to try the library without evaluation limitations.

## Conclusion

In this article, we have learned how to:

*   create a PowerPoint presentation programmatically;
*   add a new slide in the presentation with a predefined slide layout;
*   generate a QR code image and add it to the presentation;
*   create a barcode and insert it into the presentation;
*   read a QR image from a PowerPoint presentation using C#.

Besides, you can learn more about **_Aspose.BarCode for .NET_** API using the [documentation][36]. In case of any ambiguity, please feel free to contact us on the [forum][37].

## See Also

*   [Create Barcode in Word using C#][38]
*   [Generate Barcode in Excel using C#][39]
*   [Add Barcode to PDF using C#][40]
*   [Generate Barcode with Logo using C#][41]
*   [Generate and Display Barcode Image in ASP.NET MVC][42]




[1]: #What-is-QR-Code
[2]: #CSharp-API-to-Add-QR-Code-to-PowerPoint-Presentation
[3]: #Generate-and-Add-QR-Code-to-Presentation-in-CSharp
[4]: #Add-QR-Code-to-Existing-Presentation-in-CSharp
[5]: #Add-Barcode-to-PowerPoint-Presentation-in-CSharp
[6]: #Read-QR-Code-from-Presentation-in-CSharp
[7]: https://docs.fileformat.com/presentation/ppt/
[8]: https://docs.fileformat.com/presentation/pptx/
[9]: https://products.aspose.com/slides/net
[10]: https://products.aspose.com/barcode/net/
[11]: https://docs.aspose.com/slides/net/supported-file-formats/#supported-file-formats
[12]: https://apireference.aspose.com/slides/net/aspose.slides/presentation/
[13]: https://apireference.aspose.com/slides/net/aspose.slides/presentation/save/
[14]: https://apireference.aspose.com/slides/net/aspose.slides/islide/
[15]: https://docs.aspose.com/barcode/net/barcode-types-and-image-formats/
[16]: https://apireference.aspose.com/barcode/net/aspose.barcode.generation/barcodegenerator
[17]: https://apireference.aspose.com/barcode/net/aspose.barcode.generation/encodetypes
[18]: https://apireference.aspose.com/barcode/net/aspose.barcode.generation.barcodegenerator/save/methods/2
[19]: https://apireference.aspose.com/barcode/net/aspose.barcode.generation/barcodeimageformat/
[20]: https://apireference.aspose.com/barcode/net/aspose.barcode.barcoderecognition/barcodereader
[21]: https://downloads.aspose.com/barcode/net
[22]: https://www.nuget.org/packages/aspose.barcode
[23]: https://apireference.aspose.com/slides/net/aspose.slides/iimagecollection/addimage
[24]: https://apireference.aspose.com/slides/net/aspose.slides/presentation/images/
[25]: https://apireference.aspose.com/slides/net/aspose.slides/islidecollection/addemptyslide
[26]: https://apireference.aspose.com/slides/net/aspose.slides/ishapecollection/addpictureframe
[27]: https://apireference.aspose.com/slides/net/aspose.slides.export/saveformat/
[28]: https://apireference.aspose.com/slides/net/aspose.slides/iimagecollection/addimage
[29]: https://apireference.aspose.com/slides/net/aspose.slides/presentation/images/
[30]: https://apireference.aspose.com/slides/net/aspose.slides/ishapecollection/addpictureframe
[31]: https://apireference.aspose.com/slides/net/aspose.slides.export/saveformat/
[32]: https://apireference.aspose.com/barcode/net/aspose.barcode.barcoderecognition/barcodereader/constructors/2
[33]: https://apireference.aspose.com/barcode/net/aspose.barcode.barcoderecognition/barcodereader/methods/readbarcodes
[34]: https://apireference.aspose.com/barcode/net/aspose.barcode.barcoderecognition/barcoderesult
[35]: https://purchase.aspose.com/temporary-license
[36]: https://docs.aspose.com/barcode/net/
[37]: https://forum.aspose.com/c/barcode/13
[38]: https://blog.aspose.com/2022/05/31/create-barcode-in-word-documents-using-csharp/
[39]: https://blog.aspose.com/2022/05/26/generate-barcode-in-excel-using-csharp/
[40]: https://blog.aspose.com/2022/05/14/add-barcode-to-pdf-using-csharp/
[41]: https://blog.aspose.com/2022/04/23/generate-barcode-with-logo-using-csharp/
[42]: https://blog.aspose.com/2022/04/04/generate-and-display-barcode-image-in-asp-net-mvc/





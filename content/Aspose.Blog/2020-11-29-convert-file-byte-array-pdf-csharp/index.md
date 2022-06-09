---
title: 'Convert PDF File to Byte Array or Byte Array to PDF using C#'
seoTitle: ""
description: ""
date: Sun, 29 Nov 2020 19:13:48 +0000
draft: false
url: /2020/11/29/convert-file-byte-array-pdf-csharp/
author: Farhan Raza
summary: '[**Byte Array**][1] is helpful for storing or transmitting data. Likewise, the PDF file format is popular because of its features and compatibility. You can convert PDF File to Byte Array as well as a Byte Array to PDF File using C# language.'
tags: ['Byte Array to PDF', 'C# Byte Array to File', 'C# File to Byte Array', 'Convert Byte Array to File', 'PDF to Byte Array']
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/C-Convert-PDF-File-Byte-Array.png" alt="C# Convert PDF File Byte Array">}}


[Byte Array][2] is helpful for storing or transmitting data. Likewise, the PDF file format is popular because of its features and compatibility. You can convert PDF File to Byte Array as well as a Byte Array to PDF File using C# language. This can help you store and archive PDF files in the database, more efficiently. You can also serialize the data by working with the Byte Array. Let us explore the inter-convertibility of these formats.

*   [PDF File to Byte Array and Byte Array to PDF File Conversion – API Installation][3]
*   [Convert PDF File to Byte Array using C#][4]
*   [Convert Byte Array to PDF File using C#][5]

## PDF File to Byte Array and Byte Array to PDF File Conversion – API Installation {#section1}

[Aspose.PDF for .NET][6] API offers a lot of features to work with PDF documents. You can create, edit, manipulate, or convert PDF files with simple and easy API calls. For converting PDF files to Byte Array or vice versa, you need to install the API either by downloading it from the [official website][7], or from [NuGet][8] gallery using the below installation command in Visual Studio IDE.

```
PM> Install-Package Aspose.Pdf
```

## Convert PDF File to Byte Array using C# {#section2}

You can convert PDF to Byte Array in order to transmit or store it for further processing. For instance, you might need to serialize a PDF document then converting it to a byte array can help. You need to follow the steps below for converting PDF to a byte array:

1.  Load input PDF File
2.  Initialize a Byte Array
3.  Initialize [FileStream][9] object
4.  Load the file contents in the byte array

After following all these steps, now you can process the PDF file in the form of a byte array. For example, you can pass it over to another function like the example below.

The following code shows how to convert a PDF File to a Byte Array using C# where the resultant ByteArray is passed to a method for converting input file to images:

{{< gist aspose-com-gists 82f890d8ed5fbc4801695381a19dfc4d "PDFtoByteArray.cs" >}}

## Convert Byte Array to PDF File using C# {#section3}

Let us proceed another step further, a Byte Array can be converted to a PDF File. Let us learn this by the example of converting an image as a Byte Array to a PDF file. You need to follow the following steps for converting a Byte Array to a PDF file.

1.  Load input file
2.  Initialize byte array
3.  Load input image into Byte Array
4.  Initialize an instance of [Document][10] class
5.  Add image on a PDF page
6.  Save output PDF File

The following code explains how to convert a Byte Array to PDF File programmatically using C#:

{{< gist aspose-com-gists 82f890d8ed5fbc4801695381a19dfc4d "ByteArraytoPDF.cs" >}}

## Conclusion

In this article, we have explored how to convert PDF File to Byte Array as well as Byte Array to PDF File using C# programming language. If you are interested in working further with the PDF file, then kindly share your requirements with us via [Free Support Forum][11]. Moreover, you can also explore the [API Documentation][12] and [API References][13] for an in-depth analysis of the features offered by the API. We look forward to getting in touch with you!

## See Also

[Convert JSON to CSV and CSV to JSON using C# or VB.NET][14]




[1]: https://docs.microsoft.com/en-us/dotnet/api/system.byte?view=net-5.0
[2]: https://docs.microsoft.com/en-us/dotnet/api/system.byte?view=net-5.0
[3]: #section1
[4]: #section2
[5]: #section3
[6]: https://products.aspose.com/pdf/net
[7]: https://releases.aspose.com/
[8]: https://www.nuget.org/packages/Aspose.Pdf
[9]: https://docs.microsoft.com/en-us/dotnet/api/system.io.filestream?view=net-5.0
[10]: https://apireference.aspose.com/pdf/net/aspose.pdf/document
[11]: https://forum.aspose.com/c/pdf
[12]: https://docs.aspose.com/pdf/net/
[13]: https://apireference.aspose.com/pdf/net
[14]: https://blog.aspose.com/2020/11/24/convert-csv-json-charp-vb-net/






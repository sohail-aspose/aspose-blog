---
title: 'Search and Extract Text from PDF Programmatically using C#'
seoTitle: ""
description: ""
date: Sat, 16 May 2020 16:10:00 +0000
draft: false
url: /2020/05/16/extract-text-from-pdf-csharp-vb-net/
author: Farhan Raza
summary: 'Extract text from PDF documents. You can extract from a specific page or region, or whole PDF file. Read text using .NET C# language.'
tags: ['Extract Text', 'Extract Text from PDF', 'Search Text in PDF', 'Text extraction', 'read text from PDF', 'search and extract text from PDF', 'search text']
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/Extract_Text_PDF-150x150.png" alt="Extract Text PDF">}}


PDF file format is popular because file contents can not be modified easily, as compared to other word processing file formats. However, you can extract text from PDF documents with Aspose.PDF for .NET API. In this article, let us explore a few of the many possibilities for searching and extracting text from PDF files using C#. Following is a list of features we will be discussing in this blog:

*   [Extract Text from a Whole PDF Document using C#][1]
*   [Search and Extract Text from a Specific Page in PDF Document using C#][2]
*   [Search and Extract Text from Specific Region of PDF Page using C#][3]
*   [Search or Extract Specific Text from PDF file with Regular Expressions using C#][4]
*   [Extract Text from Table Cells in PDF Document using C#][5]
*   [Search & Extract Highlighted Text from PDF Document using C#][6]
*   [Extract PDF Text with Low Memory Consumption using C#][7]

## Extract Text from a Whole PDF Document using C# {#section0}

Reading text contents from a PDF document is a frequently used feature. You can extract all text from all pages of the document by following the steps below:

1.  Load PDF document
2.  Create [TextAbsorber][8] object
3.  Accept the absorber for all pages
4.  Write extracted text to a file and save it

Below code snippet follows these steps and shows how to extract text from a whole PDF document using C#:

{{< gist aspose-cloud 7b6fd21096e2fbbda3548cdd8c565b96 "Extract-Text-All-Pages.cs" >}}

## Search and Extract Text from a Specific Page in PDF in C# {#section1}

After exploring the text extraction at the document level, let us extract text from a specific page of a PDF document. Simply follow the below steps to achieve your requirements:

1.  Load PDF document
2.  Create [TextAbsorber][9] object
3.  Accept the absorber for a specific page
4.  Write extracted text to a file and save it

Following code snippet follows these steps to read text from any page of a PDF file using C#:

{{< gist aspose-cloud 7b6fd21096e2fbbda3548cdd8c565b96 "Extract-PDF-text-page.cs" >}}

## Search and Extract Text from Specific Region of PDF Page in C# {#section2}

Let us take this text extraction another step further. Consider finding some text from a specific area of the page. It is important to understand here that the basic measuring unit in Aspose.PDF for .NET is point, where 72 points equal 1 inch. Moreover, the left bottom corner is considered as the origin (0,0) of the page. The following are the steps to read text from a specific area or section of Page in PDF document:

1.  Load source PDF document
2.  Create [TextAbsorber][10] object
3.  Set [TextSearchOptions][11] and specify rectangular coordinates
4.  Accept the absorber for specific page
5.  Write extracted text to a file

The code snippet below demonstrates these steps to extract text from specific region using C#:

{{< gist aspose-cloud 7b6fd21096e2fbbda3548cdd8c565b96 "Extract-PDF-Text-Region.cs" >}}

## Search or Extract Specific Text from PDF file with Regular Expressions using C# {#section3}

You can extract specific text from a PDF document that matches some pattern. For instance, you might want to extract some specific words or numbers. For this purpose, you would need to design a regular expression. The API will utilize that regex to find matching text in the PDF document. Below steps are the guidelines to search and extract specific text from PDF files:

*   Load input PDF document
*   Create [TextAbsorber][12] object
*   Design and set a regular expression to match some text
*   Loop through each extracted text fragment

Following C# code snippet uses a regex that searches for the text containing 4 digits, for instance, 1999,2000, etc. across all pages of the document.

{{< gist aspose-cloud 7b6fd21096e2fbbda3548cdd8c565b96 "Extract-Text-RegEx.cs" >}}

## Extract Text from Table Cells in PDF Document using C# {#section4}

Extracting text from Tables on a PDF page is a little different. We have been working with TextAbsorber class in previous examples, but extracting text from a Table is a bit different. Therefore, you need to follow the below steps to extract text from Table objects:

1.  Load source PDF file
2.  Create an object of [TableAbsorber][13] class
3.  Iterate through [AbsorbedTable][14]
4.  Loop through each cell in each row of Table

Below code snippet follows these steps and efficiently extracts the text from Table cells in PDF document using C#:

{{< gist aspose-cloud 7b6fd21096e2fbbda3548cdd8c565b96 "Extract-Text-Table-PDF.cs" >}}

## Search & Extract Highlighted Text from PDF Document using C# {#section5}

Highlighted text is present as Annotation in PDF files. They contain Marked Text which makes them different from the conventional text in a document. Below steps describe how to read highlighted text using C#:

1.  Load source document
2.  Loop through all the annotations
3.  Filter [TextMarkupAnnotation][15]
4.  Retrieve highlighted text fragments

The following is a code snippet based on the steps above, it can be used to get highlight text from PDF files:

{{< gist aspose-cloud 7b6fd21096e2fbbda3548cdd8c565b96 "Extract-Highlight-Text-PDF.cs" >}}

## Extract PDF Text with Low Memory Consumption using C# {#section7}

The following are two different approaches to optimize memory consumption while extracting text from PDF documents using C# language.

### i) Using **_Reset()_** and **_FreeMemory()_** Method

Sometimes the text extraction may consume huge memory and processor. Possibly when the input file is huge and contains a lot of text. Because [TextFragmentAbsorber][16] object stores all found text fragments in the memory.

Therefore, the solution we recommend here is to call **_absorber.Reset()_** method after processing each page. Moreover, if you are doing read operations only then you can also free the memory held by page objects, with **_page.FreeMemory()_** method. So you need to follow the below steps to utilize minimal resources:

1.  Load source PDF document
2.  Specify [TextEditOptions][17]
3.  Read [TextFragment][18]
4.  Call [Reset()][19] method
5.  Call [FreeMemory()][20] method

The following code snippet demonstrates text extraction from PDF documents using C#:

{{< gist aspose-cloud 7b6fd21096e2fbbda3548cdd8c565b96 "Extract-Text-LowMemory.cs" >}}

We have tested this code snippet with a huge sample file containing 450 pages, 24500 text fragments, and a lot of raster and vector images. The process consumed a mere 500MB of memory. Another tip here is that you may charge .NET garbage collector to decrease maximum memory consumption to around 250MB with an additional cost of 10 seconds of processing time.

### ii) Using _MemorySaving_ enumeration

Aspose.PDF for .NET API supports configuring memory saving mode while reading text from a PDF file. The **_TextExtractionOptions.TextFormattingMode_** enumeration serves the purpose of optimal consumption of resources. Following steps summarize the steps you need to follow for this approach:

1.  Load source PDF file
2.  Create [TextDevice][21] object
3.  Set [TextExtractionOptions][22]
4.  Extract text and write text to a file

Below code snippet demonstrates the memory saving approach using C#:

{{< gist aspose-cloud 7b6fd21096e2fbbda3548cdd8c565b96 "Extract-Text-MemorySaving.cs" >}}

## Conclusion

We have explored a few of the many useful use cases in this article, there are endless possibilities of extracting text from PDF documents using C# with Aspose.PDF for .NET API. You can learn more via [API documentation][23]. In case of any inquiry, please reach out to us at [Free Support Forums][24].

## See Also

[Convert PDF File to PowerPoint Presentation in C#][25]




[1]: #section0
[2]: #section1
[3]: #section2
[4]: #section3
[5]: #section4
[6]: #section5
[7]: #section7
[8]: https://apireference.aspose.com/pdf/net/aspose.pdf.text/textabsorber
[9]: https://apireference.aspose.com/pdf/net/aspose.pdf.text/textabsorber
[10]: https://apireference.aspose.com/pdf/net/aspose.pdf.text/textabsorber
[11]: https://apireference.aspose.com/pdf/net/aspose.pdf.text/textsearchoptions
[12]: https://apireference.aspose.com/pdf/net/aspose.pdf.text/textabsorber
[13]: https://apireference.aspose.com/pdf/net/aspose.pdf.text/tableabsorber
[14]: https://apireference.aspose.com/pdf/net/aspose.pdf.text/absorbedtable
[15]: https://apireference.aspose.com/net/pdf/aspose.pdf.annotations/textmarkupannotation
[16]: https://apireference.aspose.com/pdf/net/aspose.pdf.text/textfragmentabsorber
[17]: https://apireference.aspose.com/pdf/net/aspose.pdf.text/texteditoptions
[18]: https://apireference.aspose.com/pdf/net/aspose.pdf.text/textfragment
[19]: https://apireference.aspose.com/pdf/net/aspose.pdf.text/textfragmentabsorber/methods/reset
[20]: https://apireference.aspose.com/net/pdf/aspose.pdf/page/methods/freememory
[21]: https://apireference.aspose.com/pdf/net/aspose.pdf.devices/textdevice
[22]: https://apireference.aspose.com/pdf/net/aspose.pdf.text/textextractionoptions
[23]: https://docs.aspose.com/display/pdfnet/Home
[24]: https://forum.aspose.com/
[25]: https://blog.aspose.com/2020/03/18/convert-pdf-to-powerpoint-ppt-pptx-in-csharp-net/






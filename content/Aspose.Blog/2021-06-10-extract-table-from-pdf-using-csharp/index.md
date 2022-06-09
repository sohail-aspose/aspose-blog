---
title: 'Extract Data from Tables in PDF using C#'
seoTitle: "Extract Table Data in PDF using C# | Extract Tables in PDF Files using C#"
description: "Use C# PDF API to extract data from the PDF table using C#. Extract tables from all pages or a specific region of a page in PDF."
date: Thu, 10 Jun 2021 15:05:09 +0000
draft: false
url: /2021/06/10/extract-table-from-pdf-using-csharp/
author: Usman Aziz
summary: '[PDF][1] has become one of the most widely used document formats in a multitude of fields. In various cases, it is used to generate invoices where data appears to be in a tabular form. In such cases, you may need to parse the PDF to read data from the tables programmatically. To achieve this, the article covers **how to extract data from PDF tables using C#**.'
tags: ['Csharp API to Extract PDF Tables', 'Extract Data from PDF Tables in Csharp', 'Extract Table from a Specific Area of Page in Csharp']
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/Extract-PDF-Tables.jpg" alt="Extract PDF Tables">}}


[PDF][2] has become one of the most widely used document formats in a multitude of fields. In various cases, it is used to generate invoices where data appears to be in a tabular form. In such cases, you may need to parse the PDF to read data from the tables programmatically. To achieve this, the article covers **how to extract data from PDF tables using C#**.

*   [C# API to Extract PDF Tables][3]
*   [Extract Data from PDF Tables in C#][4]
*   [Extract Table from a Specific Area of Page][5]

## C# API to Extract Tables from PDF {#API-to-Extract-Table-from-PDF}

In order to extract data from the tables in PDF files, we will use [Aspose.PDF for .NET][6]. It is a powerful API that provides a wide range of PDF manipulation features. You can either [download][7] the API or install it using [NuGet][8].

```
PM> Install-Package Aspose.PDF
```

## Extract Data from PDF Tables in C# {#Extract-Data-from-PDF-Table}

The following are the steps to extract data from tables in a PDF using C#.

*   Load the PDF document using the [Document][9] class.
*   Loop through the pages in PDF using [Document.Pages][10] collection.
*   In each iteration, initialize the [TableAbsorber][11] object and visit the selected page using [TableAbsorber.Visit(Page)][12] method.
*   In a nested loop, iterate through the list of the tables in [TableAbsorber.TableList][13] collection.
*   For each [AbsorbedTable][14] in the collection, iterate through the collection of rows in [AbsorbedTable.RowList][15].
*   For each [AbsorbedRow][16] in the collection, iterate through the collection of cells in [AbsorbedRow.CellList][17].
*   Finally, loop through the [TextFragments][18] collection of each [AbsorbedCell][19] and print the text.

The following code sample shows how to extract text from PDF table in C#.

{{< gist aspose-com-gists 16e1a2087c91cfb4f0fa6cddd047fa02 "extract-text-from-pdf-table.cs" >}}

## Extract Table from a Specific Area of Page {#Extract-Table-from-a-Specific-Area-of-Page}

The following are the steps to extract a table from a specific part of the page in a PDF using C#.

*   Load the PDF document using the [Document][20] class.
*   Select the desired [Page][21] from [Document.Pages][22] collection.
*   Extract the Square annotation of the page.
*   Initialize the [TableAbsorber][23] object and visit the page using [TableAbsorber.Visit(Page)][24] method.
*   In a nested loop, iterate through the list of the tables in [TableAbsorber.TableList][25] collection.
*   If the table is in the region then perform the following steps.
    *   Iterate through the collection of rows in [AbsorbedTable.RowList][26].
    *   For each [AbsorbedRow][27] in the collection, iterate through the collection of cells in [AbsorbedRow.CellList][28].
    *   Finally, loop through the [TextFragments][29] collection of each [AbsorbedCell][30] and print the text.

The following code sample shows how to extract table from a specific region of the PDF page.

{{< gist aspose-com-gists 16e1a2087c91cfb4f0fa6cddd047fa02 "extract-text-from-pdf-table-specific-area.cs" >}}

## Get a Free License {#Get-a-Free-License}

You can use Aspose.PDF for .NET without evaluation limitations using a [temporary license][31].

## Conclusion

In this article, you have learned how to extract data from tables in a PDF using C#. Furthermore, you have seen how to extract a table from a specific region of the page in PDF. You can explore more about the C# PDF API using the [documentation][32]. Also, you can post your queries on our [forum][33].

## See Also

*   [Create PDF Files using C# – .NET PDF API][34]




[1]: https://docs.fileformat.com/pdf/
[2]: https://docs.fileformat.com/pdf/
[3]: #API-to-Extract-Table-from-PDF
[4]: #Extract-Data-from-PDF-Table
[5]: #Extract-Table-from-a-Specific-Area-of-Page
[6]: https://products.aspose.com/pdf/net
[7]: https://downloads.aspose.com/pdf/net
[8]: http://nuget.org/packages/Aspose.PDF
[9]: https://apireference.aspose.com/pdf/net/aspose.pdf/document
[10]: https://apireference.aspose.com/pdf/net/aspose.pdf/document/properties/pages
[11]: https://apireference.aspose.com/pdf/net/aspose.pdf.text/tableabsorber
[12]: https://apireference.aspose.com/pdf/net/aspose.pdf.text/tableabsorber/methods/visit
[13]: https://apireference.aspose.com/pdf/net/aspose.pdf.text/tableabsorber/properties/tablelist
[14]: https://apireference.aspose.com/pdf/net/aspose.pdf.text/absorbedtable
[15]: https://apireference.aspose.com/pdf/net/aspose.pdf.text/absorbedtable/properties/rowlist
[16]: https://apireference.aspose.com/pdf/net/aspose.pdf.text/absorbedrow
[17]: https://apireference.aspose.com/pdf/net/aspose.pdf.text/absorbedrow/properties/celllist
[18]: https://apireference.aspose.com/pdf/net/aspose.pdf.text/absorbedcell/properties/textfragments
[19]: https://apireference.aspose.com/pdf/net/aspose.pdf.text/absorbedcell
[20]: https://apireference.aspose.com/pdf/net/aspose.pdf/document
[21]: https://apireference.aspose.com/pdf/net/aspose.pdf/page
[22]: https://apireference.aspose.com/pdf/net/aspose.pdf/document/properties/pages
[23]: https://apireference.aspose.com/pdf/net/aspose.pdf.text/tableabsorber
[24]: https://apireference.aspose.com/pdf/net/aspose.pdf.text/tableabsorber/methods/visit
[25]: https://apireference.aspose.com/pdf/net/aspose.pdf.text/tableabsorber/properties/tablelist
[26]: https://apireference.aspose.com/pdf/net/aspose.pdf.text/absorbedtable/properties/rowlist
[27]: https://apireference.aspose.com/pdf/net/aspose.pdf.text/absorbedrow
[28]: https://apireference.aspose.com/pdf/net/aspose.pdf.text/absorbedrow/properties/celllist
[29]: https://apireference.aspose.com/pdf/net/aspose.pdf.text/absorbedcell/properties/textfragments
[30]: https://apireference.aspose.com/pdf/net/aspose.pdf.text/absorbedcell
[31]: https://purchase.aspose.com/temporary-license
[32]: https://docs.aspose.com/pdf/net/overview/
[33]: https://forum.aspose.com/
[34]: https://blog.aspose.com/2020/12/02/create-pdf-files-using-csharp/






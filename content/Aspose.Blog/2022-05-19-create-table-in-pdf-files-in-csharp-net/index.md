---
title: 'Create Table in PDF Files using C# .NET'
date: Thu, 19 May 2022 15:39:16 +0000
draft: false
url: /2022/05/19/create-table-in-pdf-files-in-csharp-net/
author: ''Usman Aziz''
summary: 'Tables are used to represent data in the form of rows and columns. It lets the readers go through the data quickly without reading a lot of text. When generating the [PDF][1] files programmatically, you may often come across the requirement of creating tables. In accordance with that, this article covers **how to create tables in PDF files in C# .NET**.'
tags: ['Apply Auto Fit Settings to PDF Tables in Csharp', 'Create a Table in a PDF File in Csharp', 'DotNet API to Create Tables in PDF', 'DotNet PDF Generator API', 'Set Borders and Margins in PDF Tables in Csharp']
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/Create-Tables-in-PDF.jpg" alt="Create Table in PDF Files in C# .NET">}}


Tables are used to represent data in the form of rows and columns. A table lets the readers go through the data quickly without reading a lot of text. When generating the [PDF][2] files programmatically, you may often come across the requirement of creating tables. In accordance with that, this article covers **how to create tables in PDF files using C# .NET**.

*   [.NET API to Create Tables in PDF][3]
*   [Create a Table in a PDF File][4]
*   [Set Borders and Margins in PDF Tables][5]
*   [Apply Column Adjustment to PDF Tables][6]

## C# .NET API to Create Tables in PDF Files {#API-to-Create-Tables-in-PDF}

We will use [Aspose.PDF for .NET][7] to create tables in PDF files. The API is designed to perform PDF generation and manipulation within the .NET applications. It allows you to create PDF files of simple and complex layouts seamlessly. You can either [download][8] the API's binaries or install it using [NuGet][9].

```
PM> Install-Package Aspose.PDF
```

## Create a Table in a PDF File in C# {#Create-a-Table-in-a-PDF-File}

You can create tables in either a new or an existing PDF file using Aspose.PDF for .NET. The following are the steps to create a table in a PDF file in C#.

*   Load the PDF file (or create a new one) using [Document][10] class.
*   Initialize a table and set its columns and rows using [Table][11] class.
*   Set table’s settings (i.e. borders).
*   Populate the table by creating rows using [Table.Rows.Add()][12] method.
*   Add the table to the page using [Document.Pages\[index\].Paragraphs.Add(Table)][13] method.
*   Save the PDF file using [Document.Save(string)][14] method.

The following code sample shows how to create a table in a PDF file using C#.

{{< gist aspose-com-gists ab90ede4c0a043dd31ffbffd6443eedb "create-table-in-pdf.cs" >}}

The following is the output of the above code sample.



{{< figure align=center src="images/Create-Tables-in-PDF.png" alt="Create a Table in a PDF File in C#">}}


## Create PDF Table with Customized Borders and Margins {#Set-Borders-and-Margins-in-PDF-Tables}

You can also customize the borders and margins of the tables in PDF as per your requirements. For example, you can set the border width, border style, and top, bottom, left, and right margins. The following are the steps to set borders and margins for the tables in PDF files in C#.

*   Load the PDF file (or create a new one) using [Document][15] class.
*   Initialize a table and set its columns and rows using [Table][16] class.
*   Create an instance of [BorderInfo][17] class to apply border styling.
*   Create an instance of [MarginInfo][18] class to set margins for the table.
*   Populate the table by creating rows using [Table.Rows.Add()][19] method.
*   Add the table to the page using [Document.Pages\[index\].Paragraphs.Add(Table)][20] method.
*   Save the PDF file using [Document.Save(string)][21] method.

The following code sample shows how to set borders and margins for tables in PDF using C#.

{{< gist aspose-com-gists ab90ede4c0a043dd31ffbffd6443eedb "create-table-in-pdf-margin-border.cs" >}}

The following screenshot shows the output of the above code sample.



{{< figure align=center src="images/Create-Tables-in-PDF-Border-and-Margins.png" alt="Create PDF Table with Customized Borders and Margins C#">}}


## Apply Column Adjustment to PDF Tables in C# {#Apply-Auto-Fit-Settings-to-PDF-Tables}

Aspose.PDF for .NET also allows you to customize the column adjustment of the table in a PDF. For example, you can auto-fit the table to the window or the content. The following are the steps to set the column adjustment of a table in PDF using C#.

*   Load the PDF file (or create a new one) using [Document][22] class.
*   Initialize a table and set its columns and rows using [Table][23] class.
*   Set borders and margins.
*   Set [Table.ColumnAdjustment][24] property to the desired value of [ColumnAdjustment][25] enum.
*   Populate the table by creating rows using [Table.Rows.Add()][26] method.
*   Add the table to the page using [Document.Pages\[index\].Paragraphs.Add(Table)][27] method.
*   Save the PDF file using [Document.Save(string)][28] method.

The following code sample shows how to set the column adjustment of the table in PDF using C#.

{{< gist aspose-com-gists ab90ede4c0a043dd31ffbffd6443eedb "create-table-in-pdf-autofit.cs" >}}

## Get a Free License {#Get-a-Free-License}

You can [get a free temporary license][29] in order to use Aspose.PDF for .NET without evaluation limitations.

## Conclusion

In this article, you have learned how to create tables in PDF files using C#. Furthermore, you have seen how to customize the borders. margins, and column adjustment of a table in PDF. Besides, you can explore more about the C# PDF API using the [documentation][30]. In case you would have any questions or queries, you can contact us via our [forum][31].

## See Also

*   [Add or Remove Annotations in PDF Files using C#][32]
*   [Extract Images from PDF using C#][33]
*   [Create PDF File from Images using C#][34]




[1]: https://docs.fileformat.com/pdf/
[2]: https://docs.fileformat.com/pdf/
[3]: #API-to-Create-Tables-in-PDF
[4]: #Create-a-Table-in-a-PDF-File
[5]: #Set-Borders-and-Margins-in-PDF-Tables
[6]: #Apply-Auto-Fit-Settings-to-PDF-Tables
[7]: https://products.aspose.com/pdf/net/
[8]: https://downloads.aspose.com/pdf/net/
[9]: http://nuget.org/packages/Aspose.PDF
[10]: https://apireference.aspose.com/pdf/net/aspose.pdf/document
[11]: https://apireference.aspose.com/pdf/net/aspose.pdf/table
[12]: https://apireference.aspose.com/pdf/net/aspose.pdf/rows/methods/add
[13]: https://apireference.aspose.com/pdf/net/aspose.pdf/paragraphs/methods/add
[14]: https://apireference.aspose.com/pdf/net/aspose.pdf.document/save/methods/5
[15]: https://apireference.aspose.com/pdf/net/aspose.pdf/document
[16]: https://apireference.aspose.com/pdf/net/aspose.pdf/table
[17]: https://apireference.aspose.com/pdf/net/aspose.pdf/borderinfo
[18]: https://apireference.aspose.com/pdf/net/aspose.pdf/margininfo
[19]: https://apireference.aspose.com/pdf/net/aspose.pdf/rows/methods/add
[20]: https://apireference.aspose.com/pdf/net/aspose.pdf/paragraphs/methods/add
[21]: https://apireference.aspose.com/pdf/net/aspose.pdf.document/save/methods/5
[22]: https://apireference.aspose.com/pdf/net/aspose.pdf/document
[23]: https://apireference.aspose.com/pdf/net/aspose.pdf/table
[24]: https://apireference.aspose.com/pdf/net/aspose.pdf/table/properties/columnadjustment
[25]: https://apireference.aspose.com/pdf/net/aspose.pdf/columnadjustment
[26]: https://apireference.aspose.com/pdf/net/aspose.pdf/rows/methods/add
[27]: https://apireference.aspose.com/pdf/net/aspose.pdf/paragraphs/methods/add
[28]: https://apireference.aspose.com/pdf/net/aspose.pdf.document/save/methods/5
[29]: https://purchase.aspose.com/temporary-license
[30]: https://docs.aspose.com/pdf/net/
[31]: https://forum.aspose.com/
[32]: https://blog.aspose.com/2021/01/04/add-or-remove-annotations-in-pdf-using-csharp/
[33]: https://blog.aspose.com/2021/06/15/extract-images-from-pdf-in-csharp/
[34]: https://blog.aspose.com/2021/04/20/create-pdf-from-images-using-csharp/





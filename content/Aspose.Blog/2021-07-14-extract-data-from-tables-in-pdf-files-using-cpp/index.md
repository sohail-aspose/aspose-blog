---
title: 'Extract Data from Tables in PDF Files using C++'
seoTitle: "Extract Data from Tables in PDF Files using C++ | Extract PDF Tables"
description: "Extract data from PDF tables using C++. Extract data from tables in a specific area of a PDF page by using the Aspose.PDF for C++ API."
date: Wed, 14 Jul 2021 17:31:32 +0000
draft: false
url: /2021/07/14/extract-data-from-tables-in-pdf-files-using-cpp/
author: Muhammad Ahmad
summary: '[PDF][1] files are a standard format for exchanging documents over the internet. Documents like invoices and product guides are usually shared in the form of PDFs. There might be situations where you have multiple invoices containing tabular data that you want to extract and process further. It will be more efficient to extract this data programmatically. To that end, this article will teach you **how to extract data from PDF tables using C++**.'
tags: ['C++ API for Extracting Data from PDF Tables', 'Extract Data from PDF Tables using C++', 'Extract Table Data from Specific Area of PDF Page using C++']
categories: ['Aspose.PDF Product Family']
---

[PDF][2] files are a standard format for exchanging documents over the internet. Documents like invoices and product guides are usually shared in the form of PDFs. There might be situations where you have multiple invoices containing tabular data that you need to extract and process further. It will be more efficient to extract this data programmatically. To that end, this article will teach you **how to extract data from PDF tables using C++**.

*   [C++ API for Extracting Data from Tables in PDF Files][3]
*   [Extract Data from PDF Tables using C++][4]
*   [Extract Data from a Table in a Specific Area of a PDF Page][5]

## C++ API for Extracting Data from Tables in PDF Files {#CPP-API-for-Extracting-Data-from-Tables-in-PDF-Files}

[Aspose.PDF for C++][6] is a C++ library that allows you to create, read, and update PDF files. Furthermore, the API supports extracting data from tables in PDF files. You can either install the API through [NuGet][7] or download it directly from the [downloads][8] section.

```
PM> Install-Package Aspose.PDF.Cpp
```

## Extract Data from PDF Tables using C++ {#Extract-Data-from-PDF-Tables-using-CPP}

The following are the steps to extract data from PDF tables.

*   Load the PDF document using the [Document][9] class.
*   Iterate through the pages of the document using the [Document->get\_Pages()][10] method.
*   In each iteration, create an instance of the [TableAbsorber][11] class and specify the page for extracting tables using the [TableAbsorber->Visit(System::SharedPtr<Page> page)][12] method.
*   Get the tables using the [TableAbsorber->get\_TableList()][13] method and iterate over them.
*   For each [AbsorbedTable][14], iterate though the rows using the [AbsorbedTable->get\_RowList()][15] method.
*   For each [AbsorbedRow][16], iterate through the cells using the [AbsorbedRow->get\_CellList()][17] method.
*   Get [TextFragmentCollection][18] for each [AbsorbedCell][19] using the [AbsorbedCell->get\_TextFragments()][20] method and loop through it.
*   Get [TextSegmentCollection][21] for each [TextFragment][22] using the [TextFragment->get\_Segments()][23] method and loop through it.
*   Retrieve the text from each [TextSegment][24] and print it.

The following sample code shows how to extract data from PDF tables using C++.

{{< gist aspose-com-gists 0fbf54fdf5406ad739b76e02e3a2f00e "Extract_Text_From_PDF_Table.cpp" >}}

## Extract Data from a Table in a Specific Area of a PDF Page {#Extract-Data-from-a-Table-in-a-Specific-Area-of-a-PDF-Page}

In order to extract data from a table in a specific area of a PDF page, please follow the steps given below.

*   Load the PDF document using the [Document][25] class.
*   Retrieve the page containing the table using the [Document->get\_Pages()->idx\_get(int32\_t index)][26] method.
*   Loop through the annotations and get the square annotation.
*   Create an instance of the [TableAbsorber][27] class and specify the page for extracting tables using the [TableAbsorber->Visit(System::SharedPtr<Page> page)][28] method.
*   Get the tables using the [TableAbsorber->get\_TableList()][29] method and iterate over them.
*   If the table is in the region, perform the following steps:
    *   Iterate through the rows of the [AbsorbedTable][30] using the [AbsorbedTable->get\_RowList()][31] method.
    *   For each [AbsorbedRow][32], iterate through the cells using the [AbsorbedRow->get\_CellList()][33] method.
    *   Get [TextFragmentCollection][34] for each [AbsorbedCell][35] using the [AbsorbedCell->get\_TextFragments()][36] method and loop through it.
    *   Get [TextSegmentCollection][37] for each [TextFragment][38] using the [TextFragment->get\_Segments()][39] method and loop through it.
    *   Retrieve the text from each [TextSegment][40] and print it.

The following sample code demonstrates how to extract data from a table in a specific area of a PDF page using C++.

{{< gist aspose-com-gists 0fbf54fdf5406ad739b76e02e3a2f00e "Extract_Text_From_PDF_Table_Specific_Area.cpp" >}}

## Get a Free License

In order to try the API without evaluation limitations, you can request [a free temporary license][41].

## Conclusion

In this article, you have learned how to extract data from PDF tables using C++. Moreover, you have learned how to extract data from a table in a specific region of the PDF page. Aspose.PDF for C++ API provides many additional features for working with PDF files. You can explore the API in detail by visiting the [official documentation][42]. In case of any questions, please feel free to reach us on our [free support forum][43].

## **See Also**

*   [Working with Annotations in PDF Files using C++][44]
*   [Convert PDF to HTML using C++][45]




[1]: https://docs.fileformat.com/pdf/
[2]: https://docs.fileformat.com/pdf/
[3]: #CPP-API-for-Extracting-Data-from-Tables-in-PDF-Files
[4]: #Extract-Data-from-PDF-Tables-using-CPP
[5]: #Extract-Data-from-a-Table-in-a-Specific-Area-of-a-PDF-Page
[6]: https://products.aspose.com/pdf/cpp
[7]: https://www.nuget.org/packages/Aspose.Pdf.cpp
[8]: https://downloads.aspose.com/pdf/cpp
[9]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.document
[10]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.document#a481178a0c2c6277ae9b6b931d63e4122
[11]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.text.table_absorber
[12]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.text.table_absorber#a6b903eb9598c39e1d6e537438cb1c34d
[13]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.text.table_absorber#a18b0f0eba96750bf32a4ee27c1622a88
[14]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.text.absorbed_table
[15]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.text.absorbed_table#a3abce806fb358852aed04f36b1e4b702
[16]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.text.absorbed_row
[17]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.text.absorbed_row#a79bfb37b560b8f2ecb7d771415373f24
[18]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.text.text_fragment_collection
[19]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.text.absorbed_cell
[20]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.text.absorbed_cell#aefae7c1f2cb0e3711af46a639671b6d6
[21]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.text.text_segment_collection
[22]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.text.text_fragment
[23]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.text.text_fragment#a1f715b4444b322e8d5bf72f754e8d2cf
[24]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.text.text_segment
[25]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.document
[26]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.page_collection#a30682a62c7630948c39bb950f47e4ba1
[27]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.text.table_absorber
[28]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.text.table_absorber#a6b903eb9598c39e1d6e537438cb1c34d
[29]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.text.table_absorber#a18b0f0eba96750bf32a4ee27c1622a88
[30]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.text.absorbed_table
[31]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.text.absorbed_table#a3abce806fb358852aed04f36b1e4b702
[32]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.text.absorbed_row
[33]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.text.absorbed_row#a79bfb37b560b8f2ecb7d771415373f24
[34]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.text.text_fragment_collection
[35]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.text.absorbed_cell
[36]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.text.absorbed_cell#aefae7c1f2cb0e3711af46a639671b6d6
[37]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.text.text_segment_collection
[38]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.text.text_fragment
[39]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.text.text_fragment#a1f715b4444b322e8d5bf72f754e8d2cf
[40]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.text.text_segment
[41]: https://purchase.aspose.com/temporary-license
[42]: https://docs.aspose.com/pdf/cpp/
[43]: https://forum.aspose.com/c/pdf/10
[44]: https://blog.aspose.com/2021/04/14/working-with-annotations-in-pdf-files-using-cpp/
[45]: https://blog.aspose.com/2021/05/07/convert-pdf-to-html-using-cpp/






---
title: 'Convert Excel to HTML using C++'
seoTitle: "Convert Excel to HTML using C++ | XLSX XLS to HTML Conversion"
description: "Use the C++ Excel to HTML converter API to convert Excel to HTML format. Generate customized HTML output by options provided by the Aspose.Cells for C++ API"
date: Sat, 06 Feb 2021 10:14:10 +0000
draft: false
url: /2021/02/06/convert-excel-to-html-using-cpp/
author: Muhammad Ahmad
summary: 'Excel spreadsheets are useful in organizing, managing, and computing data. Similarly, [HTML][1] is useful for displaying content in the browser. Both formats are handy in their specific use cases. There might be cases where you have to show excel data on websites. In those cases, HTML would be the better format to use. To achieve this, you will have to convert the required Excel file to HTML. In light of this, we will learn **how to convert Excel to HTML using C++**.'
tags: ['Convert Excel to HTML C++', 'Excel to HTML', 'Excel to HTML C++', 'XLS to HTML C++', 'XLSX to HTML C++']
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/Excel-to-HTML-Logo.jpg" alt="C++ Excel to HTML">}}


Excel spreadsheets are useful in organizing, managing, and computing data. Similarly, [HTML][2] is useful for displaying content in the browser. Both formats are handy in their specific use cases. There might be cases where you have to show Excel data on websites. In those cases, HTML would be the better format to use. To achieve this, you will have to convert the required Excel file to HTML. In light of this, you will learn **how to convert Excel files to HTML using C++**.

*   [C++ Excel to HTML Converter API – Free Download][3]
*   [Excel to HTML C++ Conversion][4]
*   [C++ Excel to HTML Conversion with Additional Options][5]
*   [Get a Free License][6]

## C++ Excel to HTML Converter API – Free Download {#CPP-Excel-to-HTML-Converter-API-Free-Download}

[Aspose.Cells for C++][7] is a C++ native API for creating, converting, and manipulating Excel spreadsheets. You can use the API's built-in converter to convert Excel files to HTML. Please install the API via [NuGet][8] or download it directly from the [Downloads][9] section.

```
PM> Install-Package Aspose.Cells.Cpp
```

## Excel to HTML C++ Conversion {#Excel-to-HTML-CPP-Conversion}

The following are the steps to convert Excel files to HTML:

*   Load the Excel file by using the [IWorkbook][10] class.
*   Save the file as HTML by using the [IWorkbook->Save(intrusive\_ptr<Aspose::Cells::Systems::String> fileName, Aspose::Cells::SaveFormat saveFormat)][11] method.

The following is the C++ code snippet for converting Excel files to HTML:

{{< gist aspose-com-gists 2800e712494bb83c2e93ca91416fae6f "Convert-Excel-to-HTML.cpp" >}}

## C++ Excel to HTML Conversion with Additional Options {#CPP-Excel-to-HTML-Conversion-with-Additional-Options}

Aspose.Cells for C++ API provides the [IHtmlSaveOptions][12] class for customizing the converted HTML file. The following are the options provided by the [IHtmlSaveOptions][13] class.

### Options provided by the IHtmlSaveOptions class

*   [AttachedFilesDirectory][14]: The directory for saving the attached files.
*   [AttachedFilesUrlPrefix][15]: Specify the URL prefix for the attached files.
*   [CellCssPrefix][16]: Set the prefix for the CSS name.
*   [DefaultFontName][17]: Specify the default font used when the original font does not exist.
*   [Encoding][18]: Specify the encoding.
*   [ExpImageToTempDir][19]: Indicate whether to export the images to a temp directory.
*   [ExportActiveWorksheetOnly][20]: Indicate whether to export only the active worksheet or the whole workbook to HTML.
*   [ExportBogusRowData][21]: Specify whether to export bogus bottom row data.
*   [ExportDataOptions][22]: Specify whether to export only the table or all the data of the HTML file.
*   [ExportFrameScriptsAndProperties][23]: Indicate whether to export frame scripts and properties.
*   [ExportGridLines][24]: Indicates whether to export grid lines.
*   [ExportHiddenWorksheet][25]: Specify whether to export the hidden worksheet to HTML.
*   [ExportImagesAsBase64][26]: Specify whether to save the images in Base64 format.
*   [FullPathLink][27]: Specify whether to use the full path link in sheet00x.htm,filelist.xml and tabstrip.htm.
*   [HiddenColDisplayType][28]: Specify whether to export the hidden column (column with the width of 0) to HTML.
*   [HiddenRowDisplayType][29]: Specify whether to export the hidden row (the row with the height of 0) to HTML.
*   [HtmlCrossStringType][30]: Specify the behavior of the cells when the text is larger than the cell size.
*   [LinkTargetType][31]: Specify the link target type in the HTML anchor tag.
*   [ParseHtmlTagInCell][32]: Indicate to parse HTML tags in a cell.
*   [PresentationPreference][33]: Set this to true to get a more beautiful HTML presentation.

### Converting Excel to HTML with IHtmlSaveOptions

The following are the steps to convert Excel to HTML with additional options:

*   Firstly, load the Excel file with the [IWorkbook][34] class.
*   Create an instance of the [IHtmlSaveOptions][35] class.
*   Set additional options with [IHtmlSaveOptions][36] class such as [ExportHiddenWorksheet][37].
*   Finally, save the Excel file as HTML by using the [IWorkbook->Save(intrusive\_ptr<Aspose::Cells::Systems::String> fileName, intrusive\_ptr<Aspose::Cells::ISaveOptions> saveOptions)][38] method.

The following code sample shows how to convert Excel files to HTML with additional options:

{{< gist aspose-com-gists 2800e712494bb83c2e93ca91416fae6f "Convert-Excel-to-HTML-with-Additional-Options.cpp" >}}

## Get a Free License {#Get-a-Free-License}

You can try the API without evaluation limitations by requesting [a free temporary license][39].

## Conclusion

In this article, you have learned how to convert an Excel file to HTML using C++. Furthermore, you have seen different options to customize the Excel to HTML conversion, such as whether to export hidden worksheets. You can explore more about Aspose.Cells for C++ using [documentation][40].

## See Also

*   [Convert Excel Files to Images using C++][41]




[1]: https://docs.fileformat.com/web/html/
[2]: https://docs.fileformat.com/web/html/
[3]: #CPP-Excel-to-HTML-Converter-API-Free-Download
[4]: #Excel-to-HTML-CPP-Conversion
[5]: #CPP-Excel-to-HTML-Conversion-with-Additional-Options
[6]: #Get-a-Free-License
[7]: https://products.aspose.com/cells/cpp
[8]: https://www.nuget.org/packages/Aspose.Cells.Cpp
[9]: https://downloads.aspose.com/cells/cpp
[10]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_workbook
[11]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_workbook#a9460f52a2dec8f4bf623a4905167d997
[12]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_html_save_options
[13]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_html_save_options
[14]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_html_save_options#a94bb4defde21cd1f73e9a30101ce4300
[15]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_html_save_options#a47464fa585bb4778cc2693df97695449
[16]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_html_save_options#a6e0136009391ba09405b83c63c6f0ac2
[17]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_html_save_options#acfe274e92c6c747770b56247b2061462
[18]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_html_save_options#a228cf90b98f6ede9c845f569b62772a7
[19]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_html_save_options#acbcd6a377c6d3c393edd44bdc2f795a1
[20]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_html_save_options#a6b92a3c363d69999bb0cf08b8a59e820
[21]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_html_save_options#a5926b3e971d18a05b4c493e6e6a44b73
[22]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_html_save_options#a17302f8b78e67c12903491322690903e
[23]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_html_save_options#adf16b824def8a21adeb0bc5e01aa05cf
[24]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_html_save_options#ae2f98d3548dcfef3a3b334d58f2cf4a4
[25]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_html_save_options#adc95df66de748689b5eed4da43426026
[26]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_html_save_options#ae13887edb52535980c25524b9687952a
[27]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_html_save_options#a448a10e05bd3b51a9adbe57364f61409
[28]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_html_save_options#ab0f620afdbccc778b99a26b516c6df40
[29]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_html_save_options#a3fb13d2bab76332bc9a3be432136a727
[30]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_html_save_options#a28b366584075596610d7f93df1dee78c
[31]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_html_save_options#ab94cae4e761e64947a222c1af47c5836
[32]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_html_save_options#a7fe19bb1b46f886ac88533d94b2bf731
[33]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_html_save_options#a0c3335b7aac8ff56b2942389cfebec8b
[34]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_workbook
[35]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_html_save_options
[36]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_html_save_options
[37]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_html_save_options#adc95df66de748689b5eed4da43426026
[38]: https://apireference.aspose.com/cells/cpp/class/aspose.cells.i_workbook#a5dc7de23f7ceba76a05dc1d49f51502e
[39]: https://purchase.aspose.com/temporary-license
[40]: https://docs.aspose.com/cells/cpp/
[41]: https://blog.aspose.com/2021/01/28/convert-excel-files-to-images-using-cpp/






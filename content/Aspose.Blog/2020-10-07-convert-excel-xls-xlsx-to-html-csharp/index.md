---
title: 'Convert Excel XLS/XLSX to HTML using C#'
seoTitle: "Excel to HTML using C# | Convert XLS or XLSX to HTML using C#"
description: "Convert MS Excel XLS/XLSX file to HTML using C# or VB.NET. Convert Excel to HTML with tooltips and presentation preferences options using .NET converter API."
date: Wed, 07 Oct 2020 18:27:58 +0000
draft: false
url: /2020/10/07/convert-excel-xls-xlsx-to-html-csharp/
author: Usman Aziz
summary: 'Excel to HTML conversion could be useful in various scenarios such as converting sheets to web pages or embedding the content of the sheets within the web applications and so on. In this article, you will learn how to convert MS Excel (XLS/XLSX) files to HTML using C#. Furthermore, you will come to know how to use additional options to customize the Excel to HTML conversion.'
tags: ['convert excel to html csharp', 'xls to html csharp', 'xlsx to html csharp']
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/Excel-to-HTML-Logo.jpg" alt="excel to html C#">}}


Excel to HTML conversion could be useful in various scenarios such as converting sheets to web pages or embedding the content of the sheets within the web applications and so on. In this article, you will learn **how to convert MS Excel XLSX or XLS files to HTML using C#**. Furthermore, you will come to know how to use additional options to customize the Excel to HTML conversion.

*   [Excel to HTML C# API][1]
*   [Convert Excel to HTML using C#][2]
*   [Enable Tooltips in Converted HTML using C#][3]
*   [Use Presentation Preference in Excel to HTML Conversion][4]

## Excel to HTML C# API {#Excel-to-HTML-CSharp-API}

[Aspose.Cells for .NET][5] is a well-known spreadsheet manipulation API that lets you create, read, and modify Excel files without MS Office. The API also provides a built-in spreadsheet converter that allows you to convert Excel worksheets to HTML files with high fidelity. You can [download][6] the API or install it within your application using [NuGet][7].

```
PM> Install-Package Aspose.Cells
```

## Excel XLSX to HTML C# Conversion {#Convert-Excel-to-HTML-using-CSharp}

Excel to HTML conversion can be achieved within a couple of lines of code. Just load the Excel file and save it with _.html_ extension. The following are the steps to perform this operation.

*   Load the Excel XLS/XLSX file using [Workbook][8] class.
*   Convert XLS/XLSX to HTML using [Workbook.Save(String)][9] method.

The following code sample shows how to convert XLS/XLSX file to HTML using C#.

{{< gist aspose-com-gists da22d973f26a723a870656f524d2be06 "excel-to-html.cs" >}}

## C# XLSX to HTML - Enable Tooltips {#Enable-Tooltips-in-Excel-to-HTML-using-CSharp}

There might be the case when the text's length exceeds the width of cells in the worksheets. In such a scenario, the text gets cut off in the converted HTML file. To tackle this issue, Aspose.Cells for .NET provides the option for enabling tooltips in the HTML file. The following are the steps to do so.

*   Load the Excel file using [Workbook][10] class.
*   Create an object of [HtmlSaveOptions][11] class.
*   Enable tooltip using [HtmlSaveOptions.AddTooltipText][12] property.
*   Save Excel file as HTML using [Workbook.Save(String, HtmlSaveOptions)][13] method.

The following code sample shows how to enable tooltips in Excel to HTML conversion in C#.

{{< gist aspose-com-gists da22d973f26a723a870656f524d2be06 "excel-to-html-tooltip.cs" >}}

## Use Presentation Preference in Excel to HTML Conversion {#Use-Presentation-Preference-in-Excel-to-HTML-Conversion}

Aspose.Cells for .NET provides [HtmlSaveOptions.PresentationPreference][14] property that makes you enhance the rendering of the spreadsheet's layout in the resultant HTML file. In other words, it is used to get a more attractive presentation of Excel workbooks.

The following code sample shows how to enhance the presentation of Excel files.

{{< gist aspose-com-gists da22d973f26a723a870656f524d2be06 "excel-to-html-presentation-preference.cs" >}}

## Conclusion

In this article, you have learned how to convert Excel XLSX and XLS files to HTML using C#. Furthermore, you have seen how to enable tooltips and presentation preference options in Excel to HTML conversion. You can read more about Aspose.Cells for .NET using [documentation][15].

## See Also

*   [Create MS Excel Files in C# without MS Office][16]




[1]: #Excel-to-HTML-CSharp-API
[2]: #Convert-Excel-to-HTML-using-CSharp
[3]: #Enable-Tooltips-in-Excel-to-HTML-using-CSharp
[4]: #Use-Presentation-Preference-in-Excel-to-HTML-Conversion
[5]: https://products.aspose.com/cells/net
[6]: https://downloads.aspose.com/cells/net
[7]: http://nuget.org/packages/Aspose.Cells
[8]: https://apireference.aspose.com/cells/net/aspose.cells/workbook
[9]: https://apireference.aspose.com/cells/net/aspose.cells.workbook/save/methods/2
[10]: https://apireference.aspose.com/cells/net/aspose.cells/workbook
[11]: https://apireference.aspose.com/cells/net/aspose.cells/htmlsaveoptions
[12]: https://apireference.aspose.com/cells/net/aspose.cells/htmlsaveoptions/properties/addtooltiptext
[13]: https://apireference.aspose.com/cells/net/aspose.cells.workbook/save/methods/4
[14]: https://apireference.aspose.com/cells/net/aspose.cells/htmlsaveoptions/properties/presentationpreference
[15]: https://docs.aspose.com/cells/java/getting-started/
[16]: https://blog.aspose.com/2020/01/21/create-excel-xls-xlsx-programmatically-in-csharp-net/






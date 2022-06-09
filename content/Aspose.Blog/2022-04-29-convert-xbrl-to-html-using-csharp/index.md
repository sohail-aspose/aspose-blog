---
title: 'Convert XBRL to HTML using C#'
seoTitle: "Convert XBRL to HTML using C# | XBRL to HTML in C# | XML to HTML C#"
description: "Programmatically convert XBRL to HTML using C# with Aspose.Finance for .NET API. Convert XBRL XML files to HTML webpages using C#. XBRL to HTML Converter API"
date: Fri, 29 Apr 2022 09:51:50 +0000
draft: false
url: /2022/04/29/convert-xbrl-to-html-using-csharp/
author: Muzammil Khan
summary: 'As a .NET developer, you can easily convert XBRL files or financial data from XML files to HTML webpages programmatically. In this article, you will learn **how to convert XBRL to HTML using C#**.'
tags: ['Convert XBRL in Csharp', 'Convert XBRL to HTML', 'Convert XBRL to HTML in C#', 'View XBRL in Browser C#', 'XBRL', 'XBRL to HTML', 'XBRL to HTML in C#', 'XBRL to XLSX']
categories: ['Aspose.Cells Product Family', 'Aspose.Finance Product Family']
---



{{< figure align=center src="images/convert-xbrl-to-html-using-csharp.jpg" alt="Convert XBRL to HTML using C#">}}


[XBRL][1] (_eXtensible Business Reporting Language_) is an XML-based markup language used for standardized business reporting of a company’s financial performance. It provides a way to communicate and exchange business information between business systems. In certain cases, we may need to extract and share XBRL data in an [HTML][2] webpage to view in web browsers. In this article, we will learn **how to convert XBRL to HTML using C#**.

The following topics shall be covered in this article:

*   [C# API to Convert XBRL to HTML][3]
*   [Convert XBRL to HTML][4]
*   [Export XBRL XML to HTML][5]

## C# API to Convert XBRL to HTML {#CSharp-API-to-Convert-XBRL-to-HTML}

For converting XBRL to an HTML file, we will follow a two-step procedure. Firstly, we will be using the [Aspose.Finance for .NET][6] to convert XBRL to [XLSX][7], and then we will convert the XLSX to HTML using [Aspose.Cells for .NET][8] APIs. Please either [download][9] the DLLs of the APIs or install them using [NuGet][10].

```
PM> Install-Package Aspose.Finance
PM> Install-Package Aspose.Cells
```

## Convert XBRL to HTML in C# {#Convert-XBRL-to-HTML-in-CSharp}

We can easily convert the XBRL files (.xbrl) to HTML webpages by following the steps given below:

*   Firstly, load the XBRL file using the **_[XbrlDocument][11]_** class.
*   Next, create an instance of the**_ [SaveOptions][12]_** class and set the **_[SaveFormat][13] _**as XLSX.
*   Then, convert XBRL to XLSX and save it in a _FileStream _object using **_[XbrlDocument.Save()][14]_** method.
*   After that, open the XLSX _FileStream _object using the **_[Workbook][15]_** class.
*   Finally, call the **_[Workbook.Save()][16]_** method to save the document in HTML format. It takes the output file path and the [**_SaveFormat_**][17] type (HTML) as arguments.

The following code sample demonstrates **how to convert XBRL to HTML using C#**.

{{< gist aspose-com-gists 8a42ccd9d8e34d8f87b21535ab34dfd4 "ConvertXBRLtoHTML_CSharp_ConvertXBRL.cs" >}}



{{< figure align=center src="images/Convert-XBRL-to-HTML-in-CSharp-1024x555.jpg" alt="Convert XBRL to HTML in C#." caption="Convert XBRL to HTML in C#.">}}


## **Export XBRL XML to HTML using C#** {#Export-XBRL-XML-to-HTML-using-CSharp}

We can also convert the XBRL data from an XML file (.xml) to an HTML webpage by following the steps mentioned earlier. However, we just need to input the .xml file instead of the .xbrl file in the first step.

The following code sample demonstrates **how to export data from an XML file to HTML using C#**.

{{< gist aspose-com-gists 8a42ccd9d8e34d8f87b21535ab34dfd4 "ConvertXBRLtoHTML_CSharp_ExportXML.cs" >}}

## Get a Free License {#Get-a-Free-API-License}

You can [get a free temporary license][18] to try the library without evaluation limitations.

## Conclusion

In this article, we have learned **how to convert an XBRL file to an HTML webpage**. We have also seen **how to save XBRL data from an XML file to HTML** programmatically. Besides, you can learn more about Aspose.Finance for .NET API using the [documentation][19]. In case of any ambiguity, please feel free to contact us on the [forum][20].

## See Also

*   [Create, Parse and Validate XBRL and iXBRL Financial Reports using C#][21]
*   [Convert XBRL to PDF using C#][22]




[1]: https://docs.fileformat.com/finance/xbrl/
[2]: https://docs.fileformat.com/web/html/
[3]: #CSharp-API-to-Convert-XBRL-to-HTML
[4]: #Convert-XBRL-to-HTML-in-CSharp
[5]: #Export-XBRL-XML-to-HTML-using-CSharp
[6]: https://products.aspose.com/finance/net
[7]: https://docs.fileformat.com/spreadsheet/xlsx/
[8]: https://products.aspose.com/cells/net
[9]: https://downloads.aspose.com/
[10]: https://www.nuget.org/packages/Aspose.Finance/
[11]: https://apireference.aspose.com/finance/net/aspose.finance.xbrl/xbrldocument
[12]: https://apireference.aspose.com/finance/net/aspose.finance.xbrl/saveoptions
[13]: https://apireference.aspose.com/finance/net/aspose.finance.xbrl/saveformat
[14]: https://apireference.aspose.com/finance/net/aspose.finance.xbrl/xbrldocument/methods/save
[15]: https://apireference.aspose.com/cells/net/aspose.cells/workbook
[16]: https://apireference.aspose.com/cells/net/aspose.cells.workbook/save/methods/3
[17]: https://apireference.aspose.com/cells/net/aspose.cells/saveformat
[18]: https://purchase.aspose.com/temporary-license
[19]: https://docs.aspose.com/finance/net/
[20]: https://forum.aspose.com/c/finance/
[21]: https://blog.aspose.com/2020/04/29/create-xbrl-instances-and-parse-and-validate-xbrl-and-ixbrl-files-in-csharp-asp.net/
[22]: https://blog.aspose.com/2022/03/20/convert-xbrl-to-pdf-using-csharp/





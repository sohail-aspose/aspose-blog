---
title: 'Convert XBRL to PDF using C#'
date: Sun, 20 Mar 2022 16:36:01 +0000
draft: false
url: /2022/03/20/convert-xbrl-to-pdf-using-csharp/
author: ''Muzammil Khan''
summary: 'As a .NET developer, you can easily convert XBRL files or financial data from XML files to PDF documents. In this article, you will learn **how to convert XBRL to PDF using C#**.'
tags: ['Convert XBRL in Csharp', 'Convert XBRL to PDF', 'Convert XBRL to PDF in C#', 'Convert XML to PDF in C#', 'XBRL', 'XBRL to PDF', 'XBRL to PDF in C#', 'XBRL to XLSX']
categories: ['Aspose.Finance Product Family']
---



{{< figure align=center src="images/convert-xbrl-to-pdf-using-csharp.jpg" alt="Convert XBRL to PDF using C#">}}


[XBRL][1] (_eXtensible Business Reporting Language_) file provides digital business reporting to exchange business information. It provides a way to communicate business and financial data such as balance sheets, cash flow statements, ledgers, etc. In various cases, we may need to extract and share XBRL data in [PDF][2] format. In this article, we will learn **how to convert XBRL to PDF using C#**.

The following topics shall be covered in this article:

*   [C# API to Convert XBRL to PDF][3]
*   [Convert XBRL to PDF][4]
*   [Convert XBRL XML to PDF][5]

## C# API to Convert XBRL to PDF {#CSharp-API-to-Convert-XBRL-to-PDF}

For converting XBRL to PDF documents, we will follow a two-step procedure. Firstly, we will be using the [Aspose.Finance for .NET][6] to convert XBRL to XLSX, and then we will convert the XLSX to a PDF document using [Aspose.Cells for .NET][7] APIs. Please either [download][8] the DLLs of the APIs or install them using [NuGet][9].

```
PM> Install-Package Aspose.Finance
PM> Install-Package Aspose.Cells
```

## Convert XBRL to PDF in C# {#Convert-XBRL-to-PDF-in-CSharp}

We can easily convert the XBRL file (.xbrl) to a PDF document by following the steps given below:

*   Firstly, load the XBRL file using the **_[XbrlDocument][10]_** class.
*   Next, create an instance of the **_[SaveOptions][11]_** class and set the **_[SaveFormat][12]_** as XLSX.
*   Then, convert XBRL to XLSX and save in a _FileStream_ object using **_[XbrlDocument.Save()][13]_** method.
*   After that, open the XLSX _FileStream_ object using the **_[Workbook][14]_** class.
*   Finally, call the **_[Workbook.Save()][15]_** method to save the document in PDF format. It takes the output file path and the [**_SaveFormat_**][16] type (PDF) as arguments.

The following code sample demonstrates **how to convert XBRL to a PDF using C#**.

{{< gist aspose-com-gists 15e45a549297be1e5e16493a240dd5ca "ConvertXBRLtoPDF_CSharp_XBRLToPDF.cs" >}}



{{< figure align=center src="images/Convert-XBRL-to-PDF-in-CSharp-1024x512.jpg" alt="Convert XBRL to PDF in C#" caption="Convert XBRL to PDF.">}}


## Convert XBRL XML to PDF using C# {#Convert-XBRL-XML-to-PDF-using-CSharp}

We can also convert the XBRL data from an XML file (.xml) to a PDF document by following the steps mentioned earlier. However, we just need to input the .xml file instead of the .xbrl file in the first step.

The following code sample demonstrates **how to convert an XML file to a PDF document using C#**.

{{< gist aspose-com-gists 15e45a549297be1e5e16493a240dd5ca "ConvertXBRLtoPDF_CSharp_XMLToPDF.cs" >}}

## Get a Free License {#Get-a-Free-API-License}

You can [get a free temporary license][17] to try the library without evaluation limitations.

## Conclusion

In this article, we have learned **how to convert an XBRL file to a PDF document**. We have also seen **how to save XBRL data from an XML file to a PDF document** programmatically. Besides, you can learn more about Aspose.Finance for .NET API using the [documentation][18]. In case of any ambiguity, please feel free to contact us on the [forum][19].

## See Also

*   [Create, Parse and Validate XBRL and iXBRL Financial Reports using C#][20]




[1]: https://docs.fileformat.com/finance/xbrl/
[2]: https://docs.fileformat.com/pdf/
[3]: #CSharp-API-to-Convert-XBRL-to-PDF
[4]: #Convert-XBRL-to-PDF-in-CSharp
[5]: #Convert-XBRL-XML-to-PDF-using-CSharp
[6]: https://products.aspose.com/finance/net
[7]: https://products.aspose.com/cells/net
[8]: https://downloads.aspose.com/
[9]: https://www.nuget.org/packages/Aspose.Finance/
[10]: https://apireference.aspose.com/finance/net/aspose.finance.xbrl/xbrldocument
[11]: https://apireference.aspose.com/finance/net/aspose.finance.xbrl/saveoptions
[12]: https://apireference.aspose.com/finance/net/aspose.finance.xbrl/saveformat
[13]: https://apireference.aspose.com/finance/net/aspose.finance.xbrl/xbrldocument/methods/save
[14]: https://apireference.aspose.com/cells/net/aspose.cells/workbook
[15]: https://apireference.aspose.com/cells/net/aspose.cells.workbook/save/methods/3
[16]: https://apireference.aspose.com/cells/net/aspose.cells/saveformat
[17]: https://purchase.aspose.com/temporary-license
[18]: https://docs.aspose.com/finance/net/
[19]: https://forum.aspose.com/c/finance/
[20]: https://blog.aspose.com/2020/04/29/create-xbrl-instances-and-parse-and-validate-xbrl-and-ixbrl-files-in-csharp-asp.net/





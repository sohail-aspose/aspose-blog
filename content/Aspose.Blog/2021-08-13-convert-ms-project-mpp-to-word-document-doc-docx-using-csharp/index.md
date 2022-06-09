---
title: 'Convert MS Project MPP to Word Document (DOC/DOCX) using C#'
seoTitle: "Convert MS Project MPP to Word Document (DOC/DOCX) using C#"
description: "Convert Microsoft Project MPP files to Word (DOC/DOCX) format using Aspose.Tasks for .NET and Aspose.PDF for .NET APIs within your .NET applications."
date: Fri, 13 Aug 2021 14:28:38 +0000
draft: false
url: /2021/08/13/convert-ms-project-mpp-to-word-document-doc-docx-using-csharp/
author: Muhammad Ahmad
summary: 'Microsoft Project ([MPP][1] files are used for different project management tasks like organizing and tracking projects and managing resources. If you want the project data in a document form to modify and share further, you can achieve that by converting the MPP file to Word [DOC][2]/[DOCX][3] format. In this article, you will learn **how to convert MPP files to Word documents using C#**.'
tags: ['Convert MPP to DOC using C#', 'Convert MPP to DOCX using C#', 'Convert MPP to Word using C#', 'Convert MS Project to Word using C#']
categories: ['Aspose.PDF Product Family', 'Aspose.Tasks Product Family']
---



{{< figure align=center src="images/MPP-to-Word.jpg" alt="DOCX) using C#">}}


Microsoft Project ([MPP][4] files are used for different project management tasks like organizing and tracking projects and managing resources. If you want the project data in a document form to modify and share further, you can achieve that by converting the MPP file to Word [DOC][5]/[DOCX][6] format. In this article, you will learn **how to convert MPP files to Word documents using C#**.

*   [C# APIs for Converting MPP Files to Word Documents][7]
*   [Convert MPP Files to Word DOC/DOCX Files using C#][8]

## C# APIs for Converting MPP Files to Word Documents {#CSharp-APIs-for-Converting-MPP-Files-to-Word-Documents}

We will perform this conversion using the [Aspose.Tasks for .NET][9] and [Aspose.PDF for .NET][10] APIs. The former is an API for working with Microsoft Project (MPP) files, whereas the latter is an API for creating, reading, and updating PDF files. We will use the Aspose.Tasks for .NET API to convert MPP files to PDF format and Aspose.PDF for .NET API to convert the generated PDF files to Word files. You can either install the APIs through NuGet or download them directly from the [Downloads][11] section.

```
PM> Install-Package Aspose.Tasks
PM> Install-Package Aspose.PDF
```

## Convert MPP Files to Word DOC/DOCX Files using C# {#Convert-MPP-Files-to-Word-DOC-DOCX-Files-using-CSharp}

You can easily convert your MPP files to Word documents using the steps given below.

*   Load the MPP file using the [Project][12] class.
*   Create an instance of the [MemoryStream][13] class.
*   Save the project to the stream as a PDF using the [Project.Save(Stream stream, SaveFileFormat format)][14] method.
*   Load the PDF from the stream using the [Document][15] class.
*   Save the PDF as a Word document using the [Document.Save(string outputFileName, SaveFormat format)][16] method.

The following sample code shows how to convert an MPP file to a Word document using C#.

{{< gist aspose-com-gists bccd1b214896e9691893914d72fe49df "Convert_MPP_To_DOCX.cs" >}}

## Get a Free License

In order to try the API without evaluation limitations, you can request [a free temporary license][17].

## Conclusion

In this article, you have learned how to convert Microsoft Project MPP files to Word documents using C#. We used the Aspose.Tasks for .NET API to convert the MPP file to PDF format and Aspose.PDF for .NET API to convert the PDF to Word format. You can learn more about these APIs by exploring their official documentation. In case of any questions, please feel free to reach us at our [free support forum][18].

*   [Aspose.Tasks for .NET Documentation][19]
*   [Aspose.PDF for .NET Documentation][20]

## See Also

*   [Convert MPP to Excel XLSX or CSV Programmatically in C#][21]




[1]: https://docs.fileformat.com/project-management/mpp/)
[2]: https://docs.fileformat.com/word-processing/doc/
[3]: https://docs.fileformat.com/word-processing/docx/
[4]: https://docs.fileformat.com/project-management/mpp/)
[5]: https://docs.fileformat.com/word-processing/doc/
[6]: https://docs.fileformat.com/word-processing/docx/
[7]: #CSharp-APIs-for-Converting-MPP-Files-to-Word-Documents
[8]: #Convert-MPP-Files-to-Word-DOC-DOCX-Files-using-CSharp
[9]: https://products.aspose.com/tasks/net/
[10]: https://products.aspose.com/pdf/net/?gclid=EAIaIQobChMIloj0ofmr8gIV3ca7CB0ZeAn-EAEYASAAEgLF7PD_BwE
[11]: https://downloads.aspose.com/total
[12]: https://apireference.aspose.com/tasks/net/aspose.tasks/project
[13]: https://docs.microsoft.com/en-gb/dotnet/api/system.io.memorystream?view=net-5.0
[14]: https://apireference.aspose.com/tasks/net/aspose.tasks.project/save/methods/1
[15]: https://apireference.aspose.com/pdf/net/aspose.pdf/document
[16]: https://apireference.aspose.com/pdf/net/aspose.pdf.document/save/methods/5
[17]: https://purchase.aspose.com/temporary-license
[18]: https://forum.aspose.com/
[19]: https://docs.aspose.com/tasks/net/
[20]: https://docs.aspose.com/pdf/net/
[21]: https://blog.aspose.com/2021/07/23/convert-mpp-to-excel-xlsx-csv-csharp/






---
title: 'Convert MPP File to PDF Programmatically using C# .NET'
seoTitle: "Convert Microsoft Project MPP File to PDF Programmatically in C# .NET"
description: "Convert MPP file (Microsoft Project) to PDF Programmatically using C#. You can export MPP file in .NET Framework using VB.NET as well."
date: Mon, 24 May 2021 13:14:00 +0000
draft: false
url: /2021/05/24/convert-mpp-file-to-pdf-programmatically-using-csharp-net/
author: Farhan Raza
summary: 'Microsoft Project Files are used to organize and manage different tasks in a project. You can convert MPP files to PDF programmatically using C#. You can find several options for the conversion in the following headings.'
tags: ['MPP to PDF Conversion .NET', 'MPP to PDF conversion', 'MPP to PDF csharp', 'convert MPP to PDF', 'mpp to pdf']
categories: ['Aspose.Tasks Product Family']
---



{{< figure align=center src="images/Convert-MPP-to-PDF.png" alt="Convert MPP to PDF">}}


Microsoft Project Files are used to organize and manage different tasks in a project. You can convert [MPP][1] files to [PDF][2] programmatically using C#. You can find several options for the conversion in the following headings:

*   [MPP to PDF Conversion – C# API Installation][3]
*   [Convert MPP to PDF Programmatically using C#][4]
*   [MPP to Multiple Pages PDF Conversion in C#][5]
*   [Convert MPP to Password Protected and Encrypted PDF File in C#][6]

## MPP to PDF Conversion – C# API Installation {#section1}

[Aspose.Tasks for .NET][7] API support working with Microsoft Project files. You can easily install the API by downloading the DLL file from [New Releases][8] section, or via [NuGet][9] Package Manager with the following installation command:

```
PM> Install-Package Aspose.Tasks
```

## Convert MPP to PDF Programmatically using C# {#section2}

You can convert MPP file to PDF documents with the following steps:

1.  Load input Project file (MPP).
2.  Export the output PDF file with [Save()][10] method.

The code below shows how to convert MPP file to PDF programmatically using C#:

{{< gist aspose-com-gists 920d26296d6511da9bf9ef8b503341f7 "MPP-to-PDF.cs" >}}

## MPP to Multiple Pages PDF Conversion in C# {#section3}

Sometimes you might need to convert different pages of an MPP file to separate PDF files. You can follow the steps below for converting a Project file to multiple pages:

1.  Load input MPP (Microsoft Project) file with [Project][11] class.
2.  Initialize [PdfSaveOptions][12] class object.
3.  Set [SaveToSeparateFiles][13] property to true.
4.  Specify the page numbers to export.
5.  Save the output PDF file.

The following code demonstrates how you can convert MPP file to multiple PDF files programmatically in C#:

{{< gist aspose-com-gists 920d26296d6511da9bf9ef8b503341f7 "MPP-to-Multiple-PDF.cs" >}}

## Convert MPP to Password Protected and Encrypted PDF File in C# {#section4}

MPP files can contain sensitive information about a project so you may need to share it only with authorized users. You can convert MPP file to an encrypted and password-protected PDF file with the following steps:

1.  Load input (MPP) Project file.
2.  Initialize [PdfEncryptionDetails][14] class object.
3.  Set permissions for the output PDF file.
4.  Initialize [PdfSaveOptions][15] class object.
5.  Save the output PDF file.

The code sample below explains how to convert MPP file to a password protected and encrypted PDF file using C#:

{{< gist aspose-com-gists 920d26296d6511da9bf9ef8b503341f7 "MPP-to-PDF-password.cs" >}}

## Get Free API License

You can evaluate the API in its full capacity by requesting a [Free Temporary License][16].

## Conclusion

In conclusion, you have learned how to convert an MPP file to PDF document programmatically using C#. Moreover, you have explored different features like encryption and password protection for the output PDF file. You may visit [API Documentation][17] to explore several other features offered by the API. In case you have some different requirements or want to discuss any concerns about your POC with the API, please feel free to contact us via the [Free Support Forum][18]. We will be glad to assist you.

## See Also

[Create MS Project Files Programmatically in C# or VB.NET][19]




[1]: https://docs.fileformat.com/project-management/mpp/
[2]: https://docs.fileformat.com/pdf/
[3]: #section1
[4]: #section2
[5]: #section3
[6]: #section4
[7]: https://products.aspose.com/tasks/net
[8]: https://downloads.aspose.com/tasks/net
[9]: https://www.nuget.org/packages/Aspose.Tasks/
[10]: https://apireference.aspose.com/tasks/net/aspose.tasks/project/methods/save/index
[11]: https://apireference.aspose.com/tasks/net/aspose.tasks/project
[12]: https://apireference.aspose.com/tasks/net/aspose.tasks.saving/pdfsaveoptions
[13]: https://apireference.aspose.com/tasks/net/aspose.tasks.saving/pdfsaveoptions/properties/savetoseparatefiles
[14]: https://apireference.aspose.com/tasks/net/aspose.tasks.saving/pdfencryptiondetails
[15]: https://apireference.aspose.com/tasks/net/aspose.tasks.saving/pdfsaveoptions
[16]: https://purchase.aspose.com/temporary-license
[17]: https://docs.aspose.com/tasks/net/
[18]: https://forum.aspose.com/c/tasks
[19]: https://blog.aspose.com/2020/05/05/create-ms-project-files-programmatically-add-tasks-and-resources-in-csharp-asp.net/






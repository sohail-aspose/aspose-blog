---
title: 'Add Data from Database to PDF in C# .NET'
date: Fri, 20 May 2022 15:48:37 +0000
draft: false
url: /2022/05/20/add-data-from-database-to-pdf-in-csharp-net/
author: ''Usman Aziz''
summary: 'Databases are almost everywhere to store and manage the data. It is a common practice of the programmers to retrieve the data from the databases and load it into the applications. When generating [PDF][1] files programmatically, one may need to populate the document with the data in database. To accomplish that in .NET applications, this article shows **how to add data from database to PDF files in C#**.'
tags: ['Add Data from Database to PDF Csharp', 'Add Data from Database to PDF in Entity Framework', 'DotNet API to Add Data from Database to PDF', 'DotNet PDF Generator API']
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/Create-Tables-in-PDF.jpg" alt="Add Data from Database to PDF in C#">}}


Databases are almost everywhere to store and manage the data. It is a common practice of the programmers to retrieve the data from the databases and load it into the applications. When generating [PDF][2] files programmatically, one may need to populate the document with the data in database. To accomplish that in .NET applications, this article shows **how to add data from database to PDF files in C#**.

*   [.NET API to Add Data from Database to PDF][3]
*   [Add Data from Database to PDF][4]
*   [Add Data from Database to PDF in Entity Framework][5]

## C# .NET API to Add Data from Database to PDF {#API-to-Add-Data-from-Database-to-PDF}

We will use [Aspose.PDF for .NET][6] to add data from database to PDF files. It is a popular PDF generation and manipulation API that allows you to create PDF files of simple and complex layouts seamlessly. You can either [download][7] the API's binaries or install it using [NuGet][8].

```
PM> Install-Package Aspose.PDF
```

## Add Data from Database to PDF in C# {#Add-Data-from-Database-to-PDF}

In most of the cases, the data is fetched from a database table into a _DataTable_ or _DataView_. Therefore, for demonstration, we will use a _DataTable_ to add data to a PDF file. To keep the things simpler, we will create and populate the _DataTable_ programmatically without using a database. The following are the steps to add data to a PDF file from database in C#.

*   Load the data into a [**DataTable**][9] from database.
*   Create a new PDF or load existing one using [**Document**][10] class.
*   Create an instance of [**Table**][11] class and set its properties, i.e. column width, borders, etc.
*   Import data from database to PDF table using [**Table.ImportDataTable()**][12] method.
*   Add the table to the page using [**Document.Pages\[index\].Paragraphs.Add(Table)**][13] method.
*   Save the PDF file using [**Document.Save(string)**][14] method.

The following code sample shows how to import data from database to PDF in C#.

{{< gist aspose-com-gists 3468179e05f17f74100ebd6c80955836 "add-data-to-pdf-from-database.cs" >}}

The following is the output of the above code sample.



{{< figure align=center src="images/Import-Data-from-Database-to-PDF.png" alt="Add Data from Database to PDF in C#">}}


## Add Data from Database to PDF in Entity Framework {#Add-Data-from-Database-in-Entity-Framework}

These days, Entity Framework (EF) is being commonly used by the developers. Therefore, it would be handy to extend the _Table_ class to populate PDF documents with lists or grouped data in EF. The following is the implementation of how to populate a PDF table using a list and grouped data. In both methods, the _Table_ and data is passed as arguments of the method.

{{< gist aspose-com-gists 3468179e05f17f74100ebd6c80955836 "add-data-to-pdf-from-database-ef.cs" >}}

## Get a Free License {#Get-a-Free-License}

You can [get a free temporary license][15] in order to use Aspose.PDF for .NET without evaluation limitations.

## Conclusion

In this article, you have learned how to add data from database into PDF files in C#. You have seen how to import data from a _DataTable_ into a table in PDF file. In addition, we have covered the implementation of importing data into PDF using Entity Framework. Besides, you can explore more about the C# PDF API using the [documentation][16]. In case you would have any questions or queries, you can contact us via our [forum][17].

## See Also

*   [Add or Remove Annotations in PDF Files using C#][18]
*   [Extract Images from PDF using C#][19]
*   [Create PDF File from Images using C#][20]




[1]: https://docs.fileformat.com/pdf/
[2]: https://docs.fileformat.com/pdf/
[3]: #API-to-Add-Data-from-Database-to-PDF
[4]: #Add-Data-from-Database-to-PDF
[5]: #Add-Data-from-Database-in-Entity-Framework
[6]: https://products.aspose.com/pdf/net/
[7]: https://downloads.aspose.com/pdf/net/
[8]: http://nuget.org/packages/Aspose.PDF
[9]: https://docs.microsoft.com/en-us/dotnet/api/system.data.datatable
[10]: https://apireference.aspose.com/pdf/net/aspose.pdf/document
[11]: https://apireference.aspose.com/pdf/net/aspose.pdf/table
[12]: https://apireference.aspose.com/pdf/net/aspose.pdf.table/importdatatable/methods/1
[13]: https://apireference.aspose.com/pdf/net/aspose.pdf/paragraphs/methods/add
[14]: https://apireference.aspose.com/pdf/net/aspose.pdf.document/save/methods/5
[15]: https://purchase.aspose.com/temporary-license
[16]: https://docs.aspose.com/pdf/net/
[17]: https://forum.aspose.com/
[18]: https://blog.aspose.com/2021/01/04/add-or-remove-annotations-in-pdf-using-csharp/
[19]: https://blog.aspose.com/2021/06/15/extract-images-from-pdf-in-csharp/
[20]: https://blog.aspose.com/2021/04/20/create-pdf-from-images-using-csharp/





---
title: 'Convert Excel Files to Google Sheets in C# .NET'
date: Thu, 10 Mar 2022 09:30:25 +0000
draft: false
url: /2022/03/10/convert-excel-to-google-sheets-in-csharp/
author: 'Usman Aziz'
summary: "Spreadsheets are commonly used for storing small or large-scale data in the form of rows and columns. Various applications are available to create and manipulate spreadsheets, of which [MS Excel][1] is a popular one. Alongside, Google provides [Google Sheets][2], which is used to create and update spreadsheets online. In addition, Google Sheets lets you share the spreadsheets with multiple people in real-time. In certain cases, you may need to export data from Excel XLS or XLSX files to a spreadsheet in Google Sheets programmatically. So let's see **how you can read data from an Excel file and write it to Google Sheets' spreadsheet in C# .NET**."
tags: ['Excel to Google Sheets in Csharp', 'Export Excel Data to Google Sheets in Csharp', 'XLS to Google Sheets in Csharp', 'XLSX to Google Sheets in Csharp']
categories: ['Aspose.Cells Product Family']
---

This article covers **how to convert MS Excel XLS or XLSX to Google Sheets programmatically in C# .NET**.



{{< figure align=center src="images/Convert-Excel-to-Google-Sheets.png" alt="Convert Excel XLS or XLSX to Google Sheets in C# .NET">}}


Spreadsheets are commonly used for storing small or large-scale data in the form of rows and columns. Various applications are available to create and manipulate spreadsheets, of which [MS Excel][3] is a popular one. Alongside, Google provides [Google Sheets][4], which is used to create and update spreadsheets online. In addition, Google Sheets lets you share the spreadsheets with multiple people in real-time. In certain cases, you may need to export data from Excel XLS or XLSX files to a spreadsheet in Google Sheets programmatically. So let's see **how you can read data from an Excel file and write it to Google Sheets' spreadsheet in C# .NET**.

*   [Prerequisites - Convert Excel File to Google Sheets][5]
    
    *   [Google Cloud Project][6]
    
    *   [.NET APIs for Excel to Google Sheets Conversion][7]
*   [Steps to Export Data from Excel XLSX to Google Sheets][8]
*   [Complete Source Code][9]

## Prerequisites - Convert Excel File to Google Sheets in C# {#Convert-Excel-XLS-XLSX-to-Google-Sheets-Prerequisites}

### Google Cloud Project {#Google-Cloud-Platform-Project}

To communicate with Google Sheets, we will have to create a project on [Google Cloud][10] and enable Google Sheets API. The following are the steps to create a project and enable the API.

1.  Go to [Google Cloud][11] console.
2.  [Create a new project][12] on the console.
    *   Select the project you have just created.
3.  From the navigation menu, select **APIs and Services** and then **Dashboard**.
    *   Click **Enable APIs and Services** button ([see details][13].
    *   Search and enable **Google Sheets API**.
4.  [Configure OAuth Consent Screen][14] and set scopes of the application.
    *   Add test users, which are used when application is not published.
5.  On [APIs and Services][15] page, go to **Credentials**.
    *   Click **Create Credentials** button and select **OAuth client ID**.
    *   In application type, select **Desktop App** (as we are creating a console application in this aritcle).
    *   Download the JSON file.

### C# .NET APIs for Excel to Google Sheets Conversion {#APIs-for-Excel-to-Google-Sheets-Conversion}

To export data from Excel XLS/XLSX files to Google Sheets, we will need the following APIs.

*   [Aspose.Cells for .NET][16] - To read the data from Excel files.
*   [Google.Apis.Sheets.v4][17] - To create and update spreadsheets on Google Sheets.

At the time of writing this article, we used **Aspose.Cells for .NET 22.2** and **Google.Apis.Sheets.v4 1.56.0.2608**.

## Export Data from Excel XLSX to Google Sheets in C# {#Steps-to-Export-Data-from-Excel-XLSX-to-Google-Sheets}

The following is the step-by-step guide on how to read data from an Excel XLSX file and write it to Google Sheets in a C# console application.

**1\.** Create a new console application project in Visual Studio 2013 or later.



{{< figure align=center src="images/Create-C-Console-Application.png" alt="Export Data from Excel XLSX to Google Sheets in C#">}}


**2\.** Install Aspose.Cells for .NET and Google Sheets APIs in the project.

```
PM> Install-Package Aspose.Cells
PM> Install-Package Google.Apis.Sheets.v4
```

**3\.** Copy the JSON file (we have downloaded after creating credentials in **Google Cloud**) and paste it into project's directory.

**4.** Initialize the Google Sheets service using the credentials (JSON file) and define the scopes of the application. The scopes define the access permissions to the sheets and their properties. The following function initializes the Google Sheets service and returns the **SheetsService** object.

{{< gist aspose-com-gists 33eaa207f475e2009d81e8b33244b29d "ConnectToGoogle.cs" >}}

**5\.** Create **CreateSpreadsheet** function that creates a new spreadsheet on Google Sheets, sets the name of the default sheet, and returns a **Spreadsheet** object.

{{< gist aspose-com-gists 33eaa207f475e2009d81e8b33244b29d "CreateSpreadsheet.cs" >}}

**6.** Create an **AddSheet** function to add a new sheet in the Google spreadsheet.

{{< gist aspose-com-gists 33eaa207f475e2009d81e8b33244b29d "AddSheet.cs" >}}

**7\.** Now, create a new function **ExportDataFromExcelToGoogleSheet**, which reads and exports data from an Excel file to Google Sheets. In this function, first, load the Excel XLS/XLSX file using Aspose.Cells for .NET and get the name of the first worksheet in the workbook.

{{< gist aspose-com-gists 33eaa207f475e2009d81e8b33244b29d "LoadExcelFile.cs" >}}

**8.** Then, call the **CreateSpreadsheet** function to create a new spreadsheet on Google Sheets.

{{< gist aspose-com-gists 33eaa207f475e2009d81e8b33244b29d "CreateNewSpreadsheet.cs" >}}

**9\.** Loop through the worksheets in the Excel file. In each iteration, read data from the worksheet and add it to a list.

{{< gist aspose-com-gists 33eaa207f475e2009d81e8b33244b29d "ReadExcelFile.cs" >}}

**10\.** For each worksheet in the Excel file, create a request to write data to the spreadsheet in the Google Sheets.

{{< gist aspose-com-gists 33eaa207f475e2009d81e8b33244b29d "WriteToGoogleSheets.cs" >}}

The complete function to export data from an Excel file to a spreadsheet in Google Sheets is given below.

{{< gist aspose-com-gists 33eaa207f475e2009d81e8b33244b29d "ExportDataFromExcelToGoogleSheet.cs" >}}

## Complete Source Code {#Complete-Source-Code}

The following is the complete source code to convert an Excel XLSX file to Google Sheets in C#.

{{< gist aspose-com-gists 33eaa207f475e2009d81e8b33244b29d "ConvertExcelToGoogleSheets.cs" >}}

## Demo - Convert Excel to Google Sheets in C#

<figure class="wp-block-embed is-type-video is-provider-youtube wp-block-embed-youtube wp-embed-aspect-16-9 wp-has-aspect-ratio"><div class="wp-block-embed__wrapper">https://www.youtube.com/watch?v=3Ygt0KCaOPI</div></figure>

## Get a Free Aspose.Cells License {#Get-a-Free-License}

You can get a free [temporary license][18] and use Aspose.Cells for .NET without evaluation limitations.

## Conclusion

In this article, you have learned how to convert Excel XLS or XLSX files to Google Sheets in C#. We have covered how to create a project on Google Cloud, enable Google Sheets API, read Excel files, and export data from Excel files to Google Sheets. Besides, you can explore other features of Aspose.Cells for .NET using the [documentation][19]. Also, you can ask your questions via our [forum][20].

## See Also

*   [Create, Read, and Edit Excel Spreadsheets in ASP.NET MVC][21]
*   [Create Excel Files in C# without MS Office][22]




[1]: https://www.microsoft.com/en-ww/microsoft-365/excel
[2]: https://www.google.com/sheets/about/
[3]: https://en.wikipedia.org/wiki/Microsoft_Excel
[4]: https://en.wikipedia.org/wiki/Google_Sheets
[5]: #Convert-Excel-XLS-XLSX-to-Google-Sheets-Prerequisites
[6]: #Google-Cloud-Platform-Project
[7]: #APIs-for-Excel-to-Google-Sheets-Conversion
[8]: #Steps-to-Export-Data-from-Excel-XLSX-to-Google-Sheets
[9]: #Complete-Source-Code
[10]: https://console.cloud.google.com/home/dashboard
[11]: https://console.cloud.google.com/home/dashboard
[12]: https://developers.google.com/workspace/guides/create-project
[13]: https://developers.google.com/workspace/guides/enable-apis)
[14]: https://developers.google.com/workspace/guides/configure-oauth-consent
[15]: https://console.cloud.google.com/apis/dashboard
[16]: https://products.aspose.com/cells/net/
[17]: https://www.nuget.org/packages/Google.Apis.Sheets.v4/
[18]: https://purchase.aspose.com/temporary-license
[19]: https://docs.aspose.com/cells/net
[20]: https://forum.aspose.com/
[21]: https://blog.aspose.com/2021/08/25/create-read-edit-excel-spreadsheet-in-asp-net-mvc/
[22]: https://blog.aspose.com/2020/01/21/create-excel-xls-xlsx-programmatically-in-csharp-net/





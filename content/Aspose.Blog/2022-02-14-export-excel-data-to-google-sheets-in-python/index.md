---
title: 'Export Excel Data to Google Sheets in Python'
seoTitle: "Export Excel Data to Google Sheets in Python | Python Google Sheets API"
description: "Export Excel XLS or XLSX date to spreadsheets in Google Sheets in Python. Complete guide to export Excel files to Google Sheets in Python."
date: Mon, 14 Feb 2022 07:06:00 +0000
draft: false
url: /2022/02/14/export-excel-data-to-google-sheets-in-python/
author: Usman Aziz
summary: '[Excel][1] files are widely used to store the data and perform various types of operations on it, such as generating charts, applying formulas. On the other hand, [Google Sheets][2] is a popular online application for creating and manipulating spreadsheets. Google Sheets also provides real-time sharing of spreadsheets with multiple people. In certain cases, you may need to export Excel XLS or XLSX files to Google Sheets programmatically. To achieve that, this article provides a complete guide on **how to set up a Google project and export data from Excel files to Google Sheets in Python**.'
tags: ['Convert Excel File to Google Sheets Python', 'Export Data from Excel XLSX to Google Sheets Python', 'Export Excel to Google Sheet in Python']
categories: ['Aspose.Cells Product Family']
---

In this article, you will learn **how to export Excel data to Google Sheets programmatically in Python**.



{{< figure align=center src="images/Convert-Excel-to-Google-Sheets.png" alt="Export Excel Files to Google Sheets in Python">}}


[Excel][3] files are widely used to store the data and perform various types of operations on it, such as generating charts, applying formulas. On the other hand, [Google Sheets][4] is a popular online application for creating and manipulating spreadsheets. Google Sheets also provides real-time sharing of spreadsheets with multiple people. In certain cases, you may need to export Excel XLS or XLSX files to Google Sheets programmatically. To achieve that, this article provides a complete guide on **how to set up a Google project and export data from Excel files to Google Sheets in Python**.

*   [Prerequisites - Export Excel Files to Google Sheets][5]
    
    *   [Google Cloud Project][6]
    
    *   [Python Libraries for Excel to Google Sheets Conversion][7]
*   [Export Data from Excel XLSX to Google Sheets][8]
*   [Complete Source Code][9]

## Prerequisites - Export Excel Data to Google Sheets in Python {#Convert-Excel-XLS-XLSX-to-Google-Sheets-Prerequisites}

### Google Cloud Project {#Google-Cloud-Platform-Project}

To communicate with Google Sheets, we will have to create a project on [Google Cloud][10] and enable Google Sheets API. Also, we need to create credentials that are used to authorize the actions we are going to perform with our code. You can read the guidelines on [how to create a Google Cloud project and enable Google Sheets API][11].

After creating the Google Cloud project and enabling the Google Sheets API, we can proceed to install the following APIs in our Python application.

### Python Libraries to Export Excel Files to Google Sheets {#APIs-for-Excel-to-Google-Sheets-Conversion}

To export data from Excel XLS/XLSX files to Google Sheets, we will need the following APIs.

*   [Aspose.Cells for Python][12] - To read the data from Excel files.
*   [Google Client Libraries][13] - To create and update spreadsheets on Google Sheets.

## Export Data from Excel to Google Sheets in Python {#Steps-to-Export-Data-from-Excel-XLSX-to-Google-Sheets}

The following is the step-by-step guide on how to read data from an Excel XLSX file and write it to Google Sheets in a Python application.

**1\.** Create a new Python application.

**2\.** Install **Aspose.Cells** and **Google client libraries** in the project.

```
pip install aspose.cells  
pip install --upgrade google-api-python-client google-auth-httplib2 google-auth-oauthlib 
```

**3\.** Place the JSON file (we have downloaded after creating credentials in **Google Cloud**) into the project's directory.

**4\.** Write a method named **create\_spreadsheet** that creates a new spreadsheet on Google Sheets, sets the name of the default sheet, and returns the ID of the spreadsheet.

{{< gist aspose-com-gists 9d23880f1c6e2063d5a089dad9147b50 "create_spreadsheet.py" >}}

**5.** Write another method named **add\_sheet** to add a new sheet in the Google spreadsheet.

{{< gist aspose-com-gists 9d23880f1c6e2063d5a089dad9147b50 "add_sheet.py" >}}

**6.** Now, initialize the Google Sheets service using the credentials (JSON file) and define the scopes of the application. The scopes parameter is used to specify the access permissions to Google Sheets and their properties.

{{< gist aspose-com-gists 9d23880f1c6e2063d5a089dad9147b50 "connect_to_google.py" >}}

**7\.** Then, load the Excel XLS or XLSX file using Aspose.Cells and get the name of the first worksheet in the workbook.

{{< gist aspose-com-gists 9d23880f1c6e2063d5a089dad9147b50 "load_excel_file.py" >}}

**8.** Call the **create\_spreadsheet** method to create a new spreadsheet on Google Sheets.

{{< gist aspose-com-gists 9d23880f1c6e2063d5a089dad9147b50 "create_new_spreadsheet.py" >}}

**9\.** Loop through the worksheets in the Excel file. In each iteration, read data from the worksheet and add it to an array.

{{< gist aspose-com-gists 9d23880f1c6e2063d5a089dad9147b50 "read_excel_file.py" >}}

**10\.** For each worksheet in the Excel file, create a request to write data to the Google Sheets.

{{< gist aspose-com-gists 9d23880f1c6e2063d5a089dad9147b50 "write_to_google_sheet.py" >}}

The following is the complete function to export data from an Excel file to a spreadsheet in Google Sheets.

{{< gist aspose-com-gists 9d23880f1c6e2063d5a089dad9147b50 "export_data_from_excel_to_google.py" >}}

## Complete Source Code {#Complete-Source-Code}

The following is the complete source code to export an Excel XLSX file to Google Sheets in Python.

{{< gist aspose-com-gists 9d23880f1c6e2063d5a089dad9147b50 "export_excel_to_google_sheets.py" >}}

## Get a Free Aspose.Cells License {#Get-a-Free-License}

You can get a free [temporary license][14] and use Aspose.Cells for Python without evaluation limitations.

## Conclusion

In this article, you have learned how to export Excel data to Google Sheets in Python. We have covered how to create a project on Google Cloud, enable Google Sheets API, read Excel files, and export data from Excel files to Google Sheets. To explore more about Aspose.Cells for Python, you can visit the [documentation][15]. Also, you can ask your questions via our [forum][16].

## See Also

*   [Create MS Excel Files using Python – Python Excel API][17]




[1]: https://www.microsoft.com/en-ww/microsoft-365/excel
[2]: https://www.google.com/sheets/about/
[3]: https://www.microsoft.com/en-ww/microsoft-365/excel
[4]: https://www.google.com/sheets/about/
[5]: #Convert-Excel-XLS-XLSX-to-Google-Sheets-Prerequisites
[6]: #Google-Cloud-Platform-Project
[7]: #APIs-for-Excel-to-Google-Sheets-Conversion
[8]: #Steps-to-Export-Data-from-Excel-XLSX-to-Google-Sheets
[9]: #Complete-Source-Code
[10]: https://console.cloud.google.com/home/dashboard
[11]: https://blog.aspose.com/2022/03/10/convert-excel-to-google-sheets-in-csharp/#Google-Cloud-Platform-Project
[12]: https://products.aspose.com/cells/python-java/
[13]: https://cloud.google.com/apis/docs/client-libraries-explained#google_api_client_libraries
[14]: https://purchase.aspose.com/temporary-license
[15]: https://docs.aspose.com/cells/pythonjava
[16]: https://forum.aspose.com/
[17]: https://blog.aspose.com/2020/08/19/create-excel-xls-xlsx-using-python-excel-api/





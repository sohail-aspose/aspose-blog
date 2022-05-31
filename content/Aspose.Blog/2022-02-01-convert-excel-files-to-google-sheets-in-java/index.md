---
title: 'Convert Excel Files to Google Sheets in Java'
date: Tue, 01 Feb 2022 12:03:00 +0000
draft: false
url: /2022/02/01/convert-excel-files-to-google-sheets-in-java/
author: 'Usman Aziz'
summary: "[Google Sheets][1] is a popular online application that lets you create and manipulate spreadsheet documents. Furthermore, it allows you to share the spreadsheets with multiple people in real-time. Therefore, often you have to export data from [Excel][2] workbooks to a spreadsheet in Google Sheets programmatically. In this article, we will give a complete walk-through of **how to export Excel data to a Google Sheets' spreadsheet in Java**."
tags: ['Convert Excel File to Google Sheets in Java', 'Export Excel Data to Google Sheets in java', 'How to Use Google Sheets API in Java', 'Java APIs for Excel to Google Sheets Conversion']
categories: ['Aspose.Cells Product Family']
---

This article shows **how to convert MS Excel XLS or XLSX to Google Sheets programmatically in Java**.



{{< figure align=center src="images/Convert-Excel-to-Google-Sheets.png" alt="Convert Excel XLS or XLSX to Google Sheets in Java">}}


[Google Sheets][3] is a popular online application that lets you create and manipulate spreadsheet documents. Furthermore, it allows you to share the spreadsheets with multiple people in real-time. Therefore, often you have to export data from [Excel][4] workbooks to a spreadsheet in Google Sheets programmatically. In this article, we will give a complete walk-through of **how to export Excel data to a Google Sheets' spreadsheet in Java**.

*   [Prerequisites - Convert Excel File to Google Sheets][5]
    
    *   [Google Cloud Project][6]
    
    *   [Java APIs for Excel to Google Sheets Conversion][7]
*   [Steps to Export Excel XLSX to Google Sheets][8]
*   [Complete Source Code][9]

## Prerequisites - Convert Excel File to Google Sheets in Java {#Convert-Excel-XLS-XLSX-to-Google-Sheets-Prerequisites}

### Google Cloud Project {#Google-Cloud-Platform-Project}

[Google Cloud][10] is a cloud computing platform, which provides various types of services that we can utilize in our applications. To use Google Sheets API, we will have to create a project on the Google Cloud console and enable Google Sheets API. You can read the step-by-step guide on [how to create a Google Cloud project and enable Sheets API][11].

### Java APIs for Excel to Google Sheets Conversion {#APIs-for-Excel-to-Google-Sheets-Conversion}

To export data from Excel XLS/XLSX files to Google Sheets, we will need the following APIs.

*   [Aspose.Cells for Java][12] - To read the data from Excel files.
*   Google Client APIs for Java - To create and update spreadsheets on Google Sheets.

To install these APIs, you can use the following configurations in your pom.xml file.

```
<repositories>
	<repository>
		<id>AsposeJavaAPI</id>
		<name>Aspose Java API</name>
		<url>http://repository.aspose.com/repo/</url>
	</repository>
</repositories>
<dependencies>
	<dependency>
		<groupId>com.google.api-client</groupId>
		<artifactId>google-api-client-gson</artifactId>
		<version>1.33.0</version>
	</dependency>
	<dependency>
		<groupId>com.google.oauth-client</groupId>
		<artifactId>google-oauth-client-jetty</artifactId>
		<version>1.32.1</version>
	</dependency>
	<dependency>
		<groupId>com.google.apis</groupId>
		<artifactId>google-api-services-sheets</artifactId>
		<version>v4-rev20210629-1.32.1</version>
	</dependency>
	<dependency>
		<groupId>com.aspose</groupId>
		<artifactId>aspose-cells</artifactId>
		<version>22.2</version>
	</dependency>
</dependencies>
```

## Export Excel Data to Google Sheets in Java {#Steps-to-Export-Data-from-Excel-XLSX-to-Google-Sheets}

The following are the steps to read an Excel file and then export its data to Google Sheets in a Java console application.

**1\.** Create a new Java application (desktop).

**2\.** Install Aspose.Cells for Java and Google Client APIs in the project, as mentioned in the previous section.

**3\.** Copy the JSON file (the one we have downloaded after creating credentials in Google Cloud) and paste it into the project's directory.

**4.** Specify the scopes of the application that define the access permissions to the sheets. Also, create variables for the token directory path and JSON factory.

{{< gist aspose-com-gists 8c31b5d53e56a7c70d6a39ec6e65c9ed "variables.java" >}}

**5.** Create a **getCredentials** method that authorizes the user using the credentials file.

{{< gist aspose-com-gists 8c31b5d53e56a7c70d6a39ec6e65c9ed "getCredentials.java" >}}

**6\.** Create **createSpreadsheet** method to create a new spreadsheet on Google Sheets and set the name of the default sheet. This method returns a **Spreadsheet** object.

{{< gist aspose-com-gists 8c31b5d53e56a7c70d6a39ec6e65c9ed "createSpreadsheet.java" >}}

**7.** Create an **addSheet** method to add a new sheet in the Google spreadsheet.

{{< gist aspose-com-gists 8c31b5d53e56a7c70d6a39ec6e65c9ed "addSheet.java" >}}

**8\.** Now, create the **exportExcelToGoogle** method, and in this method, initialize the Sheets service.

{{< gist aspose-com-gists 8c31b5d53e56a7c70d6a39ec6e65c9ed "startService.java" >}}

**9.** Then, load the Excel XLS/XLSX file using Aspose.Cells for Java. Also, get the name of the first worksheet in the workbook.

{{< gist aspose-com-gists 8c31b5d53e56a7c70d6a39ec6e65c9ed "loadExcelFile.java" >}}

**10.** Call the **createSpreadsheet** method to create a new spreadsheet on Google Sheets.

{{< gist aspose-com-gists 8c31b5d53e56a7c70d6a39ec6e65c9ed "createNewSpreadsheet.java" >}}

**11\.** Read data from each worksheet and save it into a list.

{{< gist aspose-com-gists 8c31b5d53e56a7c70d6a39ec6e65c9ed "readExcelFile.java" >}}

**12\.** For each worksheet in the Excel file, create a request to write data to the spreadsheet in the Google Sheets.

{{< gist aspose-com-gists 8c31b5d53e56a7c70d6a39ec6e65c9ed "writeToGoogleSheets.java" >}}

The complete method to read and export data from an Excel file to a spreadsheet in Google Sheets is given below.

{{< gist aspose-com-gists 8c31b5d53e56a7c70d6a39ec6e65c9ed "exportExcelToGoogle.java" >}}

## Complete Source Code {#Complete-Source-Code}

The following is the complete source code to convert an Excel XLSX file to Google Sheets in Java.

{{< gist aspose-com-gists 8c31b5d53e56a7c70d6a39ec6e65c9ed "ConvertExcelToGoogleSheets.java" >}}

## Demo - Convert Excel Files to Google Sheets in Java

<figure class="wp-block-embed is-type-video is-provider-youtube wp-block-embed-youtube wp-embed-aspect-16-9 wp-has-aspect-ratio"><div class="wp-block-embed__wrapper">https://www.youtube.com/watch?v=DL8ivgUT9mg</div></figure>

## Get a Free Aspose.Cells License {#Get-a-Free-License}

You can get a free [temporary license][13] and use Aspose.Cells for Java without evaluation limitations.

## Conclusion

In this article, you have learned how to convert Excel XLS or XLSX files to Google Sheets programmatically in Java. We have provided the complete guidelines on how to create a Google Cloud project, enable Google Sheets API, read Excel files, and export data from Excel files to Google Sheets. You can also visit the [documentation][14] to read more about Aspose.Cells for Java. In case you would have any questions or queries, let us know via our [forum][15].

## See Also

*   [Create Excel Files using Java without MS Office][16]




[1]: https://en.wikipedia.org/wiki/Google_Sheets
[2]: https://en.wikipedia.org/wiki/Microsoft_Excel
[3]: https://en.wikipedia.org/wiki/Google_Sheets
[4]: https://en.wikipedia.org/wiki/Microsoft_Excel
[5]: #Convert-Excel-XLS-XLSX-to-Google-Sheets-Prerequisites
[6]: #Google-Cloud-Platform-Project
[7]: #APIs-for-Excel-to-Google-Sheets-Conversion
[8]: #Steps-to-Export-Data-from-Excel-XLSX-to-Google-Sheets
[9]: #Complete-Source-Code
[10]: https://en.wikipedia.org/wiki/Google_Cloud_Platform
[11]: https://blog.aspose.com/2022/03/10/convert-excel-to-google-sheets-in-csharp/#Google-Cloud-Platform-Project
[12]: https://products.aspose.com/cells/java/
[13]: https://purchase.aspose.com/temporary-license
[14]: https://docs.aspose.com/cells/java/
[15]: https://forum.aspose.com/
[16]: https://blog.aspose.com/2020/10/13/create-excel-xlsx-xls-using-java-without-ms-office/





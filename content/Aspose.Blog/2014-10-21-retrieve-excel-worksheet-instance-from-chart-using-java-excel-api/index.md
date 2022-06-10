---
title: 'Retrieve Excel Worksheet Instance from Chart using Java'
date: Tue, 21 Oct 2014 12:14:50 +0000
draft: false
url: /2014/10/21/retrieve-excel-worksheet-instance-from-chart-using-java-excel-api/
author: Babar Raza
summary: ''
tags: ['Aspose.Cells for Java', 'Babar Raza', 'Excel API', 'Excel Files', 'Java API', 'Spreadsheet Version', 'Workbook Properties', 'charts', 'spreadsheet']
categories: ['Aspose.Total Product Family', 'Aspose.Cells Product Family']
---



{{< figure align=center src="images/aspose-Cells-for-Java_100.png" alt="Aspose.Cells for Java">}}


We are pleased to announce that the Aspose.Cells for Java 8.2.2 is now available for public use. Head to the [download][1] section to give the new release a try. While you are downloading the latest version, here is a look at the biggest features in this month’s release. For a full list of bug fixes and improvements please refer to the release notes for [Aspose.Cells for Java 8.2.2][2], and if you are planning to upgrade the API from any previous version, we would suggest you to check the [Public API Changes][3] section.

## Get Worksheet Instance of the Chart using Java

Before the release of Aspose.Cells for Java 8.2.2, retrieving the Worksheet instance from the Chart object was not possible. The latest version has made this possible by exposing the Worksheet property for the Chart class. Please check the usage scenario below and the detailed article on [Getting Worksheet of a Chart][4].

```
 //Load a spreadsheet into an instance of Workbook
Workbook workbook = new Workbook("sample.xlsx");

//Get an instance of Chart from the collection of Charts in a Worksheet
Chart chart  = workbook.getWorksheets().get(0).getCharts().get(0);

//Get the instance of Worksheet in which the Chart object was contained
Worksheet  worksheet = chart.getWorksheet();

//Display Worksheet name
System.out.println("Chart's Sheet Name: " + worksheet.getName());
```

## Get a Spreadsheet's Application Version using Java

Microsoft Excel application allows the user to save spreadsheets to different formats corresponding to the application versions such as Microsoft Excel version 2003, 2007, 2010 and 2013. This information is embedded in the spreadsheet, and can be used for version identification. Aspose.Cells for Java now provides the means to get and set this information with the BuiltInDocumentPropertyCollection.Version property. Check the detailed article on [Getting the Version Number of the Application that Created the Excel Document][5].

## Other Enhancements & Improvements

The latest release of Aspose.Cells for Java 8.2.2 has fixed numerous problems, and the most notable of these  enhancements are:

*   Enhanced the overall performance of the Aspose.Cells API.
*   Tweaked the Worksheet2Image & Chart2Image rendering mechanisms.
*   Improved the Formula Engine to correct issues related to AVERAGEID, SUMPRODUCT & INDIRECT functions.

Please visit the [documentation][6] for details, and if you still have any questions, we always welcome inquiries on [Aspose.Cells Support Forum][7].




[1]: https://downloads.aspose.com/cells/java
[2]: https://products.aspose.com/cells/java
[3]: https://docs.aspose.com/cells/java/migrating-from-earlier-versions-of-aspose-cells/
[4]: https://docs.aspose.com/cells/java/get-worksheet-of-the-chart/
[5]: https://docs.aspose.com/cells/java/get-the-version-number-of-the-application-that-created-the-excel-document/
[6]: https://docs.aspose.com/cells/java/
[7]: https://forum.aspose.com/





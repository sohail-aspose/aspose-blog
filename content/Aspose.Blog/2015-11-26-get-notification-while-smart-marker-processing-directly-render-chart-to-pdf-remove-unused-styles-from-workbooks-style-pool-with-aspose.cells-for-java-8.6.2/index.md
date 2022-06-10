---
title: 'Get Notification for Smart Markers and Render Excel Chart to PDF using Java'
date: Thu, 26 Nov 2015 15:50:32 +0000
draft: false
url: /2015/11/26/get-notification-while-smart-marker-processing-directly-render-chart-to-pdf-remove-unused-styles-from-workbooks-style-pool-with-aspose.cells-for-java-8.6.2/
author: Babar Raza
summary: ''
tags: ['Babar Raza']
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/aspose-Cells-for-Java_100.png" alt="Aspose.Cells for Java">}}


Aspose.Cells for Java API has been upgraded to 8.6.2, and we are pleased to announce, this month's release contains many useful features and improvements along with some critical bug fixes. Please refer to the release notes of [Aspose.Cells for Java 8.6.2][1] for a full list of enhancements. If you are planning to upgrade the API from any previous version, we strongly suggest you to check the Public API Changes section to know what has been changed since your current revision of the API.

While you are downloading the latest build, here is a look at the biggest features in this release.

## Get Notification while Processing Smart Markers

Smart Markers are one of the advanced features offered by Aspose.Cells APIs to dynamically merge data with the help of specialized markers defined in a designer spreadsheet. Such spreadsheets can be considered as templates as they contain the formatting as well as the formulas along with markers but no contents, where the data gets populated at runtime based on the marker definition and associated data source. Aspose.Cells APIs have provided the specialized WorkbookDesigner class that is used to load the designer spreadsheets and process them against the particular source to populate the data.

Recently we have received requests in Aspose.Cells support forum to provide call back facility for the WorkbookDesigner class so that the process could emit notifications about the cell and/or smart marker being processed. With the release of Aspose.Cells for Java 8.6.2, the API has exposed the ISmartMarkerCallBack interface along with the WorkbookDesigner.CallBack property to fulfill this requirement. The current implementation of ISmartMarkerCallBack interface allows to capture the references of worksheet, cell & smart marker being processed.

The following piece of code demonstrates the usage of ISmartMarkerCallBack interface to define a new class that handles the call back for WorkbookDesigner.process method.

```
public class SmartMarkerCallBack implements ISmartMarkerCallBack 
{
	Workbook workbook;
	SmartMarkerCallBack(Workbook workbook)
	{
	    this.workbook = workbook;
	}

	@Override
	public void process(int sheetIndex, int rowIndex, int colIndex, String tableName, String columnName)
	{
	    System.out.println("Processing Cell : " + workbook.getWorksheets().get(sheetIndex).getName() + "!" + CellsHelper.cellIndexToName(rowIndex, colIndex));
	    System.out.println("Processing Marker : " + tableName + "." + columnName);
	}
} 
```

Rest of the process includes loading the designer spreadsheet containing the Smart Markers with an instance of WorkbookDesigner or creating a new designer spreadsheet from scratch and process it by setting the data source. However, in order to enable the notifications, it is necessary to set the WorkbookDesigner.CallBack property before calling the WorkbookDesigner.process method as demonstrated below.

```
//Instantiate a new Workbook designer
WorkbookDesigner report = new WorkbookDesigner();

//Get the first worksheet of the workbook
Worksheet sheet = report.getWorkbook().getWorksheets().get(0);

//Set the Variable Array marker to a cell
//You may also place this Smart Marker into a template file manually using Excel and then open this file via WorkbookDesigner 
sheet.getCells().get("A1").putValue("&=$VariableArray");

//Set the data source for the marker(s)
report.setDataSource("VariableArray", new String[] { "English", "Arabic", "Hindi", "Urdu", "French" });

//Set the CallBack property
report.setCallBack(new SmartMarkerCallBack(report.getWorkbook()));

//Process the markers
report.process(false); 
```

## Render Excel Chart to PDF in Java

The Aspose.Cells for Java 8.6.2 has introduced the Chart.toPdf method in order to simplify the task of rendering charts in PDF format. The previous solution was to copy the required chart onto a new Worksheet then render the worksheet to PDF while specifying the area containing the chart shape. This solution was prone to error due to the number of statements to accomplish the same goal that can now be achieved in a single statement. The Chart.toPdf method currently accepts a parameter of type String as file path location to store the resultant PDF directly onto the disk.

The following sample code explains the usage of Chart.toPdf method to [render a Chart in PDF format][2].

```
//Load spreadsheet containing charts
Workbook workbook = new Workbook(inputFilePath);

//Access first worksheet
Worksheet worksheet = workbook.getWorksheets().get(0);

//Access first chart inside the worksheet
Chart chart = worksheet.getCharts().get(0);

//Save the chart in PDF format
chart.toPdf(outputFilePath); 
```

## Remove Unused Styles from Workbook's Style Pool

It is fairly possible that a spreadsheet may contain styles that are not in use. Such scenario may easily occur when user copies cells from another workbook because in this case some styles are copied too. Due to the reason that styles are shared for many objects such as cells, rows, columns and so on, when one cell's content (including style) is replaced by the copied one, the Aspose.Cells APIs do not remove the old style from the style pool. Imagine if the user does the copy operation repeatedly, there will be more and more styles in the style pool. Such unused styles can now be removed from the object of the Workbook while using the newly exposed removeUnusedStyles method. However, the aforementioned method could impose performance plenty because it has to check all objects to make sure that one style is not being used by any object, so we recommend to use this method with great caution.

Following is the simple usage scenario to remove unused styles.

```
//Load spreadsheet
Workbook workbook = new Workbook(inputFilePath);

//Remove all unused styles from the template
workbook.removeUnusedStyles();
```

## Other Enhancements & Improvements

The most notable enhancements in this release are as follow:

*   Exposed Cells.Style property that can be used to access the default style for a particular Worksheet.
*   Exposed two new [events for the Aspose.Cells.GridWeb component][3], namely, AjaxCallFinished & CellModifiedOnAjax.
*   Provided support for nested objects with Smart Markers.
*   Enhanced the PDF & image rendering engines for a few cases related to charts.

## Aspose.Cells for Java Resources

The resources, you may need to accomplish your tasks:

*   [Home page for Aspose.Cells for Java API][4].
*   [Download Aspose.Cells for Java][5].
*   Aspose.Cells for Java online documentation – help documentation and API reference documents.
*   [Aspose.Cells Product Family Forum][6] – post your technical questions and queries, or any other problem you are facing while working with Aspose.Cells APIs.
*   [Enable blog Subscription][7] – Do not limit yourself, you can keep yourself updated with the latest news on Aspose.Cells APIs, new features, fixes and other API related topics by subscribing to Aspose.Cells blog.
*   [Aspose.Cells for Java Examples][8] – We have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: https://downloads.aspose.com/cells/java
[2]: https://docs.aspose.com/display/cellsjava/Chart+Rendering#ChartRendering-RenderingCharttoPDF
[3]: https://docs.aspose.com/display/cellsjava/Working+with+GridWeb
[4]: http://www.aspose.com/java/excel-component.aspx
[5]: http://www.aspose.com/community/files/72/java-components/aspose.cells-for-java/default.aspx
[6]: https://forum.aspose.com/
[7]: https://blog.aspose.com/
[8]: https://github.com/asposecells/Aspose_Cells_Java





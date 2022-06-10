---
title: 'Modify Excel VBA Code and Convert DataBar to Image using Java'
date: Thu, 19 Mar 2015 10:04:01 +0000
draft: false
url: /2015/03/19/modify-excel-vba-code-convert-databar-to-image-using-java/
author: Babar Raza
summary: ''
tags: ['Babar Raza', 'convert excel databar to image using java', 'modify excel VBA code using Java']
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/aspose-Cells-for-Java_100.png" alt="Aspose.Cells for Java">}}


[Aspose.Cells for Java][1] 8.4.0 has been released and we are pleased to announce that this month’s release contains many useful improvements and features including the long awaited feature to manipulate VBA code embedded inside the spreadsheets. Please refer to the release notes of [Aspose.Cells for Java 8.4.0][2] for a full list of bug fixes and improvements along with details on what has been changed in the public API since the previous release. If you are planning to upgrade the Aspose.Cells for Java API to the latest revision, we would strongly suggest you to check the complete Public API Changes section to know what has been changed in the API so far.

While you are downloading the latest build, here is a look at the showcased features of this release.

## Access & Modify Excel VBA Code using Java

Many of the Aspose.Cells users had been waiting for this feature, and now it is available with the release of Aspose.Cells for Java 8.4.0. The latest build of the API has exposed a new package and a few classes to provide the means to access the VBA code embedded inside the macro enabled spreadsheets, and to amend the code as per requirement. The details of the newly exposed classes are as follow.

*   VbaProject class can be used to fetch the VBA project from a given spreadsheet.
*   VbaModuleCollection class represents the collection of VBA modules that are part of a given VbaProject.
*   VbaModule class represents a single module from the VbaModuleCollection.

The following code snippet shows how to dynamically modify the VBA code segments.

```
 Workbook workbook = new Workbook("source.xlsm");

//Access the modules from the spreadsheet
VbaModuleCollection modules = workbook.getVbaProject().getModules();
//Iterate over the modules collection
for(int i=0; i < modules.getCount(); i++)
{
        //Access a particular module
	VbaModule module = modules.get(i);
        //Access the module code
        String code = module.getCodes();

        //Replace the original message with the modified message
        if (code.contains("This is test message."))
        {
              code = code.replace("This is test message.", "This is Aspose.Cells message.");
              module.setCodes(code);
        }
}

//Save the result
workbook.save("output.xlsm"); 
```

## Remove Pivot Table from Worksheet

Another worth mentioning feature is the support for Pivot Table removal. Aspose.Cells for Java 8.4.0 has provided this feature by exposing two new methods for the PivotTableCollection class that allows to delete a specific PivotTable from the collection depending upon the input parameter.

Here are a few details about the newly exposed methods whereas the code snippets are available in the detailed article as linked above.

*   PivotTableCollection.remove method accepts an object of PivotTable, and removes it from the collection.
*   PivotTableCollection.removeAt method accepts a zero index based integer value and removes the particular PivotTable from the collection.

## Support for Different Pivot Table Layouts

Microsoft Excel has predefined layouts for the Pivot Tables as listed below. Upon choosing any of these layouts, Microsoft Excel formats the Pivot Tables accordingly.

*   Compact Form
*   Outline Form
*   Tabular Form

Aspose.Cells for Java 8.4.0 provides the same functionality while using the newly exposed methods for the PivotTable class that allows to dynamically set the layouts as discussed above. Detailed article and sample code snippets are available at Changing the Layout of Pivot Table.

## Convert Excel DataBars to Images using Java

With the release of v8.4.0, the Aspose.Cells API has provided the DataBar.toImage method to save the conditionally formatted DataBar in image format. The DataBar.toImage method accepts two parameters as detailed below.

*   The first parameter is of type Cell on which conditional formatting has been applied.
*   The second parameter is of type ImageOrPrintOptions in order to set different parameters of the resultant image.

The following sample code demonstrates the use of DataBar.toImage method to render the DataBar in image format.

```
 Workbook workbook = new Workbook("source.xlsx");

//Access first worksheet
Worksheet worksheet = workbook.getWorksheets().get(0);

//Access the cell which contains conditional formatting databar
Cell cell = worksheet.getCells().get("C1");

//Get the conditional formatting of the cell
FormatConditionCollection fcc = cell.getFormatConditions();

//Access the conditional formatting databar
DataBar dbar = fcc.get(0).getDataBar();

//Create image or print options
ImageOrPrintOptions opts = new ImageOrPrintOptions();
opts.setImageFormat(ImageFormat.getPng());

//Get the image bytes of the databar
byte[] imgBytes = dbar.toImage(cell, opts);

//Write image bytes on the disk
FileOutputStream out = new FileOutputStream("databar.png");
out.write(imgBytes);
out.close(); 
```

## Custom Properties for the Document Information Panel

Aspose.Cells can be used to add custom properties inside the workbook object which are visible in the Document Information Panel when accessed through Microsoft Excel using the File > Info > Properties > Show Document Panel menu.

The following code snippet uses the ContentTypePropertyCollection.add method to add two custom properties.

```
 //Create a new spreadsheet of type XLSX
Workbook workbook = new Workbook(FileFormatType.XLSX);

//Add simple property without any type
workbook.getContentTypeProperties().add("MK31", "Simple Data");

//Add date time property with type
workbook.getContentTypeProperties().add("MK32", "04-Mar-2015", "DateTime");

//Save the result
workbook.save("output.xlsx"); 
```

## Other Enhancements & Fixes

Aspose.Cells for Java 8.4.0 has fixed a number of issues and enhanced the core to accommodate many customer requested features. Following are a few worth mentioning enhancements & fixes.

*   Provided the public API to control the bogus data while converting spreadsheets to HTML format.
*   Provided support for Japanese calender to format Data & Time in spreadsheets.
*   Provided the support to display Cell comments in the Aspose.Cells.GridWeb component.
*   Improved the generation of EMF (Enhanced Metafile) for spreadsheet rendering.
*   Improved the internal functioning of Anti Aliasing & other rendering hints for over all rendering module.
*   Enhanced the chart rendering mechanism to avoid the overlapping of Data Labels for certain cases.
*   Addressed a few exceptions related to Pivot Table refreshing and loading XLS type spreadsheets with Aspose.Cells for Java API.

Please visit the documentation for details, and if you still have any questions, we always welcome inquiries on [Aspose.Cells Support Forum][3].




[1]: https://products.aspose.com/cells/java
[2]: https://products.aspose.com/cells/java
[3]: https://forum.aspose.com/





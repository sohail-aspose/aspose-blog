---
title: 'Group Pivot Fields in the Pivot Table and Get DrawObject and Bound using DrawObjectEventHandler class with Aspose.Cells for Java 18.3'
date: Thu, 29 Mar 2018 12:30:59 +0000
draft: false
url: /2018/03/29/group-pivot-fields-in-the-pivot-table-and-get-drawobject-and-bound-using-drawobjecteventhandler-class-with-aspose.cells-for-java-18.3/
author: Mshakeel Faiz
summary: ''
tags: ['Muhammad Shakeel Faiz', 'Group pivot fields in the Excel Pivot Table in Java']
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/aspose-Cells-for-Java_100.png" alt="Aspose.Cells for Java">}}


We are pleased to announce the release of [Aspose.Cells for Java 18.3][1]. This release includes many new features and enhancements along with some critical bug fixes that further improve the overall stability of the APIs. We also recommend our clients to [use the powerful Aspose for Java APIs directly in their Maven Projects with simple configurations][2]. Please check the [release notes][3] in order to get an idea about what is new and what has been fixed with this revision of Aspose.Cells for Java. Here is a look at the major features in this release.

## Group Pivot Fields in the Pivot Table

Microsoft Excel allows you to group pivot fields in the Pivot Table. When there is a large amount of data related to a pivot field, it is better to group them into sections. Aspose.Cells provides this feature via the **PivotTable.setManualGroupField()** method. This was a long-awaited feature requested by many users. The following sample code loads the template Excel file and performs grouping operation on the first pivot field in the Pivot Table using the **PivotTable.setManualGroupField()** method.

```
//Load sample workbook
Workbook wb = new Workbook(dirPath + "sampleGroupPivotFieldsInPivotTable.xlsx");

//Access the second worksheet
Worksheet ws = wb.getWorksheets().get(1);

//Access the pivot table
PivotTable pt = ws.getPivotTables().get(0);

//Specify the start and end date time
DateTime dtStart = new DateTime(2008, 1, 1);//1-Jan-2018
DateTime dtEnd = new DateTime(2008, 9, 5); //5-Sep-2018

//Specify the group type list, we want to group by months and quarters
ArrayList groupTypeList = new ArrayList();
groupTypeList.add(PivotGroupByType.MONTHS);
groupTypeList.add(PivotGroupByType.QUARTERS);

//Apply the grouping on first pivot field
pt.setManualGroupField(0, dtStart, dtEnd, groupTypeList, 1);

//Refresh and calculate pivot table
pt.setRefreshDataFlag(true);
pt.refreshData();
pt.calculateData();
pt.setRefreshDataFlag(false);

//Save the output Excel file
wb.save(dirPath + "outputGroupPivotFieldsInPivotTable.xlsx"); 
```

Please see the following article for more detail on how to group pivot fields in the Pivot Table for your reference.

*   [Group Pivot Fields in the Pivot Table][4]

## Get DrawObject and Bound while Rendering to PDF using DrawObjectEventHandler Class

Aspose.Cells provides an abstract class **DrawObjectEventHandler** which has a **draw()** method. Users can implement DrawObjectEventHandler and utilize the draw() method to get the DrawObject and Bound while rendering Excel to PDF or Image. If you are rendering an Excel file to PDF, then you can utilize the DrawObjectEventHandler class with **PdfSaveOptions.DrawObjectEventHandler**. Similarly, if you are rendering an Excel file to Image, you can utilize the DrawObjectEventHandler class with **ImageOrPrintOptions.DrawObjectEventHandler**. The following sample code explains the usage of the DrawObjectEventHandler class with the PdfSaveOptions.DrawObjectEventHandler.

```
//Implement the concrete class of DrawObjectEventHandler
class clsDrawObjectEventHandler extends DrawObjectEventHandler
{
	public void draw(DrawObject drawObject, float x, float y, float width, float height)
	{
		System.out.println();

		//Print the coordinates and the value of Cell object
		if (drawObject.getType() == DrawObjectEnum.CELL)
		{
			System.out.println("[X]: " + x + " [Y]: " + y + " [Width]: " + width + " [Height]: " + height + " [Cell Value]: " + drawObject.getCell().getStringValue());
		}

		//Print the coordinates and the shape name of Image object
		if (drawObject.getType() == DrawObjectEnum.IMAGE)
		{
			System.out.println("[X]: " + x + " [Y]: " + y + " [Width]: " + width + " [Height]: " + height + " [Shape Name]: " + drawObject.getShape().getName());
		}

		System.out.println("----------------------");
	}
}
	 
//-------------------------------------------------------------
	 
void Run() throws Exception
{
	//Load sample Excel file
	Workbook wb = new Workbook(dirPath + "sampleGetDrawObjectAndBoundUsingDrawObjectEventHandler.xlsx");
 
	//Specify Pdf save options
	PdfSaveOptions opts = new PdfSaveOptions();
 
	//Assign the instance of DrawObjectEventHandler class
	opts.setDrawObjectEventHandler(new clsDrawObjectEventHandler());
 
	//Save to Pdf format with Pdf save options
	wb.save("outputGetDrawObjectAndBoundUsingDrawObjectEventHandler.pdf", opts);
} 
```

Please see the following article for more detail about this feature.

*   [Get DrawObject and Bound while rendering to Pdf using DrawObjectEventHandler class][5]

## Export Similar Border Style when Border Style is not Supported by Web Browsers

Microsoft Excel also supports dashed border types that are not supported by most web browsers. When you convert such an Excel file into HTML using Aspose.Cells, the borders are removed. However, Aspose.Cells allows you to accomplish the task and supports to display such borders with **HtmlSaveOptions.ExportSimilarBorderStyle** property. For more detail on the feature, please see this article for your reference.

*   [Export similar Border Style when Border Style is not supported by Web Browsers][6]

## Find if the Worksheet is Dialog Sheet

Dialog sheet is an older format that contains a dialog box. You can find if a sheet is a dialog or some other type with **Worksheet.Type** property. If it returns enumeration value **SheetType.DIALOG**, then it means, you are dealing with the Dialog sheet. For more detail, please see this article.

*   [Find if the Worksheet is Dialog Sheet][7]

## Access and Modify the Display Label of the Linked OLE Object

Microsoft Excel allows you to change the display label of the Ole Object. You can also access or modify the display label of the Ole object via Aspose.Cells APIs using the **OleObject.Label** property. Please see the following article with sample code and attachments explaining how to access and modify the display label of the linked Ole Object for your reference.

*   [Access and Modify the Display Label of the Linked Ole Object][8]

## Preserve Single Quote Prefix of Cell Value or Range

When you put some value inside a cell that has leading apostrophe or single quote mark, then Microsoft Excel hides it, but when you select the cell, it displays the leading apostrophe or single quote in a formula bar. Aspose.Cells provides **StyleFlag.QuotePrefix** property that will handle either preserving the quote or not preserving the quote for your needs. For more detail, please see this article.

*   [Preserve single quote prefix of cell value or range][9]

## Read Axis Labels after Calculating the Chart

You can read axis labels of your chart after calculating its values using the **Chart.calculate()** method. Please use the **Axis.AxisLabels** property for this purpose that will return the list of axis labels. For more detail, please see the following article.

*   [Read Axis Labels after Calculating the Chart][10]

## Specify Document Version of the Excel File using BuiltIn Document Properties

You can change the **Version number** of Excel file by right clicking the file and then selecting **Properties > Details** and then editing the Version number field. Please use **BuiltInDocumentPropertyCollection.DocumentVersion** property to change it programmatically using Aspose.Cells APIs. For more detail, please see the following article.

*   [Specify Document Version of the Excel File using BuiltIn Document Properties][11]

## Aspose.Cells for Java Resources

The resources, you may need to accomplish your tasks:

*   [Home of Aspose.Cells for Java API][12].
*   [Download Aspose.Cells for Java from Maven][13].
*   [Aspose.Cells for Java Documentation][14] – up-to-date documentation containing Programmer's Guide, Knowledge Base and much more.
*   [Aspose.Cells for Java API Reference Guide][15] – detailing the publicly exposed classes, methods, properties, constants & interfaces.
*   [Aspose.Cells Product Family Forum][16] – post your technical questions and queries, or any other problem you are facing while working with Aspose.Cells APIs.
*   [Aspose.Cells for Java Examples][17] – we have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: http://maven.aspose.com/repository/simple/ext-release-local/com/aspose/aspose-cells/18.3/
[2]: https://blog.aspose.com/2014/08/12/aspose-for-maven-aspose-cloud-maven-repository/
[3]: https://docs.aspose.com/display/cellsjava/Aspose.Cells+for+Java+18.3+Release+Notes
[4]: https://docs.aspose.com/display/cellsjava/Group+Pivot+Fields+in+the+Pivot+Table
[5]: https://docs.aspose.com/display/cellsjava/Get+DrawObject+and+Bound+while+rendering+to+Pdf+using+DrawObjectEventHandler+class
[6]: https://docs.aspose.com/display/cellsjava/Export+similar+Border+Style+when+Border+Style+is+not+supported+by+Web+Browsers
[7]: https://docs.aspose.com/display/cellsjava/Find+if+the+Worksheet+is+Dialog+Sheet
[8]: https://docs.aspose.com/display/cellsjava/Access+and+Modify+the+Display+Label+of+the+Linked+Ole+Object
[9]: https://docs.aspose.com/display/cellsjava/Preserve+Single+Quote+Prefix+of+Cell+Value+or+Range
[10]: https://docs.aspose.com/display/cellsjava/Read+Axis+Labels+after+Calculating+the+Chart
[11]: https://docs.aspose.com/display/cellsjava/Specify+Document+Version+of+the+Excel+File+using+BuiltIn+Document+Properties
[12]: https://products.aspose.com/cells/java
[13]: http://maven.aspose.com/repository/simple/ext-release-local/com/aspose/aspose-cells/
[14]: https://docs.aspose.com/display/cellsjava/home
[15]: https://apireference.aspose.com/java/cells
[16]: https://forum.aspose.com/c/cells
[17]: https://github.com/aspose-cells/Aspose.Cells-for-Java





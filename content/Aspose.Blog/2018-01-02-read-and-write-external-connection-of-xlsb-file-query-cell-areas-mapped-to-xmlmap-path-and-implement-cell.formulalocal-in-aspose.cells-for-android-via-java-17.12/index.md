---
title: 'Read and Write External Connection of XLSB file, Query Cell Areas Mapped to XmlMap Path and Implement Cell.FormulaLocal in Aspose.Cells for Android via Java 17.12'
date: Tue, 02 Jan 2018 09:04:25 +0000
draft: false
url: /2018/01/02/read-and-write-external-connection-of-xlsb-file-query-cell-areas-mapped-to-xmlmap-path-and-implement-cell.formulalocal-in-aspose.cells-for-android-via-java-17.12/
author: Amjad Sahi
summary: ''
tags: []
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/aspose-Cells-for-Android_100.png" alt="Aspose.Cells for Android logo">}}


We are pleased to announce the release of [Aspose.Cells for Android via Java 17.12][1]. This release includes a number of features, enhancements and bug fixes that further improve the overall stability and usability of the API. We also recommend our clients to [use the powerful Aspose for Java APIs directly in their Maven Projects with simple configurations][2]. Please check the [release notes][3] in order to get an idea about what is new and what has been fixed with this revision of Aspose.Cells for Android via Java. While you are downloading the latest build, here is a look at the most worth mentioning features in this release.

## Read and Write External Connection of XLSB file

Aspose.Cells already supports read and write external connection of xlsx file but now, it also supports this feature for xlsb file. However, the code is same for both types of format. Please see the following article that explains how to make use of this feature.

*   [Read and Write External Connection of XLSB file][4]

## Specify how to cross string in output HTML using HtmlCrossType

When cell contains text or string but it is larger than the width of the cell, then the string overflows if the next cell in next column is null or empty. When you save your Excel file into HTML, you can control this overflow by specifying the cross type using the **HtmlCrossType** enumeration.

*   [Specify how to cross string in output HTML using HtmlCrossType][5]

## Interrupt or Cancel the Formula Calculation of Workbook

Aspose.Cells provides a mechanism to interrupt or cancel the formula calculation of workbook using the **AbstractCalculationMonitor.interrupt()** method. This is useful when formula calculation of workbook is taking too much time and you want to cancel its processing.

*   [Interrupt or Cancel the Formula Calculation of Workbook][6]

```
//Implement calculation monitor class
class clsCalculationMonitor extends AbstractCalculationMonitor
{
    public void beforeCalculate(int sheetIndex, int rowIndex, int colIndex)
    {
        //Find the cell name
        String cellName = CellsHelper.cellIndexToName(rowIndex, colIndex);
  
        //Print the sheet, row and column index as well as cell name
        System.out.println(sheetIndex + "----" + rowIndex + "----" + colIndex + "----" + cellName);
  
        //If cell name is B8, interrupt/cancel the formula calculation
        if (cellName.equals("B8") == true)
        {
            this.interrupt("Interrupt/Cancel the formula calculation");
        }//if
  
    }//beforeCalculate
  
}//clsCalculationMonitor
  
//---------------------------------------------------------     
//---------------------------------------------------------
  
public void Run() throws Exception
{   
    //Load the sample Excel file
    Workbook wb = new Workbook(dirPath + "sampleCalculationMonitor.xlsx");
 
    //Create calculation options and assign instance of calculation monitor class
    CalculationOptions opts = new CalculationOptions();
    opts.setCalculationMonitor(new clsCalculationMonitor());
 
    //Calculate formula with calculation options
    wb.calculateFormula(opts);
}
```

## Set the Values Format Code of Chart Series

You can set the values format code of chart series using the **Series.ValuesFormatCode** property. This property is not only useful for the series which are based on the range inside the worksheet but also works well for the series created with array of values.

*   [Set the Values Format Code of Chart Series][7]

## Utilize Sheet.SheetId property of [OpenXml][8] using Aspose.Cells

Sheet.SheetId property is found inside the DocumentFormat.OpenXml.Spreadsheet namespace and is part of OpenXml. You can see this property and its value inside workbook.xml. Aspose.Cells provides the equivalent property as **Worksheet.TabId**.

*   [Utilize Sheet.SheetId property of OpenXml using Aspose.Cells][9]

## Find the root element name of Xml Map

Aspose.Cells allows you to find the root element name of XML map using **XmlMap.RootElementName** property. For more detail, please see this article.

*   [Find the Root Element Name of Xml Map][10]

## Query Cell Areas Mapped to Xml Map Path

You can query cell areas mapped to xml map path with Aspose.Cells using the **Worksheet.xmlMapQuery()** method. If the path exists, it will return the list of cell areas related to that path inside xml map. The first parameter of **Worksheet.xmlMapQuery()** method specifies the xml element path and the second parameter specifies the xml map you want to query.

*   [Query Cell Areas Mapped to Xml Map Path using Worksheet.XmlMapQuery method][11]

The following sample code queries the xml map two times and prints the list of cell areas returned by the **Worksheet.xmlMapQuery()** method on console.

```
//Load sample Excel file having Xml Map
Workbook wb = new Workbook(dirPath + "sampleXmlMapQuery.xlsx");

//Access first XML Map
XmlMap xmap = wb.getWorksheets().getXmlMaps().get(0);

//Access first worksheet
Worksheet ws = wb.getWorksheets().get(0);

//Query Xml Map from Path - /MiscData
System.out.println("Query Xml Map from Path - /MiscData");
ArrayList ret = ws.xmlMapQuery("/MiscData", xmap);

//Print returned ArrayList values
for (int i = 0; i < ret.size(); i++)
{
    System.out.println(ret.get(i));
}

System.out.println("");

//Query Xml Map from Path - /MiscData/row/Color
System.out.println("Query Xml Map from Path - /MiscData/row/Color");
ret = ws.xmlMapQuery("/MiscData/row/Color", xmap);

//Print returned ArrayList values
for (int i = 0; i < ret.size(); i++)
{
    System.out.println(ret.get(i));
} 
```

## Determine Smart Art Shape and Convert it to Group Shape

Smart Art shapes are special shapes that allow you create complex diagrams automatically. Aspose.Cells allows you to detect Smart Art shapes and convert them to Group shape that enables you to handle smart art shape like a group shape. Consequently, you will have access to the individual parts or shapes of the group shape.

*   [Determine if Shape is Smart Art Shape][12]
*   [Convert the Smart Art to Group Shape][13]

## Create and Protect a Shared Workbook

Microsoft Excel allows you to create a shared workbook. When you share the workbook, then more than one user can edit the workbook. Aspose.Cells enables you to create a shared workbook with **Workbook.Settings.Shared** property. Besides, you can protect or unprotect a shared workbook.

*   [Create a Shared Workbook with Aspose.Cells][14]
*   [Password Protect or Unprotect the Shared Workbook][15]

## Render Sequence of Pages using PageIndex and PageCount Properties of ImageOrPrintOptions

Aspose.Cells allows you to render sequence of pages of your Excel file to images using **ImageOrPrintOptions.PageIndex** and **ImageOrPrintOptions.PageCount** properties. These properties are useful when there are so many pages in your worksheet but you need to render a few pages only. This will not only save the processing time but also saves the memory consumption of the rendering process.

*   [Render Sequence of Pages using PageIndex and PageCount Properties of ImageOrPrintOptions][16]

## Ignore Errors while Rendering Excel to PDF

You can ignore all errors during the conversion process using the **PdfSaveOptions.IgnoreError** property. This way, conversion process will be completed smoothly without throwing any error or exception but data loss may occur.

*   [Ignore Errors while Rendering Excel to Pdf][17]

## Implement Cell.FormulaLocal similar to Excel VBA Range.FormulaLocal

Microsoft Excel formulas may have different names in different locales/regions or languages. For example, SUM function is called SUMME in German. Aspose.Cells cannot work with non-English function names. In Microsoft Excel VBA, there is **Range.FormulaLocal** property that returns the name of the function as per its language or region. Aspose.Cells also provides **Cell.FormulaLocal** property for this purpose. However, this property will only work when you will implement **GlobalizationSettings.getLocalFunctionName(String standardName)** method. For more detail, please see this article.

*   [Implement Cell.FormulaLocal similar to Excel VBA Range.FormulaLocal][18]

The following sample code explains how to implement **GlobalizationSettings.getLocalFunctionName(String standardName)** method.

```
//Implement GlobalizationSettings class
class GS extends GlobalizationSettings {

	public String getLocalFunctionName(String standardName)
	{
		//Change the SUM function name as per your needs.
		if(standardName.equals("SUM"))
		{
			return "UserFormulaLocal_SUM";				
		}
				
		//Change the AVERAGE function name as per your needs.
		if (standardName.equals("AVERAGE"))
		{
			return "UserFormulaLocal_AVERAGE";
		}

		return "";
	}//getLocalFunctionName
}//GS extends GlobalizationSettings

//-----------------------------------------
//-----------------------------------------

public void Run() throws Exception {

	//Create workbook
	Workbook wb = new Workbook();

	//Assign GlobalizationSettings implementation class
	wb.getSettings().setGlobalizationSettings(new GS());

	//Access first worksheet
	Worksheet ws = wb.getWorksheets().get(0);

	//Access some cell
	Cell cell = ws.getCells().get("C4");

	//Assign SUM formula and print its FormulaLocal
	cell.setFormula("SUM(A1:A2)");
	System.out.println("Formula Local: " + cell.getFormulaLocal());

	//Assign AVERAGE formula and print its FormulaLocal
	cell.setFormula("=AVERAGE(B1:B2, B5)");
	System.out.println("Formula Local: " + cell.getFormulaLocal());
} 
```

## Render Office Add-Ins while converting Excel to Pdf

Aspose.Cells now supports to render MS Office Add-ins (in Excel files) in the output PDF. You do not need to use any special method or property to render Office Add-Ins in the output PDF. For more detail, please see this article.

*   [Render Office Add-Ins while converting Excel to Pdf][19]

## Auto populate Smart Markers data to other worksheets if data is too large to handle in a single worksheet

Sometime, you want to auto populate smart marker data to other worksheets if it is too large. Suppose, your data source has 1500000 records. These are too many records for a single worksheet, then you can move the rest of the records to next worksheet. For more detail and sample code, please see this article.

*   [Auto Populate Smart Marker Data to Other Worksheets if Data is too Large][20]

## Set the Shape type of Data labels of chart

You can change the shape type of data labels of the chart using the **DataLabels.ShapeType** property. It takes the value of **DataLabelShapeType** enumeration and changes the shape type of data labels accordingly. For more detail, please see this article.

*   [Set the Shape Type of Data Labels of Chart][21]

## Export worksheet CSS separately in output HTML

Aspose.Cells provides the feature to export worksheet CSS separately when you convert your Excel file to HTML file format. Please use **HtmlSaveOptions.ExportWorksheetCSSSeparately** property for this purpose and set it to true while saving Excel file to HTML format. For more detail on the feature, please see this article/document for your reference.

*   Export Worksheet CSS Separately in Output HTML

## Prefix Table elements Styles with HtmlSaveOptions.TableCssId property

Aspose.Cells allows you to prefix table elements styles with **HtmlSaveOptions.TableCssId** property. For more detail, please see this article.

*   [Prefix Table Elements Styles with HtmlSaveOptions.TableCssId property][22]

## Aspose.Cells for Android via Java Resources

The resources, you may need to accomplish your tasks:

*   [Home of Aspose.Cells for Android via Java API][23].
*   [Aspose.Cells for Android via Java Download Section][24].
*   [Aspose.Cells for Android via Java Documentation][25] – up-to-date documentation containing Programmer's Guide, Knowledge Base and much more.
*   [Aspose.Cells for Android via Java API Reference Guide][26] – detailing the publicly exposed classes, methods, properties, constants & interfaces.
*   [Aspose.Cells Product Family Forum][27] – post your technical questions and queries, or any other problem you are facing while working with Aspose.Cells APIs.
*   [Enable Blog Subscription][28] – do not limit yourself, you can keep yourself updated with the latest news on Aspose.Cells APIs, new features, fixes and other API related topics by subscribing to Aspose.Cells blog.
*   [Aspose.Cells for Android via Java Examples][29] – we have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: https://downloads.aspose.com/cells/androidjava/new-releases/aspose.cells-for-android-via-java-17.12/
[2]: https://blog.aspose.com/2014/08/12/aspose-for-maven-aspose-cloud-maven-repository/
[3]: https://docs.aspose.com/display/cellsjava/Aspose.Cells+for+Android+via+Java+17.12+Release+Notes
[4]: https://docs.aspose.com/display/cellsjava/Read+and+Write+External+Connection+of+XLSB+file
[5]: https://docs.aspose.com/display/cellsjava/Specify+how+to+cross+string+in+output+HTML+using+HtmlCrossType
[6]: https://docs.aspose.com/display/cellsjava/Interrupt+or+Cancel+the+Formula+Calculation+of+Workbook
[7]: https://docs.aspose.com/display/cellsjava/Set+the+Values+Format+Code+of+Chart+Series
[8]: http://en.wikipedia.org/wiki/Office_Open_XML
[9]: https://docs.aspose.com/display/cellsjava/Utilize+Sheet.SheetId+property+of+OpenXml+using+Aspose.Cells
[10]: https://docs.aspose.com/display/cellsjava/Find+the+Root+Element+Name+of+Xml+Map
[11]: https://docs.aspose.com/display/cellsjava/Query+Cell+Areas+Mapped+to+Xml+Map+Path+using+Worksheet.XmlMapQuery+method
[12]: https://docs.aspose.com/display/cellsjava/Determine+if+Shape+is+Smart+Art+Shape
[13]: https://docs.aspose.com/display/cellsjava/Convert+the+Smart+Art+to+Group+Shape
[14]: https://docs.aspose.com/display/cellsjava/Create+Shared+Workbook+with+Aspose.Cells
[15]: https://docs.aspose.com/display/cellsjava/Password+Protect+or+Unprotect+the+Shared+Workbook
[16]: https://docs.aspose.com/display/cellsjava/Render+Sequence+of+Pages+using+PageIndex+and+PageCount+Properties+of+ImageOrPrintOptions
[17]: https://docs.aspose.com/display/cellsjava/Ignore+Errors+while+Rendering+Excel+to+Pdf
[18]: https://docs.aspose.com/display/cellsjava/Implement+Cell.FormulaLocal+similar+to+Excel+VBA+Range.FormulaLocal
[19]: https://docs.aspose.com/display/cellsjava/Render+Office+Add-Ins+while+converting+Excel+to+Pdf
[20]: https://docs.aspose.com/display/cellsjava/Auto+Populate+Smart+Marker+Data+to+Other+Worksheets+if+Data+is+too+Large
[21]: https://docs.aspose.com/display/cellsjava/Set+the+Shape+Type+of+Data+Labels+of+Chart
[22]: https://docs.aspose.com/display/cellsjava/Prefix+Table+Elements+Styles+with+HtmlSaveOptions.TableCssId+property
[23]: https://products.aspose.com/cells/android-java
[24]: https://downloads.aspose.com/cells/androidjava
[25]: https://docs.aspose.com/display/cellsandroidjava/Aspose.Cells+for+Android+via+Java+Home
[26]: https://apireference.aspose.com/java/cells
[27]: https://forum.aspose.com/c/cells
[28]: https://blog.aspose.com/category/aspose-products/aspose-cells-product-family/
[29]: https://github.com/aspose-cells/Aspose.Cells-for-Java





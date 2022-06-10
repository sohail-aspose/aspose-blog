---
title: 'Implement Cell.FormulaLocal similar to Excel VBA Range.FormulaLocal and Render Office Add-Ins while converting Excel to Pdf with Aspose.Cells for Java 17.12'
date: Fri, 29 Dec 2017 12:47:50 +0000
draft: false
url: /2017/12/29/implement-cell.formulalocal-similar-to-excel-vba-range.formulalocal-and-render-office-add-ins-while-converting-excel-to-pdf-with-aspose.cells-for-java-17.12/
author: Mshakeel Faiz
summary: ''
tags: ['Muhammad Shakeel Faiz', 'Aspose.Cells', 'Excel VBA Range.FormulaLocal in Java', 'Range.FormulaLocal in Java', 'VBA Range.FormulaLocal in Java']
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/aspose-Cells-for-Java_100.png" alt="Excel VBA Range.FormulaLocal in Java">}}


We are pleased to announce the release of [Aspose.Cells for Java 17.12][1]. This release includes many new features and enhancements along with some critical bug fixes that further improve the overall stability of the APIs. We also recommend our clients to [use the powerful Aspose for Java APIs directly in their Maven Projects with simple configurations][2]. Please check the [release notes][3] in order to get an idea about what is new and what has been fixed with this revision of Aspose.Cells for Java. Here is a look at the major features in this release.

# Implement Cell.FormulaLocal similar to Excel VBA Range.FormulaLocal

Microsoft Excel formulas may have different names in different locales/regions or languages. For example, SUM function is called SUMME in German. Aspose.Cells cannot work with non-English function names. In Microsoft Excel VBA, there is **Range.FormulaLocal** property that returns the name of the function as per its language or region. Aspose.Cells also provides **Cell.FormulaLocal** property for this purpose. However, this property will only work when you will implement **GlobalizationSettings.getLocalFunctionName(String standardName)** method. For more detail, please see this article.

*   [Find and Refresh the Nested or Children Pivot Tables of Parent Pivot Table][4] [Implement Cell.FormulaLocal similar to Excel VBA Range.FormulaLocal][5]

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

# Render Office Add-Ins while converting Excel to Pdf

Aspose.Cells now supports to render MS Office Add-ins (in Excel files) in the output PDF. You do not need to use any special method or property to render Office Add-Ins in the output PDF. For more detail, please see this article.

*   [Render Office Add-Ins while converting Excel to Pdf][6]

# Auto populate Smart Markers data to other worksheets if data is too large to handle in a single worksheet

Sometime, you want to auto populate smart marker data to other worksheets if it is too large. Suppose, your data source has 1500000 records. These are too many records for a single worksheet, then you can move the rest of the records to next worksheet. For more detail and sample code, please see this article.

*   [Auto Populate Smart Marker Data to Other Worksheets if Data is too Large][7]

# Set the Shape type of Data labels of chart

You can change the shape type of data labels of the chart using the **DataLabels.ShapeType** property. It takes the value of **DataLabelShapeType** enumeration and changes the shape type of data labels accordingly. For more detail, please see this article.

*   [Set the Shape Type of Data Labels of Chart][8]

# Export worksheet CSS separately in output HTML

Aspose.Cells provides the feature to export worksheet CSS separately when you convert your Excel file to HTML file format. Please use **HtmlSaveOptions.ExportWorksheetCSSSeparately** property for this purpose and set it to true while saving Excel file to HTML format. For more detail on the feature, please see this article/document for your reference.

*   Export Worksheet CSS Separately in Output HTML

# Prefix Table elements Styles with HtmlSaveOptions.TableCssId property

Aspose.Cells allows you to prefix table elements styles with **HtmlSaveOptions.TableCssId** property. For more detail, please see this article.

*   [Prefix Table Elements Styles with HtmlSaveOptions.TableCssId property][9]

## Aspose.Cells for Java Resources

The resources, you may need to accomplish your tasks:

*   [Home of Aspose.Cells for Java API][10].
*   [Aspose.Cells for Java Download Section][11].
*   [Aspose.Cells for Java Documentation][12] – up-to-date documentation containing Programmer's Guide, Knowledge Base and much more.
*   [Aspose.Cells for Java API Reference Guide][13] – detailing the publicly exposed classes, methods, properties, constants & interfaces.
*   [Aspose.Cells Product Family Forum][14] – post your technical questions and queries, or any other problem you are facing while working with Aspose.Cells APIs.
*   [Aspose.Cells for Java Examples][15] – we have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: http://maven.aspose.com/repository/simple/ext-release-local/com/aspose/aspose-cells/17.12/
[2]: https://blog.aspose.com/2014/08/12/aspose-for-maven-aspose-cloud-maven-repository/
[3]: https://docs.aspose.com/display/cellsjava/Aspose.Cells+for+Java+17.12+Release+Notes
[4]: https://docs.aspose.com/display/cellsjava/Implement+Cell.FormulaLocal+similar+to+Excel+VBA+Range.FormulaLocal
[5]: https://docs.aspose.com/display/cellsjava/Implement+Cell.FormulaLocal+similar+to+Excel+VBA+Range.FormulaLocal
[6]: https://docs.aspose.com/display/cellsjava/Render+Office+Add-Ins+while+converting+Excel+to+Pdf
[7]: https://docs.aspose.com/display/cellsjava/Auto+Populate+Smart+Marker+Data+to+Other+Worksheets+if+Data+is+too+Large
[8]: https://docs.aspose.com/display/cellsjava/Set+the+Shape+Type+of+Data+Labels+of+Chart
[9]: https://docs.aspose.com/display/cellsjava/Prefix+Table+Elements+Styles+with+HtmlSaveOptions.TableCssId+property
[10]: https://products.aspose.com/cells/java
[11]: https://downloads.aspose.com/cells/java
[12]: https://docs.aspose.com/display/cellsjava/home
[13]: https://apireference.aspose.com/java/cells
[14]: https://forum.aspose.com/c/cells
[15]: https://github.com/aspose-cells/Aspose.Cells-for-Java





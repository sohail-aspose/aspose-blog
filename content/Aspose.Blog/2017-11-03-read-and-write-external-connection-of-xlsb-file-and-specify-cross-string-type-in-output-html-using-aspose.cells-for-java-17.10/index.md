---
title: 'Read and Write External Connection of XLSB file and Specify Cross String Type in Output HTML using Aspose.Cells for Java 17.10'
date: Fri, 03 Nov 2017 13:52:51 +0000
draft: false
url: /2017/11/03/read-and-write-external-connection-of-xlsb-file-and-specify-cross-string-type-in-output-html-using-aspose.cells-for-java-17.10/
author: Mshakeel Faiz
summary: ''
tags: ['Muhammad Shakeel Faiz', 'edit xlsb db connection name in java', 'load and save XLSB in java', 'read db connection name in XLSB in Java', 'read external connection in XLSB in java']
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/aspose-Cells-for-Java_100.png" alt="Java API for XLSB File">}}


We are pleased to announce the release of [Aspose.Cells for Java 17.10][1]. This release includes many new features and enhancements along with some critical bug fixes that further improve the overall stability of the APIs. We also recommend our clients to [use the powerful Aspose for Java APIs directly in their Maven Projects with simple configurations][2]. Please check the [release notes][3] in order to get an idea about what is new and what has been fixed with this revision of Aspose.Cells for Java. Here is a look at the major features in this release.

## Read and Write External Connection of XLSB file

Aspose.Cells already supports read and write external connection of xlsx file but now, it also supports this feature for xlsb file. However, the code is same for both types of format. Please see the following article that explains how to make use of this feature.

*   [Read and Write External Connection of XLSB file  
    ](https://docs.aspose.com/display/cellsjava/Read+and+Write+External+Connection+of+XLSB+file)

## Specify how to cross string in output HTML using HtmlCrossType

When cell contains text or string but it is larger than the width of the cell, then the string overflows if the next cell in next column is null or empty. When you save your Excel file into HTML, you can control this overflow by specifying the cross type using the **HtmlCrossType** enumeration.

*   [Specify how to cross string in output HTML using HtmlCrossType][4]

## Interrupt or Cancel the Formula Calculation of Workbook

Aspose.Cells provides a mechanism to interrupt or cancel the formula calculation of workbook using the **AbstractCalculationMonitor.interrupt()** method. This is useful when formula calculation of workbook is taking too much time and you want to cancel its processing.

*   [Interrupt or Cancel the Formula Calculation of Workbook][5]

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

*   [Set the Values Format Code of Chart Series][6]

## Utilize Sheet.SheetId property of [OpenXml][7] using Aspose.Cells

Sheet.SheetId property is found inside the DocumentFormat.OpenXml.Spreadsheet namespace and is part of OpenXml. You can see this property and its value inside workbook.xml. Aspose.Cells provides the equivalent property as **Worksheet.TabId**.

*   [Utilize Sheet.SheetId property of OpenXml using Aspose.Cells][8]

## Aspose.Cells for Java Resources

The resources, you may need to accomplish your tasks:

*   [Home of Aspose.Cells for Java API][9].
*   [Aspose.Cells for Java Download Section][10].
*   [Aspose.Cells for Java Documentation][11] – up-to-date documentation containing Programmer's Guide, Knowledge Base and much more.
*   [Aspose.Cells for Java API Reference Guide][12] – detailing the publicly exposed classes, methods, properties, constants & interfaces.
*   [Aspose.Cells Product Family Forum][13] – post your technical questions and queries, or any other problem you are facing while working with Aspose.Cells APIs.
*   [Aspose.Cells for Java Examples][14] – we have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: https://downloads.aspose.com/cells/java/new-releases/aspose.cells-for-java-17.10/
[2]: https://blog.aspose.com/2014/08/12/aspose-for-maven-aspose-cloud-maven-repository/
[3]: https://docs.aspose.com/display/cellsjava/Aspose.Cells+for+Java+17.10+Release+Notes
[4]: https://docs.aspose.com/display/cellsjava/Specify+how+to+cross+string+in+output+HTML+using+HtmlCrossType
[5]: https://docs.aspose.com/display/cellsjava/Interrupt+or+Cancel+the+Formula+Calculation+of+Workbook
[6]: https://docs.aspose.com/display/cellsjava/Set+the+Values+Format+Code+of+Chart+Series
[7]: http://en.wikipedia.org/wiki/Office_Open_XML
[8]: https://docs.aspose.com/display/cellsjava/Utilize+Sheet.SheetId+property+of+OpenXml+using+Aspose.Cells
[9]: https://www.aspose.com/products/cells/java
[10]: https://downloads.aspose.com/cells/java
[11]: https://docs.aspose.com/display/cellsjava/home
[12]: https://apireference.aspose.com/java/cells
[13]: https://forum.aspose.com/c/cells
[14]: https://github.com/aspose-cells/Aspose.Cells-for-Java





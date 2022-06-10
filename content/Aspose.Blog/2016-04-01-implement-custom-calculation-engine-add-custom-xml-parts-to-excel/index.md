---
title: 'Implement Custom Calculation Engine and Add Custom XML Parts to Spreadsheets using Java'
date: Fri, 01 Apr 2016 15:17:05 +0000
draft: false
url: /2016/04/01/implement-custom-calculation-engine-add-custom-xml-parts-to-excel/
author: Babar Raza
summary: ''
tags: ['Babar Raza']
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/aspose-Cells-for-Java_100.png" alt="Aspose.Cells for Java">}}


We are pleased to announce the release of [Aspose.Cells for Java 8.7.2][1]. This month’s release includes new features, enhancements and bug fixes that further improve the overall stability and usability of the API. In order to get an idea about what is new and what has been fixed with this revision, please check the release notes. If you are planning to upgrade the API from any previous version, we strongly suggest you to check the Public API Changes section to know what has been changed since your current revision of the API.

While you are downloading the latest build, here is a look at the biggest features in this release.

## Implement Custom Calculation Engine

Aspose.Cells APIs have powerful calculation engine that can calculate almost all of the Microsoft Excel functions with precision. However, sometimes the application requirement demands to override any Excel formula in order to get desired results, such as return 3 for function **\=SUM(1,1)**, which isn't possible with default Aspose.Cells calculation engine.

The recent revision of Aspose.Cells for Java allows to extend the default calculation engine to get desired results. Aspose.Cells for Java 8.7.2 has exposed two new classes for this purpose as detailed below.

*   AbstractCalculationEngine: Represents custom calculation engine to extend the default calculation engine of Aspose.Cells.
*   CalculationData: Represents the required data when calculating one function, such as function name, parameters and so forth.

By implementing custom calculation engine, users can override all Excel's native functions with more flexibility. Below provided is the simplest usage scenario to define a custom calculation engine that extends AbstractCalculationEngine in order to override the Excel's default SUM function.

```
public class CustomEngine extends AbstractCalculationEngine
{
	public void calculate(CalculationData data)
        {
		if(data.getFunctionName().toUpperCase().equals("SUM")==true)
                {
                    double val = (double)data.getCalculatedValue();
                    val = val + 30;

                    data.setCalculatedValue(val);
                }
        }
} 
```

Here is how to use the newly defined custom calculation engine to get desired results.

```
Workbook workbook = new Workbook();

Worksheet sheet = workbook.getWorksheets().get(0);

Cell a1 = sheet.getCells().get("A1");
a1.setFormula("=Sum(B1:B2)");

sheet.getCells().get("B1").putValue(10);
sheet.getCells().get("B2").putValue(10);

//Without overriding the SUM function, the value of cell A1 will be 20
workbook.calculateFormula();

System.out.println("Without Custom Engine Value of A1: " + a1.getStringValue());

//After overriding the SUM function, the value of cell A1 will be 50
CustomEngine engine = new CustomEngine();

CalculationOptions opts = new CalculationOptions();
opts.setCustomEngine(engine);

workbook.calculateFormula(opts);

System.out.println("With Custom Engine Value of A1: " + a1.getStringValue()); 
```

## Add Custom XML Parts to Spreadsheets

Custom XML parts are the XML based data files stored by different applications like SharePoint inside the spreadsheet files. This data is consumed by different applications, however, Microsoft Excel application does not make use of this data so there is no GUI to add such data in the spreadsheets. One can view this data by extracting the contents of the spreadsheet (XLSX) using applications such as WinRar, and inspect the contents of the customXml folder.

Aspose.Cells for Java API provides the ContentTypePropertyCollection.add which can be used to add Custom XML data to the spreadsheet as demonstrated below.

```
//Create an instance of Workbook
Workbook workbook = new Workbook();

//Add custom XML to the collection of ContentTypeProperty objects 
workbook.getContentTypeProperties().add("BookStore", booksXML); 
```

## Access TextBox from Collection

Aspose.Cells for Java 8.7.2 has exposed the overloaded indexer for the TextBoxCollection class in order to access the instance of TextBox using its name as demonstrated below.

```
//Create an instance of Workbook
Workbook workbook = new Workbook();

//Access the first Worksheet from the collection
Worksheet sheet = workbook.getWorksheets().get(0);

//Add a TextBox to the collection
int idx = sheet.getTextBoxes().add(10, 10, 10, 10);

//Access the TextBox using its index
TextBox box = sheet.getTextBoxes().get(idx);

//Set the name for the TextBox
box.setName("MyTextBox");

//Access the same TextBox via its name
box = sheet.getTextBoxes().get("MyTextBox"); 
```

## Other Enhancements & Improvements

The most notable enhancements in this release are as follow:

*   Enhanced the HTML parsing as well as rendering to improve the fidelity.
*   Improved PDF rendering engine for chart objects.

## Aspose.Cells for Java Resources

The resources, you may need to accomplish your tasks:

*   [Home of Aspose.Cells for Java API][2].
*   [Aspose.Cells for Java Download Section][3].
*   Aspose.Cells for Java Documentation – up-to-date documentation containing Programmer's Guide, Knowledge Base and much more.
*   [Aspose.Cells for Java API Reference Guide][4] – detailing the publicly exposed classes, methods, properties, constants & interfaces.
*   [Aspose.Cells Product Family Forum][5] – post your technical questions and queries, or any other problem you are facing while working with Aspose.Cells APIs.
*   [Enable Blog Subscription][6] – do not limit yourself, you can keep yourself updated with the latest news on Aspose.Cells APIs, new features, fixes and other API related topics by subscribing to Aspose.Cells blog.
*   [Aspose.Cells for Java Examples][7] – we have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: https://products.aspose.com/cells/java
[2]: http://www.aspose.com/java/excel-component.aspx
[3]: http://www.aspose.com/community/files/72/java-components/aspose.cells-for-java/default.aspx
[4]: http://www.aspose.com/api/java/cells/com.aspose.cells/index
[5]: https://forum.aspose.com/
[6]: https://blog.aspose.com/
[7]: https://github.com/asposecells/Aspose_Cells_Java





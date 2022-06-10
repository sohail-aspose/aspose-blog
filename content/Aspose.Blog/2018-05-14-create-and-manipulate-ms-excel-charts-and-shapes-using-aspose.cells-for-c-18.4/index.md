---
title: 'Create and Manipulate MS Excel Charts and Shapes using Aspose.Cells for C++ 18.4'
date: Mon, 14 May 2018 18:14:37 +0000
draft: false
url: /2018/05/14/create-and-manipulate-ms-excel-charts-and-shapes-using-aspose.cells-for-c-18.4/
author: Amjad Sahi
summary: ''
tags: ['Create Charts and Shapes in Excel', 'Insert or extract OLE objects in Excel', 'Manipulate charts and shapes in Excel']
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/aspose_cells-for-cpp-150x150.png" alt="Create shapes and charts in Excel">}}


Aspose Team is pleased to announce the release of [Aspose.Cells for C++ 18.4.0][1]. This release supports to create and manipulate charts and shapes in XLS, XLSX, XLSM and XLSB file formats. These were the long-awaited features for the users. It also includes other enhancements and fixes that further improve the overall stability of the API. Please check the detailed [release notes][2] in order to get an idea about what is new and what has been enhanced with this revision of Aspose.Cells for C++.

While you are downloading the API build to give it a try, here is a list of added features along with a few code snippets for quick testing.

## Create and Customize MS Excel Charts

A chart is a visual display of information. Aspose.Cells for C++ now allows developers to visualize information in charts just as Microsoft Excel does. Creating charts at runtime, based on the data in a spreadsheet, is one of Aspose.Cells' demanding feature. Aspose.Cells supports to create both Standard and Customized charts. Below, we will show a few examples with sample files on how to create some common MS Excel chart types using Aspose.Cells API.

The following code demonstrates the use of Aspose.Cells for C++ API to create a Line chart in the spreadsheet.

```
// Output directory path
StringPtr outDir = new String("..\\Data\\02_OutputDirectory\\");
 
// Path of output excel file
StringPtr outputChartTypeLine = outDir->StringAppend(new String("outputChartTypeLine.xlsx"));
 
// Create a new workbook
intrusive_ptr workbook = Factory::CreateIWorkbook();
 
// Get first worksheet which is created by default
intrusive_ptr worksheet = workbook->GetIWorksheets()->GetObjectByIndex(0);
 
// Adding sample values to cells
worksheet->GetICells()->GetObjectByIndex(new String("A1"))->PutValue(50);
worksheet->GetICells()->GetObjectByIndex(new String("A2"))->PutValue(100);
worksheet->GetICells()->GetObjectByIndex(new String("A3"))->PutValue(150);
worksheet->GetICells()->GetObjectByIndex(new String("B1"))->PutValue(4);
worksheet->GetICells()->GetObjectByIndex(new String("B2"))->PutValue(20);
worksheet->GetICells()->GetObjectByIndex(new String("B3"))->PutValue(50);
 
// Adding a chart to the worksheet
int chartIndex = worksheet->GetICharts()->Add(Aspose::Cells::Charts::ChartType::ChartType_Line, 5, 0, 20, 8);
 
// Accessing the instance of the newly added chart
intrusive_ptr chart = worksheet->GetICharts()->GetObjectByIndex(chartIndex);
 
// Adding SeriesCollection (chart data source) to the chart ranging from "A1" cell to "B3"
chart->GetNISeries()->Add(new String("A1:B3"), true);
 
// Saving the Excel file
workbook->Save(outputChartTypeLine);
```

See the document on how to [create standard and custom charts][3] for your reference.

## Insert/Extract OLE Objects into/from the Worksheet

Aspose.Cells allow you to insert an OLE object inside the worksheet. Please use **Worksheet->GetIOleObjects()->Add()** method for this purpose. You will need image in bytes that will be used to display the OLE object inside the worksheet and Ole object data bytes that will be your actual object.  
See the document on how to insert OLE Objects into the Worksheets for your reference.  
Moreover, you can extract the OLE Object from the spreadsheet, see the document on how to [extract Ole Objects from Excel workbook][4] for your reference.

## Read and Manipulate MS Excel 2016 Charts

Aspose.Cells also supports reading and manipulating Microsoft Excel 2016 charts which are not present in Microsoft Excel 2013 or earlier versions. See the document on how to [read and manipulate MS Excel 2016 charts][5] for your reference.

## Aspose.Cells for C++ Resources

The resources, you may need to accomplish your tasks:

*   [Home of Aspose.Cells for C++ API][6].
*   [Aspose.Cells for C++ Downloads][7].
*   [Aspose.Cells for C++ Documentation][8] – up-to-date documentation containing Programmer's Guide, Knowledge Base and much more.
*   [Aspose.Cells Product Family Forum][9] – post your technical questions and queries, or any other problem you are facing while working with Aspose.Cells APIs.
*   [Enable Blog Subscription][10] – do not limit yourself, you can keep yourself updated with the latest news on Aspose.Cells APIs, new features, fixes and other API related topics by subscribing to Aspose.Cells blog.

Keeping the Aspose tradition, you are welcome to shape the upcoming releases of Aspose.Cells for C++ API by posting your suggestions and concerns in the Aspose.Cells support forum.




[1]: https://www.nuget.org/packages/Aspose.Cells.Cpp/18.4.0
[2]: https://docs.aspose.com/display/cellscpp/Aspose.Cells+for+CPP+18.4+Release+Notes
[3]: https://docs.aspose.com/display/cellscpp/Creating+and+Customizing+Charts
[4]: https://docs.aspose.com/display/cellscpp/Extracting+OLE+Objects+from+Worksheet
[5]: https://docs.aspose.com/display/cellscpp/Read+and+Manipulate+Excel+2016+Charts
[6]: https://products.aspose.com/cells/cpp
[7]: https://www.nuget.org/packages/Aspose.Cells.Cpp
[8]: https://docs.aspose.com/display/cellscpp/Home
[9]: https://forum.aspose.com/c/cells
[10]: https://blog.aspose.com/category/aspose-products/aspose-cells-product-family/





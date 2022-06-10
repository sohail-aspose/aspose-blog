---
title: 'Create and Manipulate Pivot Table, Apply Conditional Formatting, and Add Hyperlinks to Excel in C++'
date: Tue, 27 Dec 2016 04:52:10 +0000
draft: false
url: /2016/12/27/create-manipulate-pivot-table-apply-conditional-formatting-add-hyperlinks-and-much-more-with-aspose.cells-for-c-16.12.0/
author: Babar Raza
summary: ''
tags: ['Excel C++ Library', 'Hyperlinks', 'ListObjects', 'conditional formatting', 'document properties', 'pivot table', 'tables']
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/aspose_cells-for-cpp.png" alt="">}}


Aspose Team is pleased to announce the second major release of Aspose.Cells for C++ API. [Aspose.Cells for C++ 16.12.0][1] has included many new features and enhancements that further improve the overall feature set of the API. Please check the detailed release notes in order to get an idea about what is new and what has been enhanced with this revision of Aspose.Cells for C++. If you are planning to upgrade the API from any previous version, we strongly suggest you check the [Public API Changes][2] section to know what has been changed since your current revision of the API.

While you are downloading the API build to give it a try, here is a list of added features along with a few code snippets for quick testing.

## Create & Manipulate Excel Pivot Tables in C++

The second release of Aspose.Cells for C++ supports creation as well as the manipulation of the Pivot Tables. Aspose.Cells for C++ provides the IPivotTable class which represents a Pivot Table object whereas IPivotTableCollection represents a collection of Pivot Tables. The IPivotTableCollection can be accessed via the IWorksheet object and a new Pivot Table can be added to the collection while using the IPivotTableCollection.Add method.

The following code snippet demonstrates how simple is to use Aspose.Cells for C++ API to [create Pivot Tables from scratch][3].  
{{< gist aspose-com-gists 0edd1c91ebaa6cd099be1200b1ec7480 "Examples-CellsCPP-PivotTables-CreatePivotTable.cpp" >}}

Besides creating new Pivot Tables, Aspose.Cells for C++ APIs also support to manipulate existing Pivot Tables. The API currently supports to change the data at the source range of the Pivot Table and then refresh it. Once the Pivot Table has been manipulated as desired, it is best to use the IPivotTable.RefreshData and IPivotTable.CalculateData methods to refresh the Pivot Table against the updated data source.

The following code snippet uses the Aspose.Cells for C++ API to [manipulate an existing Pivot Table][4].  
{{< gist aspose-com-gists 0edd1c91ebaa6cd099be1200b1ec7480 "Examples-CellsCPP-PivotTables-ManipulatePivotTable.cpp" >}}

## Add Conditional Formatting Rules in Excel using C++

Aspose.Cells for C++ now provides the ability to add conditional formatting rules to the worksheet by exposing the IFormatCondition class. The aforementioned class further provides the following methods to [apply the conditional formatting as per application requirements][5].

*   IFormatCondition.GetIAboveAverage
*   IFormatCondition.GetIColorScale
*   IFormatCondition.GetIDataBar
*   IFormatCondition.GetIIconSet
*   IFormatCondition.GetITop10

The following sample code shows how to add a conditional formatting rule of type Cell Value on cells A1 and B2.  
{{< gist aspose-com-gists 0edd1c91ebaa6cd099be1200b1ec7480 "Examples-CellsCPP-Data-ApplyConditionalFormattingInWorksheet.cpp" >}}  

## Add Hyperlinks to Excel in C++

Aspose.Cells for C++ now supports [adding hyperlinks to the worksheet cells][6]. In order to provide this feature, the Aspose.Cells for C++ 16.12.0 has exposed the IHyperlinkCollection class which is accessible via the IWorksheet object whereas a hyperlink can be added to the collection while using the IHyperlinkCollection.Add method as demonstrated below.  
{{< gist aspose-com-gists 0edd1c91ebaa6cd099be1200b1ec7480 "Examples-CellsCPP-Data-AddHyperlinksToCells.cpp" >}}

## Manage Document Properties

Excel application supports 2 types of document properties as listed below.

*   System defined (built-in) properties: Built-in properties contain general information about the document like document title, author name, document statistics and so on.
*   User-defined (custom) properties: Custom properties defined by the end-user in the form of name-value pair.

Aspose.Cells for C++ supports [managing both types of document properties][7], built-in and custom. Aspose.Cells' IWorkbook class represents an Excel file. In order to access the built-in document properties, use IWorkbook.GetBuiltInDocumentProperties whereas the custom document properties can be accessed while using the IWorkbook.GetCustomDocumentProperties.

The following sample code loads an existing sample spreadsheet and reads the built-in document properties such as Title, Subject and custom property by the name MyCustom1.  
{{< gist aspose-com-gists 0edd1c91ebaa6cd099be1200b1ec7480 "Examples-CellsCPP-LoadingSavingAndConverting-ManagingDocumentProperties.cpp" >}}

## Manage Excel Tables

An Excel table is a matrix of cells containing any number of rows and columns whereas the same table is referred to be as a List Object in Aspose.Cells for C++ APIs. The Aspose::Cells::Tables namespace contains all the necessary classes that deal with the operations related to the List Objects. Most worth mentioning classes are IListObject and IListObjectCollection which allow to [create and format List Objects][8] and so on.

## Group Rows & Columns

Aspose.Cells for C++ API can be used to group rows & columns while using the ICells class which is basically the collection of all cells in a given worksheet. The ICells class offers the GroupRows and GroupColumns methods in order to [group rows and columns][9] respectively.

The following code snippet demonstrates the simple usage scenario of both aforementioned methods.  
{{< gist aspose-com-gists 0edd1c91ebaa6cd099be1200b1ec7480 "Examples-CellsCPP-TechnicalArticles-GroupRowsAndColumnsOfWorksheet.cpp" >}}

## Other Enhancements

There are several other enhancements with this release of Aspose.Cells for C++. Here is a list of just a few worth mentioning features.

*   Ability to [apply the custom theme colors][10].
*   Ability to [copy theme across workbooks][11].
*   Support for [manipulation of theme colors][12].

## Aspose.Cells for C++ Resources

The resources, you may need to accomplish your tasks:

*   [Home of Aspose.Cells for C++ API][13].
*   [Aspose.Cells for C++ Download Section][14].
*   [Aspose.Cells for C++ Documentation][15] – up-to-date documentation containing Programmer's Guide, Knowledge Base and much more.
*   [Aspose.Cells Product Family Forum][16] – post your technical questions and queries, or any other problem you are facing while working with Aspose.Cells APIs.
*   [Enable Blog Subscription][17] – do not limit yourself, you can keep yourself updated with the latest news on Aspose.Cells APIs, new features, fixes and other API related topics by subscribing to Aspose.Cells blog.

Keeping the Aspose tradition, you are welcome to shape the upcoming releases of Aspose.Cells for C++ API by posting your suggestions and concerns in the Aspose.Cells support forum.




[1]: http://downloads.aspose.com/cells/cpp/new-releases/aspose.cells-for-c---16.12.0/
[2]: https://docs.aspose.com/display/cellscpp/Aspose.Cells+for+CPP+16.12.0+Release+Notes
[3]: https://docs.aspose.com/display/cellscpp/Create+Pivot+Table
[4]: https://docs.aspose.com/display/cellscpp/Manipulate+Pivot+Table#ManipulatePivotTable-ManipulatePivotTable
[5]: https://docs.aspose.com/display/cellscpp/Apply+Conditional+Formatting+in+Worksheet
[6]: https://docs.aspose.com/display/cellscpp/Add+Hyperlinks+to+the+Cells
[7]: https://docs.aspose.com/display/cellscpp/Managing+Document+Properties
[8]: https://docs.aspose.com/display/cellscpp/Create+and+Format+Table
[9]: https://docs.aspose.com/display/cellscpp/Group+Rows+and+Columns+of+Worksheet
[10]: https://docs.aspose.com/display/cellscpp/Apply+Custom+Theme+Colors+of+the+Workbook+using+Array+of+Colors
[11]: https://docs.aspose.com/display/cellscpp/Copy+Theme+from+one+Workbook+to+another
[12]: https://docs.aspose.com/display/cellscpp/Apply+Custom+Theme+Colors+of+the+Workbook+using+Array+of+Colors
[13]: https://products.aspose.com/cells/cpp
[14]: http://downloads.aspose.com/cells/cpp
[15]: http://docs.aspose.com/display/cellscpp/Home
[16]: https://forum.aspose.com/
[17]: https://blog.aspose.com/category/aspose-products/aspose-cells-product-family/





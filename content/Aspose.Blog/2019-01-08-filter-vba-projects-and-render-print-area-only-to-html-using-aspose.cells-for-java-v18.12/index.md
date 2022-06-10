---
title: 'Filter VBA Projects and render print area only to HTML using Aspose.Cells for Java v18.12'
date: Tue, 08 Jan 2019 15:14:13 +0000
draft: false
url: /2019/01/08/filter-vba-projects-and-render-print-area-only-to-html-using-aspose.cells-for-java-v18.12/
author: Ahsaniqbal
summary: ''
tags: []
categories: ['Aspose.Cells Product Family']
---

[![][1]](https://blog.aspose.com/wp-content/uploads/sites/2/2013/07/aspose-Cells-for-Java_100.png)We are happy to share the joyful moments of announcing the new updated version [Aspose.Cells for Java v18.12][2]. As usual, lot of new features, enhancements and bug fixes are part of this release. We are moving ahead to achieve our goals in the industry by providing state of the art products by addressing each and every concern of our customers. This is all possible due to continuous support and feedback by the developers community.  We are in the process of day by day learning like many times bugs or issues lead us to enhancements and new features which increases our customer base.   
  
We always provide [Release notes][3] which provide a detailed information about the new features, enhancements and bug fixes in the new release. Every time we release new version, special resources and efforts are put with respect to improving the performance like users were facing issues in loading huge files using LightCells. This issue is addressed and performance is improved unto maximum extent. You may go through the release notes to have a glimpse of all the changes in this new version. For more details about this product you may visit the links in the last section of this document. For an easy access and utilization, Aspose for Java APIs can be directly installed from Maven repository for which check [document][4].  
   

## Export single sheet workbook to HTML

Workbook can have multiple sheets which are rendered as multiple tab pages when converted to HTML using Excel. Similarly if a workbook contains single sheet, it shows one tab page when converted to HTML using Excel. This conversion was working fine for multiple sheets while using Aspose.Cells. However for single sheet workbook, there was no tab page and only HTML file was created without creating the separate folder containing CSS. Now Aspose.Cells has enhanced its library to create similar output for single sheet workbooks as compared to output created by Excel.

For a working example refer to the following article:

*   Export single sheet workbook to HTML

## Load workbook efficiently without loading VBA project

In complex Excel files (XLSM/XSLB) there can be large amount of macros which can be very very long. Many times there is a need to load the workbooks without loading these VBA projects like just extracting the sheet names from loaded workbook. In this case we need a filter which can load VBA projects in when they are actually required. This time Aspose.Cells has introduced a filter option LoadDataFilterOptions.VBA which can be used for this purpose.

For a working example refer to the following article:

*   [Filter VBA Project while loading a workbook][5]

## Replacing tags in Textbox within a worksheet

Textbox is very common control which can be used in a worksheet. This is not necessary that text in the textbox is fixed. It may have tags which can be replaced with some text at runtime. It helps users to configure the controls as per the data on the sheet or from some other source. Worksheet.replace can be used for this purpose and textbox can be set with the desired text.  

For a working example refer to the following article:

*   [Replace tag with text in a textbox inside the worksheet][6]

## Export print area range to HTML

We can convert worksheet to HTML but rendering entire sheet at once may not be required always. You may require just a selected area of the sheet to be rendered to HTML. Worksheets contain page setup where print area can be set. There was a need that only  this print area shall be rendered to HTML if required. HtmlSaveOptions is extended by adding a new enumerator ExportPrintAreaOnly which enables users to render only print area in the HTML.  

For a working example refer to the following article:

*   [Replace tag with text in a textbox inside the worksheet][7]

## Identification of validation as dropdown

A worksheet can have different types of validations including dropdown. There can be a need where user may want to detect the type of validation and take some decision  based on this information. Validation object can be obtained from a cell and a new function is defined for this validation which returns if validation is a dropdown or not. Use this function as Validation.getInCellDropDown() which returns a boolean value i.e. true or false.  

For a working example refer to the following article:

*   [Check if validation in cell is dropdown][8]

## Other Enhancements and Fixes

There are some other enhancements included and a few exceptions handled in the new release for the users. A few of the worth mentioning features and other improvements are as follows.

*   Does not get connection points as its returned type is 'zo\[\]'
*   Data bars are missing when XLSX is converted to HTML
*   LightCells API fails to load a huge file
*   Validation always returns true for 'getInCellDropDown()' method
*   Wrong culture custom format gets returned for different locales (Germany, French, Italy and Spain)
*   Text formatting is missing in HTML output of MS Excel range
*   Excel To PDF conversion - Gauge chart rendering issue
*   PDF rendition throws OutOfMemoryError exception

In Aspose.Cells 18.12, we fixed several important bugs and other issues. For example, Excel To PDF conversion - Gauge chart rendering issue, NumberFormatException while processing files and Icon Sets become misaligned when XLSX is converted to HTML.

## Changes to the Public API

The following is a list of any changes made to the public API such as added, renamed, removed or deprecated members as well as any non-backward compatible change made to Aspose.Cells for Java:

*   Adds **HtmlSaveOptions.ExportSingleTab property,** indicates whether exporting the single tab when the file only has one worksheet in it. The default value is false.
*   Adds **HtmlSaveOptions.ExportPrintAreaOnly property, **indicates if only exporting the print area to html file. The default value is false.
    
*   Deletes **obsoleted Workbook.Initialize() method,** use Workbook constructor instead.
    
*   Deletes **obsoleted Workbook.Styles property, **use Workbook.CreateStyle() to create and manipulate style for workbook instead of StyleCollection.Add(); Use Workbook.GetNamedStyle(string) to get named style instead of StyleCollection.
    
*   Deletes **obsoleted Workbook.CheckWriteProtectedPassword() method, **use WorkbookSettings.WriteProtection.ValidatePassword method instead.
    
*   Deletes **obsoleted Workbook.CheckWriteProtectedPassword() method, **use WorkbookSettings.WriteProtection.ValidatePassword method instead.
    
*   Adds **LoadDataFilterOptions.VBA enum, **the option used to ignore VBA projects while loading template file.
    

*   Adds **Style.InvariantCustom property, **gets the culture-independent pattern string for number format (including the pattern string for built-in number).
    

*   Adds **FindOptions.ValueTypeSensitive property, **indicates whether searched cell value type should be same with the searched key.
    

*   Obsoletes **FindOptions.SearchNext property, **use FindOptions.SearchBackward property instead, true value for this new property corresponds to false of SearchNext.
    

*   Deletes **obsoleted Cells.ImportGridView(System.Web.UI.WebControls.GridView,int ,int , bool ,bool ,bool ) method, **use Cells.ImportGridView (System.Web.UI.WebControls.GridView gridView,int firstRow,int firstColumn,ImportTableOptions options) method. instead.
    

*   Deletes **obsoleted Cells.Start property, **use Cells.FirstCell property instead.
    

*   Deletes **obsoleted Cells.End property, **use Cells.LastCell property instead.
    

*   Deletes **Cells\[int\] property, **use Cells.GetEnumerator() method to iterate all cells in this worksheet instead.
    

*   Deletes **obsoleted Cells.ImportDataColumn() methods, **use Cells.ImportData (DataTable,int,int,ImportTableOptions) method instead.
    

*   Deletes **obsoleted Cells.ImportDataReader() methods, **use Cells.ImportData (IDataReader, int, int,ImportTableOptions) method instead.
    

*   Deletes **obsoleted Shape.Rotation property,** use Shape.RotationAngle property instead.
    

*   Deletes **obsoleted Validation.AreaList property, **use Validation.Areas property instead.
    

*   Deletes **obsoleted Style constructor, **use CellsFactory.CreateStyle() or Workbook.CreateStyle() method instead.
    

*   Deletes **obsoleted Shape.IsPrinted property, **use Shape.IsPrintable property instead.
    

*   Deletes **obsoleted PivotItem.Move(int) method, **using PivotItem.Move(int , bool ) method instead.
    

*   Deletes **obsoleted  Cells.ExportDataTable(int, int, int, int,bool, bool),Cells.ExportDataTable(int, int, int, int,object\[\]), Cells.ExportDataTable(int, int, int, int,bool), **  
    **Cells.ExportDataTable(DataTable, int, int\[\],int, bool) and Cells.ExportDataTable(DataTable,int, int, int, bool, bool) methods, **use ExportDataTable(firstRow,firstColumn, totalRows, totalColumns,ExportTableOptions) method instead.
    

*   Adds **ExtPage.setServlet(HttpServletRequest req,HttpServletResponse resp), **initializes servlet context for ExtPage.
    

*   Add **ExtPage.getBean() method, **gets GridWebBean instance from ExtPage.
    

*   Deletes **ExtPage.getBean(HttpServletRequest req) method, **use ExtPage.getBean() instead.
    

*   Adds **ExtPage.Maxholders property, **indicates maximum GridWeb instances for server to be kept (creating every new page or refreshing is considered as a new control instance), default value is 000.
    

*   Adds **ExtPage.Memoryinstanceexpires property, **indicates the expiry time in seconds of control instance on server, if the time expires, it will be removed on the server, default value is 3600, about one hour.
    

*   Adds **ExtPage.MemoryCleanRateTime property, **indicates every time duration in seconds to do the check work, to check whether control instance is expired, if expired it removes it, default value is 7200, about two hours.
    

  

## Aspose.Cells for Java Resources

The resources, you may need to accomplish your tasks:

*   [Home of Aspose.Cells for Java API][9].
*   [Download Aspose.Cells for Java][10].
*   [Aspose.Cells for Java Documentation][11] – up-to-date documentation containing Programmer’s Guide, Knowledge Base and much more.
*   [Aspose.Cells for Java API Reference Guide][12] – detailing the publicly exposed classes, methods, properties, constants & interfaces.
*   [Aspose.Cells Product Family Forum][13] – post your technical questions and queries, or any other problem you are facing while working with Aspose.Cells APIs.
*   [Aspose.Cells for Java Examples][14] – we have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: https://blog.aspose.com/wp-content/uploads/sites/2/2013/07/aspose-Cells-for-Java_100.png
[2]: https://artifact.aspose.com/repo/com/aspose/aspose-cells/18.12/
[3]: https://docs.aspose.com/display/cellsjava/Aspose.Cells+for+Java+18.12+Release+Notes
[4]: https://docs.aspose.com/display/cellsjava/Installation#Installation-InstallingAspose.CellsforJavafromMavenRepository
[5]: https://docs.aspose.com/display/cellsjava/Filter+VBA+Project+while+loading+a+workbook
[6]: https://docs.aspose.com/display/cellsjava/Replace+tag+with+text+in+a+textbox+inside+the+Worksheet
[7]: https://docs.aspose.com/display/cellsjava/Replace+tag+with+text+in+a+textbox+inside+the+Worksheet
[8]: https://docs.aspose.com/display/cellsjava/Data+Validation#DataValidation-Checkifvalidationincellisdropdown
[9]: https://products.aspose.com/cells/java
[10]: https://artifact.aspose.com/repo/com/aspose/aspose-cells/
[11]: https://docs.aspose.com/display/cellsjava/home
[12]: https://apireference.aspose.com/java/cells
[13]: https://forum.aspose.com/c/cells
[14]: https://github.com/aspose-cells/Aspose.Cells-for-Java





---
title: 'Customize Pivot Tables in Excel Files and Call Client-side Scripts for GridWeb in .NET'
date: Thu, 23 Mar 2017 13:06:42 +0000
draft: false
url: /2017/03/23/customize-pivot-tables-in-excel-files-and-call-client-side-scripts-for-gridweb-in-.net/
author: Amjad Sahi
summary: ''
tags: []
categories: ['Aspose.Cells Product Family']
---

[![Aspose.Cells for .NET logo][1]](http://www.aspose.com/.net/excel-component.aspx "Aspose.Cells for .NET API")We are pleased to announce our next version of [Aspose.Cells for .NET v17.3.0][2]. The new release includes some valuable features and other enhancements with critical bug fixes. It adds a new feature to enhance the API control over the Pivot Tables. Developers can retrieve and set globalization settings of a Pivot Table for their requirements. They can also call client-side scripts on the page change event of Aspose.Cells.GridWeb control. Ourclients may [get the powerful Aspose for .NET APIs directly from NuGet repository][3]. Please see the detailed [release notes][4] in order to get an idea about what is new and what has been fixed with this version of Aspose.Cells for .NET. The release notes also list any changes made to the public API such as added, renamed, removed or deprecated members (if any) as well as any non-backward compatible change made to Aspose.Cells for .NET.

## Customizing a Pivot Table by Using Globalization Settings

Using Aspose.Cells API, developers can apply various filters to build the corresponding Pivot Table. After they create a Pivot Table report and add the fields (they require), they often want to enhance the layout and formatting of the report to improve readability and to make it more attractive. To achieve this, Aspose.Cells API allows developers to customize the globalization settings of a Pivot Table to deal with such scenarios. They can customize the Pivot Total, Sub Total, Grand Total, All Items, Multiple Items, Column Labels, Row Labels, Blank Values text as per their requirements.  
  
Developers can derive a class from the base GlobalizationSettings class. GlobalizationSettings class has various methods to further enhance the Pivot Total, Sub Total, Grand Total, All Items, Multiple Items, Column Labels, Row Labels and Blank Values text. This article shows a code example which works with the layout and format of the report: [Customize Globalization Settings for Pivot Table][5]

## Call a Client Side Script on Page Change Event of GridWeb

Aspose.Cells for .NET also includes an independent web-based grid control (Aspose.Cells.GridWeb) which is designed to work with the web applications. Developers can load an existing Excel file into its grid matrix, manipulate it and save it back. The GridWeb control can hold data in multiple pages via its Paging feature. Developers might require to call a client side script on page index change event of GridWeb. This feature covers various scenarios. Developers may require to display the page number in their .NET applications, so they can call client side script to get the page number. To achieve this, EnablePaging property of the GridWeb should be set as True. This article shows a code example which uses the OnPageChangeClientFunction property of GridWeb control to display the page number: [Execute client side function on GridWeb page change][6] 

## Validate the Entire Worksheet of GridWeb

In the past, GridWeb control was validating the updated cells and not validating the entire Excel worksheet. Using the recent version 17.3.0 of Aspose.Cells API, developers can now validate the entire worksheet on client side before the GridWeb requests to the server. They need to set the needValidateall variable inside the acwmain.js to true. This article explains on how to validate the entire Excel worksheet of GridWeb: [Validate entire worksheet instead of only the updated cells][7]

## Other Enhancements and Fixes

Aspose.Cells for .NET 17.3.0 has enhanced its core for more stability as well as fixed many critical bugs. Moreover, there are numerous minor enhancements in order to improve the overall usage of the API. A few of the worth mentioning enhancements are as follow.

*   An enhancement is made when changing pivot data source that was adding additional LinkSource
*   Handled an exception, "Index out of Array exception".

Furthermore, in this release, we have fixed several other issues. For example, issues around reading/writing MS Excel file formats, manipulating Pivot Tables, rendering shapes and drawing objects, rendering and manipulating charts, rendering HTML to Excel and vice versa, rendering images from Excel worksheets, rendering images files from charts and exporting Excel workbooks to PDF format have been resolved. The formula calculation engine is further enhanced in the new release.

## Changes to the Public API

This version of Aspose.Cells for .NET has made some changes to the Public API. A few of the worth mentioning changes are as follow:

*   GlobalizationSettings.GetPivotTotalName() method is added to the GlobalizationSettings class.
*   GlobalizationSettings.GetPivotGrandTotalName() method is added to the GlobalizationSettings class.
*   GlobalizationSettings.GetMultipleItemsName() method is added to the GlobalizationSettings class.
*   GlobalizationSettings.GetAllName() method is added to the GlobalizationSettings class.
*   GlobalizationSettings.GetColumnLablesName() method is added to the GlobalizationSettings class.
*   GlobalizationSettings.GetRowLablesName() method is added to the GlobalizationSettings class.
*   GlobalizationSettings.GetEmptyDataName() method is added to the GlobalizationSettings class.
*   GlobalizationSettings.GetSubTotalName(PivotFieldSubtotalType subTotalType) method is added to the GlobalizationSettings class.
*   OnPageChangeClientFunction property is added to the GridWeb Control.

  

## Aspose.Cells for .NET Resources

The resources, you may need to accomplish your tasks:

*   [Home of Aspose.Cells for .NET API][8].
*   [Aspose.Cells for .NET Download Section][9].
*   Aspose.Cells for .NET Documentation – up-to-date documentation containing Programmer's Guide, Knowledge Base and much more.
*   [Aspose.Cells for .NET API Reference Guide][10] – detailing the publicly exposed classes, methods, properties, constants & interfaces.
*   [Aspose.Cells Product Family Forum][11] – post your technical questions and queries, or any other problem you are facing while working with Aspose.Cells APIs.
*   [Aspose.Cells for .NET Examples][12] – we have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: https://blog.aspose.com/wp-content/uploads/sites/2/2013/08/aspose-Cells-for-net_100.png "Aspose.Cells for .NET logo"
[2]: http://www.aspose.com/downloads/cells/net/new-releases/aspose.cells-for-.net-17.3.0/
[3]: https://www.nuget.org/packages/Aspose.Cells/
[4]: https://docs.aspose.com/display/cellsnet/Aspose.Cells+for+.NET+17.3.0+Release+Notes
[5]: https://docs.aspose.com/display/cellsnet/Customize+Globalization+Settings+for+Pivot+Table
[6]: https://docs.aspose.com/display/cellsnet/Execute+client+side+function+on+GridWeb+page+change
[7]: https://docs.aspose.com/display/cellsnet/Validate+entire+worksheet+instead+of+only+the+updated+cells
[8]: https://www.aspose.com/products/cells/net
[9]: http://www.aspose.com/downloads/cells/net
[10]: http://www.aspose.com/api/net/cells
[11]: https://forum.aspose.com/
[12]: https://github.com/aspose-cells/Aspose.Cells-for-.NET





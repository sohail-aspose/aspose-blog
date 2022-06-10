---
title: 'Track conversion progress in image rendering with Aspose.Cells for .NET 19.10'
date: Thu, 21 Nov 2019 10:24:26 +0000
draft: false
url: /2019/11/21/track-conversion-progress-in-image-rendering-with-aspose.cells-for-.net-19.10/
author: Amjad Sahi
summary: ''
tags: []
categories: ['Aspose.Cells Product Family']
---

[![Aspose.Cells for .NET logo][1]](https://www.aspose.com/products/cells/net "Aspose.Cells for .NET API") Conversion of Excel spreadsheets to image formats always remains a hot topic. Sometimes, you claim the process takes too long. Others complain that the process gets stuck for larger files and they need to stop the process. Aspose.Cells has now included a useful feature where you can track the conversion progress in Sheet to image rendering in the way you want, you may notice which pages are being rendered in the process at the moment. Moreover, you can also convert your desired pages and skip other pages. There are some other useful features which might attract you. We suggest you to have a look at the release notes to get the complete list of features, enhancements and other fixes which are part of this new release. I would recommend you to review the [release notes][2] for your reference.  To get details of the public release ([Aspose.Cells for .NET v19.10][3], I am highlighting some new features and other enhancements available in it.

## Track conversion progress of Excel files

Suppose you are working with large Excel files and converting them to other formats. Sometimes it might take a lot of time for conversion and you want your user to be aware of the progress. No worries!!! This latest release has provided the demanded feature to check the conversion progress of MS Excel files. Aspose.Cells has supported to track documents' conversion progress by providing the **IPageSavingCallback** interface. The **IPageSavingCallback** interface provides **PageStartSaving** and **PageEndSaving** methods that you can implement in your custom class. You may specify your desired pages to be rendered as demonstrated in the T_estPageSavingCallback_ custom class. See the following sample code that reads the source excel file and shows its conversion progress in the console by using the _TestPageSavingCallback_ custom class that implements the **IPageSavingCallback** interface.

{{< gist aspose-com-gists 922f990b02cf4e04a328bd6f37029af8 "Examples-CSharp-LoadingSavingConvertingAndManaging-DocumentConversionProgressForTiff-1.cs" >}}

The following is the code for the _TestTiffPageSavingCallback_ custom class.

{{< gist aspose-com-gists 922f990b02cf4e04a328bd6f37029af8 "Examples-CSharp-LoadingSavingConvertingAndManaging-DocumentConversionProgressForTiff-2.cs" >}}

**Console output:**



{{< figure align=center src="images/Capture-1024x288.png" alt="">}}


The following article demonstrates the feature with sample code for your reference.

[Track Conversion Progress of Excel to TIFF][4]

## Set custom DataSource for WorkbookDesigner in Smart Markers

We all know how useful is the Smart Markers feature when it comes to data binding or merging. Aspose.Cells allows you to set your custom data source for WorkbookDesigner class. The API provides an overloaded method [WorkbookDesigner.SetDataSource][5] which takes the name of the source as the first parameter and the instance of the class that implements [ICellsDataTable][6] as the second parameter. In the following document, you will learn this useful feature with example code and sample files for your complete reference.

[Set custom DataSource for WorkbookDesigner][7]

## Support custom data sorting for the specific area in PivotTable report

You have a pivot table and you want to sort it on field values. This is easily achievable now as you can use **PivotField.AutoSortField** attribute by providing item index to sort. Using this feature you will get a variety of data representation for analysis and reporting purpose. In the following article, you will see the result of this function along with a detailed sample code and files for testing.

[Custom sorting in Pivot Table][8]



{{< figure align=center src="images/Screenshot-2019-11-20-at-6.16.33-PM-1-1024x574.png" alt="">}}


In the above article, the sample code snippet loads the sample Excel file and adds three pivot tables. The first pivot table is without custom sorting, the second pivot table is sorted on "SeaFood" row field values and the third pivot table is sorted on "28/07/2000" column field values.

## Working with Content Type Properties

MS Excel file has some default attributes, like size, tag, title etc. and if you need to add more custom properties for your needs, Aspose.Cells has included this useful option by providing **Workbook.ContentTypeProperties.Add** function. You can also mark a property as optional by setting the **ContentTypeProperty.IsNillable** to **true**. Following are the sample code and image showing the newly added properties.

{{< gist aspose-com-gists 922f990b02cf4e04a328bd6f37029af8 "Examples-CSharp-Workbook-WorkingWithContentTypeProperties-1.cs" >}}



{{< figure align=center src="images/Capture-1.png" alt="">}}


The following document demonstrates the feature with sample code for your reference.

[Working with ContentTypeProperties][9]

## Other enhancements and fixes

*   *   Raise Exception similar to Excel instead of hanging program.
    *   Extend Range.RemoveDuplicates.
    *   Range.Copy performance for large volume.
    *   Support for TEXTJOIN() function.
    *   OLE objects become pictures when copying worksheets.
    *   Fixed an error where Saving as HTML was throwing an exception when the cell has a file reference.
    *   Handled an exception when calling Workbook.RemoveUnusedStyles().

To use these features and avail other enhancements and fixes, I recommend you to try the release [Aspose.Cells for .NET v19.10][10]. Moreover, I would recommend you to see [Developers’ Guide][11] for complete details on what you can implement using Aspose.Cells APIs. Also, you are always welcome to share your review, concerns or feedback on [forums][12].




[1]: http://blog.aspose.com/wp-content/uploads/sites/2/2013/08/aspose-Cells-for-net_100.png "Aspose.Cells for .NET logo"
[2]: https://docs.aspose.com/display/cellsnet/Aspose.Cells+for+.NET+19.10+Release+Notes
[3]: https://www.nuget.org/packages/Aspose.Cells/19.10.0)
[4]: https://docs.aspose.com/display/cellsnet/Track+Conversion+Progress+of+Excel+to+TIFF
[5]: https://apireference.aspose.com/net/cells/aspose.cells.workbookdesigner/setdatasource/methods/5
[6]: https://apireference.aspose.com/net/cells/aspose.cells/icellsdatatable
[7]: https://docs.aspose.com/display/cellsnet/Set+custom+DataSource+for+WorkbookDesigner
[8]: https://docs.aspose.com/display/cellsnet/Custom+sorting+in+Pivot+Table
[9]: https://docs.aspose.com/display/cellsnet/Working+with+ContentTypeProperties
[10]: https://downloads.aspose.com/cells/net/new-releases/aspose.cells-for-.net-19.10/
[11]: https://docs.aspose.com/display/cellsnet/Developer+Guide
[12]: https://forum.aspose.com/c/cells





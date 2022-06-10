---
title: 'Tile Picture as a Texture Inside Shapes in Excel Worksheets in Android'
date: Tue, 10 Oct 2017 12:25:49 +0000
draft: false
url: /2017/10/10/tile-picture-as-a-texture-inside-excel-shapes-in-android-using-java-excel-api/
author: Amjad Sahi
summary: ''
tags: []
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/aspose-Cells-for-Android_100.png" alt="Aspose.Cells for Android logo">}}


We are pleased to announce the release of [Aspose.Cells for Android via Java 17.9][1]. This release includes a number of new features, enhancements and several bug fixes that further improve the overall stability and usability of the API. Please check the [release notes][2] in order to get an idea about what is new and what has been fixed with this revision of Aspose.Cells for Android via Java. While you are downloading the latest build, here is a look at the most worth mentioning features in this release.

## Tile Picture as a Texture Inside the Excel Shape using Java

Aspose.Cells supports image tiling feature which allows you to display images that are too large to be displayed entirely as a single unit on a typical computer. The feature allows you to display by segmenting it into smaller, more manageable image tiles.

{{< gist aspose-com-gists a20e8fa273e7cfa37d032b8211fcf8bf "Examples-src-AsposeCellsExamples-DrawingObjects-TilePictureAsTextureInsideShape.java" >}}

Please see this article that explains how to Tile Picture as a Texture inside the Shape.

*   [Tile Picture as a Texture inside the Shape][3]

## Using Formula Parameter in Smart Marker Field

Sometimes, you need to embed formula in [Smart Markers][4]. Aspose.Cells allows you to make use of the Formula parameter in Smart marker field. For more detail, please see this article.

{{< gist aspose-com-gists a20e8fa273e7cfa37d032b8211fcf8bf "Examples-src-AsposeCellsExamples-SmartMarkers-UsingFormulaParameterInSmartMarkerField.java" >}}

*   [Using Formula parameter in Smart Marker field][5]

## Apply Advanced Filter of Microsoft Excel to Display Records Meeting Complex Criteria

Microsoft Excel allows you to apply **Advanced Filter** on worksheet data to display records that meet complex criteria. You can apply Advanced Filter with Microsoft Excel via its **Data > Advanced** command as shown in this screenshot.



{{< figure align=center src="images/Microsoft-Excel-Advanced-Filtering-Interface-300x263.png" alt="">}}


Aspose.Cells also allows you to apply the Advanced Filter using the **Worksheet.advancedFilter()** method. For more detail, please see this article.

*   [Apply Advanced Filter of Microsoft Excel to Display Records Meeting Complex Criteria][6]

## Import Data from Microsoft Access Database ResultSet Object to the Worksheet

Aspose.Cells can import data to worksheet from **ResultSet** object which can be created from any database. However, the following article specifically creates ResultSet object from **Microsoft Access Database**. Since, the code is same for all types of databases, so you can use it in general.

*   [Import Data from Microsoft Access Database ResultSet Object to the Worksheet][7]

## Implement Errors and Boolean Value in Russian or Any Other Language

If you are using Microsoft Excel in Russian Locale or Language or any other Locale or Language, it will display Errors and Boolean values according to that Locale or Language. You can achieve the similar behavior of Microsoft Excel using Aspose.Cells with the **GlobalizationSettings** class. Please see the following article for more help.

*   [Implement Errors and Boolean Value in Russian or Any Other Language][8]

## Read Numbers Spreadsheet Developed by Apple Inc. using Aspose.Cells

Numbers is a spreadsheet application developed by Apple Inc. Aspose.Cells can read Numbers spreadsheet but it does not support writing to it. It can read Numbers spreadsheet's Data, Style and Formulas. Here is the article link for more detail.

*   [Read Numbers Spreadsheet Developed by Apple Inc. using Aspose.Cells][9]

## Set DefaultFont property of PdfSaveOptions and ImageOrPrintOptions

When saving to PDF or image, Aspose.Cells will first try to use Workbook’s default font. This behavior can be changed using **DefaultFont** attribute in PdfSaveOptions/ImageOrPrintOptions. For more detail, please see this article.

*   [Set DefaultFont property of PdfSaveOptions and ImageOrPrintOptions to have priority][10]

## Determine if Paper Size of Worksheet is Automatic

Most of the time, paper size of the worksheet is automatic. When it is automatic, it is often set as Letter. Sometime user sets the paper size of the worksheet as per their requirements. In this case, the paper size is not automatic. You can find if the worksheet paper size is automatic or not using the **Worksheet.getPageSetup().isAutomaticPaperSize()** method.

*   [Determine if Paper Size of Worksheet is Automatic  
    ](https://docs.aspose.com/display/cellsjava/Determine+if+Paper+Size+of+Worksheet+is+Automatic)

## Output Blank Page when there is Nothing to Print

If the sheet is empty, then Aspose.Cells will not print anything when you export the worksheet to image. You can change this behavior by using the `ImageOrPrintOptions.OutputBlankPageWhenNothingToPrint` property. When you will set it true, it will print the blank page.

*   [Output Blank Page when there is Nothing to Print][11]

{{< gist aspose-com-gists a20e8fa273e7cfa37d032b8211fcf8bf "Examples-src-AsposeCellsExamples-Rendering-OutputBlankPageWhenThereIsNothingToPrint.java" >}}

## Export Comments while Saving Excel file to Html

When you save your Excel file into HTML, comments are not exported. However, Aspose.Cells provides this feature using the `HtmlSaveOptions.IsExportComments` property. If you set it true, then HTML will also display comments present in your Excel file.

*   Export Comments while Saving Excel file to Html

## Disable Downlevel Revealed Comments while saving to HTML

When you save your Excel file to HTML, then Aspose.Cells reveal Downlevel Conditional Comments. These conditional comments are mostly relevant to old versions of Internet Explorer and are irrelevant to modern Web Browsers. You can read about them in detail at [this link][12]. Aspose.Cells allows you to eliminate these Downlevel Revealed Comments by setting the `HtmlSaveOptions.DisableDownlevelRevealedComments` property to true.

*   Disable Downlevel Revealed Comments while saving to HTML

The screenshot shows the effect of this property on output Html when it is not set true.



{{< figure align=center src="images/Disable-Downlevel-Revealed-Comments-300x221.png" alt="Disable Downlevel Revealed Comments">}}


## Add Digital Signature to an already signed Excel file

Aspose.Cells provides the `Workbook.addDigitalSignature(DigitalSignatureCollection digitalSignatureCollection)` method that you can use to add digital signature to an already signed Excel file.

Please note while adding digital signature to an already signed Excel document, if the original document is Aspose.Cells generated document, it works well. But if the original document is generated by other engines (e.g. Microsoft Excel etc.), Aspose.Cells cannot keep the file same after loading and re-saving it, this will make the original signature to be invalid.

*   [Add Digital Signature to an already signed Excel file][13]

## Copy VBA Project having User Form from Template to Target Workbook

Aspose.Cells allows you to copy VBA project from one Excel file into another Excel file. VBA project consists of various types of modules i.e. Document, Procedural, Designer etc. All modules can be copied with simple code but for Designer module, there is some extra data called Designer Storage needs to be accessed or copied. The following two methods deal with Designer Storage.

*   **VbaModuleCollection.getDesignerStorage()**
*   **VbaModuleCollection.addDesignerStorage()**

Please see the following article for more detail and sample code.

*   [Copy VBA Macro UserForm DesignerStorage from Template to Target Workbook  
    ](https://docs.aspose.com/display/cellsjava/Copy+VBA+Macro+UserForm+DesignerStorage+from+Template+to+Target+Workbook)

## Send Shape Front or Back inside the Worksheet

When there are multiple shapes present in the same location then how will they be visible is decided by their z-order positions. Aspose.Cells provides **Shape.toFrontOrBack()** method which changes the z-order position of the shape. If you want to send shape to back you will use negative number like -1, -2, -3 etc. and if you want to send shape to front, you will use positive number like 1, 2, 3 etc.

*   [Send Shape Front or Back inside the Worksheet][14]

This screenshot shows the effect of the code in the above article on the source workbook. As you can see, the z-order positions of shapes have been changed as per sample code.



{{< figure align=center src="images/Send-Shape-Front-or-Back-inside-the-Worksheet-300x221.png" alt="">}}


## Sort Data in Column with Custom Sort List

You can sort data in the column using custom list. This can be done using **DataSorter.addKey(int key, SortOrder order, String customList)** method. However, this method works only if the items in custom list do not have commas inside them. If they have commas like **"USA,US", "China,CN"** etc., then you must use **DataSorter.addKey(int key, SortOrder order, String\[\] customList)** method. Here, the last parameter is not String but Array of Strings.

*   [Sort Data in Column with Custom Sort List][15]

{{< gist aspose-com-gists a20e8fa273e7cfa37d032b8211fcf8bf "Examples-src-AsposeCellsExamples-Data-SortDataInColumnWithCustomSortList.java" >}}

## Add PDF Bookmarks with Named Destinations

Named Destinations are special kinds of bookmarks or links in PDF that do not depend on PDF pages. It means, if pages are added or deleted from PDF, bookmarks may become invalid but named destinations will remain intact. To create Named Destination, please use the **PdfBookmarkEntry.setDestinationName()** method.

*   [Add PDF Bookmarks with Named Destinations][16]

## Control loading of External Resources in MS Excel Workbook while rendering to PDF

Your Excel file may contain external resources e.g. linked images or objects. When you convert your Excel file to Pdf, Aspose.Cells retrieves these external resources and renders them to Pdf. But sometimes, you do not want to load these external resources and more than that, you want to manipulate them. You can do this using **PdfSaveOptions.StreamProvider** which implements the **IStreamProvider** interface.

*   [Control loading of External Resources in MS Excel Workbook while rendering to PDF][17]

## Aspose.Cells for Android via Java Resources

The resources, you may need to accomplish your tasks:

*   [Home of Aspose.Cells for Android via Java API][18].
*   [Aspose.Cells for Android via Java Download Section][19].
*   [Aspose.Cells for Android via Java Documentation][20] – up-to-date documentation containing Programmer's Guide, Knowledge Base, and much more.
*   [Aspose.Cells for Android via Java API Reference Guide][21] – detailing the publicly exposed classes, methods, properties, constants & interfaces.
*   [Aspose.Cells Product Family Forum][22] – post your technical questions and queries, or any other problem you are facing while working with Aspose.Cells APIs.
*   [Enable Blog Subscription][23] – do not limit yourself, you can keep yourself updated with the latest news on Aspose.Cells APIs, new features, fixes, and other API related topics by subscribing to Aspose.Cells blog.
*   [Aspose.Cells for Android via Java Examples][24] – we have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: https://downloads.aspose.com/cells/androidjava/new-releases/aspose.cells-for-android-via-java-17.9/
[2]: https://docs.aspose.com/display/cellsjava/Aspose.Cells+for+Android+via+Java+17.9+Release+Notes
[3]: https://docs.aspose.com/display/cellsjava/Tile+Picture+as+a+Texture+inside+the+Shape
[4]: https://docs.aspose.com/display/cellsjava/Using+Smart+Markers
[5]: https://docs.aspose.com/display/cellsjava/Using+Formula+parameter+in+Smart+Marker+field
[6]: https://docs.aspose.com/display/cellsjava/Apply+Advanced+Filter+of+Microsoft+Excel+to+Display+Records+Meeting+Complex+Criteria
[7]: https://docs.aspose.com/display/cellsjava/Import+Data+from+Microsoft+Access+Database+ResultSet+Object+to+the+Worksheet
[8]: https://docs.aspose.com/display/cellsjava/Implement+Errors+and+Boolean+Value+in+Russian+or+Any+Other+Language
[9]: https://docs.aspose.com/display/cellsjava/Read+Numbers+Spreadsheet+Developed+by+Apple+Inc.+using+Aspose.Cells
[10]: https://docs.aspose.com/display/cellsjava/Set+DefaultFont+property+of+PdfSaveOptions+and+ImageOrPrintOptions+to+have+priority
[11]: https://docs.aspose.com/display/cellsjava/Output+Blank+Page+when+there+is+Nothing+to+Print
[12]: https://en.wikipedia.org/wiki/Conditional_comment#Downlevel-revealed_conditional_comment
[13]: https://docs.aspose.com/display/cellsjava/Add+Digital+Signature+to+an+already+signed+Excel+file
[14]: https://docs.aspose.com/display/cellsjava/Send+Shape+Front+or+Back+inside+the+Worksheet
[15]: https://docs.aspose.com/display/cellsjava/Sort+Data+in+Column+with+Custom+Sort+List
[16]: https://docs.aspose.com/display/cellsjava/Add+PDF+Bookmarks+with+Named+Destinations
[17]: https://docs.aspose.com/display/cellsjava/Control+loading+of+External+Resources+in+MS+Excel+Workbook+while+rendering+to+PDF
[18]: https://www.aspose.com/products/cells/android-java
[19]: https://downloads.aspose.com/cells/androidjava
[20]: https://docs.aspose.com/display/cellsandroidjava/Aspose.Cells+for+Android+via+Java+Home
[21]: https://apireference.aspose.com/java/cells
[22]: https://forum.aspose.com/c/cells
[23]: https://blog.aspose.com/category/aspose-products/aspose-cells-product-family/
[24]: https://github.com/asposecells/Aspose_Cells_Java





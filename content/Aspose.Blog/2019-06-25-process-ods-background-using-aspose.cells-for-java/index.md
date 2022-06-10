---
title: 'Process ODS Background using Aspose.Cells for Java'
date: Tue, 25 Jun 2019 01:08:40 +0000
draft: false
url: /2019/06/25/process-ods-background-using-aspose.cells-for-java/
author: Ahsaniqbal
summary: ''
tags: []
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/aspose_cells-for-java-e1558954178996.jpg" alt="ODS Background with Java">}}


We are happy that once again we got the chance to present an updated and enhanced version of Aspose.Cells for Java v19.5. This time we have added new features for processing the ODS file background to create more user-friendly output files having color and image in the background. We have also enhanced our rendering features to HTML, PDF, and improvements in many functions of common use. Well, I think rather than writing a lot about these features one by one, better to have a brief overview of the new version from the [release notes][1] and then start exploring this release. What do you say?

## Read Background Information from ODS file

This time we have enhanced the capability of Aspose.Cells to process ODS files. One of the features which were requested by users was to read the background information from the ODS files. A new class [ODSPageBackground][2] is introduced which manages the background of an ODS file. Moreover, there are two options as the background of an ODS file, one is graphics, and the other is color. For this purpose, ODSPageBackgroundType enumerator is introduced which contains three values NONE, COLOR, and GRAPHIC.

For depicting the position of the background content, there are nine possible locations on the page. These are defined by introducing an enumerator named [ODSPageBackgroundGraphicPositionType.][3] Now you can not only identify the type and position but also can save the graphic to a file if required. All these features can be exercised using a ready to run code along with a sample file in the following article:

[Read Background Information from OSD file][4]

Following is the image showing the input and output using these features:



{{< figure align=center src="images/RetrieveImage.png" alt="Background Infor from OSD">}}


## Set background-color

As mentioned earlier that we have two options to set the background of an ODS file. Here I will describe the colored background for which you have to use [ODSPageBackground.Color][5] property. Coding this feature is quite simple such that first get the ODSPageBackground object from the template file and then set color and type and that's all. Have a look at the following article which provides a complete working sample code to demonstrate this feature.

[Add colored background to ODS file][6]

Following is the image of output file created by above sample code:



{{< figure align=center src="images/ODSView-1024x222.png" alt="">}}
</li></ul></figure>

Note that there is no need to set the range of text as this feature will automatically set background for the entire data in the above example.  

## Set Background Graphics

Setting a graphical background is quite common while working with worksheets. This area is also covered by this new feature where property [ODSPageBackground.GraphicData][7] is available to serve this purpose. Visit the following article which demonstrates this feature. You can see that usage is quite simple where you need to set the background type, byte array containing image data, and ODSPageBackgroundGraphicType. You may visit the following article to get a working code sample for this feature:

[Add Graphic Background to ODS file][8]

The following will be the output of this sample code in the print preview using OpenOffice Calc.



{{< figure align=center src="images/GraphicsBackground-2-1024x246.png" alt="Graphic Background in ODS">}}


## Import Custom Objects to a Merged Area

The feature of importing custom objects to Excel file is already available in Aspose.Cells, however, if the destination file contains a merged area where data is to be imported, there can be issues. This feature is available now where you can import data to a merged area in the output file. You may set [ImportTableOptions.CheckMergedCells][9] to true and Pass the [ImportTableOptions][10] object along with the list of columns/properties to the method to display your desired list of objects. Visit the following article for a detailed example:

[Importing from Custom Objects to merged area][11]

Following image provides an overview of this feature:



{{< figure align=center src="images/CustomToMerge.png" alt="Custom Objects in Excel">}}


## Other Upgrades

*   This time we have paid special attention to enhancements for related to the rendering of Excel files to PDF. Like displaying wrong values for shapes, turning over text like phone numbers, etc. and changing the text order, these all issues are resolved for rendering to PDF.
*   Similarly, Excel to HTML related issues were also addressed where sometimes transparency of charts was lost, charts were missed and rendering issues in CentOS were faced. All these issues are addressed in this latest release.
*   Data was not extracted from some MS Excel 95 files. Enhancements are done to sort out such issues in the product.
*   Some functions like DATEVALUE, VLOOKUP, and TEXT were having some minor issues which are also addressed and now these are enhanced to work more efficiently and error-free.
*   Exceptions are also handled like IllegalStateException and java.lang.ArrayIndexOutOfBoundsException while loading MS Excel 5.0/95 XLS files, both the exceptions are removed and now these files can be loaded without any issue.

Now, this is the time to go through and start using the innovative features and examples using this latest release Aspose.Cells for Java 19.5. Well organized complete examples along with the template files can be exercised by browsing Developers’ Guide and downloading a working project from Github [here][12]. Our [forums][13] are always open for you to share your thoughts and ask any query or issue related to our complete range of products.




[1]: https://docs.aspose.com/display/cellsjava/Aspose.Cells+for+Java+19.5+Release+Notes
[2]: https://apireference.aspose.com/java/cells/com.aspose.cells/ODSPageBackground
[3]: https://apireference.aspose.com/java/cells/com.aspose.cells/ODSPageBackgroundGraphicPositionType
[4]: https://docs.aspose.com/display/cellsjava/Working+with+Background+in+ODS+Files#WorkingwithBackgroundinODSFiles-ReadBackgroundInformationfromOSDfile
[5]: https://apireference.aspose.com/java/cells/com.aspose.cells/odspagebackground#Color
[6]: https://docs.aspose.com/display/cellsjava/Working+with+Background+in+ODS+Files#WorkingwithBackgroundinODSFiles-AddColoredBackgroundtoODSfile
[7]: https://apireference.aspose.com/java/cells/com.aspose.cells/odspagebackground#GraphicData
[8]: https://docs.aspose.com/display/cellsjava/Working+with+Background+in+ODS+Files#WorkingwithBackgroundinODSFiles-AddGraphicBackgroundtoODSfile
[9]: https://apireference.aspose.com/java/cells/com.aspose.cells/importtableoptions#CheckMergedCells
[10]: https://apireference.aspose.com/java/cells/com.aspose.cells/ImportTableOptions
[11]: https://docs.aspose.com/display/cellsjava/Import+and+Export+Data#ImportandExportData-ImportingfromCustomObjectstomergedarea
[12]: https://github.com/aspose-cells/Aspose.Cells-for-Java
[13]: https://forum.aspose.com/c/cells





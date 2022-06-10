---
title: 'Set ODS Background and Convert Dates to Japanese Dates in Excel using C#'
date: Thu, 27 Jun 2019 10:57:29 +0000
draft: false
url: /2019/06/27/set-ods-background-and-convert-dates-to-japanese-dates-using-aspose-cells-for-net-19-5/
author: Amjad Sahi
summary: ''
tags: []
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/aspose-Cells-for-net_100.png" alt="Aspose.Cells for .NET logo">}}


Hi Guys, in the blog you will learn how to use and implement some valuable features via Aspose.Cells. This time we have added new features regarding ODS file format. For example, you will learn on how to process the ODS file background to create furnished output files having color and image in the background. Moreover, Aspose.Cells provides a way to convert Gregorian dates to Japanese dates. You may find these exciting features and other enhancements in the release. So let's not wait another moment to review the [release notes][1].  To get essence of the public release ([Aspose.Cells for .NET v19.5][2], I am giving you preview of the new features and other enhancements available in it.

## Convert Dates to Japanese Dates in Excel

Aspose.Cells can convert Gregorian dates to Japanese dates. During this conversion, the changes in the era are also considered. This feature is demanded by some users for their scenarios. Visit the following article for detail with example:

[Converting dates to Japanese dates][3]

The following image provides an overview of this feature:



{{< figure align=center src="images/JapaneseDateConversion1.jpg" alt="">}}


## Read Background Information from OSD file

This time we have enhanced the capability of Aspose.Cells to process ODS files. One of the features which were requested by users was to read the background information from the ODS files. A new class **ODSPageBackground** is introduced which manages the background of an ODS file. Moreover, there are two options as the background of an ODS file, one is graphics and other is color. For this purpose, **ODSPageBackgroundType** enumerator is introduced which contains three values None, Color and Graphic.

For depicting the position of the background content, there are nine possible locations on the page. [](https://apireference.aspose.com/java/cells/com.aspose.cells/ODSPageBackgroundGraphicPositionType)Now you can not only identify the type and position but also can save the graphic to a file if required. All these features can be exercised using a ready to run code along with a sample file in the following article:

[Read Background Information from OSD file][4]

Following is the image showing the input and output using these features:



{{< figure align=center src="images/RetrieveImage.png" alt="">}}


## Set Background Color in ODS

As mentioned above that we have two options to set the background of an ODS file. Here I will describe the colored background for which you have to use **ODSPageBackground.Color** property. Coding this feature is quite simple such that first get the ODSPageBackground object from the template file and then set color and type and that's all. Have a look at the following article which provides a complete working sample code to demonstrate this feature.

[Add colored background to ODS file][5]

Following is the image of output file created by above sample code:



{{< figure align=center src="images/ODSView-1024x222.png" alt="">}}
</li></ul></figure>

Note that there is no need to set the range of text as this feature will automatically set background for the entire data in the above example.  

## Set Background Graphics in ODS

Setting a graphical background is quite common while working with worksheets. This area is also covered by this new feature where property **ODSPageBackground.GraphicData** is available to serve this purpose. Visit the following article which demonstrates this feature. You can see that usage is quite simple where you need to set the background type, byte array containing image data and **ODSPageBackgroundGraphicType**. You may visit the following article to get a working code sample for this feature:

[Add Graphic Background to ODS file][6]

The following will be the output of this sample code in the print preview using OpenOffice Calc.



{{< figure align=center src="images/GraphicsBackground-2-1024x246.png" alt="">}}


## Import Custom Objects to Merged Area

The feature of importing custom objects to an Excel file is already available in Aspose.Cells, however, if the destination file contains a merged area where data is to be imported, there can be issues. This feature is available now where you can import data to a merged area in the output file. You may set **ImportTableOptions.CheckMergedCells** to true and pass the **ImportTableOptions** object along with the list of columns/properties to the method to display your desired list of objects. Visit the following article for a detailed example:

[Importing from Custom Objects to merged area][7]

Following image provides an overview of this feature:



{{< figure align=center src="images/CustomToMerge.png" alt="">}}


## Other Enhancements and Fixes

*   Invalid number order when converting Arabic font to PDF.
*   Control all external data with IStreamProvider interface.
*   The method "String.StartsWith("\\0")" always returns true on macOS.
*   Exception when setting HTML string using the RGBA color model.

To use these features and avail other enhancements and fixes, I recommend you to try the release [Aspose.Cells for .NET v19.5][8]. Moreover, I recommend you to browse [Developers’ Guide][9] for your complete reference on what you can deliver using the APIs. Also, you are always welcome to share your review, concerns or feedback on [forums][10].




[1]: https://docs.aspose.com/display/cellsnet/Aspose.Cells+for+.NET+19.5+Release+Notes
[2]: https://www.nuget.org/packages/Aspose.Cells/19.5.0)
[3]: https://docs.aspose.com/display/cellsnet/Convert+Dates+to+Japanese+Dates
[4]: https://docs.aspose.com/display/cellsnet/Working+with+Background+in+ODS+Files#WorkingwithBackgroundinODSFiles-ReadBackgroundInformationfromOSDfile
[5]: https://docs.aspose.com/display/cellsnet/Working+with+Background+in+ODS+Files#WorkingwithBackgroundinODSFiles-AddColoredBackgroundtoODSfile
[6]: https://docs.aspose.com/display/cellsnet/Working+with+Background+in+ODS+Files#WorkingwithBackgroundinODSFiles-AddGraphicBackgroundtoODSfile
[7]: https://docs.aspose.com/display/cellsnet/Import+Data+into+Worksheet#ImportDataintoWorksheet-ImportingfromCustomObjectstomergedarea
[8]: https://downloads.aspose.com/cells/net/new-releases/-aspose.cells-for-.net-19.5/
[9]: https://docs.aspose.com/display/cellsnet/Developer+Guide
[10]: https://forum.aspose.com/c/cells





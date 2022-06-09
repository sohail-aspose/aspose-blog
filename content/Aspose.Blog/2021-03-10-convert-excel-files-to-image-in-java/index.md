---
title: 'Convert Excel Files to Image in Java'
seoTitle: "Convert Excel to Image in Java | XLSX to PNG, JPEG, BMP, TIFF and etc"
description: "Use Java Excel API to convert Excel XLSX or XLS files to PNG, JPEG, BMP, TIFF and other image formats using Java. Customized Excel to image conversion."
date: Wed, 10 Mar 2021 13:55:00 +0000
draft: false
url: /2021/03/10/convert-excel-files-to-image-in-java/
author: Usman Aziz
summary: 'Excel spreadsheets are widely used to store, organize and analyze data. However, you can not embed the Excel workbooks or worksheets directly into your web or desktop applications. One of the suitable options is converting worksheets to image or HTML formats. In this article, you will learn **how to convert Excel XLSX/XLS files to PNG, JPEG, BMP, and other image formats using Java**.'
tags: ['Xlsx to image java', 'convert excel to image java', 'xls to png java', 'xlsx to jpeg java', 'xlsx to png java']
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/Excel-to-Image.jpg" alt="Excel to Image Java">}}


Excel spreadsheets are widely used to store, organize and analyze data. However, you can not embed the Excel workbooks or worksheets directly into your web or desktop applications. One of the suitable options is converting worksheets to image or HTML formats. In this article, you will learn **how to convert Excel XLSX/XLS files to PNG, JPEG, BMP, and other image formats using Java**.

*   [Excel to Image Converter API][1]
*   [Convert Excel Files to Image][2]
*   [Additional Options for Excel to Image Conversion][3]
*   [Get Free License][4]

## Java Excel to Image Converter API {#Java-Excel-to-Image-Converter-API}

In order to convert Excel XLSX or XLS files to image formats, we'll use [Aspose.Cells for Java][5] API. It is a powerful spreadsheet manipulation API that provides high-quality conversion of worksheets into PNG, JPEG, BMP, and other popular image formats. Aspose.Cells for Java can be downloaded as [JAR][6] or installed using the following Maven configurations.

```
<repository>
    <id>AsposeJavaAPI</id>
    <name>Aspose Java API</name>
    <url>https://repository.aspose.com/repo/</url>
</repository>
```
```
<dependency>
    <groupId>com.aspose</groupId>
    <artifactId>aspose-cells</artifactId>
    <version>21.2</version>
</dependency>
```

Aspose.Cells for Java supports conversion of Excel files to the following image formats:

*   [EMF][7]
*   [WMF][8]
*   [JPEG][9]
*   [PNG][10]
*   [BMP][11]
*   [GIF][12]
*   [TIFF][13]
*   [SVG][14]
*   [GLTF][15]
*   PICT
*   SVM
*   Office Compatible EMF

## Convert Excel XLSX to Image in Java {#Excel-to-Image-Java-Conversion}

The following are the steps along with API references to convert a worksheet into a PNG image.

*   Load the Excel file using the [Workbook][16] class.
*   Create an instance of [ImageOrPrintOptions][17] class.
*   Set output image type using [ImageOrPrintOptions.setImageType(ImageType)][18] method.
*   Get the worksheet you want to convert into a [Worksheet][19] object.
*   Create a [SheetRender][20] object and initialize it with _Worksheet_ and _ImageOrPrintOptions_ objects.
*   Convert the worksheet and save the image file using [SheetRender.toImage(int, String)][21] method.

The following code sample shows how to convert an Excel XLSX file to image using Java.

{{< gist aspose-com-gists 634e9fb6f8515504317a7b71aa57b17a "excel-to-image.java" >}}

### Excel File



{{< figure align=center src="images/Excel-File-1.jpg" alt="Excel to Image Java">}}


### Converted PNG



{{< figure align=center src="images/Convert-Excel-to-Image.jpg" alt="XLSX to PNG java">}}


## Additional Options for Excel to Image Conversion {#Additional-Options-for-Excel-to-Image-Conversion}

Aspose.Cells for Java also provides additional options to customize XLSX to image conversion. For example, you can specify the style for gridlines, render one image per sheet, and so on. The [ImageOrPrintOptions][22] class is used to set these options. The following code sample shows how to use [ImageOrPrintOptions][23] class in Excel to image conversion.

{{< gist aspose-com-gists 634e9fb6f8515504317a7b71aa57b17a "excel-to-image-options.java" >}}

## Get a Free License {#Get-Free-License}

You can [get a free temporary license][24] in order to try the API without evaluation limitations.

## Conclusion

In this article, you have learned how to convert Excel files to PNG, JPEG, BMP, or other image formats using Java. Furthermore, you have seen how to customize Excel to image conversion with additional options. You can explore more about Java spreadsheet manipulation API using [documentation][25]. In case you would have any questions or queries, contact us via our [forum][26].

## See Also

*   [Encrypt and Decrypt Excel Files using Java][27]




[1]: #Java-Excel-to-Image-Converter-API
[2]: #Excel-to-Image-Java-Conversion
[3]: #Additional-Options-for-Excel-to-Image-Conversion
[4]: #Get-Free-License
[5]: https://products.aspose.com/cells/java
[6]: https://downloads.aspose.com/cells/java
[7]: https://docs.fileformat.com/image/emf/
[8]: https://docs.fileformat.com/image/wmf/
[9]: https://docs.fileformat.com/image/jpeg/
[10]: https://docs.fileformat.com/image/png/
[11]: https://docs.fileformat.com/image/bmp/
[12]: https://docs.fileformat.com/image/gif/
[13]: https://docs.fileformat.com/image/tiff/
[14]: https://docs.fileformat.com/page-description-language/svg/
[15]: https://docs.fileformat.com/3d/gltf/
[16]: https://apireference.aspose.com/cells/java/com.aspose.cells/Workbook
[17]: https://apireference.aspose.com/cells/java/com.aspose.cells/ImageOrPrintOptions
[18]: https://apireference.aspose.com/cells/java/com.aspose.cells/imageorprintoptions#ImageType
[19]: https://apireference.aspose.com/cells/java/com.aspose.cells/Worksheet
[20]: https://apireference.aspose.com/cells/java/com.aspose.cells/SheetRender
[21]: https://apireference.aspose.com/cells/java/com.aspose.cells/sheetrender#toImage(int,%20java.lang.String)
[22]: https://apireference.aspose.com/cells/java/com.aspose.cells/ImageOrPrintOptions
[23]: https://apireference.aspose.com/cells/java/com.aspose.cells/ImageOrPrintOptions
[24]: https://purchase.aspose.com/temporary-license
[25]: https://docs.aspose.com/cells/java/getting-started/
[26]: https://forum.aspose.com/
[27]: https://blog.aspose.com/2021/02/02/encrypt-and-decrypt-excel-files-using-java/






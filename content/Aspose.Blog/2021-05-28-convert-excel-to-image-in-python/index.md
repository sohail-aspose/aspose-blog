---
title: 'Convert Excel Files to Image in Python'
seoTitle: "Convert Excel to Image in Python | Excel to PNG, SVG, JPEG, BMP, GIF"
description: "Use Python Excel API to convert Exce files to image formats in Python. Convert Excel XLSX or XLS to PNG, SVG, JPEG, BMP, and other popular image formats."
date: Fri, 28 May 2021 15:35:22 +0000
draft: false
url: /2021/05/28/convert-excel-to-image-in-python/
author: Usman Aziz
summary: 'In various cases, Excel spreadsheets are required to be embedded in the web or desktop applications. One of the solutions in such cases is the conversion of Excel worksheets to image formats. In this article, you will learn **how to convert Excel XLSX or XLS to PNG, JPEG, SVG, or other images in Python**.'
tags: ['Convert Excel to Image in Python', 'Convert Excel to SVG in Python', 'Python Excel to Image Conversion API', 'XLSX to PNG Python', 'XLSX to SVG Python']
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/Excel-to-Image.jpg" alt="Excel to image in python">}}


In various cases, Excel spreadsheets are required to be embedded in the web or desktop applications. One of the solutions in such cases is the conversion of Excel worksheets to image formats. In this article, you will learn **how to convert Excel XLSX or XLS to PNG, JPEG, SVG, or other images in Python**.

*   [Python Excel to Image Converter API][1]
*   [Convert Excel to Image in Python][2]
*   [Convert Excel to SVG in Python][3]

## Python Excel to Image Converter API {#Python-Excel-to-Image-Conversion-API}

In order to convert Excel’s XLSX or XLS files to image formats, we will use [Aspose.Cells for Python via Java][4]. It is a spreadsheet manipulation API that lets you create, modify or convert Excel files. You can install the API using the following command.

*   `pip install aspose-cells`

Aspose.Cells for Python via Java supports conversion of Excel files to the following image formats:

*   [EMF][5]
*   [WMF][6]
*   [JPEG][7]
*   [PNG][8]
*   [BMP][9]
*   [GIF][10]
*   [TIFF][11]
*   [SVG][12]
*   [GLTF][13]
*   PICT
*   SVM
*   Office Compatible EMF

## Python Excel to Image Conversion {#Convert-Excel-to-Image-in-Python}

The following are the steps to convert Excel files to an image format, i.e. PNG, JPEG, etc. in Python.

*   Load the Excel file using the [Workbook][14] class.
*   Create an instance of [ImageOrPrintOptions][15] class and specify the output image format.
*   Access the worksheet you want to convert using [Workbook.getWorksheets().get(index)][16] method.
*   Create a [SheetRender][17] object and initialize it with _Worksheet_ and _ImageOrPrintOptions_ objects.
*   Save each page of Excel worksheet as an image using [SheetRender.toImage(pageIndex, fileName)][18] method.

The following code sample shows how to convert an Excel worksheet to PNG image.

{{< gist aspose-com-gists 5d33fa768a61d24704a7350432266781 "convert-excel-to-image.py" >}}

## Convert Excel to SVG Image in Python {#Convert-Excel-to-SVG-in-Python}

The following are the steps to convert an Excel file to SVG in Python.

*   Load the Excel file using the [Workbook][19] class.
*   Create an instance of [ImageOrPrintOptions][20] class and specify the output image format.
*   Loop through the worksheets in the Excel file using [Workbook.getWorksheets().getCount()][21] method.
*   In each iteration, perform the following operations:
    *   Create a [SheetRender][22] object and initialize it with _Worksheet_ and _ImageOrPrintOptions_ objects.
    *   Save each page of the Excel worksheet as SVG using [SheetRender.toImage(pageIndex, fileName)][23] method.

The following code sample shows how to convert Excel to SVG in Python.

{{< gist aspose-com-gists 5d33fa768a61d24704a7350432266781 "convert-excel-to-svg.py" >}}

## Get a Free API License

You can use the API without evaluation limitations by requesting a [free temporary license][24].

## Conclusion

In this article, you have learned how to convert Excel files to image formats in Python. The step-by-step guide and code samples demonstrated how to convert sheets in an Excel workbook to PNG and SVG formats. You can explore more about the Python spreadsheet API using the [documentation][25]. In case you would have any questions or queries, feel free to let us know via our [forum][26].

## See Also

*   [Create MS Excel Files using Python][27]
*   [Convert Excel to PDF in Python][28]




[1]: #Python-Excel-to-Image-Conversion-API
[2]: #Convert-Excel-to-Image-in-Python
[3]: #Convert-Excel-to-SVG-in-Python
[4]: https://products.aspose.com/cells/python-java
[5]: https://docs.fileformat.com/image/emf/
[6]: https://docs.fileformat.com/image/wmf/
[7]: https://docs.fileformat.com/image/jpeg/
[8]: https://docs.fileformat.com/image/png/
[9]: https://docs.fileformat.com/image/bmp/
[10]: https://docs.fileformat.com/image/gif/
[11]: https://docs.fileformat.com/image/tiff/
[12]: https://docs.fileformat.com/page-description-language/svg/
[13]: https://docs.fileformat.com/3d/gltf/
[14]: https://apireference.aspose.com/cells/python/asposecells.api/Workbook
[15]: https://apireference.aspose.com/cells/python/asposecells.api/ImageOrPrintOptions
[16]: https://apireference.aspose.com/cells/python/asposecells.api/worksheetcollection#Item%20(int)
[17]: https://apireference.aspose.com/cells/python/asposecells.api/SheetRender
[18]: https://apireference.aspose.com/cells/python/asposecells.api/sheetrender#toImage(int,%20java.lang.String)
[19]: https://apireference.aspose.com/cells/python/asposecells.api/Workbook
[20]: https://apireference.aspose.com/cells/python/asposecells.api/ImageOrPrintOptions
[21]: https://apireference.aspose.com/cells/python/asposecells.api/worksheetcollection#Count
[22]: https://apireference.aspose.com/cells/python/asposecells.api/SheetRender
[23]: https://apireference.aspose.com/cells/python/asposecells.api/sheetrender#toImage(int,%20java.lang.String)
[24]: https://purchase.aspose.com/temporary-license
[25]: https://docs.aspose.com/cells/pythonjava/
[26]: https://forum.aspose.com/
[27]: https://blog.aspose.com/2020/08/19/create-excel-xls-xlsx-using-python-excel-api/
[28]: https://blog.aspose.com/2021/04/02/convert-excel-files-to-pdf-in-python/






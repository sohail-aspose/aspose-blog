---
title: 'Convert Excel Files to PDF in Android'
seoTitle: "Android Library to Convert Excel XLSX XLS to PDF | Source Code"
description: "Use Android Excel library to convert Excel XLSX or XLS files to PDF in Android apps. Use additional options to convert Excel spreadsheets to PDF."
date: Wed, 21 Apr 2021 11:13:00 +0000
draft: false
url: /2021/04/21/convert-excel-files-to-pdf-in-android/
author: Usman Aziz
summary: 'In various cases, you may need to share the Excel files over the internet. To avoid tampering, it is a best practice to convert these files to PDF format before sharing. Accordingly, in this article, you will learn **how to convert Excel XLSX or XLS files to PDF in Android apps**. In addition, customization of Excel to PDF conversion will also be discussed.'
tags: ['excel to pdf android', 'excel to pdf android library', 'xls to pdf android', 'xlsx to pdf android']
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/Convert-Excel-to-PDF-Android.jpg" alt="Excel to PDF Android">}}


In various cases, you may need to share the Excel files over the internet. To avoid tampering, it is a best practice to convert these files to PDF format before sharing. Accordingly, in this article, you will learn **how to convert Excel XLSX or XLS files to PDF in Android apps**. In addition, customization of Excel to PDF conversion will also be discussed.

*   [Android Library for Excel to PDF Conversion][1]
*   [Convert Excel XLSX or XLS to PDF][2]
*   [Excel to PDF with Additional Options][3]
*   [Get a Free API License][4]

## Android Excel to PDF Converter Library {#Android-Library-for-Excel-to-PDF-Conversion}

To convert Excel spreadsheets to PDF, we'll use [Aspose.Cells for Android via Java][5]. It is a feature-rich Android library that lets you create, modify and convert Excel XLSX/XLS files seamlessly. You can either [download][6] the library or install it using the following configurations in build.gradle.

```
maven {
    url "https://repository.aspose.com/repo/" }
```
```
compile (
        group: 'com.aspose',
        name: 'aspose-cells',
        version: '21.3',
        classifier: 'android.via.java')
```

## Convert Excel XLSX or XLS to PDF in Android {#Convert-Excel-XLSX-or-XLS-to-PDF}

The following are the steps to convert an Excel XLSX file to PDF in Android.

*   Create an object of the [Workbook][7] class and initialize it with the path to the Excel file.
*   Save the Excel file as a PDF using [Workbook.save(String, SaveFormat)][8] method.

The following code sample shows how to convert an XLSX file to PDF in Android.

{{< gist aspose-com-gists 2396821770031adfbe82eee1d66854f0 "excel-to-pdf.java" >}}

## Android Excel to PDF with Additional Options {#Excel-to-PDF-with-Additional-Options}

You can also control the Excel to PDF conversion to customize the converted PDF as required. For example, you can define the PDF compliance, pages per sheet, gridlines style, a range of sheets to convert, etc. To achieve this, Aspose.Cells provides [PdfSaveOptions][9] class. The following are the steps of how to customize the XLSX/XLS to PDF conversion.

*   Load the Excel file using the [Workbook][10] class.
*   Create an instance of the [PdfSaveOptions][11] class.
*   Set the desired option such as PDF compliance using [PdfSaveoptions.setCompliance(PdfCompliance)][12] method.
*   Save the Excel file as a PDF using [Workbook.save(String, PdfSaveOptions)][13] method.

The following code sample shows how to customize Excel to PDF conversion in Android.

{{< gist aspose-com-gists 2396821770031adfbe82eee1d66854f0 "excel-to-pdfa.java" >}}

## Get a Free API License {#Get-a-Free-API-License}

You can [request a free temporary license][14] to use the API without evaluation limitations.

## Conclusion

In this article, you have learned how to convert Excel XLSX or XLS files to PDF from within the Android apps. Furthermore, you have seen how to customize the Excel to PDF conversion using different options. You can explore more about Aspose.Cells for Android via Java using the [documentation][15]. In case you would have any queries, feel free to let us know via our [forum][16].

## See Also

*   [Create, Edit or Convert Excel Files in Android][17]




[1]: #Android-Library-for-Excel-to-PDF-Conversion
[2]: #Convert-Excel-XLSX-or-XLS-to-PDF
[3]: #Excel-to-PDF-with-Additional-Options
[4]: #Get-a-Free-API-License
[5]: https://products.aspose.com/cells/android-java/
[6]: https://downloads.aspose.com/cells/androidjava
[7]: https://apireference.aspose.com/cells/java/com.aspose.cells/Workbook
[8]: https://apireference.aspose.com/cells/java/com.aspose.cells/workbook#save(java.lang.String,%20int)
[9]: https://apireference.aspose.com/cells/java/com.aspose.cells/PdfSaveOptions
[10]: https://apireference.aspose.com/cells/java/com.aspose.cells/Workbook
[11]: https://apireference.aspose.com/cells/java/com.aspose.cells/PdfSaveOptions
[12]: https://apireference.aspose.com/cells/java/com.aspose.cells/pdfsaveoptions#Compliance
[13]: https://apireference.aspose.com/cells/java/com.aspose.cells/workbook#save(java.lang.String,%20com.aspose.cells.SaveOptions)
[14]: https://purchase.aspose.com/temporary-license
[15]: https://docs.aspose.com/cells/androidjava/
[16]: https://forum.aspose.com/
[17]: https://blog.aspose.com/2013/08/06/introducing-aspose.cells-for-android/






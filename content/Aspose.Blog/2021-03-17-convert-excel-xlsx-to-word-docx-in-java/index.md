---
title: 'Convert Excel XLSX to Word DOCX in Java'
seoTitle: "Convert XLSX to DOCX in Java | Excel to Word Conversion in Java"
description: "Use Java Excel API to convert XLSX files to DOCX format using Java. Customize Excel to Word conversion using different options."
date: Wed, 17 Mar 2021 14:06:00 +0000
draft: false
url: /2021/03/17/convert-excel-xlsx-to-word-docx-in-java/
author: Usman Aziz
summary: 'Excel to Word conversion could be useful when you need to export data from an Excel worksheet to a table in a Word document. In order to automate this conversion, this article covers **how to convert Excel XLSX files to Word DOCX format using Java**. Furthermore, additional options are also discussed to customize XLSX to DOCX conversion.'
tags: ['Convert XLSX to DOCX in Java', 'Customize XLSX to DOCX Conversion in Java', 'Excel to Word Java Converter API']
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/XLSX-to-DOCX-Conversion.jpg" alt="XLSX to DOCX Java">}}


Excel to Word conversion could be useful when you need to export data from a worksheet to a table in a Word document. In order to automate this conversion, this article covers **how to convert Excel XLSX files to Word DOCX format using Java**. Furthermore, additional options are also discussed to customize XLSX to DOCX conversion.

*   [Excel to Word Java Converter API][1]
*   [Convert XLSX to DOCX in Java][2]
*   [Customize XLSX to DOCX Conversion in Java][3]
*   [Get a Free API License][4]

## Excel to Word Java Converter API {#Excel-to-Word-Java-Converter-API}

[Aspose.Cells for Java][5] is a spreadsheet manipulation API that lets you generate, process, and manipulate Excel files. In addition, the API provides high-quality conversion of Excel XLSX files to other formats including DOCX, PDF, etc. You can either [download][6] the API or install it using the following Maven configuration.

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
    <version>21.3</version>
</dependency>
```

## Convert XLSX to DOCX in Java {#Convert-Excel-XLSX-to-Word-DOCX-in-Java}

Conversion of an Excel spreadsheet to a Word document is as easy as pie. It can be done in a couple of steps using Aspose.Cells for Java. The following are the steps to convert an XLSX file to DOCX format.

*   First, load the Excel XLSX file using the [Workbook][7] class.
*   Finally, convert XLSX to DOCX using [Workbook.save(String, SaveFormat.DOCX)][8] method.

The following code sample shows how to convert an Excel XLSX file to Word DOCX using Java.

{{< gist aspose-com-gists d82ed23b0482cd74579351e65db5d1c2 "xlsx-to-docx.java" >}}

## Customize XLSX to DOCX Conversion in Java {#Customize-XLSX-to-DOCX-Conversion-in-Java}

You can also customize Excel to Word conversion using different options provided by [DocxSaveOptions][9] class. The following is the list of options that you can use.

<figure class="wp-block-table is-style-stripes"><table><thead><tr><th>Option</th><th>Description</th></tr></thead><tbody><tr><td>[CachedFileFolder](https://apireference.aspose.com/cells/java/com.aspose.cells/docxsaveoptions#CachedFileFolder)</td><td>The cache folder to store some large data.</td></tr><tr><td>[ClearData](https://apireference.aspose.com/cells/java/com.aspose.cells/docxsaveoptions#ClearData)</td><td>Make the workbook empty after saving the file.</td></tr><tr><td>[CreateDirectory](https://apireference.aspose.com/cells/java/com.aspose.cells/docxsaveoptions#CreateDirectory)</td><td>If true and the directory does not exist, the directory will be automatically created before saving the file.</td></tr><tr><td>[MergeAreas](https://apireference.aspose.com/cells/java/com.aspose.cells/docxsaveoptions#MergeAreas)</td><td>Indicates whether to merge the areas of conditional formatting and validation before saving the file.</td></tr><tr><td>[RefreshChartCache](https://apireference.aspose.com/cells/java/com.aspose.cells/docxsaveoptions#RefreshChartCache)</td><td>Indicates whether refreshing chart cache data.</td></tr><tr><td>[SortNames](https://apireference.aspose.com/cells/java/com.aspose.cells/docxsaveoptions#SortNames)</td><td>Indicates whether to sort defined names before saving files.</td></tr><tr><td>[UpdateSmartArt](https://apireference.aspose.com/cells/java/com.aspose.cells/docxsaveoptions#UpdateSmartArt)</td><td>Indicates whether to update the smart art setting.</td></tr><tr><td>[ValidateMergedAreas](https://apireference.aspose.com/cells/java/com.aspose.cells/docxsaveoptions#ValidateMergedAreas)</td><td>Indicates whether validate merged cells before saving the file.</td></tr><tr><td>[WarningCallback](https://apireference.aspose.com/cells/java/com.aspose.cells/docxsaveoptions#WarningCallback)</td><td>Gets or sets warning callback.</td></tr></tbody></table></figure>

The following code sample shows how to use [DocxSaveOptions][10] class while converting Excel XLSX to Word DOCX using Java.

{{< gist aspose-com-gists d82ed23b0482cd74579351e65db5d1c2 "xlsx-to-docx-customized.java" >}}

## Get a Free API License {#Get-a-Free-License}

You can try Aspose.Cells for Java for free by [getting a temporary license][11].

## Conclusion

In this article, you have learned how to convert Excel XLSX files to DOCX format using Java. Furthermore, you have seen how to use different options in order to customize Excel to Word conversion. You can explore more about Aspose.Cells for Java using [documentation][12]. Moreover, if you would have any questions or queries, feel free to contact us via our [forum][13].

## See Also

*   [Encrypt and Decrypt Excel Files using Java][14]




[1]: #Excel-to-Word-Java-Converter-API
[2]: #Convert-Excel-XLSX-to-Word-DOCX-in-Java
[3]: #Customize-XLSX-to-DOCX-Conversion-in-Java
[4]: #Get-a-Free-License
[5]: https://products.aspose.com/cells/java
[6]: https://downloads.aspose.com/cells/java
[7]: https://apireference.aspose.com/cells/java/com.aspose.cells/Workbook
[8]: https://apireference.aspose.com/cells/java/com.aspose.cells/workbook#save(java.lang.String,%20int)
[9]: https://apireference.aspose.com/cells/java/com.aspose.cells/DocxSaveOptions
[10]: https://apireference.aspose.com/cells/java/com.aspose.cells/DocxSaveOptions
[11]: https://purchase.aspose.com/temporary-license
[12]: https://docs.aspose.com/cells/java/
[13]: https://forum.aspose.com/
[14]: https://blog.aspose.com/2021/02/02/encrypt-and-decrypt-excel-files-using-java/






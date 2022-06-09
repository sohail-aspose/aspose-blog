---
title: 'Convert Excel Files to PDF in PHP'
seoTitle: "Convert Excel to PDF in PHP | XLSX to PDF or XLS to PDF in PHP"
description: "Use PHP spreadsheet manipulation API to convert Excel files to PDF in PHP. Convert XLSX to PDF or XLS to PDF using advanced conversion options."
date: Tue, 11 May 2021 11:50:37 +0000
draft: false
url: /2021/05/11/convert-excel-files-to-pdf-in-php/
author: Usman Aziz
summary: 'Excel spreadsheets are widely used to store and analyze data in the form of rows and columns. However, in various cases, you need to convert the Excel files to PDF before sharing them over the internet. In order to automate Excel to PDF conversion, this article shows **how to convert Excel files to PDF programmatically using PHP**. Furthermore, advanced options to customize the Excel to PDF conversion are also discussed.'
tags: ['Convert Excel to PDF in PHP', 'PHP Excel to PDF Conversion API', 'XLS to PDF in PHP', 'XLSX to PDF in PHP']
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/Convert-Excel-to-PDF.jpg" alt="Excel to PDF PHP">}}


Excel spreadsheets are widely used to store and analyze data in the form of rows and columns. However, in various cases, you need to convert the Excel files to PDF before sharing them over the internet. In order to automate Excel to PDF conversion, this article shows **how to convert Excel files to PDF programmatically using PHP**. Furthermore, advanced options to customize the Excel to PDF conversion are also discussed.

*   [PHP Excel to PDF Conversion API][1]
*   [Convert Excel XLSX/XLS to PDF][2]
*   [Advanced Options for Excel XLSX/XLS to PDF][3]

## PHP Excel to PDF Conversion API {#PHP-Excel-to-PDF-Conversion-API}

In order to convert Excel XLSX or XLS files to PDF, we will use [Aspose.Cells for PHP via Java][4]. It is a feature-rich API that lets you implement spreadsheet automation features within your web applications. You can download the API's package from [here][5].

### Usage

The following are the prerequisites that you need to fulfill in order to use _Aspose.Cells for PHP via Java_.

*   [Java SE Development Kit 1.7 or higher][6]
*   [PHP 7.0 or higher][7]
*   [Java Bridge][8]
*   [Java Inc][9]

Once you have completed the prerequisites, follow the below steps to execute the _example.php_ file for testing.

1\. Place _Java.inc_ file in the root folder of the API's package that you have downloaded.

2\. Run _JavaBridge.jar_ using the below commands in the command prompt:

```
> cd aspose.cells
> %JAVA_HOME%\bin\java -Djava.ext.dirs=lib -jar JavaBridge.jar SERVLET_LOCAL:8080
```

3\. Run _example.php_ from the API's root folder using the below command:

```
> php example.php
```

## Convert Excel XLSX or XLS to PDF in PHP {#Convert-Excel-XLSX/XLS-to-PDF}

The following are the steps to convert Excel XLSX or XLS to PDF.

*   Create an object of the [Workbook][10] class and initialize it with Excel file's path.
*   Convert Excel to PDF using [$workbook->save("output.pdf", SaveFormat::PDF)][11] method.

The following code sample shows how to convert an Excel XLSX file to PDF in PHP.

{{< gist aspose-com-gists de60ad22bd9f3f16a6011e6e5ec2d01e "excel-to-pdf.php" >}}

### Excel File



{{< figure align=center src="images/Excel-to-PDF.jpg" alt="Excel to PDF">}}


### Converted PDF



{{< figure align=center src="images/Excel-to-PDF-Converted.jpg" alt="convert Excel to PDF">}}


## Advanced Options for Excel to PDF Conversion {#Advanced-Options-for-Excel-XLSX/XLS-to-PDF}

Aspose.Cells also provides additional options to customize the Excel to PDF conversion. For example, you can set PDF compliance, compression, gridlines style, number of pages per sheet, etc. 

The following are the steps to set additional options in Excel to PDF conversion.

*   Create an object of the [Workbook][12] class and initialize it with Excel file's path.
*   Create an object of [PdfSaveOptions][13] class.
*   Set desired options such as PDF compliance using [PdfSaveOptions->setCompliance(PdfCompliance::PDF\_A\_1\_B)][14] method.
*   Convert Excel to PDF using [$workbook->save("output.pdf", PdfSaveOptions)][15] method.

The following code sample shows how to customize Excel to PDF conversion using additional options.

{{< gist aspose-com-gists de60ad22bd9f3f16a6011e6e5ec2d01e "excel-to-pdf-advanced.php" >}}

## Get a Free API License {#Get-a-Free-API-License}

In order to use the API without evaluation limitations, you can [request a free temporary license][16].

## Conclusion

In this article, you have learned how to convert Excel files to PDF using PHP. Furthermore, you have seen how to customize Excel to PDF conversion using advanced options. You can explore more about the API using the [documentation][17]. Furthermore, you can contact us via our [forum][18] in case of any query.

## See Also

*   [Create Excel XLSX/XLS Files in Node.js Applications – A Complete Guide][19]




[1]: #PHP-Excel-to-PDF-Conversion-API
[2]: #Convert-Excel-XLSX/XLS-to-PDF
[3]: #Advanced-Options-for-Excel-XLSX/XLS-to-PDF
[4]: https://products.aspose.com/cells/php-java
[5]: https://downloads.aspose.com/cells/php
[6]: https://www.oracle.com/technetwork/java/javase/downloads/java-archive-downloads-javase7-521261.html
[7]: https://www.php.net/downloads.php
[8]: https://sourceforge.net/projects/php-java-bridge/files/Binary%20package/php-java-bridge_7.2.1/exploded/JavaBridge.jar/download
[9]: http://php-java-bridge.sourceforge.net/pjb/download.php
[10]: https://apireference.aspose.com/cells/php/aspose.cells/Workbook
[11]: https://apireference.aspose.com/cells/php/aspose.cells/workbook#save(java.lang.String,%20int)
[12]: https://apireference.aspose.com/cells/php/aspose.cells/Workbook
[13]: https://apireference.aspose.com/cells/php/aspose.cells/PdfSaveOptions
[14]: https://apireference.aspose.com/cells/php/aspose.cells/pdfsaveoptions#Compliance
[15]: https://apireference.aspose.com/cells/php/aspose.cells/workbook#save(java.lang.String,%20com.aspose.cells.SaveOptions)
[16]: https://purchase.aspose.com/temporary-license
[17]: https://docs.aspose.com/cells/phpjava/
[18]: https://forum.aspose.com/
[19]: https://blog.aspose.com/2020/08/05/create-excel-files-in-node.js/






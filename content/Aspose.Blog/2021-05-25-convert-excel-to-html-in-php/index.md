---
title: 'Convert Excel Files to HTML in PHP'
seoTitle: "Convert Excel to HTML in PHP | XLSX to HTML | XLS to HTML | PHP API"
description: "Use PHP Excel API to convert Excel files to HTML in PHP. Customize XLSX to HTML or XLS to HTML conversion with additional options in web applications."
date: Tue, 25 May 2021 11:51:00 +0000
draft: false
url: /2021/05/25/convert-excel-to-html-in-php/
author: Usman Aziz
summary: 'In order to embed Excel spreadsheets within your web pages, you need to convert them into either images or HTML content. Since HTML is more suitable for websites, therefore, this article covers **how to convert Excel XLSX or XLS files to HTML pages in PHP**.'
tags: ['Convert Excel Files to HTML', 'PHP Excel to HTML Conversion API', 'XLS to HTML PHP', 'XLSX to HTML PHP']
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/Excel-to-HTML-Logo.jpg" alt="PHP Excel to HTML">}}


In order to embed Excel spreadsheets within your web pages, you need to convert them into either images or HTML content. Since HTML is more suitable for websites, therefore, this article covers **how to convert Excel XLSX or XLS files to HTML pages in PHP**.

*   [PHP Excel to HTML Conversion API][1]
*   [Convert Excel Files to HTML][2]
*   [Additional Options in Excel to HTML Conversion][3]

## PHP Excel to HTML Conversion API {#PHP-Excel-to-HTML-Conversion-API}

In order to convert Excel XLSX or XLS files to HTML, we will use [Aspose.Cells for PHP via Java][4]. The API provides a wide range of spreadsheet automation features for PHP based web applications. You can download the API’s package from [here][5].

### Usage

The following are the prerequisites that you need to fulfill in order to use _Aspose.Cells for PHP via Java_.

*   [Java SE Development Kit 1.7 or higher][6]
*   [PHP 7.0 or higher][7]
*   [Java Bridge][8]
*   [Java Inc][9]

Once you have completed the prerequisites, follow the below steps to execute the _example.php_ file for testing.

1\. Place _Java.inc_ file in the root folder of the API’s package that you have downloaded.

2\. Run _JavaBridge.jar_ using the below commands in the command prompt:

```
\> cd aspose.cells
> %JAVA\_HOME%\\bin\\java -Djava.ext.dirs=lib -jar JavaBridge.jar SERVLET\_LOCAL:8080
```

3\. Run _example.php_ from the API’s root folder using the below command:

```
\> php example.php
```

## Convert Excel Files to HTML in PHP {#Convert-Excel-Files-to-HTML}

The following are the steps to convert Excel files to HTML.

*   Load the Excel file using the [Workbook][10] class.
*   Convert Excel to HTML using [Workbook->save(string, SaveFormat::HTML)][11] method.

The following code sample shows how to convert an Excel XLSX file to HTML in PHP.

\[gist id="1b7e9c7d97807626c16302c2b4f67ad5" file="excel-to-html.php"\]

### Excel to HTML



{{< figure align=center src="images/Excel-to-HTML.jpg" alt="Excel to HTML PHP">}}


## Excel to HTML - Set Additional Options {#Set-Additional-Options-in-Excel-to-HTML}

Aspose.Cells also allows you to set additional options in Excel to HTML conversion, such as enable tooltip text, show/hide gridlines, etc. To enable or disable these options, [HtmlSaveOptions][12] class is used.

The following are the steps to set additional options while converting Excel files to HTML.

*   Load the Excel file using the [Workbook][13] class.
*   Create an object of [HtmlSaveOptions][14] class and set options, such as [HtmlSaveOptions->setAddTooltipText(true)][15].
*   Convert Excel to HTML using [Workbook->save(string, HtmlSaveOptions)][16] method.

The following code sample shows how to set additional options while converting XLSX to HTML in PHP.

\[gist id="1b7e9c7d97807626c16302c2b4f67ad5" file="excel-to-html-options.php"\]

## Get a Free API License {#Get-Free-License}

You can use the API for free without evaluation limitations using a [temporary license][17].

## Conclusion

In this article, you have learned how to convert Excel files to HTML using PHP. Furthermore, you have seen how to customize the Excel to HTML conversion. You can explore more about the PHP Excel API using the [documentation][18]. In case you would have any questions, feel free to let us know via our [forum][19].

## See Also

*   [Convert Excel Files to PDF in PHP][20]



[1]: #PHP-Excel-to-HTML-Conversion-API
[2]: #Convert-Excel-Files-to-HTML
[3]: #Set-Additional-Options-in-Excel-to-HTML
[4]: https://products.aspose.com/cells/php-java
[5]: https://downloads.aspose.com/cells/php
[6]: https://www.oracle.com/technetwork/java/javase/downloads/java-archive-downloads-javase7-521261.html
[7]: https://www.php.net/downloads.php
[8]: https://sourceforge.net/projects/php-java-bridge/files/Binary%20package/php-java-bridge_7.2.1/exploded/JavaBridge.jar/download
[9]: http://php-java-bridge.sourceforge.net/pjb/download.php
[10]: https://apireference.aspose.com/cells/php/aspose.cells/Workbook
[11]: https://apireference.aspose.com/cells/php/aspose.cells/workbook#save(java.lang.String,%20int)
[12]: https://apireference.aspose.com/cells/php/aspose.cells/HtmlSaveOptions
[13]: https://apireference.aspose.com/cells/php/aspose.cells/Workbook
[14]: https://apireference.aspose.com/cells/php/aspose.cells/HtmlSaveOptions
[15]: https://apireference.aspose.com/cells/php/aspose.cells/htmlsaveoptions#AddTooltipText
[16]: https://apireference.aspose.com/cells/php/aspose.cells/workbook#save(java.lang.String,%20int)
[17]: https://purchase.aspose.com/temporary-license
[18]: https://docs.aspose.com/cells/phpjava/
[19]: https://forum.aspose.com/
[20]: https://blog.aspose.com/2021/05/11/convert-excel-files-to-pdf-in-php/






---
title: 'Convert Excel Files to HTML using Java'
seoTitle: "Excel to HTML using Java | Convert XLSX XLS Files to HTML in Java"
description: "Convert MS Excel XLSX or XLS files to HTML using Java. Use options to enable tooltips in Excel to HTML conversion and enhance the presentation of the HTML."
date: Mon, 28 Dec 2020 10:05:51 +0000
draft: false
url: /2020/12/28/convert-excel-to-html-using-java/
author: Usman Aziz
summary: 'Excel spreadsheets allow you to store and well organize the data in tabular form. You can perform computations as well as generate different types of graphs and charts in order to analyze the data. However, in various scenarios, you may need to carry out Excel to HTML conversion to convert worksheets to HTML pages. For example, when embedding the content of the spreadsheets into web pages. In accordance with that, this article aims to cover **how to convert Excel XLSX files to HTML programmatically using Java**.'
tags: ['convert excel to html java', 'xls to html java', 'xlsx to html java']
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/Excel-to-HTML-Logo.jpg" alt="Java Excel to HTML">}}


Excel spreadsheets allow you to store and well organize the data in tabular form. You can perform computations as well as generate different types of graphs and charts in order to analyze the data. However, in various scenarios, you may need to carry out Excel to HTML conversion to convert worksheets to HTML pages. For example, when embedding the content of the spreadsheets into web pages. In accordance with that, this article aims to cover **how to convert Excel XLSX files to HTML programmatically using Java**.

*   [Excel to HTML Java Converter API][1]
*   [Excel to HTML Java Conversion][2]
*   [Convert Excel to HTML with Tooltip][3]
*   [Convert Excel to HTML with Presentation Preference][4]
*   [Get Free License][5]

## Excel to HTML Java Converter API {#Excel-to-HTML-Java-API}

[Aspose.Cells for Java][6] is a spreadsheet manipulation API that is designed to implement Excel automation within the Java applications. In addition, the API's built-in spreadsheet converter engine allows you to convert XLSX files to HTML or other formats. You can either [download][7] the API or install it within your Maven-based applications.

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
    <version>20.11</version>
</dependency>
```

## Excel to HTML Java Conversion {#Excel-to-HTML-Java-Conversion}

Excel to HTML conversion using Aspose.Cells is as easy as pie. Just load the Excel spreadsheet and save it as an HTML file. The following are the steps to convert an Excel XLSX file to HTML.

*   Load the XLSX file using the [Workbook][8] class.
*   Save the file with _.html_ extension using [Workbook.Save(String)][9] method.

The following code sample shows how to convert an Excel file to HTML using Java.

{{< gist aspose-com-gists 0a303cfc684591a40f715df5a1494c89 "excel-to-html.java" >}}

## Convert Excel to HTML with Tooltip {#Convert-Excel-to-HTML-with-Tooltip}

In certain situations, the text exceeds the width of the cell in the worksheet. When you convert such a worksheet to an HTML page, some part of the text becomes hidden. For such scenarios, you can enable tooltips to view the exceeded text. The following are the steps to enable tooltips in Excel to HTML conversion.

*   Load the XLSX file using the [Workbook][10] class.
*   Create an instance of [HtmlSaveOptions][11] class.
*   Use [HtmlSaveOptions.setAddTooltipText(true)][12] to enable tooltips.
*   Save the file with _.html_ extension using [Workbook.Save(String, HtmlSaveOptions)][13] method.

The following code sample shows how to enable tooltips in Excel to HTML conversion in Java.

{{< gist aspose-com-gists 0a303cfc684591a40f715df5a1494c89 "excel-to-html-tooltip.java" >}}

## Convert Excel to HTML with Presentation Preference {#Convert-Excel-to-HTML-with-Presentation-Preference}

Aspose.Cells for Java provides an additional feature of setting presentation preference for the rendered HTML pages. You can use this feature to get a more attractive presentation of Excel workbooks when rendered to HTML. For this, you can set [HtmlSaveOptions.setPresentationPreference(true)][14] property. The following code sample shows how to enable presentation preference in Excel to HTML conversion.

{{< gist aspose-com-gists 0a303cfc684591a40f715df5a1494c89 "excel-to-html-presentation-preference.java" >}}

## Try Aspose.Cells for Free {#Get-Free-License}

You can use Aspose.Cells for Java for free without restrictions using a [free trial license][15].

## Conclusion

In this article, you have learned how to convert Excel files to HTML using Java. Furthermore, you have seen how to enable tooltips and presentation preference in Excel to HTML conversion. You can explore more about the Java Excel API using the [documentation][16].

## See Also

*   [Create MS Excel Files using Java without MS Office][17]




[1]: #Excel-to-HTML-Java-API
[2]: #Excel-to-HTML-Java-Conversion
[3]: #Convert-Excel-to-HTML-with-Tooltip
[4]: #Convert-Excel-to-HTML-with-Presentation-Preference
[5]: #Get-Free-License
[6]: https://products.aspose.com/cells/java
[7]: https://downloads.aspose.com/cells/java
[8]: https://apireference.aspose.com/cells/java/com.aspose.cells/workbook
[9]: https://apireference.aspose.com/cells/java/com.aspose.cells/workbook#save(java.lang.String)
[10]: https://apireference.aspose.com/cells/java/com.aspose.cells/workbook
[11]: https://apireference.aspose.com/cells/java/com.aspose.cells/HtmlSaveOptions
[12]: https://apireference.aspose.com/cells/java/com.aspose.cells/htmlsaveoptions#AddTooltipText
[13]: https://apireference.aspose.com/cells/java/com.aspose.cells/workbook#save(java.lang.String,%20com.aspose.cells.SaveOptions)
[14]: https://apireference.aspose.com/cells/java/com.aspose.cells/htmlsaveoptions#PresentationPreference
[15]: https://purchase.aspose.com/temporary-license
[16]: http://docs.aspose.com/cells/java
[17]: https://blog.aspose.com/2020/10/13/create-excel-xlsx-xls-using-java-without-ms-office/






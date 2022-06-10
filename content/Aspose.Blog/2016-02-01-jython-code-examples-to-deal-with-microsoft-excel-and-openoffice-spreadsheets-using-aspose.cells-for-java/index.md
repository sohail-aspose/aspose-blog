---
title: 'Jython Code Examples to Deal with Microsoft Excel and OpenOffice Spreadsheets using Aspose.Cells for Java'
date: Mon, 01 Feb 2016 04:24:07 +0000
draft: false
url: /2016/02/01/jython-code-examples-to-deal-with-microsoft-excel-and-openoffice-spreadsheets-using-aspose.cells-for-java/
author: Fahad Adeel
summary: ''
tags: ['Aspose.Cells Java for Jython', 'Excel API for Jython', 'Jython code examples for excel', 'convert worksheet to image', 'create spreadsheets in Jython']
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/aspose_cells-for-java.png" alt="Excel API for Java">}}




{{< figure align=center src="images/jython.png" alt="Jython library for Excel and OpenOffice">}}


We are pleased to announce “[Aspose.Cells Java for Jython][1]”, a new project for Jython developers. The project is aimed to provide useful examples for [Jython][2] developers who want to utilize [Aspose.Cells for Java API][3] in their Jython applications to deal with Microsoft Word and OpenOffice documents.

## Download, Installation and Usage

Please check the links below to find instructions on downloading, installing and using Aspose.Words Java for Jython.

*   [Downloads and Installation][4]

OR

You can download the latest version from:

*   [Pypi][5]
*   [CodePlex][6]
*   [GitHub][7]

## Quick Start Tutorial

The following example demonstrates how you can create a HelloWorld Excel document.

```
from asposecells import Settings
from com.aspose.cells import Workbook
from com.aspose.cells import FileFormatType

class HelloWorld:

    def __init__(self):
        dataDir = Settings.dataDir + 'quickstart/'

        workbook = Workbook()

        sheet = workbook.getWorksheets().get(0)

        cell = sheet.getCells().get("A1")

        cell.setValue("Hello World!")

        file_format_type = FileFormatType

        workbook.save(dataDir + "HelloWorld.xls" , file_format_type.EXCEL_97_TO_2003 )

        print "Document has been saved, please check the output file.";

if __name__ == '__main__':        
    HelloWorld()
```

## Aspose.Cells Java for Jython Examples:

**Quick Start**

*   [Hello World][8]

**Working With Excel Files Jython**

*   File Handling Features
    *   [Opening Files][9]
    *   [Saving Files][10]
*   Utility Features
    *   [Converting Excel to PDF Files][11]
    *   [Converting Chart to Image][12]
    *   [Converting Worksheet to Image][13]
    *   [Managing Document Properties][14]
    *   [Converting Worksheet to SVG][15]
    *   [Converting to MHTML Files][16]
    *   [Converting Excel Files to HTML][17]

**Working With Worksheets**

*   Management Features
    *   [Managing Worksheets][18]
*   Display Features
    *   [Hide or Unhide a Worksheet][19]
    *   [Display or Hide Tabs][20]
    *   [Display or Hide Scroll Bars][21]
    *   [Display or Hide Gridlines][22]
    *   [Page Break Preview][23]
    *   [Freeze Panes][24]
    *   [Split Panes][25]
*   Security Features
    *   [Protecting Worksheets][26]
    *   [Unprotect a Worksheet][27]
*   Page Setup Features
    *   [Setting Page Options][28]
*   Value Features
    *   [Managing Page Breaks][29]
    *   Copying and Moving Worksheets

**Working With Rows And Columns**

*   [Inserting and Deleting Rows and Columns][30]
*   [Hiding and Showing Rows and Columns][31]
*   [Grouping and Ungrouping Rows and Columns][32]
*   [Adjusting Row Height and Column Width][33]
*   [Auto fit Rows and Columns][34]
*   [Copying Rows and Columns][35]

## Aspose.Cells Java for Jython Documentation

[Aspose.Cells Java for Jython Documentation][36] is available to guide developers to get familiar with the specific resources and operations within the Aspose.Cells Java for Jython.

## Start a Free Trial Today

Start a free trial today – all you need is to [sign up][37] with Aspose. Once you have signed up, you are ready to try powerful file processing features offered by Aspose file format APIs.

## Customer Feedback

Your feedback is very important to us. Please feel free to provide feedback and raise feature requirements. We are keen to implement customer driven features since we are a 100% customer driven company.




[1]: https://docs.aspose.com/
[2]: http://www.jython.org/
[3]: https://products.aspose.com/cells/java
[4]: http://docs.aspose.com/display/cellsjava/Aspose.Cells+Java+for+Jython
[5]: https://pypi.python.org/pypi/aspose-cells-java-for-python
[6]: https://docs.aspose.com/
[7]: https://github.com/asposecells/Aspose_Cells_Java/releases/tag/Aspose.Cells_Java_for_Jython-v1.0.0
[8]: http://docs.aspose.com/display/cellsjava/Hello+World+in+Jython
[9]: http://docs.aspose.com/display/cellsjava/Opening+Files+in+Jython
[10]: http://docs.aspose.com/display/cellsjava/Saving+Files+in+Jython
[11]: http://docs.aspose.com/display/cellsjava/Excel+to+Pdf+Conversion+in+Jython
[12]: https://docs.aspose.com/display/cellsjava/Home
[13]: http://docs.aspose.com/display/cellsjava/Worksheet+To+Image+in+Jython
[14]: http://docs.aspose.com/display/cellsjava/Managing+Document+Properties+in+Jython
[15]: http://docs.aspose.com/display/cellsjava/Converting+Worksheet+To+SVG+in+Jython
[16]: http://docs.aspose.com/display/cellsjava/Converting+To+Mhtml+Files+in+Jython
[17]: http://docs.aspose.com/display/cellsjava/Converting+ExcelFiles+To+Html+in+Jython
[18]: http://docs.aspose.com/display/cellsjava/Working+With+Worksheets+in+Jython
[19]: http://docs.aspose.com/display/cellsjava/Hide+Unhide+Worksheet+in+Jython
[20]: http://docs.aspose.com/display/cellsjava/Display+Hide+Tabs+in+Jython
[21]: http://docs.aspose.com/display/cellsjava/Display+Hide+Scroll+Bars+in+Jython
[22]: http://docs.aspose.com/display/cellsjava/Display+Hide+Gridlines+in+Jython
[23]: http://docs.aspose.com/display/cellsjava/Page+Break+Preview+in+Jython
[24]: http://docs.aspose.com/display/cellsjava/Freeze+Panes+in+Jython
[25]: http://docs.aspose.com/display/cellsjava/Split+Panes+in+Jython
[26]: http://docs.aspose.com/display/cellsjava/Protecting+Worksheet+in+Jython
[27]: http://docs.aspose.com/display/cellsjava/Unprotecting+Password+Protected+Worksheet+in+Jython
[28]: http://docs.aspose.com/display/cellsjava/Setting+Page+Options+in+Jython
[29]: http://docs.aspose.com/display/cellsjava/Managing+Page+Breaks+in+Jython
[30]: http://docs.aspose.com/display/cellsjava/Inserting+and+Deleting+Rows+and+Columns+in+Jython
[31]: http://docs.aspose.com/display/cellsjava/Hiding+and+Showing+Rows+and+Columns+in+Jython
[32]: http://docs.aspose.com/display/cellsjava/Grouping+and+Ungrouping+Rows+and+Columns+in+Jython
[33]: http://docs.aspose.com/display/cellsjava/Adjusting+Row+Height+and+Column+Width+in+Jython
[34]: http://docs.aspose.com/display/cellsjava/Autofit+Rows+and+Columns+in+Jython
[35]: http://docs.aspose.com/display/cellsjava/Copying+Rows+and+Columns+in+Jython
[36]: http://docs.aspose.com/display/cellsjava/Aspose.Cells+Java+For+Jython
[37]: https://id.containerize.com/signup?clientId=prod.discourse.aspose&redirectUrl=https://forum.aspose.com/session/sso





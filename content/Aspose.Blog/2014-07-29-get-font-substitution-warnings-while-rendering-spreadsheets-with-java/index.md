---
title: 'Get Font Substitution Warnings while Rendering Spreadsheets with Java'
date: Tue, 29 Jul 2014 10:38:45 +0000
draft: false
url: /2014/07/29/get-font-substitution-warnings-while-rendering-spreadsheets-with-java/
author: Babar Raza
summary: ''
tags: ['Aspose.Cells', 'Babar Raza', 'Convert Spreadsheets to PDF', 'Excel APIs', 'Font Substitution', 'Java APIs', 'PDF rendering', 'Rendering Excel files']
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/aspose-Cells-for-Java_100.png" alt="Aspose.Cells for Java">}}


We have just released this month’s improvements to [Aspose.Cells for Java][1] and upgraded the API to version 8.1.2. This release contains 25 improvements, including the showcased feature discussed below. You can download the latest Aspose.Cells for Java release from the [download section][2] now, and start exploring the new features. However, if you are planning to upgrade your project to use the latest build, we recommend you to check the Public API Changes section first.

Here is a look at just a few of the biggest features in this month’s release. For a full list of bug fixes and improvements please refer to the download page in the link above.

## Getting Warnings for Font Substitution

Aspose.Cells APIs use TrueType Fonts (TTFs) when a task involves rendering spreadsheets to images or portable formats such as PDF. Aspose.Cells detects which TTFs are required by scanning the spreadsheet styles and tries to find the required fonts on the machine where conversion is taking place. There could be situations when the required TTFs are not available. In such cases, Aspose.Cells substitutes the required font with a similar available one.

With this release, Aspose.Cells provides the means to receive warnings if a font substitution has occurred during the spreadsheet rendering process. This mechanism is available through a set of classes, interfaces and properties that have been added with version 8.1.2.

This is how you may use the latest API to Get Warnings for Font Substitution:

```
public class WarningCallback implements IWarningCallback 
{
    @Override
    public void warning(WarningInfo info) {
        if(info.getWarningType() == WarningType.FONT_SUBSTITUTION)
        {
            System.out.println("WARNING INFO: " + info.getDescription());
        }
    }
}

static void Run() throws Exception
{
    Workbook workbook = new Workbook("source.xlsx");
    PdfSaveOptions options = new PdfSaveOptions();
    options.setWarningCallback(new WarningCallback());
    workbook.save("output.pdf", options);
} 
```

## Bug Fixes

Aspose.Cells for Java 8.1.2 provides fixes for several important issues by enhancing its core. A few fixes worth mentioning are listed below.

*   Improved the HTML rendering engine to fix several issues related to the embedded image format type, hidden columns & chart rendering.
*   Improved the image quality for the PDF rendering engine.
*   Fixed issues related to charts in spreadsheets in reference to the label displacement & properties getting altered or removed.
*   Improved exception handling to tackle corrupted spreadsheets.

As always we appreciate your feedback so if you ever have anything to tell us about this release or anything else, please head to the [Aspose.Cells support forum][3] for a chat.




[1]: https://products.aspose.com/cells/java
[2]: https://downloads.aspose.com/cells/java
[3]: https://forum.aspose.com/





---
title: 'Set the Direction of Text in Shapes &amp; Enhancements to the HtmlLoadOptions in Aspose.Cells for Android 8.0.0'
date: Tue, 27 May 2014 10:40:26 +0000
draft: false
url: /2014/05/27/set-the-direction-of-text-in-shapes-enhancements-to-the-htmlloadoptions-in-aspose.cells-for-android-8.0.0/
author: Amjad Sahi
summary: ''
tags: []
categories: ['Aspose.Cells Product Family']
---

[![Aspose.Cells for Android logo][1]](https://blog.aspose.com/wp-content/uploads/sites/2/2014/06/aspose-Cells-for-Android_100.png)We are pleased to announce the release of Aspose.Cells for Android 8.0.0 with new features, enhancements and bug fixes.

There are some valuable features in this month’s release. For a full list of bug fixes and other improvements please refer to the [download page][2].

## Set the Direction of Text in Shapes

Aspose.Cells for Android 8.0.2 provides getter & setter attributes for the TextDirection method in the Shape class. The API now lets developers control the direction of the text in shapes including the spreadsheet comments. The setTextDirection method accepts a value from the constants TextDirectionType, and applies the text direction as one of the following:

*   Left to Right
*   Right to Left
*   Context

## Enhancements to the HtmlLoadOptions Class

Another notable enhancement has been made to the HtmlLoadOptions class by exposing the Boolean ConvertFormulasData attribute. Setting this property to true when using the setConvertFormulasData method allows the API to interpret any string value starting with character “=” as a formula.

This is how you can use the property.

```
//Create an instance of HTMLLoadOptions
HTMLLoadOptions load = new HTMLLoadOptions();

//Set ConvertFormulasData to true
load.setConvertFormulasData(true);

//Load a spreadsheet to be converted
Workbook book = new Workbook(sdDir + "/Book1.html", load); 
```

Please note the default value of ConvertFormulasData is false.

## Other Enhancements and Fixes

Aspose.Cells for Android 8.0.2 has provided fixes for several important issues, such as rendering & manipulating charts, converting Excel to PDF format and rendering and manipulating PivotTables.

To see a complete list of enhancements and fixes and to download Aspose.Cells for Android 8.0.0, please visit the [download page][3].




[1]: https://blog.aspose.com/wp-content/uploads/sites/2/2014/06/aspose-Cells-for-Android_100.png "Aspose.Cells for Android logo"
[2]: http://www.aspose.com/community/files/74/android-components/aspose.cells-for-android/entry548060.aspx
[3]: http://www.aspose.com/community/files/74/android-components/aspose.cells-for-android/entry548060.aspx





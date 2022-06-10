---
title: 'Get Font Substitution Warnings while Rendering Spreadsheets in Android'
date: Fri, 08 Aug 2014 15:35:21 +0000
draft: false
url: /2014/08/08/get-font-substitution-warnings-while-rendering-spreadsheets-with-aspose.cells-for-android-8.1.2/
author: Amjad Sahi
summary: ''
tags: []
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/aspose-Cells-for-Android_100.png" alt="Aspose.Cells for Android logo">}}


We are pleased to announce the release of [Aspose.Cells for Android][1] 8.1.2. The new version contains many useful enhancements.  It also includes several fixes and other improvements. Below, we list the major features and enhancements in this month’s release.

## Getting Warnings for Font Substitution

Aspose.Cells APIs generally use TrueType Fonts (TTFs) when a task involves rendering spreadsheets to images or portable formats such as PDF. Aspose.Cells detects which TTFs are required by scanning the spreadsheet styles and tries to find the required fonts on the machine where conversion is taking place. There could be situations when the required TTFs are not available. In such cases, Aspose.Cells substitutes the required font with a similar available one.

With this release, Aspose.Cells provides the means to receive warnings if a font substitution has occurred during the spreadsheet rendering process. This mechanism is available through a set of classes, interfaces and properties that have been added with version 8.1.2.

```
public class WarningCallback implements IWarningCallback {

    @Override
    public void warning(WarningInfo info) {
        if(info.getWarningType() == WarningType.FONT_SUBSTITUTION)
        {
            System.out.println("WARNING INFO: " + info.getDescription());
        }
    }
}

//........MainActivity.java........
//.................................

import java.io.File;

import android.app.Activity;
import android.os.Bundle;
import android.os.Environment;
import android.view.Menu;

import com.aspose.cells.CellsHelper;
import com.aspose.cells.IWarningCallback;
import com.aspose.cells.PdfSaveOptions;
import com.aspose.cells.WarningInfo;
import com.aspose.cells.WarningType;
import com.aspose.cells.Workbook;

public class MainActivity extends Activity {

	@Override
	protected void onCreate(Bundle savedInstanceState) {
		super.onCreate(savedInstanceState);
		setContentView(R.layout.activity_main);

try{

//Specify the fonts path directory
String sdCardPath = Environment.getExternalStorageDirectory().getPath()+ File.separator;
CellsHelper.setFontDir(sdCardPath + "fonts");

  Workbook workbook = new Workbook(sdCardPath + "source.xlsx");
  PdfSaveOptions options = new PdfSaveOptions();
  options.setWarningCallback(new WarningCallback());
  workbook.save(sdCardPath + "output.pdf", options);

}
		catch (Exception e)
		{
			e.printStackTrace();
		}
    } 
```

## Bug Fixes

Aspose.Cells for Android 8.1.2 has provided fixes and other enhancements for several important issues, such as, reading/writing Microsoft Excel files, manipulating styles and calculating formulas, manipulating charts and shapes, Sheet to image bugs, Smart Markers issue, etc.

To see a complete list of enhancements and fixes and to download Aspose.Cells for Android 8.1.2, please visit the [download page][2].




[1]: https://products.aspose.com/cells/android-java
[2]: https://downloads.aspose.com/cells/android-java





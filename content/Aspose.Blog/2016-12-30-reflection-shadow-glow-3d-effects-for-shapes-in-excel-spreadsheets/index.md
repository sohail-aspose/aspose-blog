---
title: 'Support for Reflection, Shadow, Glow and 3D Effects for Shapes in Excel Spreadsheets'
date: Fri, 30 Dec 2016 10:38:37 +0000
draft: false
url: /2016/12/30/reflection-shadow-glow-3d-effects-for-shapes-in-excel-spreadsheets/
author: Babar Raza
summary: ''
tags: ['3d', 'API to Convert Spreadsheets', 'Create Spreadsheets', 'Custom Subtotal Labels', 'Excel APIs for Android', 'Filter Objects', 'Shadow', 'Shape Effects', 'charts', 'glow', 'reflection']
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/aspose-Cells-for-Android_100.png" alt="Aspose.Cells for Android logo">}}


We are pleased to announce the release of [Aspose.Cells for Android 16.12.0][1]. This release includes a number of new features, enhancements and bug fixes that further improve the overall stability and usability of the API. Please check the [release notes][2] in order to get an idea about what is new and what has been fixed with this revision of Aspose.Cells for Android. If you are planning to upgrade the API from any previous version, we strongly suggest you to check the [Public API Changes][3] section to know what has been changed since your current revision of the API.

While you are downloading the latest build, here is a look at the most worth mentioning features in this release.

## Create Custom Subtotal Labels using Java

Aspose.Cells for Android 16.12.0 has added the support for the creation of custom subtotal labels allowing the application developers to customize the labels according to the region or personal preferences. In order to provide this feature, the latest version of the Aspose.Cells for Android has exposed the GlobalizationSettings class offering the following 2 methods which can be overridden in a custom class to get desired labels for the Subtotals.

*   GlobalizationSettings.getTotalName: Gets the total name of the function.
*   GlobalizationSettings.getGrandTotalName: Gets the grand total name of the function.

The GlobalizationSettings class can be used to customize the Subtotal labels by overriding the GlobalizationSettings.getTotalName & GlobalizationSettings.getGrandTotalName methods as demonstrated ahead.

```
public class CustomSettings extends GlobalizationSettings
{    
    public String getTotalName(int functionType)
    {
    	 switch (functionType)
         {
             case ConsolidationFunction.AVERAGE:
                 return "AVG";

             //Handle other cases

             default:
                return super.getTotalName(functionType);
         }
    }

    public String getGrandTotalName(int functionType)
    {
    	 switch (functionType)
         {
             case ConsolidationFunction.AVERAGE:
                 return "GRAND AVG";

             //Handle other cases

             default:
            	 return super.getGrandTotalName(functionType);
         }      
    }
} 
```

In order to inject custom labels, it is required to assign the WorkbookSettings.GlobalizationSettings property to an instance of the CustomSettings class defined above, before adding the Subtotals to the worksheet.

```
//Loads an existing spreadsheet containing some data
Workbook book = new Workbook(SD_PATH + "sample.xlsx");

//Assigns the GlobalizationSettings property of the WorkbookSettings class
//to the class created in first step
book.getSettings().setGlobalizationSettings(new CustomSettings());

//Accesses the 1st worksheet from the collection which contains data
//Data resides in the cell range A2:B9
Worksheet sheet = book.getWorksheets().get(0);

//Adds SubTotal of type Average to the worksheet
sheet.getCells().subtotal(CellArea.createCellArea("A2", "B9"), 0, ConsolidationFunction.AVERAGE, new int[] { 1 });

//Calculates Formulas
book.calculateFormula();

//Auto fits all columns
sheet.autoFitColumns();

//Saves the workbook on disc
book.save(SD_PATH + "output.xlsx");
```

## Render Custom Other Label for Pie Chart using Java

The GlobalizationSettings class also offers the getOtherName method which is useful to give the "Other" label of Pie charts a custom value. The following snippet defines a custom class and overrides the getOtherName method to get a custom label based on default language set for JVM.

```
public class CustomSettings extends GlobalizationSettings
{ 
    public String getOtherName()
    {
        String language = Locale.getDefault().getLanguage();
	System.out.println(language);
	switch (language)
	{
	    case "en":
	        return "Other";
	    case "fr":
	        return "Autre";
	    case "de":
	        return "Andere";

	    //Handle other cases as per requirement

	    default:
	        return super.getOtherName();
	}
    }
}
```

The following snippet loads an existing spreadsheet containing a Pie chart, and renders the chart to image while utilizing the CustomSettings class created above.

```
//Loads an existing spreadsheet containing a pie chart
Workbook book = new Workbook(SD_PATH + "sample.xlsx");

//Assigns the GlobalizationSettings property of the WorkbookSettings class
//to the class created in first step
book.getSettings().setGlobalizationSettings(new CustomSettings());

//Accesses the 1st worksheet from the collection which contains pie chart
Worksheet sheet = book.getWorksheets().get(0);

//Accesses the 1st chart from the collection
Chart chart = sheet.getCharts().get(0);

//Refreshes the chart
chart.calculate();

//Renders the chart to image
chart.toImage(SD_PATH + "output.png", new ImageOrPrintOptions());
```

Please check the detailed article on [Introduction to GlobalizationSettings Class][4] if you want to get more in-depth knowledge of the aforementioned usage scenarios.

## Improved Object Filtering for Loading Templates using Java

Sometimes, application requirement could be to load just a particular type of objects while loading existing spreadsheets in Aspose.Cells' object model. For instance, you may require to load only the cells along with formulas & formatting or just the document properties. Aspose.Cells APIs now provide a flexible yet comprehensive mechanism to achieve such requirements by exposing the LoadFilter class.

The LoadFilter class along with LoadOptions.LoadFilter property can control the type of data/objects to be loaded while initializing an instance of Workbook from a template file. The constructor of the LoadFilter class can accept constant(s) from the LoadDataFilterOptions enumeration, that specifies the type of objects to be loaded.

The LoadDataFilterOptions enumeration currently has the following constants.

*   LoadDataFilterOptions.ALL: Loads everything from the template file.
*   LoadDataFilterOptions.CELL\_BLANK: Loads the blank cells.
*   LoadDataFilterOptions.CELL\_BOOL: Loads the cells having value of type Boolean.
*   LoadDataFilterOptions.CELL\_DATA: Loads all cells data including values, formulas and formatting.
*   LoadDataFilterOptions.CELL\_ERROR: Loads cells whose value is error.
*   LoadDataFilterOptions.CELL\_NUMERIC: Loads the cells having value of type number/numeric.
*   LoadDataFilterOptions.CELL\_STRING: Loads the cells having value of type string/text.
*   LoadDataFilterOptions.CELL\_VALUE: Loads cells value regardless of the type.
*   LoadDataFilterOptions.CHART: Loads the charts.
*   LoadDataFilterOptions.CONDITIONAL\_FORMATTING: Loads conditional formatting rules.
*   LoadDataFilterOptions.DATA\_VALIDATION: Loads data validations.
*   LoadDataFilterOptions.DOCUMENT\_PROPERTIES: Loads document properties.
*   LoadDataFilterOptions.FORMULA: Load formulas including defined Names.
*   LoadDataFilterOptions.MERGED\_AREA: Loads merged cells.
*   LoadDataFilterOptions.NONE: Loads nothing.
*   LoadDataFilterOptions.PIVOT\_TABLE: Loads Pivot Tables.
*   LoadDataFilterOptions.SETTINGS: Loads settings for workbook and worksheet.
*   LoadDataFilterOptions.SHAPE: Loads all types of shapes.
*   LoadDataFilterOptions.STYLE: Loads styles for cell formatting.
*   LoadDataFilterOptions.TABLE: Loads List Objects/Tables.

Here is a simple snippet to load only the document properties from a template file.

```
//Create an instance of LoadOptions class
LoadOptions options = new LoadOptions();

//Create an instance of LoadFilter class
//Select to load document properties by passing LoadDataFilterOptions.DocumentProperties to constructor
LoadFilter filter = new LoadFilter(LoadDataFilterOptions.DOCUMENT_PROPERTIES);

//Set the LoadFilter property of LoadOptions object to the instance of LoadFilter class created above
options.setLoadFilter(filter);

//Load a template file by passing file path as well as instance of LoadOptions class
Workbook book = new Workbook(SD_PATH + "sample.xlsx", options); 
```

Following snippet loads everything from an existing spreadsheet except for the charts.

```
//Create an instance of LoadOptions class
LoadOptions options = new LoadOptions();

//Create an instance of LoadFilter class
//Select to load document properties by passing parameter to the constructor
LoadFilter filter = new LoadFilter(LoadDataFilterOptions.ALL & ~LoadDataFilterOptions.CHART);

//Set the LoadFilter property of LoadOptions object to the instance of LoadFilter class created above
options.setLoadFilter(filter);

//Load a template file by passing file path as well as instance of LoadOptions class
Workbook book = new Workbook(SD_PATH + "sample.xlsx", options); 
```

The code snippet ahead loads only the cell values along with the formulas and formatting.

```
//Create an instance of LoadOptions class
LoadOptions options = new LoadOptions();

//Create an instance of LoadFilter class
//Select to load document properties by passing parameter to the constructor
LoadFilter filter = new LoadFilter(LoadDataFilterOptions.CELL_DATA);

//Set the LoadFilter property of LoadOptions object to the instance of LoadFilter class created above
options.setLoadFilter(filter);

//Load a template file by passing file path as well as instance of LoadOptions class
Workbook book = new Workbook(SD_PATH + "sample.xlsx", options); 
```

Please check detailed article on [Filtering Objects at Load Time][5] if you want to get more in-depth knowledge of aforementioned usage scenarios.

## Support for Reflection Effects

Aspose.Cells for Android 16.12.0 has added the support for reflection effects for a Shape object as Excel provides it via Effects tab under Format Shape dialog as shown below.



{{< figure align=center src="images/reflection-effect-of-shape1.png" alt="">}}


In order to provide the said feature, Aspose.Cells for Android 16.12.0 has exposed the ReflectionEffect class along with Shape.Reflection property which together controls the reflection effects of a Shape object.

Here is a simple usage scenario of newly exposed APIs to apply reflection on an existing shape.

```
//Load a sample spreadsheet containing a shape
//Alternatively create a new spreadsheet and add a shape
Workbook book = new Workbook(SD_PATH + "sample.xlsx");

//Access first worksheet from the collection
Worksheet sheet = book.getWorksheets().get(0);

//Access first shape from the collection
Shape shape = sheet.getShapes().get(0);

//Get the instance of ReflectionEffect from the Shape object
ReflectionEffect reflection = shape.getReflection();
//Set its Blur, Size, Transparency and Distance properties
reflection.setBlur(30);
reflection.setSize(90);
reflection.setTransparency(0.5);
reflection.setDistance(80);

//Save the result in XLSX format
book.save(SD_PATH + "output.xlsx");
```

## Support for Shadow Effects

Aspose.Cells for Android 16.12.0 has added the support for Shadow Effects for a Shape object as Excel provides it via Effects tab under Format Shape dialog as shown below.



{{< figure align=center src="images/shadow-effect-of-shape.png" alt="">}}


Aspose.Cells for Android 16.12.0 has exposed the Shape.ShadowEffect property along with ShadowEffect class which together allows to set the shadow effect on a Shape object.

Here is a simple usage scenario of newly exposed APIs to apply shadow on an existing shape.

```
//Load a sample spreadsheet containing a shape
//Alternatively create a new spreadsheet and add a shape
Workbook book = new Workbook(SD_PATH + "sample.xlsx");

//Access first worksheet from the collection
Worksheet sheet = book.getWorksheets().get(0);

//Access first shape from the collection
Shape shape = sheet.getShapes().get(0);

//Get the instance of ShadowEffect from the Shape object
ShadowEffect shadow = shape.getShadowEffect();
//Set its Angle, Blur, Size, Transparency and Distance properties
shadow.setAngle(150);
shadow.setBlur(30);
shadow.setSize(90);
shadow.setTransparency(0.5);
shadow.setDistance(80);

//Save the result in XLSX format
book.save(SD_PATH + "output.xlsx");
```

## Support for Glow Effects

Aspose.Cells for Android now supports the Glow Effects for a Shape object as Excel provides it via Effects tab under Format Shape dialog as shown below.



{{< figure align=center src="images/glow-effect-of-shape.png" alt="">}}


Aspose.Cells for Android 16.12.0 has exposed the Shape.Glow property along with GlowEffect class which together allows to set the glow effect on a Shape object.

Here is a simple usage scenario of newly exposed APIs to apply glow effect on an existing shape.

```
//Load a sample spreadsheet containing a shape
//Alternatively create a new spreadsheet and add a shape
Workbook book = new Workbook(SD_PATH + "sample.xlsx");

//Access first worksheet from the collection
Worksheet sheet = book.getWorksheets().get(0);

//Access first shape from the collection
Shape shape = sheet.getShapes().get(0);

//Get the instance of GlowEffect from the Shape object
GlowEffect glow = shape.getGlow();
//Set its Size & Transparency properties
glow.setSize(90);
glow.setTransparency(0.5);

//Save the result in XLSX format
book.save(SD_PATH + "output.xlsx");
```

## Support for 3-D Formats

Aspose.Cells for Android supports the 3-D Formats for Shape objects as Excel provides it via Effects tab under Format Shape dialog as shown below.



{{< figure align=center src="images/ThreeDformat-of-shape.png" alt="">}}


Aspose.Cells for Android 16.12.0 has exposed the Shape.ThreeDFormat property along with ThreeDFormat class which together allows to set the 3D formatting for a Shape object.

Here is a simple usage scenario of newly exposed APIs to apply 3D formatting on an existing shape.

```
//Load a sample spreadsheet containing a shape
//Alternatively create a new spreadsheet and add a shape
Workbook book = new Workbook(SD_PATH + "sample.xlsx");

//Access first worksheet from the collection
Worksheet sheet = book.getWorksheets().get(0);

//Access first shape from the collection
Shape shape = sheet.getShapes().get(0);

//Get the instance of ThreeDFormat from the Shape object
ThreeDFormat threeD = shape.getThreeDFormat();
//Set its ContourWidth & ExtrusionHeight properties
threeD.setContourWidth(15);
threeD.setExtrusionHeight(30);

//Save the result in XLSX format
book.save(SD_PATH + "output.xlsx");
```

## Support for WordArt Built-in Styles

Aspose.Cells for Android APIs now support to add WordArt objects with built-in styles. In order to provide this feature, the Aspose.Cells for Android 16.12.0 has exposed the ShapeCollection.AddWordArt method along with PresetWordArtStyle enumeration which together allows to add preset WordArt objects since Excel 2007.

Here is a simple usage scenario of newly exposed APIs to add WordArt with build-in styles.

```
//Create an instance of Workbook
Workbook book = new Workbook();

//Access first worksheet from the collection
Worksheet sheet = book.getWorksheets().get(0);

//Access ShapeCollection of first worksheet
ShapeCollection shapes = sheet.getShapes();

//Add WordArt with built-in styles
shapes.addWordArt(PresetWordArtStyle.WORD_ART_STYLE_1, "Aspose File Format APIs", 00, 0, 0, 0, 100, 800);
shapes.addWordArt(PresetWordArtStyle.WORD_ART_STYLE_2, "Aspose File Format APIs", 10, 0, 0, 0, 100, 800);
shapes.addWordArt(PresetWordArtStyle.WORD_ART_STYLE_3, "Aspose File Format APIs", 20, 0, 0, 0, 100, 800);
shapes.addWordArt(PresetWordArtStyle.WORD_ART_STYLE_4, "Aspose File Format APIs", 30, 0, 0, 0, 100, 800);
shapes.addWordArt(PresetWordArtStyle.WORD_ART_STYLE_5, "Aspose File Format APIs", 40, 0, 0, 0, 100, 800);

//Save the result in XLSX format
book.save(SD_PATH + "output.xlsx");
```

## Other Enhancements & Fixes

Aspose.Cells for Android 16.12.0 has fixed a few critical bugs as well as enhanced its core for more stability. A few of the worth mentioning enhancements are as follows.

*   This release has exposed the ListColumn.Formula property in order to automatically propagate the formula to next rows of a List Object.
*   The Aspose.Cells APIs can be used to insert XML Map to Workbook or export XML Map from Workbook.
*   Aspose.Cells for Android API has exposed the Workbook.AbsolutePath property with this release. This property can be used to change the path of the external data sources.
*   Aspose.Cells APIs have exposed the FontSettingCollection.setWordArtStyle & FontSetting.setWordArtStyle methods in order to set the preset WordArt style to the text of the Shape object.
*   Aspose.Cells APIs have provided the ability to link the cells to XML Map elements by exposing the Cells.LinkToXmlMap method.
*   Aspose.Cells APIs have exposed the ExternalLink.IsVisible property to check if the external link is visible in Excel interface or not.




[1]: http://downloads.aspose.com/cells/android/new-releases/aspose.cells-for-android-16.12.0/
[2]: https://docs.aspose.com/cells/java/aspose-cells-for-android-via-java/
[3]: https://docs.aspose.com/cells/java/aspose-cells-for-android-via-java/
[4]: https://docs.aspose.com/cells/androidjava/
[5]: https://docs.aspose.com/cells/androidjava/





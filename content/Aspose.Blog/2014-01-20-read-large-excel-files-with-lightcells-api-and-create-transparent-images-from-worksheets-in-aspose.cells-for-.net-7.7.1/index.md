---
title: 'Read Large Excel Files with LightCells API and Create Transparent Images from Worksheets in Aspose.Cells for .NET 7.7.1'
date: Mon, 20 Jan 2014 14:08:29 +0000
draft: false
url: /2014/01/20/read-large-excel-files-with-lightcells-api-and-create-transparent-images-from-worksheets-in-aspose.cells-for-.net-7.7.1/
author: Amjad Sahi
summary: ''
tags: ['Convert Excel worksheet to transparent image', 'Smart Markers', 'manipulate PivotTables', 'render images files from Charts', 'rendering Charts']
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/aspose-Cells-for-net_100.png" alt="Aspose.Cells for .NET logo">}}


Aspose.Cells for .NET 7.7.1 has been released with over 80 useful new features, enhancements and bug fixes. This new release supports [reading large Excel files with LightCells API][1]. This is a useful feature. Sometimes you need to read data from a huge Microsoft Excel workbook with  millions of records and you always worry about the performance. You want it to take less time and memory to process big files. The LightCells API is useful in that scenario: to read huge Excel spreadsheets, it uses less memory, so you get better performance and efficiency.

The following sample code shows how to load an Excel file in light-weight mode. The sample code reads a big file and retrieves the total number of cells, a count of strings and a count of formulas for each worksheet in the workbook.

```
 static void Main(string[] args)
        {
            LoadOptions opts = new LoadOptions();
            LightCellsDataHandlerVisitCells v = new LightCellsDataHandlerVisitCells();
            opts.LightCellsDataHandler = v;
            Workbook wb = new Workbook("LargeBook1.xlsx", opts);
            int sheetCount = wb.Worksheets.Count;
            Console.WriteLine("Total sheets: " + sheetCount + ", cells: " + v.CellCount
                + ", strings: " + v.StringCount + ", formulas: " + v.FormulaCount);
        }

    class LightCellsDataHandlerVisitCells : LightCellsDataHandler
        {
            private int cellCount;
            private int formulaCount;
            private int stringCount;

            internal LightCellsDataHandlerVisitCells()
            {
                cellCount = 0;
                formulaCount = 0;
                stringCount = 0;
            }

            public int CellCount
            {
                get { return cellCount; }
            }

            public int FormulaCount
            {
                get { return formulaCount; }
            }

            public int StringCount
            {
                get { return stringCount; }
            }

            public bool StartSheet(Worksheet sheet)
            {
                Console.WriteLine("Processing sheet[" + sheet.Name + "]");
                return true;
            }

            public bool StartRow(int rowIndex)
            {
                return true;
            }

            public bool ProcessRow(Row row)
            {
                return true;
            }

            public bool StartCell(int column)
            {
                return true;
            }

            public bool ProcessCell(Cell cell)
            {
                cellCount++;
                if (cell.IsFormula)
                {
                    formulaCount++;
                }
                else if (cell.Type == CellValueType.IsString)
                {
                    stringCount++;
                }
                return false;
            }
        } 
```

## Finding Cells Based on Formatting

Another valuable feature is to [find the cells with some particular style or formatting][2]. Aspose.Cells supports finding all cells that have a common style or formatting. Aspose.Cells provides the FindOptions.Style property that you can use to specify the style to search cells for.

## Transparent Images

You can now create transparent images of Microsoft Excel worksheet. Sometimes, you need to generate an image of your worksheet as a transparent image. For example, you might want to apply transparency to all the cells which have no fill color. Aspose.Cells provides the ImageOrPrintOptions.Transparent property which applies transparency to a  worksheet image. When this property is false, then the cells with no fill color are drawn with white background, and when it is true, cells with no fill color are rendered transparent.

## Several Enhancements and Fixes

In this version, we have refactored the PivotTables module. We've made tremendous enhancements and fixed several issues.

Several important issues and other enhancements have been addressed in this release as well. For example, issues around reading and writing Microsoft Excel file formats, [manipulating conditional formatting][3], [rendering and manipulating pivot tables][4], [rendering images from Excel worksheets][5], reading and writing HTML files, rendering shapes and controls, [Smart Markers][6], manipulating embedded OLE objects, rendering and manipulating charts, [rendering images files from charts][7] and exporting Excel workbooks to PDF format have been resolved. A few improvements are also made pertaining to the formula calculation engine of Aspose.Cells for .NET, it now supports the BITAND  function (Microsoft Excel 2013).

We have also made a few enhancements in the grid suite provided by Aspose.Cells for .NET. Now, you can import or load bigger Excel files.

To see a complete list of enhancements and fixes, and to download Aspose.Cells for .NET 7.7.1, please visit the [download page][8].




[1]: https://docs.aspose.com/display/cellsnet/Using+LightCells+API
[2]: https://docs.aspose.com/display/cellsnet/Find+cells+with+specific+style
[3]: https://docs.aspose.com/display/cellsnet/Home
[4]: https://docs.aspose.com/display/cellsnet/Home
[5]: http://docs.aspose.com/display/cellsnet/Converting+Worksheet+to+Image
[6]: http://docs.aspose.com/display/cellsnet/Smart+Markers
[7]: https://docs.aspose.com/display/cellsnet/Home
[8]: https://downloads.aspose.com/cells/net





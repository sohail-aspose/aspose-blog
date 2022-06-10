---
title: 'Aspose.Total for Java Q1 2009'
date: Fri, 27 Mar 2009 15:51:00 +0000
draft: false
url: /2009/03/27/aspose-total-for-java-q1-2009/
author: Muhammad Rashid
summary: ''
tags: []
categories: ['Aspose.Total Product Family']
---

**What’s New in Aspose.Total for Java Q1 2009:**

**Aspose.Words for Java**

_New Features_

1. Only one key to preserve Metafiles in output document: SaveOptions.setHtmlExportMetafileAsRaster(false).

2. Workaround for old IBM (1.4) JIT JMM bug.

_Bug Fixes_

1. Borders around pictures in the template document cause “XmlStreamException” while saving to HTML format.

2. The document with cropped metafiles causes UnsupportedOperationException while converting from DOC to HTML.

3. The document with broken ticks (DataTime) number in Comments, etc. causes FileCorruptedException upon opening.

4. Null 'Author' and 'Initial' fields cause a NullPointerException during document save.

5. Track change disappears after open/save document using Aspose.Words.

**Aspose.Cells for Java**

_New Features_

1. Supports to Read and Write Open Document Spreadsheet file(ODS): Cell data and style, Row/Column style, Merged Cells, Worksheet/Workbook properties, Document properties, Formula/Name.

2. Supports setting shared formula.

3. Supports manipulating controls: Check box, Button, Radio button, Combo box, List box, Group box, Scroll bar, spinner, Label.

4. Supports Page setup Header(s) and Footer(s) in xls2pdf.

5. Allows copying Chart when copying Worksheet/Workbook.

6. Supports copying Shape related objects.

7. Supports saving worksheet as html to stream.

8. Supports PivotChart.

9. Supports getting image data of Picture and OleObject.

10. Supports reading and writing Color theme for 2007 file format.

11. Supports Encryption type: Microsoft Strong Cryptographic Provider.

_Bug Fixes_

1. NullPointerException in Cell.getPrecedents.

2. Support removing ASeries from NSeries collection.

3. Bug while saving Hyperlinks for Excel2007 format.

4. Bug in SUMIF formula.

5. Issues of formula: #VALUE returned by ROUND, #N/A returned by VLOOKUP.

6. PivotChart's DataLabels setting such as border and area lost.

7. Sets property of OleObject: OleSize.

8. Creates AutoFilter.

9. Saves FillFormat of Area in Chart.

10. Truncates cells that exceed row/column limit of Excel2003 file format.

11. Inserts more than 65k rows.

12. Moves formula when inserting Row/Column.

13. Sets color of ASeries’ Area in Chart.

14. Checks datasource when creating PivotTabel.

15. Sets bool value for Shape's properties.

16. Converts numeric text to number for SmartMarker.

17. Sets active cell of Worksheet.

18. Loses some properties of Chart when reading it from template file.

19. ASeries changed improperly after inserting/deleting columns/rows.

20. PageSetup.setFitToPagesTall/setFitToPagesWide.

21. Saves Excel2007 file for Mac OS.

**Aspose.Slides for Java**

_New Features_

1. Ported latest PPTX updates from .NET version of Aspose.Slides.

2. Additional optimization of PPT format reading and writing.

3. Improved rendering of autoshapes.

_Bug Fixes_

1. Table.deleteColumn() IndexOutOfBoundsException occurs when delete last column.

2. Slide.getBackground() returns null on slides with empty background created in MS PowerPoint 2007.

3. NullPointerException occurs when try to read properties of corrupt shapes.

4. Added support for names of master slides.

5. Added support for presentation level tags.

6. Presentation.write()IndexOutOfBoundsException occurs.

7. PptReadException occurs when read TextFrame with more than 64k characters.

8. Added support for new PowerPoint 2007 gradients.

9. ShadowFormat.ShadowColor and ShadowFormat.LightColor return and set wrong color values.

10. Color opacity in FillFormat and LineFormat return wrong value because of incorrect rounding.

11. IndexOutOfBoundsException occurs when read and write Notched Right Arrow autoshape.

12. FitTextToShape doesn’t change space between lines.

13. Grouped autoshapes can be scaled after slide cloning.

**Aspose.Pdf.Kit for Java**

_New Features_

1. Some new methods are added in PdfFileStamp class to support adding header/footer/page number.

2. New method removeFieldAction is added into FormEditor which can be used to delete unsafe script from PDF.

3. A new method setFieldAlignment is also added into FormEditor to support setting alignment for field.

4. Signing PDF for multiple times is now supported.

_Bug Fixes_

1. The PdfExtractor is improved to support more powerful attachment extracting feature.

**Aspose.Metafiles for Java**

_New Features_

1. Added possibility to extract all images embedded in a metafile.

_Bug Fixes_

1. Shapes are not filled with gradient background.

2. Missing text when WMF metafile is rendered.

3. Arc based shapes with angle < 1 degree are not rendered properly.

4. Shapes filled with wrong color.

5. Japanese and other MBCS character sets are rendered as boxes instead of characters.

6. Characters of Japanese and other MBCS character sets can be overlapped.

7. NegativeArraySizeException is thrown in case WMF metafile has broken header with negative metafile dimensions.

**Download Aspose.Total for Java:**

[http://www.aspose.com/community/files/50/product-suites/aspose.total/category1200.aspx][1]




[1]: http://www.aspose.com/community/files/50/product-suites/aspose.total/category1200.aspx





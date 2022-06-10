---
title: 'Aspose.Total Product Family Q3 2010 Releases'
date: Thu, 30 Sep 2010 16:53:00 +0000
draft: false
url: /2010/09/30/aspose-total-product-family-q3-2010-releases/
author: Muhammad Rashid
summary: ''
tags: []
categories: ['Aspose.Total Product Family']
---

Aspose is proud to announce the Q3 releases of its Aspose.Total family of products. The Q3 2010 releases of Aspose.Total include several new features and updates for all product lines to help developers in building more reliable and robust solutions with less effort.

**What’s New in Aspose.Total for .NET Q3 2010:  **

**Aspose.Words for .NET**

_New Features_

1.  Support Structured Document Tags (SDT) (Content Controls)
2.  Support OOXML Diagrams and Charts
3.  Images are missed from document after open/save DOCX document.
4.  SmartArt (DrawingML) objects are missed from document after open/save.
5.  Support OpenType PostScript fonts in rendering
6.  Text in text frames loose positioning when exported to PDF.
7.  Add an option to embed full font into PDF and XPS instead of embedding subset.
8.  Implement embedding of OpenType PostScript fonts as Type 1 fonts into PDF
9.  Allow specifying Color Depth during converting document to Image.
10.  Join spans with same formatting in HTML export
11.  Document Outline should include automatic numbers
12.  Hyperlink inside a TOC field (table of contents) should ignore the Hyperlink character style
13.  Breaks in DOC and DOCX should be processed in different ways.
14.  "Arial Bold" font is specified in the document, but rendered as Times New Roman
15.  Support "split apart page break and paragraph mark" compatibility option.
16.  Render endnotes
17.  Add support of MERGEFIELD formatting switches.
18.  Allow public access to list numbers
19.  Allow format strings in any culture
20.  Support nested XE fields
21.  After open/save CommandButton lose its functionality.
22.  Top spacing on the second page appears bigger then on the first page during rendering.
23.  Provide a method to verify that a digital signature is present on a DOC file
24.  Split Aspose.Words documentation into two sets one for Java and one for .NET
25.  Provide a method to verify that a digital signature is present on a DOCX file.
26.  Page number in the header disappears during rendering. - pgNum not supported
27.  Verify if digital signature on a document is present
28.  Implement dependency of border width on border style in HTML export
29.  Improve export of legacy lists to HTML
30.  Render footnotes
31.  Condensed font is not condensed in layout.
32.  The Document.BackgroundColor property.
33.  Support IncludeText field.
34.  Allow detecting whether the loaded document is a template.
35.  Follow the Unified pattern for Document loading and save
36.  Change all events into interfaces
37.  Provide a method to verify that a digital signature is present on a ODT file.
38.  Saving to TIFF CCITT compression makes documents hard to read
39.  “Black and White” image option is ignored upon rendering and converting to PDF.

_Bug Fixes_

1.  Update all code examples and documentation so it is up to date with the new public API.
2.  Write a documentation topic that lists all the breaking changes in the new API and simple instructions for customers to fix their code.
3.  Reflect that legacy PDF conversion facility has been removed from AW.
4.  Implement new shortcut icons for the installer.
5.  Investigate if XPS supports full embedded OpenType PostScript fonts.
6.  Investigate how difficult it is to subset an OpenType PostScript font for XPS.
7.  Images are lost after the document is opened/saved.
8.  Saving the document to a client browser causes error on Win2003 64-bit.
9.  System.FormatException: Adler chksum doesn't match - when opening the file.
10.  Images are not read from DOC file.
11.  Font is changed after open/save DOT file.
12.  StackOverflowException occurs during loading document.
13.  FileCorruptedException occurs during loading.
14.  FileCorruptedException occurs during loading.
15.  InvalidCastException occurs during loading document.
16.  FileCorruptedException exception occurs upon opening document.
17.  EndOfStreamException occurs upon loading document.
18.  FileCorruptedException occurs during loading.
19.  FileCorruptedException occurs during loading.
20.  Add "how to use Aspose.Words in ColdFusion" article.
21.  Shape is lost when loading a DOCX.
22.  Bookmak which is a direct child of Body is missed upon loading.
23.  Some data that should be inside a table is displayed outside the table in ADE.
24.  IF fields conditions in Header/Footer do not work as expected upon rendering.
25.  Part of footer disappears during rendering.
26.  IF fields conditions do not work as expected.
27.  Incorrect formatting for TOC entry marked by style
28.  Number formatting is incorrect.
29.  Make font reading (of unused fonts) process silent.
30.  Some fonts are improperly rendered with the latest version of AW.
31.  Formatting set in DocumentBuilder is lost when processing fragment with InsertHtml.
32.  Html import takes long time if document consist of only one paragraph and lots of BR.
33.  List label appears at the previous page if it follows a PageBreak.
34.  Alignment of footnote is incorrect during rendering.
35.  Text is missed upon renderign if character scaling is zero.
36.  Number of pages is invisible after convertign to PDF.
37.  NullReferenceException occurs during rendering.
38.  Position of list item text is incorrect after rendering.
39.  Position of right aligned tab is incorrect upon rendering.
40.  Rendering document to pdf, fails during layout.
41.  InvalidCastException exception occurs upon executing mail merge.
42.  Number formating is incorect in German culture.
43.  “FileCorruptedException” exception occurs upon opening EML(MHTML) file.
44.  Multilevel list generated by Aspose.Words is displayed not properly in Word 2007.
45.  Formatting of border between tables cells is unexpected.
46.  CCITT3 compression for images is not working.
47.  Futura fonts are not embedded into PDF.
48.  The size of TextInputs is incorrect during rendering.
49.  DINOT fonts are not embedded into PDF.
50.  Horizontal lines made from text become larger when rendered.
51.  NullReferenceException occurs after UpdatePageLayout/UpdateFields.
52.  “Brush Script Std” font is changed to “MS Sans Serif” upon rendering.
53.  Grey text disappears during converting to image with TiffCompression.Ccitt3, Ccitt4.
54.  Trade Gothic font is changed to other font upon converting to PDF/XPS.
55.  Barcode font is changed during rendering.
56.  Consider supporting macintosh fonts durign rendering.
57.  List item text is moved right upon rendering.
58.  "neutradisp" font is changed upon rendering.
59.  UnsupportedFontFormatException occurs during converting to PDF/XPS.
60.  Extra gap appears between runs during rendering to image.
61.  Table layout is incorrect during rendering.
62.  Page Color is changed during rendering.
63.  UnsupportedFontFormatException occurs during converting to PDF/XPS.
64.  Table width is incorrect during rendering.
65.  FileCorruptedException occurs during loading.
66.  FileCorruptedException occurs during loading.
67.  Document.HasRevisions returns true, but document doesn’t contain revisions.
68.  UpdateFields method does not update some CustomDocumentProperties and DocVariebles.
69.  Shapes disappears after open/save document.
70.  InvalidCastException occurs during loading.
71.  ArrayIndexOutOfBoundsException occurs during saving to DOC.
72.  Chinese font defined in Theme is changed after open/save.
73.  AutoShape lines look incorrect after open/save.
74.  themeFontLang (Theme Font Languages) is not supported in DOCX.
75.  STYLEREF field shows error “Error! No text of specified style in document.” in the output PDF document.
76.  Nested IF field is not evaluated.
77.  SUM(ABOVE) is calculated improperly if there is merged cells.
78.  IF filed condition is not updated during MailMerge.
79.  Additional item are displayed in the TOC after updatgin using AW.
80.  Cross-refferences in TOC are broken after updating.
81.  Numbering of TOC is incorrect after updating.
82.  Text in an ellipse is placed incorrectly
83.  Invisible borders are shown as gray borders. Rendering/PDF.
84.  Character spacing is ignored during rendering converting to PDF.
85.  Paragraph marks and line height became different.
86.  PageBreak and SectionBreakOddPage at the end of the same page produces two empty pages in PDF.
87.  A small difference in pagination location causes big difference on a large file.
88.  Child region is untouched if it is inside IF field.
89.  IndexOutOfRange exception occurs during MailMerge.
90.  Mergefields TableStart/TableEnd should be ignored during MailMerge.Execute.
91.  Font of mergefield is changed even if MERGEFORMAT switch is used.
92.  In WordML rectangle shapes can also have images.
93.  Format of date is not correct after updating fields.
94.  DetectFileFormat method returns “Doc” during checking XLS file.
95.  Font is changed from Times New Roman to Calibri after appending one document to another with KeepSourceFormatting option.
96.  Paragraph SpacingAfter is changed after appending document.
97.  Font is changing after appending to a document.
98.  Wrong font selected for rendering because themeFontLang (Theme Font Languages) is not supported.
99.  Image is placed incorrectly when converting DOC to ODT.
100.  Table fill color is lost when viewed in OpenOffice.
101.  Table row height is lost when converting DOC to ODT.
102.  Paragraph shading is lost when converting DOC to ODT.
103.  meta:value-type of user-defined properties is not preserved after open/save document using Aspose.Words.
104.  Font is changed upon converting document to PDF.
105.  Font “Humnst777 Blk BT” is rendered as normal “Humnst777 BT” during converting to PDF.
106.  Japanese text does not break to the next line in table cells during rendering/ converting to PDF.
107.  “Helvetica” fonts are changed to “Times New Roman” during rendering/converting to PDF.
108.  Output the original font name to PDF.
109.  Watermark image transparency is changed during rendering.
110.  Font is changed during converting to PDF.
111.  PDF produced by AW is corrupted if "Barcode 39HRtall" font is used.
112.  Text is clipped to almost invisible in small shapes.
113.  Table borders are lost at page break location.
114.  Width of Textboxes is less than needed.
115.  Page number style is changed from Roman to Arabic during Rendering / Converting to PDF.
116.  Font is changed from Calibri to Times New Roman after appending one document to another.
117.  Meta files are rendered incorrectly in PDF and XPS.
118.  Font is changed during rendering.
119.  Asian fonts are rendered in the wierd way.
120.  List item text is moved right upon rendering.
121.  “System.IndexOutOfRangeException: Index was outside the bounds of the array.” occurs during rendering.
122.  Position of CheckBox is incorrect after rendering.
123.  TestDefect18322 fails.
124.  Support nested TC and XE fields in RTF.
125.  Font is changed from Arial to Times New Romam during processing WML document using Aspose.Words.
126.  “Aspose.Words.FileCorruptedException: The document appears to be corrupted and cannot be loaded.” occurs during loading document.
127.  Shapes disapears upon importing WML document.
128.  Metafile is rendered incorrectly into XPS.
129.  Create UserDocsApiLinker utility.
130.  DEBT: Left and Right Indents for LTR vs RTL Paragraphs.
131.  Rework visiting of NodeRange.
132.  Delete old PDF conversion code.
133.  Use new templates for Demos.
134.  Make order of font declarations in OPF stable.
135.  Test ODT Export and Import.
136.  REF and PAGEREF fields are broken after open/save the document using Aspose.Words.
137.  Image is compressed horizontally upon rendering.
138.  “Aspose.Words.FileCorruptedException: The document appears to be corrupted and cannot be loaded.” occurs during opening.
139.  REF field loses its functionality after open/save document.
140.  FileCorruptedException occurs during loading.
141.  REF field values is not updated.
142.  Two items of TOC are lost after updating fields.
143.  UpdateFields with a TOC in a large document is slow.
144.  Souvienne font is rendered incorrectly.
145.  TestGoldHtmlFontResources.TestFontResourcesStreams Failed.
146.  InvalidOperationException occur upon opening large HTML document.
147.  No horizontal spacing in table cells before text.
148.  Using \[div\] in InsertHtml sets SpaceAfterAuto to true.
149.  Unnecessary gray area is shown at the top-left corner. Rendeing/Convertign to PDF.
150.  Text is displayed improperly in PDF and XPS.
151.  Inline shape in the document header pushes content of the document down upon rendering.
152.  Japanese characters look improperly after rendering to PDF and XPS.
153.  Part of content was cropped during rendering.
154.  Background turns to lilac while rendering.
155.  Header appears on the first page during rendering.
156.  Footnote layout code time grows exponentially.
157.  Document is truncated during layout.
158.  Document is rendered incorrectly into image\\PDF\\XPS.
159.  SmartTags are not removed when accept all revisions.
160.  REF to bookmark is not updated.
161.  “System.NullReferenceException: Object reference not set to an instance of an object.” occurs during rendering.
162.  Support Legacy List Formatting - Spaces after numbers in numbering list are incorrect.
163.  Bullet appears underlined during rendering.
164.  Unexpected behavior upon updating TOC if heading paragraphs contains pagebreaks.
165.  Textboxes are misplaced after open/save ODT document.
166.  One of the output ODT files in Excel2Word sample can't be opened.
167.  Table disappears after open/save ODT document.
168.  ODF Plugfest 20100415. Text color is changed during ODT to ODT conversion.
169.  ODF Plugfest 20100415. Tab positions get changed during ODT to ODT conversion.
170.  Graphics is displased when converting ODT to DOCX.
171.  Text background changes when converting ODT to DOCX.
172.  Document looks ugly when converted ODT to DOC.
173.  Document looks really ugly when converted ODT to DOC.
174.  ODF Plugfest 20090615. Numbering incorrect for 2nd numbered list in ODT 2 ODT.
175.  ODF Plugfest 20090615. Page margins are incorrect in ODT 2 ODT import.
176.  Paragraphs becomes with gray background after rendering/converting to PDF.
177.  “System.ArgumentException: Item has already been added. Key in dictionary: '” occurs during rendering to PDF and XPS.
178.  Shading should have no gaps between conforming paragraphs.
179.  Rendering of a barcode font does not work - renders normal text instead.
180.  Background color has been changed during converting to PDF and XPS.
181.  Paragraph borders are rendered improperly.
182.  Content of page and NUMPAGES field disappear upon rendering document.
183.  Lines are missed from Meta file during rendering.
184.  Meta file is cropped during rendering to PDF and XPS.
185.  Table cell border becomes double line upon rendering.
186.  “ArgumentOutOfRangeException: 'capacity' must be non-negative.” Exception occurs upon saving to XPS.
187.  Extra line has been added into the output document during rendering.
188.  “System.InvalidOperationException: Requested a name string that is not present in the font.” occurs during rendering.
189.  The header form the first page appears on the 3rd page.
190.  Position of footer is incorrect during rendering.
191.  GDI+ exception occurs during rendering.
192.  Table row is overlapped by paragraph with multiple 0.2 line spacing.
193.  Part of content is moved to the previous page during rendering in Windows 2003.
194.  Extra white spaces were added between words during rendering..
195.  Top margin is incorrect during rendering.
196.  Black rectangle appears in the left top corner of page during rendering.
197.  NullReferenceException occurs during rendering.
198.  Undefined characters are shown upon converting to PDF and XPS.
199.  Aspose.Words hangs during rendering.
200.  Part of table border disappears during rendering.
201.  Part of table content is truncated during rendering.
202.  Table is clipped upon rendering.
203.  TC fields are lost upon RTF import.
204.  BuiltInDocumentProperties.Version returns value of RevisionNumber when work with RTF document.
205.  XE fields are missed during loading RTF document.
206.  System.NullReferenceException occurs during rendering.
207.  “Not enough storage space is available to complete this operation” exception occurs during printing document using XpsPrintHelper.
208.  Transparent background is not rendered to XPS.
209.  Check XPS test on different display resolutions.

**Aspose.Cells for .NET**

_New Features_

1.      Includes Smart Tags support for XLSX files.

2.      Converts Sparklines to images.

3.      Provides support for image Smart Markers.

4.      Supports Cell’s gradient fills and theme of XLS file.

5.      Renders Cell’s pattern fills in the generated PDF file.

6.      Adds support for Pdf/A-1b compliance.

7.      Improves performance and quality of the generated PDF files.

8.      Converts hierarchical custom collections to Dataset which contain relations.

9.      Includes Scroll event.

10.  Provides an overloaded version for the SumSelectedRanges method to exclude hidden cells.

11.  Supports setting visibilities of context menu items.

12.  Provides support for text rotation (90 and -90 degrees).

13.  Supports firing CellDataChanged event when a formula is evaluated.

14.  Enhances the performance of saving PDF files.

15.  Supports clicking column header to select entire column, clicking top-left corner to select entire sheet’s cells similar to MS Excel’s behavior.

16.  Provides support for iterative calculations.

17.  Supports named ranges.

18.  Allows obtaining data field name at client side.

19.  Includes printing feature at client side.

20.  Adds valuable functions to the supported formulas list: CELL, ERROR.TYPE, ISBLANK, ISERROR, ISLOGICAL, ISNA, ISNONTEXT, ISTEXT, ISREF, N, NA, TYPE, COUNTBLANK, LARGE, MAXA, MINA, AVERAGEA, MODE, PERCENTILE, PERCENTRANK, RANK, CHOOSE, HLOOKUP, VLOOKUP.

21.  Allows undoing changes by code.

22.  Supports undoing changes of comments.

23.  Provides support to set visibilities of comments.

24.  Supports to set indent (style) while formatting cells.

25.  Imports or exports pictures of Excel files.

26.  Adds valuable functions to the supported formulas list: ERROR.TYPE, ISBLANK, ISERROR, ISLOGICAL, ISNA, ISNONTEXT, ISTEXT, ISREF, N, NA, TYPE, COUNTBLANK, LARGE, MAXA, MINA, AVERAGEA, MODE, PERCENTILE, PERCENTRANK, RANK, CHOOSE, HLOOKUP, OFFSET, INDIRECT.

_Bug Fixes_

1.            Borders are not rendered for the merged cells

2.            Changes the duplicate worksheet’s name in ImportExcelFile method

3.            Converts chart to image

4.            Data tables, Values and Category are lost for XY Scatter graphs

5.            Excel Chart to image problem

6.            Bubble charts

7.            Aspose.Cells throwing out of memory exceptions in Azure

8.            Export different to Excel's

9.            Find error saving PDF File

10.        One font in XLSX results in two fonts in PDF

11.        Currency formatted blank cells

12.        Issue of converting Excel to PDF

13.        Decimal values are not displayed if only zeroes are there

14.        Built In Properties

15.        Excel to PDF Conversion Issue

16.        Saving to PDF - Troubles with font

17.        PDF document appears to be corrupted

18.        Issue of saving PDF

19.        Calculated formulas not updating on conversion from Cells to PDF

20.        Conversion Issue with Data showing up as Number signs

21.        Calculated formulas not updating on conversion from Cells to PDF

22.        Conversion Issue with Data showing up as Number signs

23.        Invalid end column index exception

24.        Not Properly Format Numeric data

25.        Line in graphics not converted

26.        The performance of worksheet2image

27.        No response from SheetRender

28.        How to find grouped rows and columns

29.        Calculate external formulas

30.        Conditional formatting formula

31.        Moving range behaves incorrect

32.        This file was created using a later version

33.        Sorting within groups does not work

34.        Shape.AlternativeText

35.        Supports adding Tif Image with Pictures.Add() method

36.        Worsheet.Copy is pegging CPU at 100%

37.        Supports PageLayoutView

38.        Compatibility Problem with MS Excel

39.        Incorrect Formula(Cell.formula and ExternalLink)

40.        Supports copying hyperlink in copying range.

41.        Lost macros when saving in XLSM-format

42.        How to set transparent color to a picture

43.        How to move the Command Button

44.        Existing Conditional Formatting Changes

45.        Value was either too large or too small for an Int16

46.        Pivot Table Page Fields not working in Excel 2007

47.        Subtotals Issue

48.        The issue of opening XLSM file.

49.        Invalid end column index exception with XLSX file

50.        Chart title with formula issue

51.        Chart tick label format issue when converting to PDF

52.        Chart\_Overlapping issue

53.        Truncated data label issue

54.        Invalid Cell Name while saving in PDF format

55.        Layout and design of first sheet is lost and text overlaps

56.        ToImage throws Exception

57.        Office 2010 has detected a problem with the XLS file

58.        Problem with saving as XLS

59.        Offset Combinations issue

60.        CalculateFormula on my file gives error

61.        Combine with charts causing plot area mismatch

62.        Issues with a simple chart

63.        Textbox Format is lost for Excel 2007 workbook

64.        Hyperlinks for Embedded Objects are lost

65.        Remove ConditonalFormatting of the range

66.        Conditional Formatting issue

67.        Print Area/ Chart

68.        Conversion to PDF through Aspose.Cells Shrinks text

69.        Look and feel of generated PDF is not same as Excel

70.        SaveAs PDF Issue - Corrupted PDF

71.        Error converting Excel2003XML to XLSX

72.        Combine with charts causing plot area mismatch

73.        Conditional Formatting issue as of version 4.8.1

74.        Copy Excel having Command button event handler

75.        Document becomes unreadable

76.        Error Opening Large Files Aspose.Cells v4.7.1.0

77.        Office 2010 has detected a problem with this XLS file

78.        PivotTables unable to view

79.        Problem on attribute IsStrikeout

80.        Undesired behavior of Worksheet.Move method

81.        Bar chart format lost when saved

82.        Line chart format lost when saved

83.        Picture reference deleted with Version 5.1.1.0

84.        Pivot tables corrupted on passing through Aspose.Cells

85.        Workbook.CalculateFormula() doesn't calculate the values

86.        Bug of formula calculation engine

87.        Entered percent values are treated as string value.

88.        WebWorksheets.AddCopy() misses copying formulas.

89.        Enable to copy a WebWorksheet object from specified GridWeb control.

90.        GridWeb control is rendered very tall in Visual Studio 2010.

91.        A StackOverflowException will be raised

92.        Serialization issue.

93.        Cells data format issue - Dates turn into numbers

94.        An exception is raised when merging 0 rows or 0 columns range.

95.        VLOOKUP function does not support using double or int value

96.        Saving Excel document as HTML takes very long

97.        Missing Logo and Fuzzy / Light Text

98.        PDF Conversion problem

99.        Difference in printing from Excel and Outputting to PDF

100.    Image width shrunk in conversion to PDF

101.    PDF look and feel differs from XLSX

102.    Date format

103.    Filesize = 0 when converted to PDF

104.    Convert this file to PDF

105.    Excel File cannot be converted to PDF due to Invalid pdf format error

106.    Text comes out of table and fails to print completely

107.    2003 XLS with PivotTables corrupted

108.    DataBordyRange is not returning correct area

109.    Pivot table causes errors in XLSX files but works fine in XLS

110.    SpreadsheetML document opening issue with namespace attributes

111.    Copy Excel having Command button event handler

112.    getPrecedents returns a column 164

113.    Error on Named Range Array Formula

114.    Problems of save table as Excel97to2003

115.    Excel document with grouped images issue

116.    LoadOptions. ConvertNumericData

117.    Issue with Passwords and Excel 2003

118.    INDEX AND LOOKUP FORMULAS issue in GridWeb.

119.    Losing individual data point label formats

120.    Problem in adding Hyperlink to Cell

121.    ImportTwoDimensionArray seems to invalidate some cells

122.    Excel Found unreadable content error dialog

123.    Cannot open Excel workbook containing chart

124.    Problems with worksheets with comma character

125.    Exact format of excel cell data not captured

126.    Lock cells not working

127.    Scroll bar issue

128.    Excel found unreadable content in 'file.xlsx'

129.    Error opening workbook

130.    Sparklines issue – Office 2010

131.    Extracting values as a result of formula, the values come out wrong

132.    It gives error (Object reference not set to an instance) when I'm loading this simple Excel 2007 file

133.    Unable to change cell borders

**Aspose.Pdf for .NET**

_New Features_

1.      Add start/end indent properties rendering.

2.      Add Page sequence master testing class method

3.      Add margin bottom, left, right, top rendering function

4.      Create number-columns-repeated function

5.      Implement, word-spacing property, unit test

6.      Add padding before/bottom/end/left/right/start property rendering

7.      Added the support for HTML controls while transforming HTML contents into PDF file.

_Bug Fixes_

1.      Images in HTML Text are not displayed             

2.      Embedding two Postscript fonts, generates an error     

3.      Replaceable Symbols support

4.      Paragraphs.Add does not add new pages          

5.      Object reference not set to an instance of an object        

6.      Index was outside the bounds of the array.                     

7.      Producer field must be "\[Product Name\] \[Product Version\]"         

8.      Add start/end indent properties rendering.                                

9.      Add Page sequence master testing class method           

10.  Add margin bottom, left, right, top rendering function     

11.  Create number-columns-repeated function                                  

12.  Implement, word-spacing property, unit test                    

13.  Add padding before/bottom/end/left/right/start property rendering         

14.  Add 'fit-to-page' property/method        

15.  will the GetMaxColumnWidth become obsolete ?

16.  Issue with PositioningType.PageRelative          

17.  Bottom border of table row is not displaying on subsequent pages         

18.  XML Template stopped working after upgrade                            

19.  Throw exception if embedded font is not found 

20.  Dollar signs causing previous text on line to be removed                        

21.  Background coloring eats cell border lines.                     

22.  MyriadProBold font cannot be used in 4.1.2       

23.  System Defined Bullets are not working for heading object                      

24.  return value of GetStringWidth has changed from v4.1.2 to v4.4              

25.  Inconsistency in the text placement using different sizes of font.           

26.  All the text is bold when using HTML text to generate PDF          

27.  Improve products performance

28.  StackOverflow Exception is occurring when using HTML text inside table

29.  IsBroken Nested table Issue

30.  Nested Tables, textual area cell IsBroken-Issue

31.  IsBroken not working correctly when using inside a Nested Tables

32.  ImageInfo.DefaultFile is not working

33.  Problem converting multipage tiff to PDF using MemoryStream

34.  Create line-height function support

**Aspose.Slides for .NET**

_New Features_

1.      Video frame read as picture frame

_Bug Fixes_

1.      Title text gets inverted during PDF conversion

2.      "Parameter is not valid" exception when converting PPT to PDF

3.      Fonts and Background theme changed when exporting to PDF

4.      Text missing in title slide, Text formatting losing & white color

5.      All slides get blank in the exported PDF

6.      Slide text missing in generated PDF

7.      “Unsupported Format” exception on opening PowerPoint 2010 PPTX

8.      “IndexOutOfBound” exception on exporting to PDF

9.      Convert PPT to PDF causing “UnsupportedFontHeadVersion” exception

10.  “UnsupportedFormat” exception when opening PowerPoint 2003 PPTX file

11.  Problem removing Master Slides in PPTX

12.  Not a Microsoft PowerPoint 2007 presentation

13.  Add and Remove methods for Slide.SlideComments

14.  Tabs not handled properly as text got shifted

15.  Improper Image rendering in generated PDF

16.  Automatic video playback setting lost for PPTX

**Aspose.Pdf.Kit for .NET**

_New Features_

1.      Changing image color depth

2.      Ignore blank pages while converting PDF to TIFF

3.      Allow to set orientation - landscape or portrait - while converting to TIFF

4.      Allow setting margins while converting to TIFF

5.      Provide support to check whether file is a 'PDF Portfolio'

6.      PdfConverter throws exception while converting to EMF

7.      Allow to specify new font size while replacing text

8.      Provide support to specify Font Family while replacing text

9.      Provide support to specify Font Color while replacing text

10.  Provide support to specify Font Style while replacing text

11.  Force to produce monochrome images while using CCITT4 compression

12.  Provide support to check whether file is a 'PDF Portfolio'   

13.  Remove OpenAction command with GoTo Page action from the files   

14.  XMP manipulation

_Bug Fixes_

1.      Pdf to Image Conversion spikes memory

2.      Memory spikes during DoConvert and never returns back

3.      Text goes out of borders when printed with PdfViewer

4.      SaveAsTIFF produces output image 4X larger in memory size

5.      Some text which is invisible in view mode while shown when converted to image

6.      Partial PDF to image conversion

7.      Text color and line art is changed on the output images

8.      Text color and line art is changed on the output images 2

9.      Unable to delete the output file after concatenation

10.  Aspose does not support Field Flattening in append mode

11.  The output file produced by Concatenate method is unreadable

12.  Unable to find option list for specified field

13.  Problem concatenating PDF files

14.  Append method produces 0 byte output file

15.  Concatenate: Error processing the page - Problem reading document

16.  Multiple issues with a set of PDF files while concatenating

17.  Aspose.Pdf.Kit.PdfFileEditor Concatenate incorrect order and some garbage PDFs

18.  Improve ExtractText performance

19.  GetNextImage takes 20 second for a single page

20.  PDF to Image conversion takes a lot of time

21.  Gradient fill quality improvements

22.  API Enhancement - Form.FieldsNames should be Form.FieldNames

23.  Reduce TIFF file size in converting to TIFF

24.  ExtractText is too slow

25.  Font Arial Bold is not being applied in FormattedText

26.  PDF to TIFF Conversion Issue

27.  Exception pages are corrupt or too many pages on HasNextImage

28.  PDF to Image Adding Extra Text in Images

29.  A special symbol is placed when text is replaced with small letters

30.  Problem getting field caption

31.  Incorrect text is produced on converting PDF to image

32.  Null pointer exception at file parsing

33.  Font changed when field is filled and flattened

34.  Unable to flatten all the fields

35.  Setting AllowFillIn to false is not working properly

36.  Wrong text extracting, please check your PDF.: v4.3.0.2

37.  PdfConverter throws exception during convert to \*.emf

38.  Background colors are lost on image conversion

39.  PdfConverter produces empty table without any text data

40.  Pages Corrupt Error

41.  A generic error occurred in GDI+ while using ColorDepth.Format1bpp

42.  PageModeUseOC not working

43.  Unable to fill fields using ImportXml

44.  Checkbox is not filled using ImportXml 1   

45.  Checkbox is not filled using ImportXml 2   

46.  Checkbox is not filled using ImportXml 3   

47.  Checkbox is not filled using ImportXml 4   

48.  Checkboxes are not filled ImportXml   

49.  Problem while concatenating files containing barcode field   

50.  Aspose PDF Kit not working for some of the PDF Files   

51.  Signature is not visible in Signature Panel when visibility set to false   

52.  Using Form object twice throws exception: Stream does not support writing.   

53.  PdfConverter output image quality concern   

54.  Text is cut off when field is filled using Form class   

55.  Annotations are duplicated after modifying author   

56.  DeleteAnnotations problem in 4.7.0.0   

57.  NullPointerException: Object reference not set to an instance of object   

58.  SetSubmitButtonUrl not working in 4.6.0   

59.  Problem processing encrypted file   

60.  Problem adding Japanese text stamp   

61.  Extracted images are not correct   

62.  Unable to flatten bar code field   

63.  Text is repeated on the converted images   

64.  Concatenate loses Javascript in the output file   

65.  Flattening fields filled with Arabic and Chinese characters   

66.  Attachment is lost when file is encrypted   

67.  Unable to fill the fields from the XML

68.  Using MemoryStreams with Certificate or PdfFileSignature throws exception

69.  Adobe Illustrator files to JPEG

**Aspose.BarCode for .NET**

_New Features_

1.      Introduced new RecognitionHints called ThresholdHints, allowing users to choose the algorithm of threshold calculating

_Bug Fixes_

1.      Barcode is not found from tif image when area is specified

2.      System.IndexOutOfRangeException on BarCodeReader.Read() method

3.      Barcode license does not work on 64 bit OS

4.      AZTEC barcode recognition problem

5.      Aztec recognition test for area detect fix

6.      PDF417 Columns not working

7.      Barcode recognition dll crashes with VS 2010 and .NET 4.0

8.      EAN128 : ERROR on FNC1 Encoding

**Aspose.Task for .NET**

_New Features_

1.      Read ACWP data from MPP 2003/2007/2010 files

2.      Read TotalSlack data from MPP 2003/2007/2010 files

3.      Read project settings for earned values calculation

4.      Calculate BCWS, BCWP, ACWP, CV values

5.      Implement ProjectReader and ProjectWriter events for XML data processing customization

6.      Add Calendar's support methods for next working day start and previous working day finish calculation 

7.      Read StartVariance and FinishVariance for tasks and resource assignments from MPP files

8.      Read Outline codes definition from MPP files when look-up table contains wrong rows

9.      Write updated MPP file common project properties back to MPP file

10.  Provide support for ManualStart, ManualFinish and ManualDuration for MS Project 2010 MPP and XML formats

11.  Provide read support for MS Project 2010 XML format

12.  MS Project 2010 Data Interchange XML write support

_Bug Fixes_

1.      Improve project common properties reading

2.      Invalid empty tasks importing from XML project files

3.      Reading project Outline Codes from MPP 2007 files

4.      Incorrect WorkContour data reading from MPP files

5.      Incorrect MPP TimePhased data reading

6.      Task's WBS codes missed when read project data from MPP file

7.      Exception on Project's outline codes definitions reading  from MPP file

8.      Incorrect Baseline duration data reading from MPP files

**Aspose.Network for .NET**

_New Features_

1.      Add support for Outlook PST file format 97 - 2002

2.      Access outlook contacts from PST file

3.      Added EntryID property in Aspose.Network.Outlook.Pst.MessageInfo and FolderInfo

4.      Added PreserveOriginalDates in MailMessage class, if set to true, created and modified dates of original message is preserved in EML to MSG conversion

_Bug Fixes_

1.      ImapClient.ChangeMessageFlags does not work with recent and flagged

2.      Embedded images are not loaded properly from an MHT file

3.      Message with embedded image is not saved properly using MailMessageSaveType.OutlookMessageFormatUnicode option

4.      When comma character is used in meeting requests an extra backslash character is added

5.      Folder information is not received correctly after sending the status command

6.      SmtpClient throws exception if PickupDirectory method is used to send email

7.      ImapClient - Cannot add message to a folder with space in its name

8.      PersonalStorage.FromFile() method throws exception

9.      message flags are not correctly set after listing messages from Imap server

10.  using Imap on Gmail, only Inbox folder is selectable

11.  cannot move a message to trash folder in Gmail using Imap

12.  Special characters are not handled properly by MapiMessage.BodyRtf

13.  Custom headers are not fetched correctly by ExchangeClient

14.  Meeting organizer options are not available in Outlook after sending the appointment

15.  When EML files with TNEF attachments are saved again in EML format, attachments are not saved in TNEF format

16.  PST FolderInfo.GetContents() throws exception while reading a folder from PST

17.  Exception thrown while extracting message from various large and complex PST files

18.  Swedish characters are not saved properly when converting message from MSG to MHT or EML format

19.  ImapClient.NewMessageCount property returns incorrect values

20.  ImapMessageInfo.Subject, From and To contain null or blank for un-read messages

21.  Outlook calendar attachment contains missing information, when saved from an MSG file

**Aspose.Form for .NET**

_New Features_

1.      Support for InfoPath to PDF/A conversion.

2.      Converting InfoPath forms to PDF/A through API only.

**Aspose.Flash for .NET**

_New Features_

1.      Allow to exclude sound while converting FLV to SWF

_Bug Fixes_

1.      Merging XML and SWF    

2.      Unsupported audio format' exception while unpacking FLV

3.      Unexpected font parsing issue

4.      The sound is not good in SWF created from FLV

5.      FromSVG causes 'Index was outside the bounds of the array' error

6.      Extract Chinese characters from the SWF file

**Aspose.Report for .NET**

_New Features_

1.      Extended query parsing (Ability to parse queries which are not saved using AdHoc.Web component)

2.      Ability to control the transparency of data points through XML

3.      API to control the width of a legend marker (Line and Curve chart types)

4.      API to control the dash style of a legend marker (Line and Curve chart types)

5.      API to suppress the validation messages

_Bug Fixes_

1.      Incorrect SQL parsing using AdHoc.ParseSQLStatement.        

2.      Parsing error: First group breaks into rules on page 2.     

3.      Incorrect parsing of WHERE statement when first group exists.

4.      Incorrect parsing of WHERE statement when first group exists.                

5.      All items should be visible in the drop down on page 2 of the AdHoc component.

**Aspose.Slides for SharePoint**

_New Features_

1.      PPT, PPS, POT, PPTX, PPSX, POTX to PDF, TIFF, XPS conversion

**Download Aspose.Total for .NET**

<figure class="wp-block-embed"><div class="wp-block-embed__wrapper">http://www.aspose.com/community/files/51/.net-components/aspose.total-for-.net/default.aspx</div></figure>

**What’s New in Aspose.Total for Java Q3 2010:**

**Aspose.Cells for Java**

_New Features_

1.      Provides support for AES encryption type for Excel 2007 files.

2.      Supports reading/writing PivotTables for Excel 2007 files.

3.      Adds svg/svgz image format support for Chart to Image feature.

4.      Supports multiple print areas for PageSetup options.

5.      Sets custom number formats for PivotField.

6.      Includes new Built-in document properties for Excel 2007 file.

7.      Combines multiple Workbooks.

8.      Supports to save PDF to Stream for the direct Excel to PDF feature.

9.      An enhancement is made for reading/writing Excel 2007 files.

10.  An enhancement is made for reading/writing Excel 2003 files.

11.  An enhancement is made for reading XLS template files.

12.  Includes Sheet to Image, Sheet to Print and Workbook to Print features

13.  Supports Conditional formatting for Excel to Pdf feature

14.  Provides support for grouping pivot table fields in Excel2007 files

15.  Keeps macros when converting Excel97-2003 files to Excel2007 files

16.  Renders Shapes when converting to Pdf files, e.g. TextBox, Rectangle, Oval, Arc

17.  Supports to get/set full name of the source file for the Ole Object

18.  Enhancement is made for reading/saving Conditional formatting

19.  Enhancement is made for Chart to Image feature

20.  Enhancement is made for direct Excel to Pdf feature

21.  Enhancement is made for formatting of cell values

22.  Enhancement is made for removing header/footer of PageSetup

23.  Enhancement is made for copying cells

24.  Supports more flexible model for calculating custom functions.

25.  Includes error checking options for cells.

26.  Mathematical calculation of Range parameters in formulas is added.

27.  Provides support to set linked cells for chart frames such as Title, Data Labels.

28.  Supports to manipulate window position and size properties for Workbook.

29.  Reading/Saving Excel 2007 files operation is enhanced.

30.  Chart to Image feature is enhanced.

31.  Direct Excel to PDF feature is enhanced.

32.  Formatting Cell values is enhanced.

33.  Reading Excel 97-2003 files operation is enhanced.

34.  Saving charts module is enhanced.

35.  Formula Calculation Engine is enhanced.

_Bug Fixes_

1.      AES encryption type for Excel 2007 files

2.      Combine workbooks

3.      Direct xls2pdf: save to OutputStream

4.      Reading the template file

5.      Line coloring, RichText format

6.      Column width issue

7.      Generated PDF remains empty

8.      getStringValue()

9.      Chart2Image

10.  Dynamic formulas

11.  Copy worksheet, copy formula

12.  Setting standard column width for sheet

13.  Saving Pdf

14.  Saving Pivot Table for Excel 2007 file

15.  Setting font name for Excel 2007 file

16.  Cell.getDependents() throws exception

17.  Print areas in exported PDF

18.  Removing worksheet with pictures

19.  Improving performance of saving Pdf

20.  Excel 2007 Document Properties

21.  Setting custom format to pivotField dataField

22.  Saving Chart for Excel 2007 files

23.  Saving document property for Excel 2007 file

24.  Getting DataLabels properties

25.  PivotTable

26.  Use direct xls2pdf instead of xsl2pdf with Aspose.Pdf

27.  Copy cells

28.  Number format

29.  Source file name of OleObject

30.  Read excel2007 file

31.  Conditional formattings

32.  Formula

33.  Sheet2Print, Sheet2Image

34.  Save shapes for excel2007

35.  Draw textbox to pdf

36.  Remove header/footer

37.  Group pivottable

38.  Keep macros when saving excel2007

39.  Multiple Datasets with long names

40.  toImage() Method

41.  Sheet’s VeryHidden property

42.  Protect type MODIFY\_FILE

43.  Save shapes for excel2007

44.  Shape.getLinkedCell

45.  Number format

46.  Encryption for excel2007

47.  Conditional formattings for pdf

48.  Legend order

49.  Formula calculation

50.  Save Excel2007 file

51.  Read Excel2007 file

52.  Cells.getMaxDataColumn()

53.  Error check options

54.  Save Chart for excel2003 file

55.  Linked cells for ChartFrames such as Title/DataLabels

56.  Cell borders

57.  WaterFall Chart using StackedBar chart

58.  Get shape's size, Read style

59.  Cell.getStringValue()/getValueType

60.  Calculate array formula with empty cells in range

61.  3-Condition limit for conditional formattings

62.  Calculate custom functions

63.  Calculate formula with ICustomFunctionEx

64.  Calculate custom functions

65.  IF function calculation for empty cells

66.  Get window position and size properties

67.  VALUE function for empty cells

68.  Support Name for INDIRECT function

**Aspose.Pdf for Java**

_New Features_

1.      In order to improve Java interface, new overloaded methods (bindXML(InputStream) and save(OutputStream stream)) are added to Pdf class.

_Bug Fixes_

1.      Pdf file opening issue

2.      Issue while adding image to PDF from remote URL

3.      load XML contents from memory

4.      Multiple call of setLicence method cause runtime exception

5.      Can't set BMP image from memory

6.      Printing a paragraph from a new PDF page

7.      It is impossible to print whitespaces sequence with an underline to PDF document

8.      Issue with PositioningType.PageRelative

9.      setLicense fails  

**Aspose.Slides for Java**

_Bug Fixes_

1.      NullPointerException while opening PPT file

2.      Tables sometimes not rendered and not exported to PDF

3.      Improper slide thumbnail generated

4.      SlideEx.GetThumnail raises NullPointerException

5.      NullPointer Exception while cloning PPTX

6.      Problem Reading PPTX slides having tables

7.      Problem Reading PPTX if contains hyperlinks

8.      Headless exception problem with 2.2.0 for Java

9.      Pink background in slide thumbnail

10.  Error reading Fonts, if Fonts inherit styles from Master Slide (PPTX)

11.  Headless exception when generating slide thumbnail in Oracle Application Server Environement

12.  NullPointerException thrown on pdf save in Unix/Linux

13.  NullPointerException on thumbnail generation

14.  Slide index needed in Unsupported Image type

15.  setDateTimeFormat() in HeaderFooter class unavailable

16.  Add/Remove Slide.SlideComments()

**Aspose.Pdf.Kit for Java**

_New Features_

1.      Allow to wordwrap the string while replacing text

2.      Specify output image quality level

3.      Provide support to specify Font Color while replacing text

4.      Provide support to specify Font Style while replacing text

5.      Provide support to specify Font Family while replacing text

6.      Allow to find the font size of an existing text

_Bug Fixes_

1.      All text is not extracted from the specified rectangle

2.      Extracted text using rectangle method is weird

3.      Unable to extract text properly

4.      A special symbol is placed when text is replaced with small letters

5.      Problem extracting text from rectangle

6.      Unable to cast object: Error encounted while saving a PDF form

7.      Replace text is not working properly

8.      Annotations end up in the lower-left corner on flattening

9.      Unable to replace Swedish characters

10.  Unable to replace Norwegian characters

11.  Throw proper exception when page is out of range

12.  Word space and new lines are missing while extracting text

13.  Unable to replace Norwegian characters

14.  Exception "invalid value Off is specified for the element"

15.  Unable to flatten all the fields

16.  Throws NullPointerException on flattenAllFields

17.  Re-package the JAR file with classes in unique package name

18.  Minimize temporary files usage to ensure multithread-safety

19.  PdfExtractor,  PdfConverter and PDfViewer don't work in Linux

20.  Form.save throws 'Unknown Source' exception on Weblogic

21.  Russian text replaced with Russian text does not work

22.  Exception on PdfConverter in Servlet/Weblogic environment

23.  Swedish characters are lost when form is filled

24.  Stamped file is rotated with duplicate contents 2

25.  Stamped file is rotated with duplicate contents

26.  English text replaced with Russian text shows incorrect letters

27.  Class cast exception

**Aspose.BarCode for Java**

_New Features_

1.      Italian Post 25 barcode generation

2.      Italian Post 25 barcode recognition

3.      IATA 2 of 5 barcode generation

4.      IATA 2 of 5 barcode recognition

5.      "Royal Mail 4-state Customer Code" barcode generation

6.      Aztec 2D barcode recognition

_BugFixes_

1.      MacroPDF binary encoding issue

2.      FNC1 encode error in EAN128 generation

3.      "CloneNotSupportedException" is thrown while recognizing some datamatrix barcodes

4.      PDF417 Columns not working correctly

**Aspose.Report for Java**

_New Features_

1.      Support for XML serialization of all 2D charts

2.      Support for XML deserialization of all 2D charts

3.      Support for customization of spaces between the markers

4.      Support for additional customization of grid lines

5.      Improved plotting of Curve charts

6.      Ability to customize the labels’ area of a Radar Chart

7.      Separate build for Java 1.4 environment

8.      Separate build for Java 1.5 environment

9.      Structure of the packages after obfuscation.

_Bug Fixes_

1.      Some surface chart areas is painted incorrectly.

2.      Custom markers' lines for secondary axis.

3.      The area of surface chart is shifted.

4.      Gaps in Surface chart.

5.      Axis step is not defined.

6.      The exception occurs while Pie chart is being built.

**Aspose.Network for Java**

_New Features_

1.      Read Outlook MSG files and its properties like subject, recipients, sender, body etc

2.      Create new or update existing MSG file and update its properties

3.      Read and extract attachments from MSG file

4.      Read Outlook MAPI properties

**Download Aspose.Total for Java**

<figure class="wp-block-embed"><div class="wp-block-embed__wrapper">http://www.aspose.com/community/files/72/java-components/aspose.total-for-java/default.aspx</div></figure>

**What’s New in Aspose.Total for Reporting Services Q3 2010:**

**Aspose.Slides for Reporting Services**

_New Features_

1.      Support for SQL Server 2008 SP2 CU8

_Bug Fixes_

1.      Cells padding and border rendering issue in exported presentation

2.      Missing Slide and data in exported PPT

**Aspose.Cells for Reporting Services**

_New Features_

1.      Supports ODS export format.

2.      Supports XLSB export format.

_Bug Fixes_

1.      Aspose Cells suppressing headers on export.

2.      Exception of type 'System.OutOfMemoryException' was thrown.

3.      How to install a new version.

4.      How to install a new version.

5.      Can't install on SQL 2008 64-bit. 

6.      Page breaks not happening. 

7.      Unreadable content found in Excel after downloading from report using Aspose.Cells.ReportingServices.

8.      Aspose.Cells for Reporting Services OpenDocument format support.

9.      Not able to export SSRS report header into Excel.

10.  Incorrect Row Height.

11.  RunningValue function.

**Aspose.Pdf for Reporting Services**

1.  _Font size rendering issue  
    _
2.  _Integrating Aspose.Pdf.ReportingServices with Microsoft Report Viewer in Local_
3.  _Mode does not work  
    _
4.  _Component throwing exception after solution conversion  
    _
5.  _Problem while generating Table of Contents in PDF  
    _
6.  _ReportViewer extension bookmarks handling exception on MS sample  
    _
7.  _Unknown attribute in Heading element. The attribute name is Width.  
    _
8.  _Large images are generated in TOC demo in Aspose.Pdf SSRS 1.7.0  
    _
9.  _ReportViewer 2008 extension throws exception on demo conversion  
    _
10.  _Un-installation doesn't remove all information  
    _
11.  _Exception while report conversion from web-interface  
    _
12.  _Invalid parameter value exception  
    _

**Aspose.BarCode for Reporting Services**

_New Features_

1.  RM4SCC (Royal Mail 4-state Customer Code) barcode type generation
2.  Improved the IDE designer

_Bug Fixes_

1.  PDF417 Columns not working

**Download Aspose.Total for Reporting Services**

<figure class="wp-block-embed"><div class="wp-block-embed__wrapper">http://www.aspose.com/community/files/52/ssrs-rendering-extensions/aspose.total-for-reporting-services/default.aspx</div></figure>

**What’s New in Aspose.Total for JasperReports Q3 2010:**

**Aspose.Slides for JasperReports**

_Bug Fixes_

1.  Blurred Charts in PPT with Aspose.Slides for JasperReports

**Aspose.BarCode for JasperReports**

_New Features_

1.  Italian Post 25 barcode generation with checksum support and automatic grouping of codetext
2.  Support RM4SCC (Royal Mail Four States Customer) barcode generation with checksum support and automatic calculation of height of four state bars
3.  IATA 2 of 5 (International Air Transport Assosiation 2 of 5) barcode generation with checksum support

**Download Aspose.Total for JasperReports**

<figure class="wp-block-embed"><div class="wp-block-embed__wrapper">http://www.aspose.com/community/files/67/jasperreports-exporters/aspose-total-for-jasperreports/default.aspx</div></figure>









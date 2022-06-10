---
title: 'Aspose.Total for Java Q4 2008'
date: Sat, 27 Dec 2008 04:58:00 +0000
draft: false
url: /2008/12/27/aspose-total-for-java-q4-2008/
author: Salman Sarfraz
summary: ''
tags: []
categories: ['Aspose.Total Product Family']
---

**What’s New in Aspose.Total for Java Q4 2008:**

**Aspose.Words for Java**

_New Features_

1.      Supported loading Microsoft Office 2007 Open XML (DOCX) documents.

2.      New save formats (DOCX, DOCM, DOTX & DOTM) are added in SaveFormat enumeration.

3.      Add Smart Tags/Smart Document support.

4.      Supports OLE embedded and linked objects.

5.      Supports digital signatures for VBA projects.

6.      Foreach iteration for NodeCollection children.

7.      Added Comment.getDateTime() property to Java API.

8.      Supports writing of styles in Word 2007 format.

9.      Hacked remaining undocumented document properties.

10.  Supported page border art.

11.  Allow badly formatted HTML.

12.  Need to ignore CSS page breaks instead of throwing.

13.  Allow specifying border around floating image

14.  Support mirror margins and other page setup options in the interface.

15.  Workaround for JDBC drivers whose ResultSets doesn't implement getTableName().

16.  IBM's JVM with enabled JIT fails to load optimized Aspose.Words jar.

17.  Added support for outline numbered lists.

18.  Supported comment date,

19.  Added Name property to Shape class.

20.  All collection classes such as Paragraphs, Runs, Tables & Bookmarks etc. have been renamed into ParagraphCollection, RunCollection, TableCollection & BookmarkCollection etc. respectively.

_Bug Fixes_

1.      Image is not visible in Word 97.

2.      Embedded image is not displayed after saving document in DOC format.

3.      “IllegalArgumentException” exception occurs during mail merge if merge field date switch contains uppercase YYYY.

4.      “NullPointerException” exception occurs while setting PaperSize.CUSTOM.

5.      Pattern or texture fills are not saved to DOC.

6.      TestChuckChanCrash Out.doc is too big.

7.      Table borders are read incorrectly by Aspose.Words.

8.      Setting Document.ProtectionType to ReadOnly is lost after opening or saving the document.

9.      “The document does not have a piece table” exception occurs when opening document.

10.  “NullReferenceException” exception occurs in RunPrFiler when opening document.

11.  Font is changed after populating data into bookmarks.

12.  “This property is only allowed for list styles” exception occurs when saving document.

13.  Paragraph indents are lost in styles.

14.  Document.RemoveMacros() method does not remove all macros from document.

15.  Aspose.Words.FileCorruptedException” exception occurs while opening documents.

16.  “NullReferenceException” occurs when trying to save document with empty section.

17.  “OutOfMemoryException” exception is thrown on document loading.

18.  Font.HighlightColor doesn’t work for DOCX documents.

19.  “FileCorruptedException” exception occurs while opening document.

20.  “OutOfMemoryException” exception occurs when reading the document.

21.  “Unsupported version of the stylesheet” exception occurs when opening document.

22.  “FileCorruptedException” occurs when opening DOCX file.

23.  Use MHTML to store images inside exported files.

24.  Generate list numbers only when needed for HTML export.

25.  Generate list numbers for paragraphs with Heading styles.

26.  Use ol.start when converting document to HTML.

27.  “System.NotSupportedException” exception occurs when saving document in HTML format.

28.  List items are exported as ordinary paragraphs if belong to H1...H6 styles.

29.  Export correct standard HTML bullets to HTML.

30.  Join runs of same formatting on request.

31.  “System.ArgumentException” exception occurs when creating DocumentBuilder or saving document.

32.  Consider paragraph break font direct formatting in list label properties calculation.

33.  “System.FormatException” exception occurs when opening file.

34.  Unexpected spaces appear after InsertHtml call.

35.  A picture in the document is not visible in Word 97.

36.  Separate styles from content when exporting to HTML.

37.  Document can’t be opened by MS Word 2007 after processing with Aspose.Words.

38.  Table alignment does not work in created DOC files - probably FIB problem.

39.  Get rid of DocPr.ExtraBytes.

40.  “Unrecognized format of the form field” exception occurs while opening document.

41.  Supported writing of styles in Word 2007 format.

42.  Hack remaining undocumented document properties.

43.  “Cannot find form field node in a form field declaration” exception occurs when saving DOCX.

44.  “Unexpected subdocument type” exception occurs when saving DOCX file in DOC format.

45.  Styles lost after converting document to DOCX.

46.  Supported docPr.revisionView in import and export.

47.  “System.ArgumentOutOfRangeException” exception occurs when inserting HTML.

48.  Borders appear around HTML images after converting DOC to HTML.

49.  “com.aspose.words.FileCorruptedException” exception occurs when opening HTML document.

50.  Font of merge field is changed after mail merge.

51.  Parent node of Inline class is casted to Paragraph without check.

52.  Document.ViewType.Reading does not work.

53.  Text inserted by FormField.SetTextInputValue does not have an expected formatting.

54.  “The document contains captions” exception occurs while opening document.

55.  Cannot insert PNG image, error Unable to read beyond the end of the stream.

56.  RTL table becomes too wide.

57.  DOCX generated by Apsose.Words is corrupted to open with Word 2007.

58.  Background shape is lost when opening or saving documents.

59.  Freeform shape is processed incorrectly when opening or saving documents.

60.  Font size changes from 11pt to 10pt during OpenSaveOpen.

61.  Support proper protection password export in DOCX.

62.  Macros and digital sugnatures are not saved during DOCX export.

63.  UnifiedTestIncludePictureNoSeparator fails

64.  Add Name property to Shape class.

65.  As Icon, Icon Label, Icon Path and Icon Index are not supported for OLE objects

66.  Add Smart Tags/Smart Document support

67.  ArgumentOutOfRangeException during document save - bookmark related.

68.  The list bullet picture defined for lists is incorrectly interpreted as shape inside a paragraph.

69.  Hyperlink targets to unexpected URL.

70.  Cloning a document could be more efficient.

71.  The extracted embedded OLE object is corrupted.

72.  “'System.OutOfMemoryException” exception occurs when extracting OLE objects from document.

73.  “There is not enough memory or disk space to display or print the picture” occurs when opening document in MS Word.

74.  “System.OutOfMemoryException” exception occurs while extracting OLE10 object from document.

75.  File causes "Cannot find stream 'META' in the storage." exception when opened in Aspose.Words.

76.  Customer asked to support page border art.

77.  Text is lost in organizational diagram when opened and save by Aspose.Words.

78.  Problem inserting file modified by Aspose.Words in MS Word.

79.  Organization diagram casuses MS Word to crash.

80.  RTL paragraph alignment is incorrect in TestHebrew.

81.  RTL paragraph indents are incorrect.

82.  Vertical text direction is lost in TestRtlIssue.

83.  HtmlExportScaleImageToShapeSize does not work during HTML export.

84.  An email hyperlink causes exception.

85.  An HTML document falls into infinite loop.

86.  Allow badly formatted HTML.

87.  Export of cell borders to HTML does not work.

88.  Cannot import background scroll value.

89.  Cannot import border color #000000.

90.  List item with a certain inline style throws during HTML import.

91.  Add code examples to all new model methods.

92.  Merge fields in endnotes may not be working.

93.  Setting the result of a form field removes the formatting.

94.  Allow specifying border around floating image.

95.  Support mirror margins and other page setup options in the interface.

96.  “System.NullReferenceException” exception occurs when you trying to read form field with a paragraph break as the first character.

97.  The marathi characters are converted into square boxes.

**Aspose.Cells for Java**

_New Features_

1.      Supported manipulating charts in Excel97-2003 template files.

2.      Supported opening and saving Excel2007 XLSM, XLTX & XLTM files.

3.      Supported drawing objects such as Shapes and Charts etc. in Excel2007 format.

4.      Setting outline border for a range is supported.

5.      Supports reading OleObject from template file.

6.      Insert AVI file as OleObject.

7.      Copy Macros when copying Workbook.

8.      Supported images in XLS2PDF.

9.      Supported new Excel formula functions: MROUND, FDIST & NEGBINOMDIST.

10.  Improved performance of reading Excel2007 files.

11.  Enhanced the APIs of chart attributes.

_Bug Fixes_

1.      Fixed bugs related to reading and writing some special files.

2.      Fixed a bug in saving Excel file as HTML.

3.      Fixed a bug in saving Excel file as CSV.

4.      Fixed a bug in saving header and footer of PageSetup.

5.      Fixed a bug of adding picture by InputStream from URLConnection.

6.      Fixed a bug of parsing Date value for Date and Time function.

7.      Fixed a bug of sorting Names.

8.      A bug with copying formula is fixed.

9.      Fixed a bug with calculating and saving formula.

10.  Fixed a bug in Cell.getStringValue() method.

11.  Fixed a bug in Cell.setValue(Long) method.

12.  Fixed a bug in Cells.deleteRows() method.

13.  Fixed a bug with Validation and Conditional Formatting's formula.

**Aspose.Pdf for Java**

_New Features_

1.      HeaderFooter class has been rewritten to provide more flexibility.

2.      Various types of borders like page border, table border, header border and footer border are supported.

3.      Accessing the width and height of an image is supported.

4.      Most of the replaceable symbols are supported in Text.

5.      Image's margin property is enhanced.

_Bug Fixes_

1.      Table added in HeaderFooter is not shown.

2.      Add a bookmark with a heading object without showing the heading in the PDF content.

3.      Positioning an Image.

4.      Page orientation issue.

5.      HeaderFooter is overwritten.

6.      Adding text objects - different results within different containers.

7.      BorderSide.None doesn't have any effect in table and cell.

8.      Setting page border issue.

9.      Fixed an issue with header & footer page number.

10.  Getting image dimensions issue.

11.  Autofit table to contents.

12.  setDefaultCellTextInfo is not working for cell or row.

13.  Set line spacing issue when set within PDF object.

14.  An issue with setting word spacing is fixed.

15.  Setting table border versus cell border issue.

**Aspose.Slides for Java**

_Bug Fixes_

1.      Improved cleaning PPT files (removing XML tags) created in MS PowerPoint 2007.

2.      Exception on reading PPT files with more than ~2000 slides created in MS PowerPoint.

3.      fitTextToShape() method didn't work properly. Space between lines wasn't changed.

**Aspose.Pdf.Kit for Java**

_New Features_

1.      New class PdfBookMarkEditor is added to manipulate PDF bookmarks.

2.      New features of modifying comments (annotations) and flattening annotation are supported.  

3.      Supports new feature of replacing/deleting images from a PDF document.

4.      New methods are added in PdfFileSignature to support reading/disposing more information of digital certificate.

5.      The feature of replacing text is enhanced. Some special words (e.g. with hyphen) can be replaced properly.

6.      Supports multiline-text in both AcroForm and XfaForm.

_Bug Fixes_

1.      Lines cannot be printed properly.

2.      Fixed an issue with mending Japanese characters.

3.      Replacing text corrupts the document.

4.      Fields with umlauted characters can’t be filled.

5.      “NullReferenceException” exception is thrown when extracting links.

**Aspose.Metafiles for Java**

_Bug Fixes_

1.      Clipping error.

2.      Rendering EMF with MapMode and transform matrices.

3.      Added workaround for metafiles with wrong recordCount property.

4.      Possible ArrayIndexOutOfBoundsException on rendering metafiles.









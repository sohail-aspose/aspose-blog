---
title: 'Aspose.Total for .NET Q4 2008'
date: Sat, 27 Dec 2008 02:49:00 +0000
draft: false
url: /2008/12/27/aspose-total-for-net-q4-2008/
author: Salman Sarfraz
summary: ''
tags: []
categories: ['Aspose.Total Product Family']
---

**What’s New in Aspose.Total for .NET Q4 2008:**

**Aspose.Words for .NET**

_New Features_

1. Direct conversion to PDF without using Aspose.Pdf.

2. Print Word® documents in any server or client application without utilizing Microsoft Word®.

3. View and save document pages as PNG, JPEG, BMP or EMF files.

4. Full DrawingML support with import and export features is provided.

5. Supported MHTML import.

6. Supported EPUB export (Beta).

7. Load OpenDocument (OpenOffice Writer) documents.

8. Smart tags in DOC, OOXML, RTF and WordML document formats are supported.

9. Provided TLB (COM type library) and IDL (Interface Definition Language) to simplify use from unmanaged code.

10. Supported numbering override within one list (PDF, HTML).

11. Supported #$UNICODE macro in PDF export.

12. Supported TitlesOfParts and HeadingPairs document properties.

_Bug Fixes_

1. Images are missed when opening DOCX document.

2. Exporting a document to HTML or PDF throws an exception.

3. Improve export of paragraphs consisting of spaces.

4. Wrapping polygons for shapes are ignored.

5. List numbering is incorrect after ODT import for NumberStyle.Arabic.

6. The margin of list numbering is exported incorrectly.

7. The table row height is exported incorrectly.

8. Superfluous element in the list end.

9. Wrong bullet symbol in bulleted list.

10. Font setting is not applied to link when saving document in ODT format.

11. Page size and margins are not correct when opening ODT file.

12. Output Widows/Orphans control to PDF.

13. Inline boxes are centered in the table cell in DOC but come left aligned in the output PDF.

14. Member of group shape is improperly anchored.

15. Remove result of ASK fields from PDF output.

16. Page number is misaligned in footer.

17. Label size is resulted incorrectly in some cases.

18. Expand/Collapse Top Level modes in Acrobat is not working for some files.

19. Complex clipping region rendering to PDF is incorrect.

20. Some bitmap formats are rendered to PDF incorrectly.

21. WMF formula rendered to PDF poorly.

22. CharactersWithSpaces built-in document property lost.

23. “FileCorruptedException” exception occurs while opening document.

24. “System.OverflowException” exception occurs when saving DOCX document.

25. “System.InvalidCastException” occurs when opening DOCX file.

26. “FileCorruptedException” exception occurs when opening DOCX document.

27. Aspose.Words should ignore “\_x000d\_” in document properties.

28. It takes up to 15 minutes to open DOCX document.

29. Possible problem with generated DOCX files in Word 2003 + Compatibility Pack

30. DOCX created by Aspose.Words is corrupted to open in MS Word 2007.

31. Handle header rows in tables properly.

32. Allow custom document properties to link to range or bookmark.

33. BMP image is not inserted correctly into the document.

34. “System.ArgumentException: duplicate” exception occurs when saving document in any format.

35. List item numbering is incorrect.

36. UseDestinationStyles creates additional style in the destination document.

37. “NullReferenceException” exception occurs when saving document.

38. Text of text boxes and shapes is not exported.

39. Parameterize check box simulation in PDF export.

40. Character category is detected incorrectly.

41. “System.InvalidCastException” exception occurs when saving DOC in Aspose.Pdf format.

42. Encoding is treated incorrectly when loading RTF document.

43. ansicpg keyword is ignored during import of document properties.

44. Asian RTF files are converted incorrectly using Aspose.Words.

45. Characters are swapped with CharactersWithSpaces in RTF load and save.

46. Japanese characters are spoiled after converting RTF document.

47. RTF document hangs on loading.

48. MS Word is capable to read shapes defined in inappropriate places (not conforming to schema).

49. Aspose.Words doesn’t render the part of WML document.

50. “FileCorruptedException” exception occurs when opening WML document.

51. FormatException: Input string was not in a correct format.

52. Dates are exported using current culture and that creates invalid WordML.

**Aspose.Cells for .NET**

_New Features_

1. Supported exporting PivotTable to Excel2007 file.

2. Supported adding pivot calculated item to pivot table in 97-2003 XLS file.

3. Supports Page setup Header(s) and Footer(s) in Worksheet2Image.

4. Supported reading and writing XLTM and XLMX document formats.

5. Supports Excel2007 XLSX file encryption and decryption.

6. Supported reading/writing charts and shapes in Excel2007 XLSX file.

7. Get and set the cell Gradient style in Excel2007 file.

8. Supported reading and writing conditional formatting in Excel2003 SpreadsheetML file.

9. Supported reading/writing Data Bar, Color Scale and Icon Set conditional formatting in Excel2007 XLSX file.

10. Enhanced Xls2Pdf conversion.

11. Enhanced Chart2Image conversion.

12. Enhanced Worksheet2Image conversion and worksheet printing.

13. Copying worksheet is improved.

14. Supported non-contiguous print area.

15. Supported whole row(s) or column(s) as named range.

16. Calculation mode is supported.

17. Supported reading and writing Auto filter range.

18. Supported FREQUENCY, TRIM and LOGEST functions.

19. Supported calculating the "SEARCH" function.

20. Supports NonContiguousRange as a param of the function.

21. Supported reading MS Equation type of the OLE Object.

22. Supported Code Name.

23. Supported Date1904.

_Bug Fixes_

1. Inverts the color if negative.

2. Imports the date format.

3. Multiple rows in header(s) or footer(s).

4. Repeat images in the print title rows.

5. Fixed the issue with PageSetup.Order.

6. Merge cells if the smart marker is in a merged cell.

7. Invalid named range is exported to SpreadsheetML file.

8. Font color is changed.

9. Invalid RC formula.

10. Incorrect column width.

11. Converts the RC formula to A1 Formula.

12. Defined name "PrintTitles" is exported twice.

13. Clear all 2007 data before saving the workbook.

14. Saving with NamedRanges of the worksheet produces bad file.

15. Invalid result of “Round” function.

16. The defined name of the worksheet in calculating engine.

17. Compare array with a single value in calculating engine.

18. The list data source of the data validation is a named range.

19. Cell.Formula returns null.

20. InsertColumns: Not update the named range.

21. Find defined name ignoring the case.

22. Remove external links in the chart.

23. All 2000+ worksheets have pictures in headers.

24. PivotField contains more than 32k unique items.

25. Overload the method Cells.ExportDataTable().

26. Add the defined name of the worksheet, not global name.

27. Aspose.Cells leads to OutOfMemoryException.

28. ArgumentOutOfRangeException on Workbook.Open()

29. Check whether the password is valid in Excel2007 file.

30. Empty custom property is lost.

31. Tab color is lost.

32. Read the shared formula.

33. Export rich text to the file.

34. Export chart gradient fills.

35. MS Excel 2008 could not open the created file.

36. Fixed a few bugs while reading/writing Excel 97-2003 XLS file in some special cases.

37. Fixed a bug while inserting rows and columns.

38. Fixed some bugs while calculating formulas.

39. Fixed a data sorting bug.

40. Fixed a copying charts bug.

41. Fixed some bugs in autofit feature.

**Aspose.Pdf for .NET**

_New Features_

1. PDF/A-1 is fully supported (Beta version).

2. Supported Widows/Orphans control.

3. Supported macro #$UNICODE(). The number in the macro will be translated into Unicode character, e.g., #$UNICODE(9633) will be rendered as '□'.

4. Supported direct stream mode.

5. Supported auto-select font function.

6. 'IsKeptWithNext' function for table and canvas is enhanced.

7. Supported Z-order of watermark.

8. Supported new list attribute: 'Label'. It is going to replace 'CaptionLabel' and 'UserLabel' after one year.

_Bug Fixes_

1. Helvetica font support.

2. Table background color problem.

3. Word shapes are not appearing in PDF.

4. Page numbers are wrong in TOC.

5. Unwanted rows are repeated.

6. Misaligned heading's label, text area and spacing errors of text.

7. Table border appears around some cells inside table.

8. Japanese characters are missing from PDF.

9. Japanese characters disappear when converting from Excel to PDF.

10. Tables are not being rendered correctly during Word to PDF conversion.

11. Keep with next is not working when converting from Word to PDF.

12. Fixed table background color issue.

13. Fixed a wrong position issue with Word to PDF conversion.

14. Table.ColumnWidths is not working with Dutch regional settings.

**Aspose.Slides for .NET**

_New Features_

1. MSI installer contains Aspose.Slides.dll for .NET 2.0. If you need version for .NET 1.1, please download Aspose.Slides.zip and install it manually.

2. Metafiles are converted to PNG images now.

3. Improved rendering quality of transparent JPEG images to PDF.

4. LineFormat.JoinStyle property is added.

5. New PDF Rendering engine. Public API wasn't changed so please check Presentation.SaveToPdf method.

6. Additional cleaning of PPT files (embedded XML) created in PowerPoint 2007.

_Bug Fixes_

1. FitTextToShape method didn't work properly.

**Aspose.Pdf.Kit for .NET**

_New Features_

1. Supported new features of replacing and deleting images from a PDF document.

2. Supported new features of editing comments (annotations).

3. Added new methods for removing digital signature, supporting multi-line text in both AcroForm and XfaForm etc.

4. The scalability of PdfFileEditor is improved. For some operations like merging and splitting, the size limitation of PDF is doubled and the performance for processing large PDF files is improved.

5. The feature of image conversion is enhanced. An adaptive algorithm is taken to support more complicated PDF files.

6. Some exception handlers are improved and exception handling for PdfConverter is supported.

_Bug Fixes_

1. Page disabled after creating bookmarks.

2. Fixed a problem with bookmarks extraction.

3. Adding page number as watermark gives error.

4. Error handler for converting to image.

5. XML Import failed at radio button field.

6. 'Object Reference not set' error when calling ImportDataTable method.

7. Reading a PDF with usage rights enabled doesn’t show fields.

8. Specified cast is not valid in stamping.

9. The VerifySigned method always return false.

**Aspose.BarCode for .NET**

_New Features_

1. Supported International Standard of Application Identifiers (AI) for EAN128 barcode generation.

2. Compatibility and performance improvements for x64 platform.

3. Improved barcode recognition accuracy for image position.

4. Added Aspose.BarCode for WPF (Windows Presentation Foundation).

5. Fully integrated to Microsoft Visual Studio 2008.

6. Performance improvements for barcode recognition.

_Bug Fixes_

1. Setting symbology error for Interleaved2of5 barcode recognition.

2. Return wrong location while reading PostNet barcodes.

3. Fixed a bug related to EAN13 barcodes.

**Aspose.Network for .NET**

_New Features_

1. Supported listing mail messages on Exchange Server by Message Id.

2. Supported DataColumnMapping for Mail Merge.

3. Supported .NET Framework 3.5.

4. Supported sending Appointment Request / Cancel / Update in email messages.

5. Integrated Aspose.iCalendar into Aspose.Network. The product Aspose.iCalendar has been merged to Aspose.Network. All classes of Aspose.iCalendar are placed under the same namespace without changes. The existing Aspose.iCalendar customers don't need to change legacy code for this change, but only reference the new Aspose.Network.dll.

6. Supports setting the MessageFlags for Outlook Message files.

7. Use MapiMessage.SetMessageFlags method to set new message flags for outlook messages.

8. Supports decoding S/MIME Outlook Message files.

9. Enhanced FtpClient performance by using asynchronous socket programming technology.

10. Merged FileDrop control into Aspose.Network.dll.

11. Fully supports Outlook Message Format (\*.msg) reading and writing.

a. Create and Delete Attachments;

b. Add and Remove Recipients;

c. Supports Microsoft Outlook 2003, Microsoft Outlook 2007, and Microsoft Outlook 2008

12. Supports converting Email Message files (\*.eml) to Outlook Message files (\*.msg).

13. Improved converting Outlook Message files (\*.msg) to Email Message files (\*.eml).

_Bug Fixes_

1. Absent content-type throw exception.

2. Html encoding issue.

3. Calendar not compliant to some exchange server.

4. Calendar not compliant to hotmail calendar.

5. Calendar description and summary property doesn’t work.

6. ExchangeClient cookie bug.

7. FtpClient needs to release socket quickly.

**Aspose.Tasks for .NET**

_Bug Fixes_

1. “NullReferenceException” exception occurs when exporting to XML Calendar with BaseCalendar property equal to null.

**Aspose.Workflow for .NET**

_New Features_

1. ODP.NET support for .NET 3.5.

2. Improved database persistence performance.

_Bug Fixes_

1. Some configuration related bugs are fixed.

**Aspose.Editor for .NET**

_New Features_

1. Provides special builds of Aspose.Editor.Server.DLL. In these builds, Aspose.Editor.Server.EditorControl has ClassId property which can be used to specify full content of the "classId" attribute of the "object" tag inserted into the web page. This can be used if you have issues when page is accessed over HTTPS. Specify page relative location of the Aspose.Editor.Client.DLL in this property.

2. Four DLLs are provided for .NET 1.1 and .NET 2.0 based on 3.0.1 and 2.3.0 versions of Aspose.Editor.

**Aspose.Spell for .NET**

_Bug Fixes_

1. The Spell.GetCorrectWordList() works too slowly when word is very long.

**Aspose.Form for .NET**

_New Features_

1. Supported Downlevel Mode rendering for XmlFormView controls.

2. Supported the Inline Image control.

3. Supported the Ink Picture control.

4. Supported the Linked Image control.

5. Added three new methods to XmlFormView control.

_Bug Fixes_

1. Layout issue for InkPicture.

**Aspose.Flash for .NET**

_New Features_

1. Added possibility to compile ActionScript flash.

2. Added DefineShape4.ShapeId (read/write) property.

3. Added FlashObject.Id (read/write) property.

_Bug Fixes_

1. One more workaround for SWF files with "broken" tags which have wrong tag size.

**Aspose.AdHoc for .NET**

_New Features_

1. Support of grouping the rules is added.

_Bug Fixes_

1. Comparing to Date fields may cause unexpected filtered result.

**Download Aspose.Total for .NET:**

[http://www.aspose.com/community/files/50/product-suites/aspose.total/category1075.aspx][1]




[1]: http://www.aspose.com/community/files/50/product-suites/aspose.total/category1075.aspx





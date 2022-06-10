---
title: 'Aspose.Total for Java Q2 2009'
date: Tue, 30 Jun 2009 18:05:00 +0000
draft: false
url: /2009/06/30/aspose-total-for-java-q2-2009/
author: Muhammad Rashid
summary: ''
tags: []
categories: ['Aspose.Total Product Family']
---

**What’s New in Aspose.Total for Java Q2 2009:**

**Aspose.Words for Java**

_New Features_

1. Supports RTF file format:

· Read and write files in the RTF format of any version.

· Over 95% of the RTF 1.8 Specification supported.

· Unknown keywords (unsupported or from newer specifications) are safely ignored.

2. Supports loading OpenDocument 1.1 and 1.2 documents and saving documents in the OpenDocument 1.1 format.

3. Full DrawingML support.

4. HTML Image Export Customizations.

5. Smart tags are now supported in DOC and OOXML.

6. Access to Font Information and Panose.

7. The documentation now includes a topic on using Aspose.Words from PHP, Perl, Python and other languages.

8. Supports latent styles in the model and in all formats.

9. Supports Behavior Attributes for Styles (Locked, UI Priority, Auto Redefine, Unhide When Used, Semi Hidden).

10. Supports File Sharing Password in documents.

11. Supports the Read Only Recommended setting in documents.

12. Supports Smart Tags in DOC.

13. Supports DrawingML import and export.

14. Supports TitlesOfParts and HeadingPairs document properties.

15. Supports color names like ‘lightgrey’ during HTML import.

16. Implements SaveOptions.HtmlExportImageSaving event.

17. Supports picture bullets in HTML.

18. Added an option to turn off conversion to PNG during HTML output.

19. When reading multiple copies of same image, read only once to memory.

20. Added the possibility of specifying a prefix or postfix for image files names when exporting to HTML.

21. Allows setting the encoding for HTML export in SaveOptions.

22. Added image naming feature.

23. Export images using original file name, not generated.

24. Added “Don’t hyphenate” option to ParagraphFormat.

25. Expose Document.FontInfos with all underlying classes and properties.

_Bug Fixes_

1. Images are resized during DOC->DOCX->DOC roundtrip under some European locales.

2. Word 2007 SP2 says "file was created using a newer version of Microsoft Word" when opening a file created by Aspose.Words.

3. Aspose.Words should ignore “\_x000d\_” in document properties.

4. Improve parameterization when exporting image.

5. Split SaveOptions.ExportImagesFolder property to HtmlExportImagesFolder and PdfExportImagesFolder.

6. Suppress explicit page breaks in tables.

7. Support incomplete tags on HTML import.

8. Improve export of paragraphs consisting of spaces.

9. Files without byte order mark (BOM) opened incorrectly.

10. Support short color codes like #a8f during HTML import.

11. Implement bool SaveOptions.HtmlExportMetafileAsRaster.

12. Allow custom document properties to link to range or bookmark.

13. Resetting Subscript resets also Superscript.

14. FontInfo.Panose should be null rather than empty.

15. “FileCorruptedException” exception occurs upon opening the document.

16. “FileCorruptedException” exception occurs during opening document.

17. CharactersWithSpaces built-in document property lost.

18. “ArgumentOutOfRangeException” exception occurs during importing paragraphs with picture bullets.

19. Track change disappears after open/save document using Aspose.Words.

20. “FileCorruptedException” exception occurs during opening document.

21. Document crashes MS Word after setting TextColumnCount using Aspose.Words.

22. Text columns disappear from document after open/save the document.

23. Left indent of list is changed after open/save document using Aspose.Words.

24. “Unknown structure of an INCLUDEPICTURE field.” Exception occurs during opening document.

25. “FileCorruptedException” exception occurs during opening document.

26. List level numbering format is read incorrectly from DOC.

27. NullReferenceException when saving a document with a comment.

28. “System.NullReferenceException” exception occurs during saving document after inserting comment.

29. Extracted embedded PDF document is corrupted.

30. Null reference exception when saving DOC.

31. “The given path's format is not supported” exception occurs during saving doc as html.

32. “Cannot add a style because a style with the same name already exists” exception occurs during inserting one document into another.

33. Images disappear after open/save DOCX document.

34. Xml parser throws during opening DOCX document with misaligned text tag.

35. Images are resized and lost during DOC->DOCX->DOC roundtrip.

36. DOCX created by AW is corrupted to open in MS Word 2007.

37. DOCX created by AW is corrupted to open in MS Word 2007.

38. Images are missed when open DOCX document.

39. Possible problem with generated DOCX files in Word 2003 + Compatibility Pack.

40. It takes up to 15 minutes to open DOCX document.

41. z-index of shapes in headers and footers is not written to DOCX.

42. Images are not displayed when opening DOCX file from website.

43. “FormatException” occurs during opening DOCX document.

44. “FileCorruptedException” exception occurs during opening DOCX document.

45. “System.InvalidCastException” occurs during opening DOCX file.

46. “System.OverflowException” exception occurs during saving DOCX document.

47. Footnote separator and continuation characters are not exported.

48. Borders are not displayed (in some versions of IE only) when convert DOC to HTML.

49. Switching HtmlExportMetafileAsRaster off gives an exception if any transform needed.

50. SaveOptions.HtmlExportMetafileAsRaster = false does not work.

51. Handle header rows in tables properly.

52. Newly created style omits paragraph attribute in CSS output if only one direct attribute specified

53. Image with wrong (too big) resolution causes “OutOfMemoryError” exception during saving the document to HTML format.

54. Script tags should be stripped away on HTML import.

55. Exporting TestNestedFields.doc to HTML throws an exception.

56. Footnote numbers don't restart after inserting a new section.

57. Number format of endnotes is changed from Arabic to Roman after open/save the document.

58. “ArgumentException” exception occurs upon converting DOC to HTML.

59. Support non-US-ASCII filenames when send document to a client browser.

60. “NullReferenceException” occurs during Saving Document.

61. UseDestinationStyles creates additional style in the destination document.

62. List item numbering is incorrect.

63. FootnoteOptions/EndnoteOptions does not work.

64. ODT and XLSX documents are recognized as DOCX.

65. Style “Caption” is moved from “All styles” to “In current document” section after open/save document using Aspose.Words.

66. Enable “Track changes” automatically when protect document with AllowOnlyRevisions protection type.

67. “NullReferenceException” exception occurs during saving document in any format.

68. System.IndexOutOfRangeException: Index was outside the bounds of the array.

69. “System.ArgumentException: duplicate” exception occurs during saving document in any format.

70. DetectFileFormat method returns “Doc” during checking XLS file.

71. FootnoteOptions.RestartRule doesn’t work.

72. BMP image is not inserted correctly into the document.

73. Getting Bookmark.Text throws exception.

74. Wrapping polygons for shapes are ignored.

75. ”ArgumentOutOfRangeException” exception occurs upon converting to TXT.

**Aspose.Metafiles for Java**

_Bug Fixes_

1. Fixed possible IllegalArgumentException on rendering EMF metafiles with embedded bitmaps.

2. Fixed possible java.io.IOException exception on converting EMF metafiles with embedded images. Added workaround for correct reading bitmaps with less than 16 bits per pixel and without palette.

**Download Aspose.Total for Java:**

[http://www.aspose.com/community/files/50/product-suites/aspose.total-for-.net-and-java/default.aspx][1]




[1]: http://www.aspose.com/community/files/50/product-suites/aspose.total-for-.net-and-java/default.aspx





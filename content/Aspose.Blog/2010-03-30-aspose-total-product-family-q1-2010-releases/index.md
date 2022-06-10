---
title: 'Aspose.Total Product Family Q1 2010 Releases'
date: Tue, 30 Mar 2010 08:09:00 +0000
draft: false
url: /2010/03/30/aspose-total-product-family-q1-2010-releases/
author: Muhammad Rashid
summary: ''
tags: []
categories: ['Aspose.Total Product Family']
---

Aspose is proud to announce the Q1 releases of its Aspose.Total family of products. The Q1 2010 releases of Aspose.Total include several new features and updates for all product lines to help developers in building more reliable and robust solutions with less effort.  

**What’s New in Aspose.Total for .NET Q1 2010:                             **  

**Aspose.Words for .NET**  

_New Features_  

1.  Update the new converters spreadsheet with the HTML export features.

*   Default installation with Just Me option registers COM so that ASP applications do not work.

*   Form field font properties are not preserved when exporting to PDF.

*   Support mirror margins in sections.

*   Add an option to render form fields as form fields to PDF.

*   Heading row occurs only on first page.

*   Text direction in table cells is ignored during layout.

*   Support mirror margins.

*   Layout and render text frames.

1.  Preserve complex elements and formatting inside fields during field update.

1.  Support cell reference, like ABOVE upon updating fields.

1.  Support bookmark and cell references in formula fields.

1.  Add support of "office:meta" elements and corresponding fields export/import, which are supported in MS Word ODT export/import.

1.  Add "text:a"->"office:target-frame-name" export/import support.

1.  Add "table:table-rows" element import.

1.  Support True Type Collections during conversion to PDF/XPS.

1.  TOC entries are displayed as hyperlinks in PDF.

1.  Provide assemblies with and without Authenticode signature.

1.  Support “Auto Line Numbers” in rendering.

*   Import multipart structures of unsupported types as if they were multipart/mixed.

*   Add the possibility to bind Comment to the arbitrary range in the document rather than paragraph mark only.

*   Update fields after insertion optionally.

*   Make Field.Update public to allow update of a single field.

*   Add "number:language" and "number:country" attributes import for date fields elements.

*   Add "number:date-style"->"number:era" attribute export/import.

*   Support chroma key in Aps and GDI renderer.

_Bug Fixes_  

1.  “FileCorruptedException” exception occurs during opening document.

*   “FileCorruptedException” exception occurs during opening the document.

*   Mention in the documentation that Execute now ignores fields inside regions.

*   Image size is changed after open/save DOCX document.

*   Page break before list label is exported after list label.

*   Table is too wide after converting HTML to DOC.

*   “InvalidOperationException” exception occurs upon opening HTML document.

*   Encode &amp; escape sequence in urls during HTML import.

*   SaveOptions.HtmlExportScaleImageToShapeSize option has no effect.

1.  Font size of subscript and superscript is inconsistent after roundtrip.

1.  AWMS - Check whether Aspose.Words MSI installer works on Windows 7.

1.  Hyperlink style is lost after MailMerge.

1.  Date switches does not work in .NET 1.1.

1.  Additional double quotes are added if merge field value is empty string.

1.  GetValue method should not be called for TableStart and TableEnd merge fields.

1.  “NullReferenceException” exception occur upon rendering document.

1.  System.ArgumentException occurs after appending one document to another.

1.  Wingdings characters inside IF fields are not rendered correctly.

1.  “Undefined Bookmark” text is shown after updating fields.

*   Images are not retained after updating IF fields.

*   Different formatting is not retained after updating IF fields.

*   Paragraphs breaks are not retained after updating fields.

*   “DivideByZeroException” exception occurs, when try to insert image into a document.

*   Hyperlink is broken after updating fields if there is nested field.

*   UpdateFields doesn't substitute YYYY in DATE field.

*   “Error! Unknown op code for conditional.” Is shown when update fields.

*   Only part of field IF value is shown after mail merge.

*   All export->import->export tests fails after changes in document validator (WORDSNET-5313)

*   Run properties of comment are not exported.

*   Winword does not open ODT document when "table:table-row" element contains "table:covered-table-cell" element.

*   NullReferenceException when shape is in shape group and LineDashStyle is set.

*   Spaces in text after/before of the merged fields are exported incorrectly.

*   Parent style is not imported for form fields.

*   Empty "text:span" element is exported when run contains the invalid xml chars only.

*   Bookmark end is exported without bookmark start when bookmark intersects withfield.

*   Unnecessary space symbol is exported at the beginning of variable name.

*   Empty "draw:g" element is exported when empty shapes group inside the shapes group.

*   Styles names should correspond to NCName specification.

*   style:graphic-properties->"draw:marker-\*" attributes are exported/imported incorrectly.

*   tag name text:drop-down" is not allowed." error during TestOdtValidator().

*   element text:database-\*" is missing "table-name" attribute"error during TestOdtValidator().

*   unexpected attribute current-state"" error during TestOdtValidator().

*   element text:h" is missing "outline-level" attribute" error during TestOdtValidator().

*   attribute text:start-value" has a bad value: "-1" does not satisfy the "nonNegativeInteger" type" error during TestOdtValidator().

*   attribute text:start-value" has a bad value: "0" does not satisfy the "positiveInteger" type" error during TestOdtValidator().

*   attribute draw:dots1-length" has a bad value..." error during TestOdtValidator().

*   attribute text:bullet-char" has a bad value: the length of the value is 2, but the required length is 1." error during TestOdtValidator().

*   element text:list-level-style-bullet" is missing "bullet-char" attribute" error during TestOdtValidator().

*   Unnecessary "style:paragraph-properties"->"fo:text-indent" is exported when paragraph is list item.

*   All files should be valid for openoffice.org ODF Validator.

*   Create automatic test for validation ODT Gold files.

*   Empty formfield is shown as sequence of non-recognizable characters in the output PDF.

*   Check how rendering of Japanese documents works on Japanese OS.

*   System.InvalidOperationException occurs during rendering.

*   InvalidOperationException occurs during rendering to PDF and XPS with ARCHITIC.TTF font.

*   System.NullReferenceException occurs during rendering.

*   System.InvalidOperationException occurs during rendering.

*   System.ArgumentException occurs during rendering.

*   “ArgumentException” exception occurs upon rendering.

*   “System.InvalidOperationException: Unknown form field type.” occurs during rendering.

*   “System.InvalidOperationException: Requested a name string that is not present in the font.” occurs during rendering.

*   Review and incorporate a patch from Alexey Zhilin 1/10/09.

*   Multicolumn document is rendered improperly.

*   “Unsupported sfnt version” exception occurs upon converting document to PDF.

*   Unexpected behavior of RestartPageNumbering when save to PDF.

*   Bullet points are not recognized during rendering/converting to PDF.

*   PDF produced by Aspose.Words cannot be properly opened in Acrobat reader.

*   All text in the PDF is bold and italic.

*   Hyperlinks to files are broken after converting document to PDF.

*   “NullReferenceException” exception occurs during saving the document.

*   Header disappears after converting RTF document to DOC/DOCX.

*   Loading RTF is too slow.

*   FileCorruptedException: Unable to read beyond the end of the stream.

*   “Aspose.Words.FileCorruptedException: The document appears to be corrupted and cannot be loaded.” occurs during opening.

*   System.NullReferenceException: Object reference not set to an instance of an object. occurs during saving (HTML, ODT, legacy PDF).

*   Document.PageCount returns not correct value.

*   Extra empty page is added upon rendering.

*   Position of image is incorrect during rendering.

*   “InvalidCastException” exception occurs upon mail merge.

*   Image with application/octet-stream content type is not imported.

*   Aspose.Words eats 100% of CPU and freezes during opening DOC file.

*   Bullets are lost upon rendering.

*   “System.IndexOutOfRangeException : Index was outside the bounds of the array.” occurs during UpdateFields.

*   Text Form Field with Type “Calculation” is absent in FormFields collection.

*   Table in a Comment is not output to ODT.

*   Textboxes get black borders after DOC to ODT conversion.

*   Add "style:graphic-properties" -> "fo:wrap-option" and "style:table-cell-properties" -> "fo:wrap-option" attributes import/export.

*   REF fields are lost during converting to ODT.

*   Hyperlynk is not imported when it contains bookmark.

*   text:bookmark is imported incorrectly.

*   text:bookmark-start and "text:bookmark-end" are exported incorrectly when one of them inside cell.

*   System.NullReferenceException: Object reference not set to an instance of an object. during export checkbox.

*   MS Word throws exception when "text:a"->"xlink:href" is "http://\*" and contains blanks.

*   Validation error when nested fields is exported.

*   Validation error: element "text:h" is missing "outline-level" attribute.

*   config:config-item config:name=UseFormerLineSpacing"" is exported/imported incorrectly.

*   System.IndexOutOfRangeException: Index was outside the bounds of the array. during import.

*   System.NullReferenceException: Object reference not set to an instance of an object. during import.

*   Empty frame element is exported when image or object has no bytes and not link.

1.  System.InvalidOperationException: There was no XML start tag open. during export when list item text contains page break.

1.  System.NullReferenceException: Object reference not set to an instance of an object. during export.

1.  Attribute "text:p"->"text:style-name" is notimported when it contains a blank symbol.

1.  Multiple keywords are not recognized.

1.  Incorrect parsing of text:section.

1.  Assertion fails when rendering this document.

1.  InvalidOperationException when rendering the document.

1.  Document.PagesCount returns incorrect value.

1.  Page numbering is incorrect upon rendering.

1.  Shapes are missed during rendering.

1.  Metafiles are lost during converting document to PDF/XPS.

1.  “ArgumentOutOfRangeException” exception occurs upon rendering.

1.  Shape looks incorrect during rendering.

1.  “System.ArgumentOutOfRangeException: Index was out of range. Must be non-negative and less than the size of the collection.” occurs during rendering.

1.  Text and filling is invisible upon rendering.

1.  Empty paragraph with bookmark is ignored during rendering/converting to PDF.

1.  Header/Footer of the first page is also displayed on the second page. Rendering/Converting to PDF.

1.  Document\_Open macro does not run in Word 2000 after the document was open-saved by AW.

1.  Digital signature of VBA project is sometimes lost after open/save the document using Aspose.Words.

1.  Macros are lost after open/save document using AW.

1.  The Increase/Decrease Text Size buttons do not work in ADE.

1.  Import hangs up if treating this file as UTF-8.

1.  “System.InvalidOperationException : Unexpected node type.” occurs during UpdateFields.

1.  InvalidCastException occurs upon updating fields.

1.  “Window width is invalid” exception occurs during converting to PDF.

1.  The image disappears during rendering to PDF.

1.  ImageOptions.Resolution does not work when use Ccitt3, Ccitt4 or Rle compression.

1.  Connector lines are rendered incorrectly.

1.  Image disappears during converting to PDF and XPS.

1.  Borders appears around the picture during converting to PDF.

1.  Image in the header is cropped after converting to PDF or XPS.

1.  “System.IndexOutOfRangeException: Index was outside the bounds of the array.” occurs during rendering.

**Aspose.Pdf for .NET**  

_New Features_  

1.  Improved inline HTML.

*   Improved memory usage.

_Bug Fixes_  

1.  Stackoverflowexception in pdf.save method.

*   Segment.InLineParagraph is not working in v4.1.0.0.

*   Table Contents in wrong spot at the top of pages with tables.

*   Problems while Converting TIFF image to PDF.

*   Word to PDF conversion Discrepancies.

*   Margin of text element does not work in inlineHtml.

*   Font information is not being used in resultant PDF.

*   Escaping the dollar sign in Text String.

*   Footnote&Endnote issue in new version.

1.  Heading unmoral when TAB exists in inlineHtml.

1.  HTML Formatting incorrectly in generated PDF.

1.  IsImageNotFoundErrorIgnored Property is added.

1.  "H1" tag in HTML2PDF is not properly being rendered inside PDF.

1.  Heading Label is not setting to Italic.

1.  DropDown disappears when Security settings are applied.

1.  Text based watermark is not displaying properly on PDF.

1.  Problem while adding web image to PDF.

1.  TOC Wrapping issue.

1.  Table IsBroken Property is not working.

*   Word to PDF - removal of random spaces between words.

*   Table Width Issue.

*   Text wrapped in a  tag should only have a single line between paragraphs.

*   Table border colors are not displaying in resultant PDF.

*   Cellpadding and Cellspacing are being ignored during PDF generation.

*   IsSubsequentPagesOnly for Headers Section is not working in Direct-to-File mode.

*   Header not shown on random pages when using Direct-to-File mode.

*   Fit to a page is not working when Excel file is converted to PDF.

*   Problems when processing Asian characters.

*   Overlapping text and unnecessary carriage returns.

*   Unwanted newline is added during Word to PDF conversion.

*   Justification problem for mixed Chinese and English text.

**Aspose.Slides for .NET**  

_New Features_  

1.  Accessing Group shape names.

*   Revision no property of a presentation.

*   Provision of DocumentProperties.Template property.

*   Print functionality for presentations.

*   Export PPT to HTTP Response Object.

*   ShapEx.Name property similar to Shape.Name.

*   SlideEx.Name property similar to Slide.Name.

_Bug Fixes_  

1.  Save to PDF does not work due to missing font registry value.

*   Out of bound exception while saving the PPT.

*   Text with Shadow doubled on exporting PPT to PDF.

*   Shadows appearing in text when saving PPT as PDF.

*   DocumentProperties.Remove() not working for PPTX.

*   Slide.GetThumbnail throws exception on rendering to png format.

*   Problem writing PDF to stream using SaveToPdf(stream) method.

*   ShapeEx.AlternativeText is null.

*   Text sharpness lost on PPT -> PDF.

1.  Text Margin problem with PPTX -> PDF.

1.  Producer field for PPTX to PDF export.

1.  Null Pointer Exception on reading custom AutoShape without connection points.

1.  Removal of Aspose.Slides created Tags.

1.  DocumentProperties.EditTime = TimeSpan.Zero raises exception.

**Aspose.Pdf.Kit for .NET**  

_New Features_  

1.  Allow setting submit flag for a particular submit button.

*   Setting background color with FormattedText.

*   Provide method to extract text using specified encoding.

*   XFA Support.

*   CompressionLevel in Aspose.Pdf.Kit.

*   3.3.0.0 - Use Certificate in HTTPClientCertificate class in .Net to Sign Pdf.

*   Provide support for signature field.

_Bug Fixes_  

1.  Problem Creating Images.

*   Change SubmitFormFlag doesn'twork.

*   Data being dropped when converted to image.

*   Rotated text is not properly rotated.

*   Swedish characters are not printed properly.

*   PdfFileSignature is showing "Object reference not set to an instance of an object".

*   Rotation is not working properly.

*   ReplaceText does not work correctly.

*   Text is overlapped when fields are flattened after applying license.

1.  In some cases color of the text appears wrongly.

1.  Inserting page from one PDf into another fails (contain forms).

1.  Portrait and landscape page in same pdf prints as portrait only.

1.  GetNextImage produces image without any text.

1.  PDF meta data scrambled after setting password.

1.  Form.FillField method adds a new Node to the Xml structure.

1.  Form.ImportXml method adds new Nodes.

1.  Form.ImportXml ignoring CData section.

1.  Exception on getting form field façade.

1.  results shade-images in converting pdf.

*   Error when FlattenAllFields.

*   Aspose.Pdf.Kit.PdfExtractor seeming to freeze for a pdf document.

*   Concatenate method uses a lots of memory.

*   Printed PDF looks really light.

*   Image extraction performance is slower in 3.9 as compared to 3.3.

*   PdfConverter not work properly on 2003 sever.

*   Unicode Support.

*   Docx to TIF (Docx to PDF to Tif).

*   Do Aspose support PDF printing with Aspose.pdf.kit.

*   Wrong conversion, please check your pdf - error with a normal PDF file.

*   Aspose.Pdf.Kit for .Net - OutOfMemmory Issue.

*   FillField throws 'Object reference not set to an instance...' exception.

*   DeleteImage and/or ReplaceImage.

*   SaveAsTiff only converting bold text while missing normal text.

*   FormattedText with background covers all the area under the text.

*   Image is not placed properly using AddImage method.

*   'Object reference not set error' when image is passed as stream in AddImage.

*   ReplaceText not working for a PDF file.

*   ReplaceText not working for the sample PDF file.

*   Unable to replace text in sample file.

*   Some text on the document is not displayed.

*   OutOfMemory exception while using Concatenate method.

*   PdfViewer misses characters when printing the PDF.

*   DecodeAllPages problem.

*   PDF to PNG conversion is not done properly.

*   ReplaceText throws InvalidCastException.

*   While flattening annotations text annotation is lost.

*   Setting privileges invalidates the signature.

*   Unable to fill XFA form fields.

*   GetNextImage produces PNG image with white lines.

*   SaveAsTiff method produces a TIFF file with corrupted data.

*   Excess margins when printed using PdfViewer.

*   Concatenate method produces corrupt output PDF file.

*   Problem printing Czech characters.

*   Converter produces strange symbols.

*   PDF preview with PDFViewer.

*   Image extracted comes upside down .

**Aspose.BarCode for .NET**  

_New Features_  

1.  Deutsche Post Identcode barcode generation and recognition.

*   PZN barcode (Pharma Zentral Nummer, Pharmazentralnummer barcode) generation and recognition.

_Bug Fixes_  

1.  BarCodeReadType is not serializable.

*   Barcode is detected from an image that does not contain any barcode.

*   Patch code barcode could not be recognized from tiff file.

*   "Index was outside the bounds of the array" exception thrown when recognizing multiple barcodes from single image.

**Aspose.Tasks for .NET**  

_New Features_  

1.  Read common project information from MS Office Project 2010 mpp file.

*   Read calendars information from MS Office Project 2010 mpp file.

*   Read tasks information from MS Office Project 2010 mpp file.

*   Read all the extended attributes from MPP files.

*   Read default project's week working days and times from mpp files.

*   Read project Current and Status dates from mpp files (LastSaved and Name are added too).

*   Read task links information from MS Project 2010 mpp files.

*   Read resources information from MS Office Project 2010 mpp file.

*   Read resource assignments information from MS Office 2010 mpp file.

1.  Read MPP files with partly damaged structure.

1.  Defining mpp file format and MSP version before/without file reading.

1.  Read subprojects information from MS Project 2010 mpp files.

1.  Read outline codes information from MS Project 2010 mpp files.

1.  Read external attributes from MS Project 2010 mpp files.

1.  Read baselines information from MS Project 2010 mpp files.

1.  Read project keywords and comment values from mpp files.

1.  Read notes text from mpp files.

1.  Add public BuildVersionInfo class to access assembly version info from partly trusted assemblies

_Bug Fixes_  

1.  Eliminating invalid resource assignments (project public method RemoveInvalidResourceAssignments was added).

*   Calendar properties change on MPP to XML conversion using Aspose.Tasks.

*   Reading extended attribute definitions for attributes without custom fields.

*   Add AssignmentBaseline class for resource assignments baselines data processing.

*   Update xml baseline data processing.

*   Incorrect work value when writing to xml.

*   Update Aspose.Tasks numeric data types.

*   Rate CostPerUsed is missed and extra RateFormat is added while exporting into xml.

*   Remove unread project fields from resulting xml.

1.  Reading resource timephased data from MSP xml files.

1.  Task baseline DurationFormat is missing.

1.  NullReferenceException while reading duration outline codes from MS Project 2007 mpp files.

1.  Just first one mask is read from MS Project 2007 outline code definition.

1.  Incorrect resource assignment data reading.

1.  Update 2003 /2007 mpp baseline data processing.

1.  Correct task IsSummary property documentation.

**Aspose.Network for .NET**  

_New Features_  

1.  Eml to Msg conversion: The embedded .eml files from eml automatically convert to .msg attachments.

*   Access named properties from Outlook msg file.

*   RTF Extensions Specification support.

*   Make "From" field optional while creating msg file.

_Bugs Fixes_  

1.  Problems in generating recurrence patterns.

*   Exception thrown while saving msg file that has an embedded msg attachment.

*   Nested msg attachment from msg file is not saved.

*   Inline images from HTML body of email messages are not loaded.

*   Attachments not properly added when message is saved as eml format.

*   PreferredTextEncoding is not setting encodings of all properties of message.

*   If msg file is an attachment, FileName, Extention properties are null.

*   Reading Norwegian letters in Recipient Name.

*   Formatting is lost while saving an msg attachment.

1.  Attachment name with Encoding is not displayed properly.

1.  Content-Disposition header is corrupted if eml file (with attachment) is loaded and saved to disk.

1.  Encoded From display name causes FormatException.

1.  Pop3Client hangs on Connect() method.

1.  Embedded images appear as attachments while Eml to Msg conversion.

1.  Formatting and images are lost when we save as .msg format.

1.  Formatting is not correct if we load mhtml file in MailMessage and save as msg file.

1.  Update iCalendar samples to refer to the correct dll.

1.  Pop3Client.Connect() method hangs if SSL settings are not specified when connecting to SSL based server.

1.  Emails with attachments cannot be downloaded using Pop3.FetchMeMessage() method.

*   Exception occurred when Pop3Client.ListMessages().

*   If we retrieve message from pop3/exchange mailbox using FetchMessage() method, attachments get corrupted.

*   MailMessage.Priority and Sensitivity shows wrong information when msg file is newly created and saved from Outlook.

*   MapiAttachment.FileName property displays different filename format for different file types

*   Null object reference exception while loading a large msg file.

*   MailMessage.IsHtml property is always false, even the email contains Html body.

*   RecurrencePattern constructor throws exception for valid pattern.

*   Return empty collection from Pop3Client.ListMessages() when 0 messages found.

*   Msg file load exception - This structured storage version is not supported.

*   Create msg file from mhtml.

*   rtf body does include correct formatting in MapiMessage.

*   Exception thrown when saving attachment of "JournalEntry" type message.

*   Msg to Mht convertion crashed for invalid email address.

**Aspose.Form for .NET**  

_New Features_  

1.  Data in the RichTextBox is not visible in the generated PDF.

*   Generated PDF displays the first item of a DropDown and not the selected item.

*   InfoPath 2010 support.

*   Ability to disable the context menu of a repeating table and restrict users from inserting a new row.

*   Support for Expression Box control. New control is supported for InfoPath 2003/2007.

*   Support for relative size (percent only) for layout elements. PDF Export function can generate cells with size in percent.

_Bug Fixes_  

1.  Error in loading a form template which is based on a data source.

*   Fix a schema reading from a XSN template.

*   RuleSet actions are not working.

*   Cannot check CheckBoxes and RadioButtons in the RepeatingTable control

*   A Button with insert new line functionality in the RepeatingTable control is not working.

**Aspose.Flash for .NET**  

_New Features_  

1.  Add support for exporting movies to animated GIF.

*   Add support for audio file to SWF conversion.

*   Add support for conversion of the TTF fonts to SWF fonts.

*   Implement sound extraction utility.

_Bug Fixes_  

1.  Movie frame size is incorrectly set after SVG import.

*   Unable to merge two SWF files.

*   Problem while embedding multiple FLVs into SWF movie.

**Aspose.Report for .NET**  

_New Features_  

1.  DataPoint constructor for Gantt chart.

*   \[Bar\] Support for Left custom axis labels alignment.

*   Legend Box line spacing support.

*   X-Axis custom labels offset.

*   \[Legend Box\] Font size auto-adjustment disabling support.

*   Ability to hide the line at position 0 of the Axis.

*   \[Legend Box\] Add xml support for spacing type and corresponding properties.

*   Add event to get the name of selected field.

_Bug Fixes_  

1.  Change watermark.

*   Incorrect SQL while grouping rules (complex case).

*   Parsing error in AdHoc.Web.ParseSQLStatement and AdHoc.Web.ParseOrderByStatement.

*   Documentation contains incorrect links.

*   \[Point chart\] BackImage is not visible when ChartArea.Transparence is 255.

*   Check and fix incorrect links to standard classes.

*   \[Legend Box\] Xml font settings not taking effect.

*   LegendBox font size problem when loaded from XML.

*   \[Legend Box\] Incorrect item’s layout when LayoutType = Row.

1.  \[Legend Box\] Incorrect width calculation when position is LeftMiddle or RightMiddle.

1.  \[Legend Box\] Incorrect layout when legend margins are set.

**Aspose.Words for SharePoint**  

_New Features_  

1.  This release makes it possible to use our converting API for programmers developing own SharePoint solutions.

*   Result list should have filtering option.

*   Added files concatenation. Multiple files in different formats can now be combined into single output document.

*   Add select/deselect all check box to file selection list when combining files.

_Bug Fixes_  

1.  A debug assertion when unregistering the trace log provider.

*   Investigate a possibility of checking destination url which would not involve elevated security context.

*   It is possible to overwrite source files with conversion results before source files are converted (xml only).

*   It is possible to overwrite the source file when converting xml files.

*   Both xml formats not disabled in the GUI when converting an xml file.

*   Access Denied page is shown during conversion.

*   Exceptions are not handled when converting a file to a stream.

*   Fix file name checking for invalid chars.

*   The file is converted to the hidden folder successfully.

1.  Fixed known issue with installation on x64 servers.

1.  Errors (with specific server settings) when working with result or selection list after session times out or when cookies are disabled.

1.  The file is converted to the hidden folder successfully.

1.  folder name instead of file name in the results.

1.  An exception when using the product on a x64 system.

1.  Destination file name extension is not displayed on starting conversion settings dialog.

1.  When file of folder name starts with an underscore, it is not converted.

1.  Page headers are propagating over subsequent documents.

1.  Precede a message about failure to save file combination result with an explanation.

**Download Aspose.Total for .NET**  
[https://downloads.aspose.com/total/net][1]

**What’s New in Aspose.Total for Java Q1 2010:**  

**Aspose.Words for Java**  

_New Features_  

1.  Comment Ranges are Supported in Aspose.Words for Java 4.0.2 BETA.

_Bug Fixes_  

*   NullPointerException occurs during converting document to PDF in Linux.

*   UnsupportedOperationException exception occurs upon saving document if set java.util.Data as value of DocProperty.

*   Aspose.Words cannot save PDF into output stream.

*   Loading Some HTML Fails.

**Aspose.Cells for Java**  

_New Features_  

1.  Provides Chart-to-Image feature.

*   Imports RichText from SpreadSheetML template file.

*   Supports to export Name object with external references for SpreadSheetML file.

*   Exports Pictures in PageSetup for Excel 2007 files.

*   Imports TextBox controls from Excel 2007 files.

*   Provides support to set record limit when importing data from ResultSet for Smart Markers.

*   Sets the position of a Shape to the center of given range.

*   Supports to add calculated field for a PivotTable.

*   Supports to get/set VeryHidden property for a Worksheet.

1.  Adds new formula to the supported formulas list: FREQUENCY

1.  Recognizes the file format automatically for LightCells API.

1.  Enhances style’s model for performance consideration.

1.  Improves the API regarding Comment for performance consideration.

1.  Enhances the performance of reading large Excel 2007 files.

1.  Boosts the performance of LightCells API for large Excel 2007 files.

1.  Reading operation for a document’s properties is enhanced.

1.  Importing CSV files operation is enhanced.

_Bug Fixes_  

1.  Gather styles.

*   Copy style when inserting rows/columns.

*   Copy cell range.

*   Read Conditional formatting.

*   LogarithmicBase property of ValueAxis.

*   Save style.

*   Read template file.

*   Read special file generated by OWC.

*   Read special file generated by OWC.

1.  Read csv file.

1.  COUNTIF formula.

1.  Auto fit columns.

1.  IF formula.

1.  Formatted value of ChartFrame.

1.  Read row height.

1.  Get marker.

1.  Read marker.

1.  Copy formulas.

1.  Read rich text.

*   Performance of reading template file.

*   Performance of reading template file.

*   ASeries’s type.

*   Hyperlink’s link type.

*   DataLabels.

*   LightCells.

*   Title’s text.

*   ImageOption.

*   Hyperlink.

*   GradientFill.

*   LightCells.

*   Read Conditional formatting.

*   ChartPoints and LegendEntries collection.

*   PlotArea’s size.

*   ErrorBar.

*   Read shared formula.

*   Read chart.

*   Datetime value.

*   Read number.

*   Picture with Mac OS.

*   Read document properties.

*   Get hyperlink of shape.

*   Read drawing object.

*   Draw chart.

*   addCalculateField() method.

*   Save String value.

*   Save document properties.

*   VeryHidden property of worksheet.

*   Unsupported Font in special environment.

*   Read PageSetup and style.

*   Position shape.

*   Copy AutoFilter.

*   Save xlsx file.

*   Save style.

*   Read AutoFilter.

*   Record limit for ResultSet datasource.

*   Picture in PageSetup.

*   Create TextBox.

*   Read xlsx file with Apache zip tool.

*   Copy Axis.

*   Formulas of FormatConditions/Validations.

*   Date format.

*   Performance of creating Comment.

*   Gradient fill.

*   Copy PageBreaks.

*   Delete data.

*   Chart2Image.

*   Copy PageSetup.

**Aspose.Pdf for Java**  

_New Features_  

1.  Floating box.

*   PDF form field.

*   PDF attachments.

*   PDF security.

*   Foot note and end note.

*   Multiple columns document.

*   Graphs including Arc, Curve, Rectangle, etc.

*   Table of Contents, List of Tables and List of Figures.

*   Rich text format including left hanging text, HTML tags in text, rich format list, etc.

1.  Creating nested tables, table broken control, row broken control, etc.

_Bug Fixes_  

1.  FullJustify issue.

*   Vertical Alignment of Text is not working.

*   Invalid message, when font name other than core font is provided.

*   Multiple columns is not supported.

*   PDF Header Line Graph not work.

*   PDF not saved when handling hyperlinks.

**Aspose.Pdf.Kit for Java**  

_New Features_  

1.  CompressionLevel in Aspose.Pdf.Kit .

_Bug Fixes_  

*   XFA Support.

*   No images extracted from file.

*   Throws NullPointerException while converting pdf to tiff image.

*   Unable to extract image from the PDF file.

*   PdfSearcher problem.

*   Replace text in PDF.

*   ReplaceText in Java.

*   Null pointer exception is thrown when PdfSearcher is used more than once.

1.  Exception thrown by PdfSearcher.

1.  extractImage method hangs and never returns control.

1.  replaceText not working for a PDF file.

1.  replaceText is not working.

1.  replaceText is not working for some files.

1.  Unable to replace text in sample file.

1.  replaceText not working for the sample PDF file.

**Aspose.BarCode for Java**  

_New Features_  

1.  PZN barcode (Pharma Zentral Nummer, Pharmazentralnummer barcode) generation and recognition.

*   Deutsche Post Identcode(as known as Deutsche Post AG Identcode, Deutsche Frachtpost Identcode, Deutsche Post AG (DHL)) generation and recognition.

*   New class Code128CodeBuilder is introduced to support generating Code128 barcodes with user-defined codeset pattern.

**Aspose.Metafiles for Java**  

_Bug Fixes_  

1.  Text rendering issues on WMF -> PNG.

**Aspose.Report for Java**  

_New Features_  

*   Supports pure date type value of axis and chart points.

*   Supports Candlestick chart's point plotting.

*   Supports serialization and deserialization of the Candlestick chart.

*   Supports different date type formats for axis points.

*   Supports auto calculation of chart points.

*   Supports convenient interface for passing any kind of chart point values and axis point values.

*   Supports the data point labels.

*   Supports additional customization of Radar chart.

1.  Supports grid lines in Radar chart.

1.  Supports the background color of the radar in a radar chart.

1.  Supports different chart border types.

1.  Supports adjusting the legend box layout.

1.  Supports handling the wrong set of the entered data.

1.  Supports additional facilities for series and series collection.

1.  Supports assigning the DateTime format value to axis step.

1.  Supports the double-precision for axes and chart points.

_Bug Fixes_  

1.  Gantt chart labels are drawn incorrectly.

*   Impossible to add series with default name.

*   Interaction between AxisIntervalType and AxisStepType.

*   Candlestick chart is not rendered for some input data sets.

**Download Aspose.Total for Java**  
[https://downloads.aspose.com/total/java][2]

**What’s New in Aspose.Total for Reporting Services Q1 2010:**

**Aspose.Slides for Reporting Services**

_Bug Fixes_

1.  Large Image cropping problem resolved that don’t fit don't fit to a page.

*   Image resize problem with SSRS 2008.

*   Text Alignment Problem.

**Aspose.Cells for Reporting Services**

_New Features_

1.  Enhanced rendering of editable Charts for SQL Server Reporting Services 2008.

*   The Performance configuration is set as the default configuration.

**Aspose.BarCode for Reporting Services**

_New Features_

1.  PZN barcode (Pharma Zentral Nummer, Pharmazentralnummer barcode) generation.

*   Improve the design-time interface for IdentCode barcode.

*   Generate Code128 barcodes with user-defined codeset pattern.

*   Enhancements in barcode designer of Visual Studio IDE.

**Download Aspose.Total for Reporting Services**  
[https://downloads.aspose.com/total/reportingservices][3]

**What’s New in Aspose.Total for JasperReports Q1 2010:**

**Aspose.Slides for JasperReports**

_New Features_

1.  Full support of latest JasperReports 3.7.1 version.

*   PPTX export from JasperServer.

*   Implementation of PPTX/PPSX export.

_Bug Fixes_

1.  Exported rectangles can have borders with wrong format.

*   Exported images can have wrong position or cropping.

*   Error writing presentation to a stream.

**Aspose.BarCode for JasperReports**

_New Features_

1.  Supports Identcode Barcode, also known as German Post (Deutsche Post AG) (Deutsche Frachtpost) Identcode barcode.

*   Supports Matrix 2 of 5 barcode, also known as 2/5 Matrix or 2 of 5 Matrix.

**Download Aspose.Total for JasperReports**  
[https://downloads.aspose.com/total/jasperreports][4]




[1]: https://downloads.aspose.com/total/net
[2]: https://downloads.aspose.com/total/java
[3]: https://downloads.aspose.com/total/reportingservices
[4]: https://downloads.aspose.com/total/jasperreports





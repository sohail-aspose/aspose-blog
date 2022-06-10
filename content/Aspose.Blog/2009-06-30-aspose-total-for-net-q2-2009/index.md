---
title: 'Aspose.Total for .NET Q2 2009'
date: Tue, 30 Jun 2009 17:57:00 +0000
draft: false
url: /2009/06/30/aspose-total-for-net-q2-2009/
author: Muhammad Rashid
summary: ''
tags: []
categories: ['Aspose.Total Product Family']
---

**What’s New in Aspose.Total for .NET Q2 2009:**  

**Aspose.Words for .NET**  

_New Features_  

1. Export documents or pages as XPS (XML Paper Specification).  

2. Added support for Table Styles, Table Style Conditional Formatting and Document Themes.  

3. Vertically merged table cells are supported when converting to PDF, rendering and printing.  

4. Added import of "fo:hyphenate" attribute of "style:text-properties" element.  

5. Added "table:number-rows-spanned" attribute import.  

6. Added "style:writing-mode" attribute import in "style:table-cell-properties" element.  

7. Added "text:date" and "text:author-name" fields import/export.  

8. Added "text:file-name" field import/export.  

9. Added "table:table-row" -> "table:number-rows-repeated" attribute import.  

10. Added "table:table-row" -> "table:default-cell-style-name" attribute import.  

11. Aspose.Words for .NET now supports exporting PDF documents that comply with the PDF/A-1b standard.  

12. GlossaryDocument and BuildingBlock classes introduced in the public API.  

13. Glossary documents are now supported when loading and saving Office OpenXML.  

14. Support navigation map in EPUB export.  

15. Import and Export PageSetup for each section to HTML.  

16. Supports < center >< /center > tags.  

17. Added an option to move to a merge field in DocumentBuilder without deleting the field.  

18. Added attribute "style:display-name" export for style elements.  

19. Added generator name with version number to meta.xml.  

20. Added "table:table-columns" element import.  

21. Added "style:default-outline-level" attribute export for "style:style" element.  

22. Added "style:vertical-align" attribute import for "style:table-cell-properties" element.  

23. Parent style of table style is not imported.  

24. Added attribute "style:background-transparency" import/export for "style:graphic-properties" element.  

25. Added "table:covered-table-cell" and "table:number-columns-spanned" import.  

26. Added import of percentile font size.  

_Bug Fixes_  

1. “Found XXXPropRMarkEx sprm with unknown value.” Exception occurs during opening document.  

2. Document cannot be opened by Word2000 after converting HTML to DOC if HTML contains nested tables.  

3. Generated file hangs or crashes MS Word 97, 2000 and 2002.  

4. Document can’t be opened by MS Word 2000 after open/save it using AW.  

5. “Cannot find a piece for the position” exception occurs during opening document.  

6. “Cannot read array shape property” exception occur during opening document.  

7. “Unexpected number of reserved styles in the stylesheet” exception occurs during opening document.  

8. “Read wrong number of bytes from Escher record” exception occurs during opening document.  

9. “Read wrong number of bytes from Escher record” exception occurs during opening document.  

10. “Found XXXPropRMarkEx sprm with unknown value” exception occurs upon opening the document.  

11. “Found XXXPropRMarkEx sprm with unknown value” exception occurs upon opening the document.  

12. DOC file is corrupted after converting RTF document to DOC.  

13. “OutOfMemoryException” exception occurs during opening the document.  

14. Document cannot be opened in MS Word 2002.  

15. “Read wrong number of bytes from Escher record” exception occurs during opening the document.  

16. “FileCorruptedException” exception occurs during opening the document.  

17. Word 2002 (XP) shows error message when try to open Document produced by Aspose.Words.  

18. “FileCorruptedException” exception occurs during opening a document.  

19. “FormatException” exception occurs during opening DOC file.  

20. Aspose.Words corrupts formatting of the document after open/save.  

21. “ArgumentOutOfRangeException” exception occurs during saving the document.  

22. Aspose.Words eats all memory and hangs during opening the document.  

23. Document cannot be opened in MS Word after Open/save the document using Aspose.Words.  

24. “End of paragraph is out of sync” exception occurs upon opening document.  

25. Stack-overflow exception while opening DOC.  

26. IsInsertRevision has wrong comment in the documentation.  

27. Support loading encrypted DOCX documents.  

28. “FileCorruptedException” exception occurs during opening DOCX document.  

29. “UnsupportedFileFormatException” exception occurs during opening DOCX document.  

30. “UnsupportedFileFormatException” exception occurs during upening DOCX document.  

31. “FileCorruptedException” exception occurs during opening DOCX document.  

32. “FileCorruptedException” exception occurs when try to open encrypted DOCX file.  

33. “UnsupportedFileFormatException” exception occurs when try to open DOCX document.  

34. “FileCorruptedException” exception occurs during opening DOCX document.  

35. DOCX produced by Aspose.Words crashes MS Word.  

36. DOCX produced by Aspose.Words cannot be opened in MS Word.  

37. Enforce EPUB validation on export.  

38. Aspose.Words cannot find an image is folder name contains white space.  

39. Incorrect encoding detected during HTML import results in gibberish.  

40. Not all CSS stylesheet was parsed exception during loading HTML.  

41. “Unexpected format of the subsidiary header” exception occurs during opening MHTML document.  

42. DetectFileFormat throws “InvalidOperationException” exception, when try to detect format of a corrupted document.  

43. “InvalidCastException” exception occurs upon saving the document to any format except DOCX, WML and TXT.  

44. GetImageSize return negative Height, when get size of BMP image.  

45. Add the Document.OriginalLoadFormat property.  

46. Make Document.DetectFileFormat detect pre-Word97 documents.  

47. Make Document.DetectFileFormat detect encrypted documents.  

48. Consider an ability to allow inserting fields with custom field codes.  

49. Consider making Apsose.Words exceptions to be serializable.  

50. Superfluous page in the document end after export.  

51. Run properties of list level are exported incorrectly.  

52. Files are various after export->import->export because of errors of rounding.  

53. Frame width and height are various after export->import->export.  

54. "style:flow-with-text" attribute of "style:graphic-properties" element is various after export->import->export.  

55. "fo:padding\*" attributes of "style:paragraph-properties" element are various after export->import->export.  

56. "fo:font-weight", "style:font-weight-\*" and "fo:font-style\*" attributes of "style:text-properties" element should not be exported when value is "normal".  

57. "style:text-properties" element is imported incorrectly for field content.  

58. Superfluous "text:span" inside "text:span" after export when FieldType.FieldMergeField.  

59. Bookmarks should not be exported into form field content.  

60. Bookmarks in header and footer is exported into "office:text" content.  

61. Section break paragraph vanishes after export->import->export.  

62. "meta:type" attribute of "meta:user-defined" element is not imported.  

63. "table:number-columns-spanned" and "table:number-rows-spanned" are exported incorrectly.  

64. Remove using StyleType.Table in reader  because it is not supported in AW model.  

65. Font size is various after export->import->export.  

66. "style:num-format" in "text:list-level-style-number" element is imported incorrectly when it is not defined.  

67. "style:default-outline-level" in "style:style" element is imported incorrectly when it is not defined.  

68. Value "Standard" of "style:parent-style-name" attribute in style of heading is imported incorrectly.  

69. "style:master-page-name" in "style:style" element is exported incorrectly when header or footer.  

70. "style:text-properties" is not imported when span in "text:drop-down".  

71. "fo:font-size" is imported into paragraph property instead of to run property when paragraph contain column break.  

72. "style:line-height-at-least" is exported instead of "fo:line-height" in "style:paragraph-properties" element.  

73. Superfluous "style:page-layout" and "style:master-page" after export.  

74. "style:writing-mode" value is not taken into consideration during import of "fo:text-align" attribute in "style:paragraph-properties" element.  

75. Error of rounding in "style:position" of "style:tab-stop" element  

76. "style:text-underline-style", "style:text-underline-type", "text-underline-mode" in "style:text-properties" are imported incorrectly.  

77. Error of rounding in "style:text-position" of "style:text-properties" element.  

78. "style:leader-style" in "style:tab-stop" element is exported incorrectly when TabLeader.MiddleDot.  

79. Percentage value of "fo:line-height" attribute in "style:paragraph-properties" element is not rounded to integer.  

80. Default value of "style:tab-stop-distance" attribute is incorrectly  after import.  

81. Paragraph.ParagraphFormat.SuppressLineNumbers is exported incorrectly.  

82. Exception when style:default-outline-level="" during import.  

83. Paragraphs styles are lost when the text contains "\\r\\n".  

84. Spaces in the paragraph beginning and after line break are imported incorrectly.  

85. Exception when length value is percent during import.  

86. Line break and tabulation are lost after import.  

87. Import hang-up when font size is percentage value.  

88. Exception when name duplication of "meta:user-defined" element.  

89. OOo throw exception when opens file after export (TestDuplicateSti, TestDefect4977, TestDefect1340, TestDefect1575).  

90. OOo throw exception when opens file after export when list in comment.  

91. OOo throw exception when  "draw:rect" element contains "text:p" element.  

92. Font size export is incorrect for normal paragraph style and default paragraph style when font size is not set.  

93. "style:master-page-name" attribute in "style:paragraph-properties" element is not imported when ODT file has been created by "KOffice/2.1 Alpha".  

94. Date styles are mixed when style of date field is not set.  

95. "style:table-cell-properties" -> "fo:border" attribute import does not work when "in", "mm" or "pt" units.  

96. "table:table-column" -> "table:number-columns-repeated" attribute import   does not work when table style is not set.  

97. default value of "style:columns"-> "fo:column-gap" attribute should be 0 instead of 1.27cm during import.  

98. Default tab stop value ("style:paragraph-properties" -> "style:tab-stop-distance") should be 2cm instead of 0cm when it is not set during import.  

99. "style:tab-stop" is imported incorrectly when attribute style:type="char" and attribute "style:char" is set.  

100. List numbering within a table is incorrect in vertically merged cells (HTML, PDF).  

101. “NullReferenceException” exception occurs during rendering/converting to PDF.  

102. Filling is missed in EMF image, when convert Word to PDF.  

103. Make sure that duplicate images are written to XPS only once.  

104. Metafile background is black.  

105. Bold text is displayed "too bold".  

106. Picture is displayed incorrectly.  

107. XPS Viewer reports an exception.  

108. Border drawn incorrectly.  

109. Test\\TestChars fails to load in XPS Viewer.  

110. Other\\TestTobyHenders6 crashes XPS Viewer.  

111. Run\\Text\\TestMarathi displayed incorrectly.  

112. Model\\Shape\\TestAlexandarDukic crashes XPS viewer.  

113. Model\\Shape\\TestDefect6690 crashes XPS Viewer.  

114. Shape\\Images\\TestImageAtEndOfPage metafile not displayed well.  

115. FieldStart and FieldEnd nodes are not removed when AcceptAllRevisions.  

116. RTF output size is too large.  

117. Table is incorrectly indented after WML to DOC conversion.  

118. “FileCorruptedException” exception occurs upon opening WML document.  

119. “FileCorruptedException” exception occurs during opening WML document.  

120. Word 2003 eats 100% of CPU and hangs during opening document produced by Aspose.Words.  

121. Word 2007 SP2 says "file was created using a newer version of Microsoft Word" when opening a file created by Aspose.Words.  

122. Internal navigation (e.g. TOC) doesn't work in Adobe Digital Editions.  

123. Roundtrip section breaks in HTML export and import.  

124. \[br style="page-break-before: always"/\] causes an extra empty paragraph at the beginning of the page.  

125. Numbered lists with bulleted number style are exported to HTML incorrectly.  

126. List with multiple levels is not converted correctly to HTML.  

127. Explicitly reset italic attribute not round tripped through HTML.  

128. Content is missed during loading HTML document.  

129. Style of numbering "bullet" is exported as "number".  

130. ODT document produced by Aspose.Words is corrupted.  

131. Style font is exported incorrectly when font and base style are not set.  

132. “FileCorruptedException” exception occurs during opening ODT document when "Standard" style is missing in ODT file.  

133. OOo throw exception when opens file after export because incorrect symbols in value of "meta:user-defined" element.  

134. OOo throw exception when opens file after export because incorrect symbols (") in attribute value of "text:user-defined" element.  

135. OOo throw exception when opens file after export when document contains smart tag.  

136. OOo throw exception when opens file after export when field start and field end are in different paragraphs.  

137. OOo throw exception when opens file after export when bookmark start and bookmark end are in different table cells.  

138. "System.InvalidOperationException: Opened initial tag XML is missing" when first paragraph of table cell is list item and last paragraph in previous table cell is not list item.  

139. "System.InvalidOperationException: Opened initial tag XML is missing" when the list element is section end and the next list element is section start.  

140. OOo throw exception when opens file after export when hyperlink contains symbol '&'.  

141. OOo throw exception when opens file after export when field contains a paragraph break.  

142. "Cannot find part ..." exception when picture path is "http\*", "https\*" or "file\*" during import.  

143. NullReferenceException during import.  

144. Element "text:s" is imported incorrectly.  

145. The first 16 Istd of built-in styles should be given to special styles (see StyleIndex constants).  

146. Empty borders in styles properties collections.  

147. “UnsupportedFileFormatException” exception occurs when try to open ODT document created by Windows 7 WordPad.  

148. NullReferenceException when "Standard" master page is missing (ODT document created by Windows 7 WordPad).  

149. System.InvalidOperationException: Cannot find part '/settings.xml' when ODT document created by Windows 7 WordPad.  

150. "meta:creation-date" and "dc:date" elements are imported variously on different computers because of various settings of time zones.  

151. System.InvalidOperationException: "The built-in styles Normal and Default Paragraph Font cannot be based on any style" during import.  

152. System.ArgumentOutOfRangeException : parameter name distanceFromText during import.  

153. "System.InvalidOperationException: Opened initial tag XML is missing" when run has revisions  

154. Top half of text line is not visible after export.  

155. "\_20 \_" in a style name should be replaced with space during import.  

156. Parent style of text styles is imported incorrectly.  

157. Run properties are not imported in hyperlink.  

158. The "None" value of "text-line-through-style" attribute is not imported.  

159. Superfluous span in FieldNumPages and FieldPage after export.  

160. Empty "style:tab-stops", "style:paragraph-properties", "text:span", "style:style" elements after export.  

161. Parent style "citation-style-name" and "citation-body-style-name" in "text:notes-configuration" are is not imported.  

162. List numbering within a table is incorrect near section breaks.  

163. Page color becomes green in output document (HTML, PDF).  

164. Missing shapes in TestClipArt.  

165. RTF generated by Aspose.Words for reporting service includes empty rows between data rows.  

166. “Unknown structure of an INCLUDEPICTURE field.” exception occurs during opening RTF document.  

167. Table is narrowed and unexpectedly repeated on every page.  

168. Two tables appear as one after RTF import.  

169. Background from one cell is propagated to another on RTF import.  

170. Font is changed from Arial to Times New Roman after open/save RTF document.  

171. “FileCorruptedException” exception occurs during opening RTF document.  

172. “FileCorruptedException” exception occurs during opening RTF document.  

173. “NullReferenceException” exception occurs during saving DOC in RTF format.  

174. “InvalidCastException” exception occurs upon opening RTF document.  

175. Image size is incorrect when save document to RTF.  

176. Size of EMF image is incorrect when save document to RTF.  

177. Left margin of table is changed after open/save RTF document using Aspose.Words.  

178. Exception: 'Unknown structure of an INCLUDEPICTURE field.'  

179. All document contents are imported to header.  

180. Images are invisible in the output documents.  

181. Texbox width is read incorrectly.  

182. “sprmPCrLf is not yet supported” exception occurs during opening document.  

183. Part of content disappears during printing document generated by AW.  

184. Range.Replace method works very slowly on DOCX document.  

185. “FileCorruptedException” exception occurs during opening DOCX file that contains embedded DOCX file.  

186. InsertHtml inserts paragraph as RTL.  

187. Text size is incorrect upon inserting HTML into the document.  

188. Bullets are lost when insert HTML in Turkish culture.  

189. “Unexpected table parent.” Exception occurs during inserting HTML table into the TextBox.  

190. “InvalidOperationException” exception occurs upon savein document in HTML format.  

191. Paper tray is not returned in LayoutPage.  

192. Japanese hieroglyphs are not shown in PDF.  

193. Saving the same document twice to PDF causes exception.  

194. “Start and end node should have the same grandparent.” Exception occurs when try to move DocumentBuilder cursor to merge field.  

195. MailMerge fails on documents with IF fields spanning several sections.  

196. Add throwing exception when attempt to create too long form field or bookmark names.  

197. A document throws InvalidCastException when combining documents.  

198. “System.InvalidOperationException” exception occurs during Updating fields.  

199. FormTextInput Field starting with newline cases null pointer exception when calling field.Result.  

200. Superfluous page break when paragraphs has differents "style:master-page-name".  

201. FormField.Result is lost during export to ODT.  

202. Font of FormField is reset to “Times New Roman” after open/save the document.  

203. Improve performance of ODT.  

204. Texbox becomes with blue background after open ODT/save DOCX ODT.  

205. Exception "System.ArgumentException: Cannot add a style because a style with the same name already exists." during document import.  

206. System.ArgumentNullException during document import.  

207. Hyperlink to a bookmark does not work after export.  

208. Paragraph wraps a picture incorrectly after export.  

209. System.NullReferenceException during shape export.  

210. "System.InvalidOperationException: Opened initial tag XML is missing" when headings are used in different sections.  

211. "text:list-header" element content is not imported.  

212. Formatting of heading is missing after import ODT and export DOCX.  

213. Content of "text:table-of-content" element is missing after import.  

214. "System.ArgumentException: This style is not a paragraph style" during import.  

215. Unnecessary page break when style contains fo:break-before="auto" and parent style contains fo:break-before="page".  

216. Table structure is imported incorrectly when document contains "table:covered-table-cell" an element.  

217. The document text is not imported after element "draw:circle".  

218. Element "style:text-properties" is not imported for style of element "text:h".  

219. “NullReferenceException” exception occurs during Rendering/Saving to PDF.  

220. RLE compression for images is not working.  

221. File size is very big after converting to PDF.  

222. “NullReferenceException” exception occurs upon saving document to PDF.  

223. It is not always suitable to apply same compression to all images in PDF.  

224. Can’t open output RTF file when use Aspose.Words in evaluation mode.  

**Aspose.Cells for .NET**  

_New Features_  

1. Directly export Excel files to PDF stream.  

2. Apply Subtotals to worksheet tables.  

3. Improved performance of encrypting and decrypting Excel 2007 file.  

_Bug Fixes_  

1. Chart Image does not look like underlying chart object.  

2. Percentage sign not showing in pie chart.  

3. Exported chart messed up.  

4. Saving workbook with chart in HTML broken.  

5. Using FillFormat.Pattern.  

6. The Category X-Axis title is not being displayed.  

7. Html broken on worksheet name containing a space.  

8. HTML export format issue.  

9. Supports hyperlink in directly converting cells to PDF.  

10. Font problems with Aspose.Cells converting to PDF.  

11. Cells 4.7.0 saving to PDF stream does not work.  

12. PDF file is too large.  

13. Key has already been added to dictionary exception.  

14. Excel to PDF produces corrupt PDF file.  

15. Some Aspose.Cells save issues.  

16. Differences in output.  

17. Index out of range.  

18. Bad SpreadsheetML when a sheet is deleted.  

19. Error when a PRINT\_AREA exists.  

20. Method EndCellinRow for Excel2007.  

21. Copy validations in copying range.  

22. Date number format with current language specified.  

23. Saved Excel file is corrupt.  

24. Supports to calculate Large function.  

25. Supports to set the function CHOOSE.  

26. Set Precision as displayed is unchecked.  

27. The issue of Workbook.Open.  

28. Update Conditional formatting when inserting/deleting columns.  

29. The issue of converting cells to PDF.  

30. Print titles error after inserting/deleting columns.  

31. I in Cell return to ?  

32. Cell.HtmlString Error.  

33. Formats lost after opening Excel file.  

34. End of stream reached opening 2003 XLS.  

35. Save Performance Issue.  

36. Non-negative number required in Workbook.Open.  

37. Supports WEEKDAY,WEEKNUM function.  

38. Getting absolute value of a range not working.  

39. Can open XLS but XLSM has Invalid Formula error.  

40. Cell.PutValue cannot handle date without year.  

41. Lack of way to detect ranged name of the worksheet.  

42. Only export DataTable header.  

43. Save as an invalid Excel2007Xlsx file.  

44. How to remove a pivot table?  

45. Stream is closed after calling Workbook.Open.  

46. Works slowly in loading XLSX file.  

47. Cannot open a XLSX file  

48. Unreadable Content error in XLSM file saved in Aspose.  

49. Problems with the PrintTitleRows feature.  

50. Background image from template missing.  

51. Outline.SummaryRowBelow not saving in XLSX files?  

52. What does the method SetFirstPageHeader do.  

53. Can't get WorkSheet.CustomProperties to work.  

54. Unable read XLSX file.  

55. Workbook.IsProtected does not work in XLSM files.  

**Aspose.Slides for .NET**  

_New features_  

1. Read/write access to standard and custom document properties.  

2. Read/write access and possibility to create new:  

· OLE objects.  

· Audio clips with embedded and linked audio files.  

· Video clips with linked video files.  

3. Read/write access to Tags on Presentation, Slide and Shape level.  

_Bugs Fixes_  

1. Fixed many slide cloning problems since the last release.  

2. Fixed exception thrown on adding new PictureFrameEx.  

3. Different font colors after cloning.  

4. Split presentations have incorrect gradient direction than original.  

5. Slides with hyperlink don't save correctly. NullReferenceException thrown.  

6. Charts are not rendered properly.  

7. Wrong FillType of charts.  

8. Connectors don't move with the connected shape.  

9. PPT file becomes locked in case of exception in the Presentation constructor.  

10. Write access for HeaderFooter.DateTimeFormat property.  

11. PPT to PDF rendering speed and generated PDF file size optimizations.  

**Aspose.Network for .NET**  

_New Features_  

1. Supports setting the Read/Unread flags on an email message with ExchangeClient.  

2. Supports Content-Disposition header in eml files parsing.  

3. Supports RemoteCertificateValidationCallback handler for ImapClient and Pop3Client.  

4. Improved the compliance for ImapClient on microsoft exchange server.  

5. Improved the compliance for Pop3client on microsoft exchange server.  

6. Optimized for X64 platform.  

_Bug Fixes_  

1. SmtpClient throws common language runtime exceptions.  

2. The attachments in an embedded outlook message file cannot load properly.  

3. CC and To fields missing problem.  

4. MessageId and Subject fields are empty.  

5. Invalid characters may cause exceptions when loading EML files.  

6. Exception thrown when we save embedded MSG file.  

7. Exception thrown when converting from EML to MSG.  

8. Loading MSG files with embedded attachments.  

**Aspose.Tasks for .NET**  

_New Features_  

1. Added support for MS Project 2007 MPP format.  

2. Added new common API for all supported formats MPP2003, MPP2007 and XML.  

_Bug Fixes_  

1. Fixed possible NullReferenceException on reading calendar exceptions in XML format.  

2. Fixed possible NullReferenceException on reading projects in MPP format.  

**Aspose.Form for .NET**  

_New Features_  

1. Supports “Choice Group” control.  

2. Supports binding to xml data.  

3. Support static binding to dropdown lists.  

4. Binding to SharePoint lists.  

5. Binding to Web Services.  

6. Binding to Database Server Tables.  

7. Supports multiple views in InfoPath document.  

8. Support accessing XSD schema from XmlFormView control.  

_Bug Fixes_  

1. Problem with DatePicker in Visual Studio 2005.  

2. Ensure that controls following a Date Selector control are displayed.  

3. XML data loading error.  

4. Horizontal Repeating Table Layout Issue.  

5. Date Picker did not work in firefox.  

6. Multiline TextBox display problem in Internet Explorer.  

7. Insert item button for repeating section is invisible.  

8. Multiple info path view problem.  

9. Insert item in the context menu is invisible for repeating section.  

10. Date time picker missing.  

11. Insert item in the context menu is not working for repeating section.  

12. XmlDataString property cannot be set on page load.  

13. Dropdowns in InfoPath 2007 rendering error.  

14. Check form posting/restoring its values inside a master page.  

15. Cannot load schema file for InfoPath 2007.  

16. Cannot be used in UserControl.  

17. Repeating Table control removes first row not the selected row.  

18. Save CheckBox value.  

**Aspose.Flash for .NET**  

_New Features_  

1. Supports Flash v8.  

2. Supports Flash v9.  

3. Supports Flash Lite.  

4. Support exporting a specific frame of the SWF file to image formats using Render() method of the FlashContainer object.  

_Bug Fixes_  

1. Error creating flash on 1.5.8.0 but works fine on 1.5.2.0.  

2. Support for frame rendering.  

3. Snapshot of a single SWF frame.  

4. FocalGradientFill doesn't have TransformMatrix member.  

**Aspose.Grid for .NET**  

_New Features_  

1. Supports importing/exporting to Excel2007xlsx file format.  

2. Supports reading merged cells’ style from Excel file.  

3. Supports Auto RowFilter and Custom RowFilter; adding IgnoreCase and IsStartWithCriteria properties to GridColumn to customize behaviors of auto rowfilter.  

4. Adds CustomMsgTitle property to Validation to customize the title of MessageBox.  

5. Adds RecalculateFormulas property whose default value is true; when it is set to false, assigning any value to a cell will not recalculate the formula.  

6. Adds Width and Height properties to Comment.  

7. Adds CommentFont property to GridDesktop to set font of Comments.  

8. Provides new versions for the overloaded list of the Add method for the CommentCollection class to specify Width and Height of Comments.  

9. Adds IsVisible property to Worksheet.  

10. Supports reading/writing CustomProperties of Worksheet in excel files, and adding read-only CustomProperties property to Worksheet.  

11. Supports vlookup function/formula.  

12. Supports Undo/Redo features when changing values of cells.  

13. Adds ContextMenuManager property to GridDesktop to manage context menu.  

14. Adds RowColumnHiddenChanged event.  

15. Supports multi-selection of rows/columns/regions.  

16. Supports importing/exporting frozen Panes from/ to Excel files.  

_Bug Fixes_  

1. Sets Single or float types value to cell displays blank.  

2. The right-bottom borders that were not shown normally.  

3. The black border of the focused cell that was not shown normally.  

4. Demo Features throws file path exception demonstrating Pictures feature.  

5. Adds SetSelectedIndex method to ComboBox to avoid recalculating all the formulas.  

6. Presses a key on ComboBox of a cell would invoke editing.  

7. Font size bug in Format Cell Dialog.  

8. The focused cell had been changed when validation failed.  

9. Pastes cells several times, certain cells’ background color are set to blue.  

10. Data sorting performance issue.  

11. Clicks header lines, the row height / column width is changed.  

12. Cannot copy content in input box of a cell via CTRL+C.  

13. Throws exception when changing a value above the frozen rows.  

14. Updates all references of the formulas when inserting or deleting rows or columns.  

15. Changes a cell's value, only the relative formulas will be recalculated and not all.  

16. Performance issue for Copying/ Pasting/ Deleting a number of cells  

17. Performance for calculating array formulas.  

18. Calculates RowsCount / ColumnsCount properties error when accessing Cells / Rows / Columns properties of Worksheet.  

19. Performance for ImportDataTable.  

20. Changes the height of hscrollbar and the width of vscrollbar from 20 pixels to 16.  

21. Adds SetSelectedIndex method to ComboBox to avoid recalculating all the formulas.  

22. Modifies colors of gridlines, header lines & selections.  

23. Calculates visible width of the drawing text error when a cell extended its text to the right cells.  

24. Performance for rendering worksheets.  

25. SetFont & SetFontColor methods of GridRow not work.  

26. An invalid cell name in the formula might cause an invalid cell reference.  

27. The behavior while navigating cells via scrollbars and arrow keys.  

28. Performance of copying / pasting large numbers of cells including lots of formulas.  

29. IComparer exception occurs when a column value contained int and string types for auto-filtering data.  

30. Utilizes FormulaError object that now returns value instead of throwing exception.  

31. Boolean value in a cell does not render to string value.  

32. Location of focused cell in rows/columns selection mode.  

33. Editing invisible focused cell issue.  

34. The formula engine calculates the null value into result of empty string.  

35. Updates formulas error when deleting rows.  

36. Enhances formula error messages.  

37. Performance issue for many error formulas.  

**Aspose.Editor for .NET**  

_New Features_  

1. Command.Text, Command.Description and Command.ImageIndex properties setters implemented.  

2. Command.Shortcut setter implemented.  

3. New methods EditorBars.Rebuild(), Range.CopyDocument(), Range.PasteDocument() implemented.  

_Bugs fixes_  

1. Error occurs while opening some documents with form fields.  

2. Nested fields are not saved properly.  

3. In some documents Aspose.Words provides extra column which is invalid.  

4. “SaveAs” standard command doesn't change the current directory on Vista.  

5. Editor doesn’t open documents with WordprocessingML <cr> tag.  

**Aspose.AdHoc for .NET**  

_Bug Fixes_  

1. Error in loading saved queries. Error in parsing the queries with grouping functionality.  

2. Error in parsing the grouping operators.  

3. Layout issue when used with master pages. Layout issue can be removed using <div style="position:relative"> wrapper.  

4. JavaScript error when used on a page with master page.  

5. Finish event provided to use with update panel in .NET 3.0.  

**Aspose.Workflow for .NET**  

_New Features_  

1. New XPDL Designer with multi version support  

2. Ability to upload XPDL (1.0 or 2.1) packages using new Aspose.Workflow Engine  

3. Ability to manage existing applications or create new applications using same API  

4. Ability to suspend or resume a process at runtime.  

5. Get Assigned Users for a Task.  

6. Exception management.  

7. Added "Description" property for Activity.  

8. Export package to PDF.  

9. Save package as BMP, JPG, GIF, and PNG.  

10. Print package.  

11. Added plugins support.  

_Bug Fixes_  

1. Error: Formal Parameter and Actual Parameter length does not match.  

2. Exception "There are no starting activities in the process - can't start it!”  

3. Misc Designer issues.  

4. Exception in toolagents editor.  

5. Increase performance.  

**Download Aspose.Total for .NET:**  

<figure class="wp-block-embed"><div class="wp-block-embed__wrapper">http://www.aspose.com/community/files/50/product-suites/aspose.total-for-.net-and-java/default.aspx</div></figure>









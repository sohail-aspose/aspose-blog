---
title: 'Aspose.Total for Java Q3 2009'
date: Wed, 30 Sep 2009 22:35:00 +0000
draft: false
url: /2009/09/30/aspose-total-for-java-q3-2009/
author: Muhammad Rashid
summary: ''
tags: []
categories: ['Aspose.Total Product Family']
---

**What’s New in Aspose.Total for Java Q3 2009:**

**Aspose.Words for Java**

_New Features_

1. “Quick Parts” are converted to plain text after open/save DOCX file using Aspose.Words.

2. Consider an ability to allow inserting fields with custom field codes.

3. Add attribute "style:display-name" export for style elements.

4. Add generator name with version number to meta.xml.

5. Add "table:table-columns" element import.

6. Add "style:default-outline-level" attribute export for "style:style" element.

7. Add "style:vertical-align" attribute import for "style:table-cell-properties" element.

8. Parent style of table style is not imported.

9. Add import of "fo:hyphenate" attribute of "style:text-properties" element.

10. Add "table:number-rows-spanned" attribute import.

11. Add "style:writing-mode" attribute import in "style:table-cell-properties" element.

12. Add "text:date" and "text:author-name" fields import/export.

13. Add "text:file-name" field import/export.

14. Add "table:table-row" -> "table:number-rows-repeated" attribute import.

15. Add "table:table-row" -> "table:default-cell-style-name" attribute import.

16. Add "style:paragraph-properties" -> "style:drop-cap" -> "style:length" attribute import/export.

17. Add SaveOptions.OdtExportStrictSchema.

18. Add import of parent style for spans and fields.

19. Add "style:style"->"style:master-page-name" attribute export for section style.

20. Add "style:paragraph-properties" -> "text:number-lines" import.

21. Add "style:paragraph-properties" -> "fo:orphans" and "style:paragraph-properties" -> "fo:widows" import for all styles.

22. Add "style:table-properties" -> "style:width" import.

23. ODT load and save have reached the "production" level.

24. Improved support for CSS when loading HTML.

25. Support for loading encrypted DOCX documents.

26. Glossary Document and Building Blocks are supported in DOCX documents.

27. Support loading w:pgNum.

28. Expose all BuiltInDocumentProperties as Properties.

29. Add an option to move to a merge field in DocumentBuilder without deleting the field.

30. Add the Document.OriginalLoadFormat property.

31. Make Document.DetectFileFormat detect pre-Word97 documents.

32. Make Document.DetectFileFormat detect encrypted documents.

33. Add "draw:line" import.

34. Add line shape export.

35. Add rectangle shape export/import.

36. Add ellipse shape export/import.

37. Add "text:variable-set" import and export.

38. Add "text:bookmark-start" and "text:bookmark-end" import.

39. Add "meta:user-defined" and "text:user-defined" import/export.

40. Add attribute "style:background-transparency" import/export for "style:graphic-properties" element.

41. Add "table:covered-table-cell" and "table:number-columns-spanned" import.

42. Add import of percental font size.

_Bug Fixes_

1. List labels are displayed improperly after inserting HTML.

2. Shape.Rotation changes width and height with some angles.

3. “Found XXXPropRMarkEx sprm with unknown value.” Exception occurs during opening document.

4. Document cannot be opened by Word2000 after converting HTML to DOC if HTML contains nested tables.

5. Generated file hangs or crashes MS Word 97, 2000 and 2002.

6. Some WordArt shapes are not displayed after open/save the document.

7. Document can’t be opened by MS Word 2000 after open/save it using AW.

8. “Cannot find a piece for the position” exception occurs during opening document.

9. “Cannot read array shape property” exception occur during opening document.

10. “Unexpected number of reserved styles in the stylesheet” exception occurs during opening document.

11. “Read wrong number of bytes from Escher record” exception occurs during opening document.

12. “Read wrong number of bytes from Escher record” exception occurd during opening document.

13. “Found XXXPropRMarkEx sprm with unknown value” exception occurs upon opening the document.

14. “Found XXXPropRMarkEx sprm with unknown value” exception occurs upon opening the document.

15. DOC file is corrupted after converting RTF document to DOC.

16. “OutOfMemoryException” exception occurs during opening the document.

17. Document cannot be opened in MS Word 2002.

18. Position of the shape is changed after open/save DOC file.

19. Table borders are changed after open/save document.

20. “Read wrong number of bytes from Escher record” exception occurs during opening the document.

21. “FileCorruptedException” exception occurs during opening the document.

22. Word 2002 (XP) shows error message when try to open Document produced by Aspose.Words.

23. “FileCorruptedException” exception occurs during opening a document.

24. “FormatException” exception occurs during opening DOC file.

25. Aspose.Words corrupt formatting of the document after open/save.

26. “ArgumentOutOfRangeException” exception occurs during saving the document.

27. Aspose.Words eats all memory and hangs during opening the document.

28. Word 2003 eats 100% of CPU and hangs during opening document produced by Aspose.Words.

29. Document cannot be opened in MS Word after Open/save the document using Aspose.Words.

30. “End of paragraph is out of sync” exception occurs upon opening document.

31. Stack-overflow exception while opening DOC.

32. AutoFit option read from DOC is incorrect.

33. “FileCorruptedException” exception occurs upon opening DOC file.

34. Support loading encrypted DOCX documents.

35. “FileCorruptedException” occurs when try to open DOCX zipped by Java-Util-Zip-Classes.

36. “ArgumentException” exception occurs during saving document in WML/DOCX format.

37. “FileCorruptedException” exception occurs during opening DOCX document.

38. “UnsupportedFileFormatException” exception occurs during opening DOCX document.

39. “UnsupportedFileFormatException” exception occurs during upening DOCX document.

40. “FileCorruptedException” exception occurs during opening DOCX document.

41. Word 2007 SP2 says "file was created using a newer version of Microsoft Word" when opening a file created by Aspose.Words.

42. “FileCorruptedException” exception occurs when try to open encrypted DOCX file.

43. “UnsupportedFileFormatException” exception occurs when try to open DOCX document.

44. “FileCorruptedException” exception occurs during opening DOCX document.

45. DOCX produced by Aspose.Words crashes MS Word.

46. DOCX produced by Aspose.Words cannot be opened in MS Word.

47. Table cells have different paddings in DOC and DOCX.

48. DOCX produced by Aspose.Words cannot be opened in MS Word.

49. Roundtrip section breaks in HTML export and import.

50. \[br style="page-break-before: always"/\] causes an extra empty paragraph at the beginning of the page.

51. Numbered lists with bulleted number style are exported to HTML incorrectly.

52. List with multiple levels is not converted correctly to HTML.

53. Explicitly reset italic attribute not roundtripped through HTML.

54. Content is missed during loading HTML document.

55. Aspose.Words cannot find an image is folder name contains white space.

56. Incorrect encoding detected during HTML import results in gibberish.

57. Not all CSS stylesheet was parsed exception during loading HTML.

58. Text is wrapped when using horizontal cell merging.

59. Table imported from HTML incorrectly.

60. CCS parser reads font-family improperly, if font name contains white spaces.

61. List in footnote or endnote handled incorrectly, not closed.

62. List bullets are imported incorrectly.

63. Output is incorrect when a section break occurs in a field.

64. Aspose.Words cannot find an image if folder name contains white space.

65. Cell paddings specified at row level are exported improperly.

66. Numbers in a numbered list are mangled when importing from HTML.

67. Exception during loading of an HTML file.

68. Improve importing of line breaks and implicit paragraph breaks.

69. Avoid hyperlinks overlapping with other tags.

70. Setting rotation angle for a shape greater than 45 deg does not work.

71. UpdateTableLayout works incorrectly if the table contains fields.

72. UpdateTableLayout method works not properly with horizontally merged cells.

73. DetectFileFormat throws “InvalidOperationException” exception, when try to detect format of a corrupted document.

74. “InvalidCastException” exception occurs upon saving the document to any format except DOCX and TXT.

75. GetImageSize return negative Height, when get size of BMP image.

76. Font is changed after open/save, when font is defined in Table Style.

77. Table styles are lost after ImportNode.

78. List labels are displayed improperly after inserting HTML.

79. NullReferenceException exception occurs when call JoinRunsWithSameFormatting after Save.

80. Shape Width and Height are swapped depending on the rotation angle.

81. NullReferenceException occurs upon converting the document to ODT.

82. Style of numbering "bullet" is exported as "number".

83. ODT document produced by Aspose.Words is corrupted.

84. Style font is exported incorrectly when font and base style are not set.

85. “FileCorruptedException” exception occurs during opening ODT document when "Standard" style is missing in ODT file.

86. OOo throw exception when opens file after export because incorrect symbols in value of "meta:user-defined" element.

87. OOo throw exception when opens file after export because incorrect symbols (") in attribute value of "text:user-defined" element.

88. OOo throw exception when opens file after export when document contains smart tag.

89. OOo throw exception when opens file after export when field start and field end are in different paragraphs.

90. OOo throw exception when opens file after export when bookmark start and bookmark end are in different table cells.

91. "System.InvalidOperationException: Opened initial tag XML is missing" when first paragraph of table cell is list item and last paragraph in previous table cell is not list item.

92. "System.InvalidOperationException: Opened initial tag XML is missing" when the list element is section end and the next list element is section start.

93. OOo throw exception when opens file after export when hyperlink contains symbol '&'.

94. OOo throw exception when opens file after export when field contains a paragraph break.

95. "Cannot find part ..." exception when picture path is "http\*", "https\*" or "file\*" during import.

96. NullReferenceException during import.

97. Element "text:s" is imported incorrectly.

98. The first 16 Istd of builtin styles should be given to special styles (see StyleIndex constants).

99. Empty borders in styles properties collections.

100. “UnsupportedFileFormatException” exception occurs when try to open ODT document created by Windows 7 WordPad.

101. NullReferenceException when "Standard" master page is missing (ODT document created by Windows 7 WordPad).

102. System.InvalidOperationException: Cannot find part '/settings.xml' when ODT document created by Windows 7 WordPad.

103. "meta:creation-date" and "dc:date" elements are imported variously on different computers because of various settings of time zones.

104. System.InvalidOperationException: "The built-in styles Normal and Default Paragraph Font cannot be based on any style" during import.

105. System.ArgumentOutOfRangeException : parameter name distanceFromText during import.

106. "System.InvalidOperationException: Opened initial tag XML is missing" when run has revisions.

107. Top half of text line is not visible after export.

108. Superfluous page in the document end after export.

109. "\_20 \_" in a style name should be replaced with space during import.

110. Parent style of text styles is imported incorrectly.

111. Run properties are not imported in hyperlink.

112. The "None" value of "text-line-through-style" attribute is not imported.

113. Superfluous span in FieldNumPages and FieldPage after export.

114. Empty "style:tab-stops", "style:paragraph-properties", "text:span", "style:style" elements after export.

115. Parent style "citation-style-name" and "citation-body-style-name" in "text:notes-configuration" are is not imported.

116. Run properties of list level are exported incorrectly.

117. Files are various after export->import->export because of errors of rounding.

118. Frame width and height are various after export->import->export.

119. "style:flow-with-text" attribute of "style:graphic-properties" element is various after export->import->export.

120. "fo:padding\*" attributes of "style:paragraph-properties" element are various after export->import->export.

121. "fo:font-weight", "style:font-weight-\*" and "fo:font-style\*" attributes of "style:text-properties" element should not be exported when value is "normal".

122. "style:text-properties" element is imported incorrectly for field content.

123. Superfluous "text:span" inside "text:span" after export when FieldType.FieldMergeField.

124. Bookmarks should not be exported into form field content.

125. Bookmarks in header and footer is exported into "office:text" content.

126. Section break paragraph vanishes after export->import->export.

127. "meta:type" attribute of "meta:user-defined" element is not imported.

128. "table:number-columns-spanned" and "table:number-rows-spanned" are exported incorrectly.

129. Remove using StyleType.Table in reader because it is not supported in AW model

130. Font size is various after export->import->export.

131. "style:num-format" in "text:list-level-style-number" element is imported incorrectly when it is not defined.

132. "style:default-outline-level" in "style:style" element is imported incorrectly when it is not defined.

133. Value "Standard" of "style:parent-style-name" attribute in style of heading is imported incorrectly.

134. "style:master-page-name" in "style:style" element is exported incorrectly when header or footer.

135. "style:text-properties" is not imported when span in "text:drop-down".

136. "fo:font-size" is imported into paragraph property instead of to run property when paragraph contain column break.

137. "style:line-height-at-least" is exported instead of "fo:line-height" in "style:paragraph-properties" element.

138. Superfluous "style:page-layout" and "style:master-page" after export.

139. "style:writing-mode" value is not taken into consideration during import of "fo:text-align" attribute in "style:paragraph-properties" element.

140. Error of rounding in "style:position" of "style:tab-stop" element.

141. "style:text-underline-style", "style:text-underline-type", "text-underline-mode" in "style:text-properties" are imported incorrectly.

142. Error of rounding in "style:text-position" of "style:text-properties" element.

143. "style:leader-style" in "style:tab-stop" element is exported incorrectly when TabLeader.MiddleDot.

144. Percentage value of "fo:line-height" attribute in "style:paragraph-properties" element is not rounded to integer.

145. Default value of "style:tab-stop-distance" attribute is incorrectly after import.

146. Paragraph.ParagraphFormat.SuppressLineNumbers is exported incorrectly.

147. Exception when style:default-outline-level="" during import.

148. Paragraphs styles are lost when the text contains "\\r\\n".

149. Spaces in the paragraph beginning and after line break are imported incorrectly.

150. Exception when length value is percent during import.

151. Line break and tabulation are lost after import.

152. ODT produced by Aspose.Words is corrupted, and cannot be opened by OpenOffice.

153. Import hang-up when font size is percentage value.

154. Exception when name duplication of "meta:user-defined" element.

155. OOo throw exception when opens file after export (TestDuplicateSti, TestDefect4977, TestDefect1340, TestDefect1575).

156. Oo throw exception when opens file after export when list in comment.

157. Oo throw exception when "draw:rect" element contains "text:p" element.

158. Table and cell widths are imported incorrectly by ODT reader.

159. Font size export is incorrect for normal paragraph style and default paragraph style when font size is not set.

160. "style:master-page-name" attribute in "style:paragraph-properties" element is not imported when ODT file has been created by "KOffice/2.1 Alpha".

161. Date styles are mixed when style of date field is not set.

162. "style:table-cell-properties" -> "fo:border" attribute import does not work when "in", "mm" or "pt" units.

163. "table:table-column" -> "table:number-columns-repeated" attribute import does not work when table style is not set.

164. default value of "style:columns"-> "fo:column-gap" attribute should be 0 instead of 1.27cm during import.

165. Default tab stop value ("style:paragraph-properties" -> "style:tab-stop-distance") should be 2cm instead of 0cm when it is not set during import.

166. "style:tab-stop" is imported incorrectly when attribute style:type="char" and attribute "style:char" is set.

167. "style:paragraph-properties" -> "fo:line-height" is imported incorrectly when units is not set.

168. "text:list-item" -> "text:start-value" is exported incorrectly.

169. Pictures of zero length are exported.

170. Incorrect value of "meta:user-defined" element after export - System.Byte\[\].

171. Background color of paragraph is exported incorrectly when Shading.Texture == TextureIndex.TextureSolid.

172. Page margins are exported incorrectly when they are not set.

173. Cells, rows and tables are lost after export.

174. List item numbering is incorrect.

175. Run properties are exported/imported incorrectly.

176. "text:notes-configuration"-> "style:num-format" attribute is imported incorrectly when it is not set.

177. "text:bookmark-end" element is exported without "text:bookmark-start" element.

178. "text:s" -> "text:c" attribute is exported incorrectly.

179. Empty spans when fields export/import.

180. "text:variable-set" -> "text:name" attribute and "text:variable-set" element value are exported/imported incorrectly.

181. Header and footer styles are exported though there are no headings corresponding to them.

182. Paragraph tab stops are exported/imported incorrectly when its parent style contains tab stops.

183. RTF generated by Aspose.Words for reporting service includes empty rows between data rows.

184. “Unknown structure of an INCLUDEPICTURE field.” exception occurs during opening RTF document.

185. Table is narrowed and unexpectedly repeated on every page.

186. Two tables appear as one after RTF import.

187. Background from one cell is propagated to another on RTF import.

188. Font is changed from Arial to Times New Roman after open/save RTF document.

189. “FileCorruptedException” exception occurs during opening RTF document.

190. “FileCorruptedException” exception occurs during opening RTF document.

191. “NullReferenceException” exception occurs during saving DOC in RTF format.

192. “InvalidCastException” exception occurs upon opening RTF document.

193. Image size is incorrect when save document to RTF.

194. Size of EMF image is incorrect when save document to RTF.

195. Left margin of table is changed after open/save RTF document using Aspose.Words.

196. FieldStart and FieldEnd nodes are not removed when AcceptAllRevisions.

197. RTF output size is too large.

198. “FileCorruptedException” exception occurs during opening RTF documents.

199. “FileCorruptedException” exception occurs upon opening RTF document.

200. Exception: 'Unknown structure of an INCLUDEPICTURE field.'

201. All document contents are imported to header.

202. “Footnote separators are expected to be processed at the document level” exception occurs during opening the document.

203. Document background goes black on some documents.

204. List bullets are converted to wrong characters.

205. Numbered bullets are shown improperly after converting HTML to DOC.

206. Texbox width is read incorrectly.

207. “sprmPCrLf is not yet supported” exception occurs during opening document.

208. Part of content disappears during printing document generated by AW.

209. “FileCorruptedException” exception occurs upon opening the document.

210. “End of paragraph is out of sync.” Exception occurs upon opening the document.

211. Word 2003 eats 100% of CPU and hangs during opening document produced by Aspose.Words.

212. “End of paragraph is out of sync” exception occurs upon opening document.

213. Range.Replace method works very slowly on DOCX document.

214. “FileCorruptedException” exception occurs during opening DOCX file that contains embedded DOCX file.

215. Loading a document where the same footer is referenced twice fails.

216. Word 2007 SP2 says "file was created using a newer version of Microsoft Word" when opening a file created by Aspose.Words.

217. Roundtrip section breaks in HTML export and import.

218. \[br style="page-break-before: always"/\] causes an extra empty paragraph at the beginning of the page.

219. Numbered lists with bulleted number style are exported to HTML incorrectly.

220. List with multiple levels is not converted correctly to HTML.

221. All text content disappears when open/save HTML document.

222. InsertHtml inserts paragraph as RTL.

223. Text size is incorrect upon inserting HTML into the document.

224. Bullets are lost when insert HTML in Turkish culture.

225. “Unexpected table parent.” Exception occurs during inserting HTML table into the TextBox.

226. “InvalidOperationException” exception occurs upon save document in HTML format.

227. Explicitly reset italic attribute not roundtripped through HTML.

228. Content is missed during loading HTML document.

229. Bullets are shown improperly after converting HTML to DOC.

230. Background color becomes blue after converting the document to HTML.

231. Allow specifying folder for exported images when saving to file.

232. Import and Export PageSetup for each section to HTML.

233. Support < center >< /center > tags.

234. “Start and end node should have the same grand parent.” Exception occurs when try to move DocumentBuilder cursor to merge field.

235. Some mergefields in the document are not recognized in AW3.0.1.

236. Date is converted to UTC (original timezone lost) when use datetime format in mergefield.

237. MailMerge fails on documents with IF fields spanning several sections.

238. Add throwing exception when attempt to create too long form field or bookmark names.

239. A document throws InvalidCastException when combining documents.

240. “System.InvalidOperationException” exception occurs during Updating fields.

241. Exception occurs during updating fields in the document.

242. Unprotect method does not remove “Password to modify”.

243. Allow save file without extension when SaveFormat is specified.

244. Exception occurs when try to move DocumentBuilder to the inline node iside SmartTag.

245. FormField.Result does not rerun correct value of the formfield.

246. Exception occurs when try to move DocumentBuilder to the inline node iside SmartTag.

247. DocumentProperty.toDateTime() getter returns obfuscated internal value instead of java.util.Date.

248. FormTextInput Field starting with newline cases nullpointer exception when calling field.Result.

249. “NullReferenceException” exception occurs upon savint file to ODT.

250. FormField name is moved to HelpText and Result is empty when open ODT.

251. Paragraph text properties are not imported to a run properties of field.

252. Superfluous page break when paragraphs has differents "style:master-page-name".

253. FormField.Result is lost during export to ODT.

254. Font of FormField is reset to “Times New Roman” after open/save the document.

255. Improve performance of ODT.

256. Texbox becomes with blue background after open ODT/save DOCX ODT.

257. Exception "System.ArgumentException: Cannot add a style because a style with the same name already exists." during document import.

258. System.ArgumentNullException during document import.

259. Hyperlink to a bookmark does not work after export.

260. Style of numbering "bullet" is exported as "number".

261. Paragraph wraps a picture incorrectly after export.

262. System.NullReferenceException during shape export.

263. "System.InvalidOperationException: Opened initial tag XML is missing" when headings are used in different sections.

264. "text:list-header" element content is not imported.

265. Formatting of heading is missing after import ODT and export DOCX.

266. Content of "text:table-of-content" element is missing after import.

267. "System.ArgumentException: This style is not a paragraph style" during import.

268. Unnecessary page break when style contains fo:break-before="auto" and parent style contains fo:break-before="page".

269. Table structure is imported incorrectly when document contains "table:covered-table-cell" an element.

270. The document text is not imported after element "draw:circle".

271. Element "style:text-properties" is not imported for style of element "text:h".

272. “FileCorruptedException” exception occurs during opening ODT document.

273. RTF generated by Aspose.Words for reporting service includes empty rows between data rows.

274. “Unknown structure of an INCLUDEPICTURE field.” exception occurs during opening RTF document.

275. Table is narrowed and unexpectedly repeated on every page.

276. Two tables appear as one after RTF import.

277. Background from one cell is propagated to another on RTF import.

278. Font is changed from Arial to Times New Roman after open/save RTF document.

279. “FileCorruptedException” exception occurs during opening RTF document.

280. “FileCorruptedException” exception occurs during opening RTF document.

281. Can’t open output RTF file when use Aspose.Words in evaluation mode.Bottom of Form.

282. “NullReferenceException” exception occurs during saving DOC in RTF format.

283. “InvalidCastException” exception occurs upon opening RTF document.

284. Image size is incorrect when save document to RTF.

285. Size of EMF image is incorrect when save document to RTF.

286. Left margin of table is changed after open/save RTF document using Aspose.Words.

287. Exception: 'Unknown structure of an INCLUDEPICTURE field.'

288. All document contents are imported to header.

**Aspose.Cells for Java**

_New Features_

1. Add new features for Open Document Spreadsheet file(ODS): Hyperlink, Page Setup options, Group outline, Conditional formatting, Data validation, AutoFilter, Page Break, PrintTitleRows/Columns, Shapes related objects(Comment, Arc, Button, CheckBox, ComboBox, GroupBox, GroupShape, Label, Line, ListBox, OleObject, Oval, Picture, RadioButton, Rectangle, ScrollBar, Spinner, TextBox), Chart.

2. Provide new features for MS Excel 2007 file format: Inserting Pictures, Adding Charts.

3. Support to update controls via the linked cell(s), and vice versa: CheckBox, ComboBox, ListBox, RadioButton, ScrollBar, Spinner.

4. Access Shape’s properties: Name, ZOrderPosition.

5. Apply Subtotals to worksheet tables.

6. Calculate Hyperlink function.

7. Delete user defined Names.

8. Include AutoFilter attributes when copying Workbook/Worksheet.

9. Support for hyperlinks in xls2pdf conversion.

10. Extract Ole Objects in the template file.

11. Fixed some bugs for R/W ODS.

_Bug Fixes_

1. Hyperlink's address.

2. Template files that contains large MSODrawing data.

3. Update controls via the linked cell, and vice versa.

4. Shape's name and ZOrderPosition.

5. Formula.

6. Comment.

7. Strong Workbook Encryption.

8. Cell.getStringValue() for rounding decimal values.

9. Reading template files that contain both BIFF7 and BIFF8 records.

10. PageSetup.Print\_Titles/Print\_Areas.

11. Merge cells.

12. Axis of Chart.

13. SUBTOTAL function.

14. Hyperlinks for xls2pdf.

15. Worksheet.unFreezePanes/freezePanes.

16. Dynamic formulas in SmartMarker.

17. SmartMarker with horizontal flag.

18. Closes user’s output stream.

19. Reading template file that created by Microsoft Jet Engine.

20. Importing/exporting CSV file format.

21. Merged cells in xls2pdf.

22. Style.isCellLocked() property for Excel2007 file format.

23. Set picture's size in Header/Footer of PageSetup.

24. Row height for Excel2007 file format.

25. Deleting user defined Name.

26. Column width.

27. Validation.

28. Formula HYPERLINK.

29. Date value for SmartMarker.

30. Checkbox.

31. Setting linked cell for controls.

32. Setting FitToPagesWide/FitToPagesTall property of PageSetup.

33. ROUND formula.

34. Style of non-standard xls template file created by Jsperreport

35. Shape properties.

36. Copy AutoFilter when copying Worksheet/Workbook.

37. SpreadSheetML.

38. Nonstandard xlsx file generated by some other tools than MSExcel.

39. OleObjects.

**Aspose.Slides for Java**

_Bug Fixes_

1. Incorrect reading vertices of custom autoshape represented by 64bit values.

2. FillFormat.getType() returns PATTERN instead of SOLID.

3. Exception while Getting Presentation object.

4. Exception when opening PPTX.

5. Transparency of a PictureFrame is not rendered.

6. PPTX porting from Aspose.Slides for .NET.

**Aspose.Pdf.Kit for Java**

_New Features_

1. Get currently selected value of the radio group.

2. Determine valid radio group values.

_Bug Fixes_

1. Text extracting feature is improved.

2. Special characters support / Unicode characters support.

3. extractText hangs and doesn't return.

4. Determine valid radio group values.

5. Reading input stream hangs.

6. PdfExtractor read wrong data.

**Aspose.Metafiles for Java**

_Bug Fixes_

1. Workaround for the incorrect processing of font glyphs in JRE 1.5 where GlyphVector.getGlyphCharIndices() returns char indexes in a wrong order.

**Aspose.Report for Java**

_New Features_

1. First version of Aspose.Report for Java has been released. Aspose.Report for Java enables users to create charts and add ad hoc capabilities to their Java applications. Aspose.Report for Java 1.0.0 includes aspose.report.adhoc.facelets and aspose.report.chart sub-components.

**Download Aspose.Total for Java:**

[http://www.aspose.com/community/files/72/java-components/aspose.total-for-java/default.aspx][1]




[1]: https://docs.aspose.com/display/wordsjava/Home





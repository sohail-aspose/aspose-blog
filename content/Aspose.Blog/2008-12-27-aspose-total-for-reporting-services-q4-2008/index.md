---
title: 'Aspose.Total for Reporting Services Q4 2008'
date: Sat, 27 Dec 2008 05:28:00 +0000
draft: false
url: /2008/12/27/aspose-total-for-reporting-services-q4-2008/
author: Salman Sarfraz
summary: ''
tags: []
categories: ['Aspose.Total Product Family']
---

**What’s New in Aspose.Total for Reporting Services Q4 2008:**

**Aspose.Words for Reporting Services**

_New Features_

1. Full support for Microsoft SQL Server 2008 Reporting Services (including tablix, richly formatted textboxes, and other features).

2. Document layout is improved for better balance between the precision of export and the editability of the document.

3. Added the PageBreaks configuration setting that allows to easily control how page breaks are inserted into the document.

4. The FlowMode configuration setting was dropped due to being ambiguous and unclear.

5. Some of the configuration settings were renamed for simplicity purposes. Old names are still valid to support backward compatibility.

6. Positioning of items is optimized in order to reduce the number of positioning tables and simplify their structure (flow layout only).

7. Added the ODT (OpenOffice/StarOffice OpenDocument) export format.

8. License model is changed for the case of integration with Report Viewer.

9. Based on the newest Aspose.Words for .NET 6.0. 

_Bug Fixes_

1. Group page breaks worked incorrectly.

2. Some complex matrices could have extra empty rows inserted.

3. Page contents often appeared higher than the page (flow layout).

4. Empty space at the end of the page did not provide a decent level of items positioning (items could be shifted throughout the document). Was replaced with page breaks (flow layout).

5. Repeatable headers/footers could appear in the middle of the page due to the shift throughout the document. Were dropped for the cases when the shift may appear with high probability.

6. Other minor fixes.

**Aspose.Cells for Reporting Services**

_New Features_

1. Integrate with Microsoft Report Viewer in Local Mode.

2. Improved rendering performance.

3. Supported 64-bit Operating Systems.

4. Improved support for nesting tables.

_Bug Fixes_

1. Fixed a bug with setting page size.

**Aspose.Pdf for Reporting Services**

_New Features_

1. Supported PDF/A-1 (Electronic document file format for long term preservation - Part 1: Use of PDF 1.4).

2. Supported bookmarks.

3. Supported the feature of inline HTML with Textbox (currently not all HTML tags are supported; please refer to HTML Tags in Text).

4. Optimized the algorithm of position, which reduces the nested level of table.

5. Improved the performance of rendering engine.

_Bug Fixes_

1. An exception would occur when the URL of hyperlink in textbox contains some special character such as '&'.

2. Permission problem which results in the failure of rendering reports.

3. Some footnotes and endnotes could not display correctly when using inline HTML.

4. The disorder of table group and table detail when they are cascade.

5. Fixed an error related to the display of custom color, such as ‘#12e32f ’, which is used for setting font and background colors.

6. Rectangles are not displayed correctly when nested in the header or footer.

7. When list is nested with the report item sub-report, its position is incorrect.

8. Fixed few bugs related to some special report items that could not locate correctly when more than one column is set for pages.

9. Fixed few bugs related to tables that usually use the same paragraph ID as the textboxes within tables.

10. Problem in report items when textbox is set to be auto-shrinking or auto-expanding.

11. Rectangle could not display in proportion when it has no content.

12. Disorder of table’s group when they are nested.

13. Fixed the algorithm which could generate a unique paragraph ID for every report item.

**Aspose.Slides for Reporting Services**

_New Features_

1. Merged with latest stable version of Aspose.Slides for .NET.

_Bug Fixes_

1. Bold, Italic and Underlined fonts are not rendered properly in some cases.

2. Wrong rendering of a matrix. Bottom borders are not rendered or rendered at wrong position.

3. Size of slides is not equal to the page size in RDL reports.

4. FitShapeToText didn't work in previous versions so it was possible that long text blocks didn't fit to calculated rectangles.

5. Text could be cut off in case it doesn't fit to a rectangle and CanGrow property set to false.

6. No text background for summary and some other fields.

**Aspose.BarCode for Reporting Services**

_New Features_

1. Supported International Standard of Application Identifiers (AI) for EAN128.

2. Supported rendering barcode images to report header.

3. Enhanced support for SQL Server 2000 Reporting Services.

4. Upgraded the configuration tool to support SQL Server 2000 Reporting Services configuration.

_Bug Fixes_

1. Code39 barcode width couldn’t set properly.

**Download Aspose.Total for Reporting Services:**

[http://www.aspose.com/community/files/50/product-suites/aspose.total.reporting.services/category1222.aspx][1]




[1]: http://www.aspose.com/community/files/50/product-suites/aspose.total.reporting.services/category1222.aspx





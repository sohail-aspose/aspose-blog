---
title: 'Aspose.Grid 1.5.2 released!'
date: Wed, 08 Mar 2006 23:57:00 +0000
draft: false
url: /2006/03/08/43581/
author: Henry
summary: ''
tags: ['Henry Xu']
---

We have released Aspose.Grid 1.5.2!

**Release Notes**

Aspose.Grid.Web

*   Fixed: client-side setting color bug
*   Fixed: TableStyle/TableItemStyle CssClass property doesn't take effect bug
*   Support Creating Pivot Table Reports
*   Support client-side multi-cells select/copy/cut/paste/set style
*   Support client-side right-click menu operations: freeze/unfreeze; insert/delete row/column; merge/unmerge cells;
*   Support Hyperlinks(Text or Image Display, UrlLink or CellCommand Action)
*   Added properties: ActiveCell, EnableClientColumnOperations, EnableClientFreeze, EnableClientMergeOperations, EnableClientRowOperations, SelectCells
*   Added Methods: WebCells.GetColumnReadonly, WebCells.SetColumnReadonly, WebCells.GetRowReadonly, WebCells.SetRowReadonly
*   Added events: SheetDataUpdated, LoadCustomData(for Sessionless mode data recovering), CellCommand, ColumnDeleted, ColumnInserted, RowDeleted, RowInserted, PageIndexChanged
*   Changed: Now the client file web-path(/agw\_client) and the client files(htc, gif, etc.) are not needed in deploying environment. These files are now embedded in the control. This simplifies the deploying and upgrading operations.

 Aspose.Grid.Desktop

Enhanced:

*   Column header text Supported.
*   Context menu Supported.
*   Hyperlinks, comments, pictures exporting supported.
*   Cell button, checkbox, combox supported.
*   CellClick, CellDoubleClick, CellKeyPressed events supported.
*   Applying style to range of cells supported.
*   Data validation supported.

Fixed:

*   Minimizing the form that contained the GridDesktop control which set the Dock property Fill, an exception is thrown.
*   Pressing "delete" key, the GridDesktop control does not raise CellDataChanged event.
*   When row number is greater than 4 digitals, row header's width is not enough.
*   When load from excel file, the font of char that input in a cell is different from the font of cell.
*   Can't input Enter in a cell, now use Control + Enter keys.
*   If there are not focused cells, textbox control will be placed at error position when input char.
*   There is a comment in a cell, and then focused the right cell; when point to the cell that contains a comment, the focused cell will glint always.
*   Hiding row column does not work.








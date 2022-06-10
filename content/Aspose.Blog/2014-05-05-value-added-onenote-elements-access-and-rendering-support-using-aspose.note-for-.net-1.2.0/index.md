---
title: 'Value-added Access to OneNote Elements and Rendering Support in Aspose.Note for .NET 1.2.0'
date: Mon, 05 May 2014 20:06:09 +0000
draft: false
url: /2014/05/05/value-added-onenote-elements-access-and-rendering-support-using-aspose.note-for-.net-1.2.0/
author: Imran Rafique
summary: ''
tags: ['Imran.Rafique']
categories: ['Aspose.Note Product Family']
---

[![][1]](https://blog.aspose.com/wp-content/uploads/sites/2/2013/08/aspose-Slides-for-net_100.png)We are pleased to announce the release of Aspose.Note for .NET 1.2.0. From this release, the content manipulation features now offer a bit more control. This new build also allows developers to render a few more elements, for example tags, tasks, tables, attached documents and hyperlinks. The DocumentVisitor abstract class has been made more flexible. It supports start and end methods for the visiting elements of OneNote documents. This gives developers an easy approach for deciding which objects need to be visited for a given scenario.

## Important Tag Notes

Microsoft Office OneNote users  can easily add tags to find important items buried in their notes, for example tag meeting decisions, ideas, definitions, key points, billable hours, questions, people's names, books to read, and so on. The Aspose.Note for .NET API now supports rendering these tags when exporting OneNote documents to any supported file format. It also allows developers to programmatically access details about these tags. A note tag can specify the font and highlight colors for the text that is associated with the tag. Please see a complete example topic: Get Note Tag Details from a OneNote Document

## Outlook Tasks from OneNote

In Microsoft Office OneNote, users can mark follow-up items from meetings or brainstorming notes as Outlook tasks. These Outlook tasks are being carried. Developers can now access and render these using the Aspose.Note API. A task tag marks an object as a follow-up item with a due date. Please have a look on this help example topic: Get Outlook Task Details from a OneNote Document

## Table Support in the OneNote Documents

Users can organize their notes by arranging information in rows and columns as tables. The Aspose.Note API allows developers to export OneNote documents along with tables to any supported format. Developers can also access tables and their child elements. This example topic shows how to extract text from a table: Extracting Plain Text from the Table of OneNote Document

## Retrieve Attached Files from OneNote Document

All files attached to a OneNote document can be retrieved. This feature is now supported. Developers can easily find attached files after converting OneNote documents via the Aspose.Note API. Please see the following topic for further help: Retrieve Attached Files from a OneNote Document

## Preserving Hyperlinks

Aspose.Note preserves hyperlinks when the OneNote document is converted to any supported format.

## Public API Changes

The following API changes in the new version are also worth noting:

1.  A new **AttachedFile** class has been added. It represents an attached file.
2.  A new **NoteTag** class has been added. It represents a note tag.
3.  A new **Table** class has been added. It represents a table.
4.  A new **TagIcon** dictionary has been added. It specifies the icon of tag or task.
5.  The **DocumentVisitor.VisitDocument** method has been renamed to **DocumentVisitor.VisitDocumentStart**.
6.  The **DocumentVisitor.VisitImage** method has been renamed to **DocumentVisitor.VisitImageStart**.
7.  The **DocumentVisitor.VisitOutline** method has been renamed to **DocumentVisitor.VisitOutlineStart**.
8.  The **DocumentVisitor.VisitOutlineElement** method has been renamed to **DocumentVisitor.VisitOutlineElementStart**.
9.  The **DocumentVisitor.VisitOutlineGroup** method has been renamed to **DocumentVisitor.VisitOutlineGroupStart**.
10.  The **DocumentVisitor.VisitPage** method has been renamed to **DocumentVisitor.VisitPageStart**.
11.  The **DocumentVisitor.VisitPageSeries** method has been renamed to **DocumentVisitor.VisitPageSeriesStart**.
12.  The **DocumentVisitor.VisitRichText** method has been renamed to **DocumentVisitor.VisitRichTextStart**.
13.  The **DocumentVisitor.VisitSection** method has been renamed to **DocumentVisitor.VisitSectionStart**.
14.  The **DocumentVisitor.VisitTitle** method has been renamed to **DocumentVisitor.VisitTitleStart**.
15.  A few end methods have been added as **DocumentVisitor.VisitDocumentEnd**, **DocumentVisitor.VisitImageEnd**, **DocumentVisitor.VisitOutlineEnd**, **DocumentVisitor.VisitOutlineElementEnd**, **DocumentVisitor.VisitOutlineGroupEnd**, **DocumentVisitor.VisitPageEnd**, **DocumentVisitor.VisitPageSeriesEnd**, **DocumentVisitor.VisitRichTextEnd**, **DocumentVisitor.VisitSectionEnd**, **DocumentVisitor.VisitTitleEnd**, **DocumentVisitor.VisitAttachedFileEnd**, **DocumentVisitor.VisitTableEnd**, **DocumentVisitor.VisitTableCellEnd**, **DocumentVisitor.VisitTableRowEnd**. It calls after visitor visited the all children nodes.
16.  A few start methods have been added as **DocumentVisitor.VisitAttachedFileStart**, **DocumentVisitor.VisitTableStart**, **DocumentVisitor.VisitTableCellStart**, **DocumentVisitor.VisitTableRowStart**. It calls before visitor visited the first child node.

## Bug Fixes & Enhancements

We’ve fixed two error messages. The first error message occurred when loading .one (2010) document to the Document class. The second error occurred when calling the Save method. These fixes improve the loading and saving features.

To view a complete list of API features and try the API at your end, please visit the following page and [download the latest version of Aspose.Note for .NET][2]. If you need any help, please feel free to ask in the [Aspose.Note forum][3]. For more details, please visit the Aspose.Note for .NET documentation.




[1]: https://blog.aspose.com/wp-content/uploads/sites/2/2014/02/AsposeNote-for-NET-100X100.png "Aspose.Slides or .NET logo"
[2]: http://www.aspose.com/community/files/51/.net-components/aspose.note-for-.net/default.aspx
[3]: http://www.aspose.com/community/forums/aspose.note-product-family/522/showforum.aspx





---
title: 'Support for DrawingML Textboxes and Many Other Improvements in Aspose.Words 14.11.0'
date: Mon, 08 Dec 2014 12:55:35 +0000
draft: false
url: /2014/12/08/drawingml-textboxes-supported-and-many-other-improvements-in-aspose.words-14.11.0/
author: Awais Hafeez
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---

[](http://www.aspose.com/.net/word-component.aspx)Aspose.Words 14.11.0 has been released. This month’s release contains over 110 useful new features, enhancements and bug fixes to the Aspose.Words products.

You can download the latest releases of Aspose.Words from the following links:

*   [Aspose.Words for .NET 14.11.0][1]
*   [Aspose.Words for Java 14.11.0][2]

Here is a look at just a few of the biggest features and API changes in this month’s release. For a full list of bug fixes and improvements please refer to the download pages in the links above.

*   Improved clipping of text frames and computation of text wrapping bounds.
*   Public API for controlling the colors of move revisions for rendering to fixed formats.
*   DrawingML textboxes supported.
*   Improvements to exporting of numbered and nested lists to HTML.
*   Improved rendering of inline Office math equations objects.
*   DrawingML image rotation is now preserved while rendering to fixed page formats.

## BuiltInDocumentProperties.NameOfApplication Property Added

In previous versions of Aspose.Words, the field NameOfApplication in the document properties contained the product name with version number. Now the version number has been removed from this field.

## RevisionOptions.MovedFromTextColor and RevisionOptions.MovedToTextColor Properties Added

A public API for controlling the colors of move revisions for rendering to fixed formats has been added. The RevisionOptions class now has the following two new public read-write properties:

*   public RevisionColor MovedFromTextColor
*   public RevisionColor MovedToTextColor

## Style.Aliases Property Added

The Style.Aliases property now returns all aliases of the style as string\[\]. If style has no aliases then empty array of string is returned.




[1]: http://www.aspose.com/community/files/51/.net-components/aspose.words-for-.net/category1188.aspx
[2]: http://www.aspose.com/community/files/72/java-components/aspose.words-for-java/category1378.aspx





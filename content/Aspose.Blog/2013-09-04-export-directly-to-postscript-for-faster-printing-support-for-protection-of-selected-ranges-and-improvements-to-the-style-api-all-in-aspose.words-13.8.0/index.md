---
title: 'Export Word Document to PostScript and Protect Selected Ranges in Word Documents in C#'
date: Wed, 04 Sep 2013 04:41:48 +0000
draft: false
url: /2013/09/04/export-directly-to-postscript-for-faster-printing-support-for-protection-of-selected-ranges-and-improvements-to-the-style-api-all-in-aspose.words-13.8.0/
author: Adam Skelton
summary: ''
tags: ['Export Word documents to PostScript', 'Improved printing speed', 'Protect Selected Ranges in Word']
categories: ['Aspose.Words Product Family']
---



{{< figure align=center src="images/aspose-Words-for-net-e1378287014402.png" alt="Aspose.Words for .NET logo">}}


We are pleased to announce the monthly release of Aspose.Words for .NET and Java 13.8.0. Our newest product Aspose.Words for Android are also due for a release within the next week or so and this will mark the second release for Aspose.Words for Android. We are pleased to announce all three product releases contain more than 142 useful improvements.

You can download the latest release of Aspose.Words from the following links:

*   [Aspose.Words for .NET 13.8.0][1]
*   [Aspose.Words for Java 13.8.0][2]

Here is a look at a few of the biggest features in this month’s release. For a full list of bug fixes and improvements please refer to the download pages in the links above.

## Export Word to PostScript 3.0 Graphics Format

PostScript is a page description language known for its wide use in the electronic and desktop publishing areas. For this reason, it is often referred to as “the printer language” as it has become the de facto standard for printing quality output.

Aspose.Words for .NET and Java now supports saving directly to PostScript format (this format is not supported in Aspose.Words for Android as it does not support printing yet). This format provides an opportunity for users to improve printing performance even further by avoiding the printing framework of the platform which can add unnecessary overhead when printing via traditional means. With support for saving directly to PostScript, these commands can be sent directly to the printer.

To save a document in PostScript format simply save a document using the **Document.Save** method in the regular fashion and use a “.ps” file extension. You can also use the **SaveFormat.Ps** enumeration and the **PsSaveOptions** class which provides the standard rendering options when saving a document.



{{< figure align=center src="images/PostScriptOutput.png" alt="Aspose.Words PostScript Output" caption="A document rendered to Postscript using Aspose.Words as viewed in GSView">}}


## Support for Protection of Selected Ranges

When a Microsoft Word document has editing restrictions and is marked to allow no changes you can still add exceptions and allow specific users to edit a certain range of a document. Aspose.Words now supports working with protected ranges and can preserve them correctly when saving to and from DOC, DOCX, WML, and RTF formats.



{{< figure align=center src="images/ProtectedRanges.png" alt="A document with protected ranges" caption="A sample document with protection enabled. The yellow highlighting signifies an editable range of text">}}


Alongside this new feature is a brand new API to access and modify the various details of protected ranges in a document. This sees the introduction of two new nodes in the Aspose.Words document object model including a façade class to allow easy access of the range a single entity.

*   **EditableRangeStart –** A node in the document which identifies the beginning of an editable region. This node is inline and therefore must be a child of a paragraph.
*   **EditableRangeEnd -** A node in the document which identifies the end of an editable region. This node is inline and therefore must be a child of a paragraph.
*   **EditableRange** - A façade much like a bookmark which provides easy access to the nodes of both the start and end of the editable region.

To have a complete editable range you need an **EditableRangeStart** and **EditableRangeEnd** node with the same ID. These nodes signify where the editable range starts and ends.

You can use the constructor to create new editable ranges and the façade object provides handy methods to change user permissions or remove the range.

## Improvements to the Document Style API

This month’s release also provides further members to the already rich API for working with document styles.

*   Use **Style.Remove** to completely remove a style from a document. If the style being removed is still used in the document then all references to the style are removed from corresponding paragraphs, runs, and tables. If the base style is removed its formatting is moved to child styles and if the style to be deleted has a linked style, then both styles are removed.
*   Use **Style.IsQuickStyle** to determine if the style appears in the Quick Styles Gallery found on the toolbar ribbon. The same property can be set to either include or exclude a particular style in a document from the quick styles gallery

This is in addition to the several behind the scenes improvements to the style API and to the many improvements to the Aspose.Words API in general.




[1]: https://downloads.aspose.com/words/net
[2]: https://downloads.aspose.com/words/java





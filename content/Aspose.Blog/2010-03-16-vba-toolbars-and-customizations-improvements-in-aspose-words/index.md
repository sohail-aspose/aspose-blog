---
title: 'VBA, Toolbars and Customizations Improvements in Aspose.Words'
date: Tue, 16 Mar 2010 15:27:00 +0000
draft: false
url: /2010/03/16/vba-toolbars-and-customizations-improvements-in-aspose-words/
author: Romank
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---

If a Microsoft Word document was opened/saved or converted by an Aspose.Words version earlier than today’s Aspose.Words for .NET 8.2.1, it could exhibit the following problems:

*   Document.Open, Document.New etc macros will no longer fire.

*   VBA project digital signature might be lost.

*   Macros Window could show no macros.

*   Custom toolbars and customizations to standard toolbars could be lost.

*   Keyboard command customizations could be lost.

All of the above has now been resolved. Aspose.Words now fully preserves and converts all of the VBA and customizations data between DOC, OOXML and WordprocessingML 2003 formats.  

**Microsoft Word 2003 displays a document converted by Aspose.Words with custom toolbars and macro names preserved.**

This type of custom toolbars is “native” to Word 97 – 2003, but did you know that such custom toolbars are still supported by Microsoft Word 2007. But your custom toolbars appear on the Add-Ins tab in Word 2007.  

**Microsoft Word 2007 displays a document with custom toolbars preserved by Aspose.Words.**

**Where in the API**

**Document.HasMacros** – there was no change to this method, it returns true if the document has a VBA project.

**Document.RemoveMacros** – there was no change to this method, it removes the VBA project AND all customizations. Let us know if you prefer to have separate methods for detecting and removing customizations because we now can provide them.

**Useful Facts**

*   Aspose.Words for .NET supports toolbars and keyboard commands customizations created in Microsoft Word 97 – 2003 (such customizations are also stored in DOCX documents created by Word 2007).

*   Aspose.Words for Java does not yet have these VBA and customizations improvements but will have them in the next release within 2 months or so.

*   Word 2007 Ribbon UI customizations are not yet supported by Aspose.Words, but this feature is planned for the near future.

Download Aspose.Words for .NET from [https://downloads.aspose.com/words][1]




[1]: https://downloads.aspose.com/words





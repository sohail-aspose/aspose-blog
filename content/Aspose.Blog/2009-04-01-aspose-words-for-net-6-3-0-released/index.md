---
title: 'Aspose.Words for .NET 6.3.0 Released'
date: Wed, 01 Apr 2009 03:35:00 +0000
draft: false
url: /2009/04/01/aspose-words-for-net-6-3-0-released/
author: Romank
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---

**What's New**

*   About 50 fixes and enhancements
*   Support for Glossary Document in OOXML import/export.
*   New classes GlossaryDocument, DocumentBase, BuildingBlock and enums.

To see all fixes and download [http://www.aspose.com/community/files/51/file-format-components/aspose.words-for-.net-and-java/default.aspx][1]

**Aspose.Words Supports Glossary Documents in OOXML**

The ECMA-376 specification (2.12 Glossary Document) defines the glossary document as:

Within a WordprocessingML file, the _glossary document_ is a supplemental storage location for additional document content which shall travel with the document, but which shall not be displayed for printed as part of  the main document until it is explicitly added to that document by deliberate action.

I can add that a Glossary Document is an "invisible document inside the main document". Microsoft Word uses Glossary Documents to store AutoText, AutoCorrect entries and Building Blocks.

Earlier versions of Aspose.Words ignored Glossary Documents and therefore after an open/save cycle using Aspose.Words your Glossary Document was always missing in the output file. This is changed now.

Aspose.Words now preserves Glossary Documents during open/save cycles (in OOXML files only at the moment). Glossary Documents can occur in OOXML and in DOC files. Support for glossary in DOC will be available later.

**New Public API for Glossary Documents/Building Blocks**

**Aspose.Words.Document** was the only class to represent a document. We have added a new class **Aspose.Words.BuildingBlocks.GlossaryDocument** to represent the glossary document. You can access the glossary document from the main document using the **Document.GlossaryDocument** property.

It turned out that the main and glossary documents have so much in common that we had to factor out common functionality into a new base class **Aspose.Words.DocumentBase**. The **DocumentBase** class contains styles, lists and font definitions.

The **GlossaryDocument** class contains **BuildingBlock** nodes as its children. You can enumerate/walk nodes in the glossary document in the same way you do in the main document. You can also find a building block using the **GlossaryDocument.GetBuildingBlock** method.

You can programmatically create/modify/delete building blocks and their content in the same way as other nodes in the document tree. However, the most important use case for building blocks is inserting them into the main document at a certain location.

To insert content of a building block into the main document, one needs to copy nodes from the building block to the right place in the main document tree. This can be done in the current release, but the process is "manual". E.g. it requires a lot of coding and dealing with nodes. We are now working to add helper methods that will allow you to insert building blocks in any place in the main document using just one line of code.

See the Aspose.Words for .NET API Reference for more information on new classes and methods.

**More Work on Glossary Documents is in Progress**

Stay tuned, future releases will have more functionality:

*   Support of Glossary Documents in DOC files (and DOC to/from OOXML conversion of course).
*   Friendly methods to insert contents of a BuildingBlock anywhere in your document.
*   Documentation examples and articles about Building Blocks.




[1]: http://www.aspose.com/community/files/51/file-format-components/aspose.words-for-.net-and-java/default.aspx





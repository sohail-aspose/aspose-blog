---
title: 'Proposed Breaking Change to Sections'
date: Tue, 24 Mar 2009 01:00:00 +0000
draft: false
url: /2009/03/24/proposed-breaking-change-to-sections/
author: Romank
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---

Hi all,

When Aspose.Words was being designed 5 or so years ago there was no OOXML and even WordprocessingML was relatively new. We did our best to design a document object model that is rich yet easy to use and resembles Microsoft Word Automation.

One of the main classes is **Section**. The document object model is a tree of nodes in Aspose.Words. The root node is the **Document** object and the next level down is **Section**.

This resulted in the following tree:

**Document**

\----**Section**

\--------**Body**

\------------Block Elements (**Paragraphs** and **Tables**)

\--------**HeaderFooter**

\------------Block Elements (**Paragraphs** and **Tables**)

E.g. **Section** is a _container_ for the main text and headers/footers of a section in a document.

Nowadays when OOXML is becoming widespread we want Aspose.Words API to bear resemblance not only to Microsoft Word Automation, but to OOXML too. Well, at least we don't want to contradict OOXML.

One of the things that stands out is that in OOXML a section is not a container. In OOXML the body of the document consists of block level elements (paragraphs and tables) and some paragraphs are section breaks. When a paragraph is not just a paragraph, but also a section break it has the section formatting attributes as well as points to the headers and footers associated with this section. Both approaches have their pros and cons when working with a document programmatically.

We are pondering about changing **Section** in Aspose.Words to work more like in OOXML. This will likely to involve:

*   Delete the **Body** class.
*   **Document** will contain **Paragraph** and **Table** nodes directly.
*   Paragraph will have methods and properties to access section formatting properties. E/g. **Paragraph.SectionBreakType**, **Paragraph.PageSetup** and so on.
*   The **Section** class - I do not think we will delete it completely, but it will change from being a node in the tree into a "facade" class more like **Bookmark**.

**Implications**

The change will be quite seriously breaking. We will try to keep most of the **Section** class functionality that is available now, but if your code was relying on accessing **Section** nodes in the tree it will require rework.

**Benefits**

Some of the features that we were deferring will be able to go ahead. IF and nested fields that contain section breaks, mail merge regions with section breaks, find & replace across paragraph and section breaks. The new upcoming feature GlossaryDocument/BuildingBlock will look more "natural" when BuildingBlock will contain Paragraph/Table nodes, not Section nodes.

Do you have anything to say?









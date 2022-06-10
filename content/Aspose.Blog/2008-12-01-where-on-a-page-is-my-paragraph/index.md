---
title: 'Where on a page is my paragraph?'
date: Mon, 01 Dec 2008 11:40:00 +0000
draft: false
url: /2008/12/01/where-on-a-page-is-my-paragraph/
author: Romank
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---

Many customers wanted to access page layout information in Aspose.Words. This included questions such as:

*   Where does a page start or end in a document?
*   Where on a page my paragraph (table, shape etc) is located?
*   How can I tell how much space is left on a page?
*   Can I get the page number of a bookmark?
*   and so on

It was not possible to support any of these scenarios in Aspose.Words because Word documents are "flow-layout" documents and do not contain information about how the document is laid out into pages.

Aspose.Words for .NET 6.0 introduces a rendering engine that formats a document into pages similar to how MS Word does it. At the moment the rendering engine only supports export to PDF, printing and imaging (rendering and saving to images). But the fact that such an engine exists means that questions above and many more scenarios will be possible to implement in Aspose.Words.

In the following Aspose.Words releases we plan to start exposing some of the rendering engine in the public API to give you access to the location of document elements on pages. Let us know if you have any requirements or suggestions for the new API. Let us know what do you want to see.









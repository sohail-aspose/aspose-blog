---
title: 'Going Transitional (exporting to XHTML)'
date: Tue, 05 Sep 2006 17:01:00 +0000
draft: false
url: /2006/09/05/55917/
author: Romank
summary: ''
tags: ['Roman Korchagin']
---

A number of customers asked for Aspose.Words to produce XHTML compliant HTML when exporting and I'm happy to tell you that we did it.

Aspose.Words used to output some unclosed tags, for example <meta ...> that were okay from HTML point of view, but precluded customers from using those as XML files.

Starting from Aspose.Words 4.0, we always output well-formed XML when exporting to HTML format. It is the main point that we addressed. We also validate almost all produced test files against the XHTML 1.0 Transitional.

Although Aspose.Words produces well-formed XML, it will not validate against the XHTML DTD for all documents. Microsoft Word documents include a number of elements that turned out to be impossible to map into any of the XHTML schemas. Here are some Word things that we don't know how to map to valid XHTML:

*   Multi-level lists are quite common in Word documents, but XHTML schema seems to define only one level for lists. It is not possible to nest UL element inside an LI element according to XHTML.
*   Bookmarks in Word documents can easily span and cut through other elements of the document. A bookmark can start in one paragraph and end in another. This is a problem not only for XHTML, but for XML too. It is not possible to represent a bookmark using a single <a> element that starts in one paragraph and ends in another because the document will not be well formed. So Aspose.Words outputs only the bookmark start into HTML now.
*   Bookmarks can intermingle with each other or be completely contained within each other in Microsoft Word. This is not allowed in XHTML. The <a> elements cannot be nested. This is also solved by exporting only the beginning of the bookmark.

Since the documents produced by Aspose.Words will not always validate against the XHTML schema we made it an option to output the XHTML schema declation:

// This option is off by default.  
doc.SaveOptions.HtmlExportXhtmlTransitional = true;  
doc.Save(@"C:\\MyFile.html", SaveFormat.FormatHtml);

When HtmlExportXhtmlTransitional is turned on, the output will begin like this:

<?xml version="1.0" encoding="utf-8" standalone="no" ?>  
<!DOCTYPE html  
PUBLIC "-//W3C//DTD XHTML 1.0 Transitional//EN"  
"http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">  
<html xmlns="http://www.w3.org/1999/xhtml" xml:lang="en" lang="en">  
...








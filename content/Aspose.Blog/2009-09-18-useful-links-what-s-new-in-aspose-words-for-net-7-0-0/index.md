---
title: 'Useful Links - What''s New in Aspose.Words for .NET 7.0.0'
date: Fri, 18 Sep 2009 01:43:00 +0000
draft: false
url: /2009/09/18/useful-links-what-s-new-in-aspose-words-for-net-7-0-0/
author: Romank
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---

In the last few days we have already blogged about most of what was coming up in Aspose.Words for .NET 7.0.0 so here is just a brief recap and a collection of useful links.

**Field Update Engine V1.0**

Aspose.Words for .NET can now update fields that are most frequently used in mail merge and report generation.

It was first announced in this blog post. With some changes it became the first topic in the Working with Fields section in the documentation. We hope to see more in this section later on.

This functionality will soon appear in Aspose.Words for Java. Next versions will support update of more field types, for example TOC. TOC update is not updated in this release.

**.NET Framework 4.0, Windows 7 and Visual Studio 2010 are Supported**

To be honest, this did not require much work from us. We've just tested and it worked well. But the most interesting thing is what test projects we were building: we created a couple of samples for Windows Azure.

**Windows Azure is Supported**

The news were first published in the Running Aspose.Words in the Windows Azure Cloud blog post.

Now there is a NEW Windows Azure feature page in the documentation.

There is also the Windows Azure Platform section in the Programmers Guide that contains more technical information and How-to articles for the samples we've created.

We take Windows Azure seriously and will fully support all your requests in the forums. There are more sample projects (and probably specialized features) for Windows Azure in the pipeline.

**Conversion to PDF Works on Mono**

First mentioned in this blog post.

Now we have a How-to: Run Aspose.Words with Mono article in the documentation.

Please note we have only tested on openSUSE 11.1 so far and not tested on other operating systems. Conversion to PDF works well in most cases (very similar to the way it works on .NET), but it still has a few rough edges, especially about configuring TrueType fonts renderer on Linux for better (more accurate from the Aspose.Words' point of view) output. This will improve and become simpler in future versions. Feel free to comment.

**Document Rendering Enhancements**

We have addressed some of the highly popular requests and issues in the document renderer.

For example, when converting to PDF or printing, shading with percentage fill color looked ugly with dot dithering. E.g. 20% yellow on solid blue background looked awfull making any text on top of it impossible to read. Now we have implemented the same algorithm like in Microsoft Word for smooth mixing of colors. This nice smooth color is output to all rendering formats PDF, XPS, images and printing.

**Shapes are Converted to Images when Exporting to HTML**

This is a cool new feature that I have not yet blogged about.

Earlier versions of Aspose.Words just ignored all AutoShapes in a document when exporting to the HTML family of formats. There were no rectangles, arrows, stars or anything except images to be found in the resulting document.

But during our earlier work on document rendering we have created all the necessary code for converting shapes into images. This time we have just made the HTML exporter to tap into the existing rendering feature and as a result, you can actually see all shapes in the exported HTML.

Really the great thing is that this works not only for HTML export, but the whole family of HTML formats supported by Aspose.Words: HTML, XHTML, MHTML and EPUB.

There are still some limitations. For example text is not rendered inside shapes to HTML, it appears after the shape as normal text. Also, floating shapes are positioned inline in HTML. But overall, it is a big step forward for Aspose.Words.

See below how all Microsoft Word Auto Shapes now appear in exported HTML.  
  
  
Any custom shapes or ClipArt is rendered well too.  
  
  

**Updated Sample Projects**

Make sure to check out the updated [Aspose.Words for NET Samples][1] download. It now includes the samples for Windows Azure and for displaying Word documents in Silverlight.

**New Articles in the Documentation**

Some are still marked as "drafts", but you can see we are cranking up the production line.

*   How-to: Run Aspose.Words with Mono
*   Display Word Documents in Silverlight
*   How-to: Convert Documents in Windows Azure
*   How-to: Print Multiple Pages on One Sheet
*   How-to: Print and Preview a Document
*   How-to: Remove Page and Section Breaks
*   How-to: Extract or Remove Comments
*   How-to: Load and Save a Document to a Database
*   How-to: Check Format Compatibility
*   Field Update

**How To Download**

As usual, for the full list of changes and to download see [Aspose.Words downloads][2].




[1]: http://www.aspose.com/community/files/51/file-format-components/aspose.words-for-.net-and-java/entry187174.aspx
[2]: http://www.aspose.com/community/files/51/file-format-components/aspose.words-for-.net-and-java/default.aspx





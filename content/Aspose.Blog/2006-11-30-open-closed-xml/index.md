---
title: 'Open - Closed XML'
date: Thu, 30 Nov 2006 06:59:00 +0000
draft: false
url: /2006/11/30/open-closed-xml/
author: Romank
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---

The Office Open XML standard is a great thing, no questions. Lots of talks and writings about the quality of openness around, so I cannot stay away from singing about what I see too.

Office Open XML Final Draft, pages 1631 to 1686.

55! pages that describe a single ST\_Border enumeration...

Doesn't this look suspicious? Who on Earth can possibly want to deal with more than 50 pages of just a border specification? When I see something like this, I couldn't stop thinking: "has that person been fired already?" :)

These pages describe Art Borders available in Microsoft Word. It is clear to me that Office Open XML specification was developed to support ALL features of previous Microsoft Word and it was a goal not to throw any feature away. So Art Borders had to be included in OpenXML. Fine.

The solution that is now in the standard for Art Borders gives a named enum value to each possible Art Border along with its picture and descriptive text, such as: "_Specifies an art border consisting of a repeated image of a baby pacifier, as follows (showing two repetitions)_". This is the stuff that takes 50 pages.

I think this approach is "antiopen" and "antistandard". Basically, what this approach means is that any organization other than Microsoft (for example Aspose), who wants to develop an application for rendering or drawing Microsoft Word documents has a task of displaying such borders faithfully and has a problem where to get these pictures from to display them.

These pictures do not come embedded in the DOCX file. The answer is only to hack around to find and extract those pictures from Microsoft Word EXE or DLLs resources (I'm not sure, but it might not be very legal after all).

**Summary: the Art Border feature is not open, it is closed.**

My point is not to complain about the Art Border feature in particular, but to draw attention to the fact there might be more closed features like this in OpenXML. I think the standard needs more reviewing.

A better solution for the Art Border problem is to just include the image into the DOCX file so other consumers can deal with such documents better. It is probably not the best solution because it would make life more complex for other DOCX producing applications, if they want to specify an Art Border, they need to provide such an image too.  

An even better solution would be if Microsoft agreed to drop or enhance some features of Microsoft Word so they become better suited for the open standard. A solution for the Art Border could be to allow any image specified as a border and include that image in the DOCX file. I mean something like <border type="Image" image="MyImage.png" />









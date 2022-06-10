---
title: 'Aspose.Words for .NET 20.2 is released'
seoTitle: "Aspose.Words for .NET 20.2 is released"
description: ""
date: Thu, 06 Feb 2020 10:50:24 +0000
draft: false
url: /2020/02/06/aspose.words-for-.net-20.2-released/
author: Andrey Noskov
summary: ''
tags: ['Aspose.Words for .NET', 'PDF to Word C#', 'Word to pdf conversion C#', 'insert ole object', 'new release of Aspose.Words', 'release notes', 'word to pdf .net core', 'word to pdf c#', 'word to pdf in .NET', 'word to pdf programmatically']
categories: ['Aspose.Words Product Family']
---

Despite the public holidays, this month was finished with good productivity, 57 improvements and fixes (with 4 Enterprise and 3 Priority Support issues among them) were included to this regular monthly release. Totally 105 issues were processed.

Loading PDF documents is now supported by Aspose.Words for .NET Standard. This is the first file format codec included as plugin in Aspose.Words. To make loading PDF documents work in your .NET Core application, you should add a reference to Aspose.Words.Pdf2Word.dll, or simply add NuGet reference to Aspose.Words. Loading PDF documents is as simple as loading a regular Word document.

Model/Conversions Team delivered several new features.  
The most notable are:

*   Word 2019 version set by default. From now all the documents are loaded to the model following MS Word 2019 behavior.
*   FieldMergingArgsBase.FieldValue property has been made settable so that instead of setting Text the user can set FieldValue which takes formatting into account instead of simply replacing the field.
*   Supported dynamic insertion of documents and images from Base64-encoded bytes and dynamic checkbox value setting for LINQ Reporting Engine.

Rendering team managed to fix various rendering issues for DrawingML Charts, VML shapes, DrawingML text effects. Background image rendering has also been improved so that it is closer to MS Word output. The first release of 3D Effects Rendering through OpenGL is on the finale stage, Java team came up with a proposal to refine the code for auto-porting, so it was decided to postpone the release until the next month, using this time to improve the code.

Layout Team improved hyphenation zone processing, clipping of paragraph borders inside text boxes, implemented user notification when document is assembled with floating shapes nested in a text box to make the layout process more informative and predictable.










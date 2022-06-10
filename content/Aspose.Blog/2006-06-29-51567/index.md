---
title: 'Aspose.Slides for .NET 2.5.5.0 released!'
date: Thu, 29 Jun 2006 00:42:00 +0000
draft: false
url: /2006/06/29/51567/
author: Alcrus
summary: ''
tags: ['Alexey Zhilin']
---

Hot fix contains:  

*   New: Polyline.Path property returns GraphicsPath for a polyline. Creating polylines and set{} little delayed. We didn't finish testing yet.  
    
*   Fixed: Fonts.GetEnumerator() returns IDictionaryEnumerator now.
*   Changed: Changed type of all FontIndex properties to int.
*   Fixed: Recognizing ole objects. It was broken in 2.5.1 hot fix.
*   Fixed: Slide.AddNotes() method call could hang application thread or make presentation broken.
*   Fixed: After restoring of serialized shape TextFrame property always was null.








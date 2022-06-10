---
title: 'Aspose.Slides for Java 1.8.0.0 Released'
date: Mon, 05 Nov 2007 22:48:00 +0000
draft: false
url: /2007/11/05/aspose-slides-for-java-1-8-0-0-released/
author: Alcrus
summary: ''
tags: []
categories: ['Aspose.Slides Product Family']
---

What's New:  

*   Memory and speed optimization of ppt files reading/writing.  
    
*   New optimized tables engine.
*   Possibility to read file name of OLE1 objects.
*   Shape.addTextFrame method returns created TextFrame now.
*   Slide.addNotes returns created Notes object.
*   If slide notes exist but don't have paragraphs then one empty default paragraph will be inserted automatically on presentation writing.
*   Presentation.deleteHandout() method.
*   Shape.hasExternalData() method to determine if shape has some hidden data (in case shape is not recognised as OleObjectFrame, AudioFrame etc.)
*   Improved text rendering on slides.  
    

Fixes:  

*   Presentation.deleteUnusedMasters() could throw exception on presentation with notes.
*   In some cases Aspose.Slides coudn't read correct bullet color.
*   In some cases Aspose.Slides coudn't read extended numbered bullets in TextHolders.
*   Numbered list treated as bulleted list in slide notes.
*   European umlaut characters (e.g. Swedish å, ä and ö) lose font after slide cloning.
*   cloneSlide could throw exception for slides with zero width autoshapes.
*   Aspose.Slides didn't delete referenced OLE and embedded sound data after removing OleObjectFrame and AudioFrame shapes.  
    
*   Font of symbols inserted to a text could be changed after slide cloning.

To download: [http://www.aspose.com/Community/Files/51/aspose.slides/default.aspx][1]




[1]: http://www.aspose.com/Community/Files/51/aspose.slides/default.aspx





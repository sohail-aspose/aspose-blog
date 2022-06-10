---
title: 'Aspose.Slides for Java 1.7.4.0 Released'
date: Sat, 23 Jun 2007 16:45:00 +0000
draft: false
url: /2007/06/23/aspose-slides-for-java-1-7-4-0-released/
author: Alcrus
summary: ''
tags: []
categories: ['Aspose.Slides Product Family']
---

Aspose.Slides for Java 1.7.4.0 hot fix contains the following changes:  

*   New: Reading and creating extended bullets on notes.
*   New: Extracting embedded text files (and other "native" documents which don't have special OLE server) from a presentation.
*   New: Notes.getSchemeColor() method.
*   Fixed: getFontColor() and getBulletColor() properties could return wrong value for Notes text.
*   Fixed: Reading default value of Presentation.getSlideShowSettings().getManualAdvance(). Advance on time didn't work by default.
*   Fixed: NullPointerException on reading presentations with tables created in the PowerPoint 2007.
*   Fixed: NullPointerException on reading presentation with Notes without Paragraphs. Actually, MS PowerPoint can't create such presentations so assume that is workaround for broken ppts.
*   Fixed: Slides exported to SVG format couldn't be opened with Mozilla Firefox.
*   Fixed: getThumbnail() could throw NullPointerException exception on slides with polylines.
*   Fixed: Cloning slides with tables, groupshapes, diagrams and autoshapes.
*   Fixed: Color of text in TextFrames on cloned slides could be changed.  
    
*   Fixed: Presentation.deleteUnusedMasters() could throw NullPointerException in presentation with notes.
*   Fixed: Slide.saveToSVG could throw NullPointerException for slides with empty polylines (polylines with 0 points).

Download URL: [http://www.aspose.com/Downloads/Aspose.Slides/Java/1.7.4.0/Default.aspx][1]




[1]: https://docs.aspose.com/display/diagramjava/How+to+Convert+a+Visio+Diagram





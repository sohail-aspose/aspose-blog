---
title: 'Aspose.Slides for .NET 2.7.2.0 Released'
date: Fri, 28 Sep 2007 20:52:00 +0000
draft: false
url: /2007/09/28/aspose-slides-for-net-2-7-2-0-released/
author: Alcrus
summary: ''
tags: []
categories: ['Aspose.Slides Product Family']
---

**Fixes:**  

*   Aspose.Slides didn't delete referenced OLE and embedded sound data after removing OleObjectFrame and AudioFrame shapes. Also Shape object now has special boolean property HasExternalData to determine if shape has some hidden data (in case shape is not recognised as OleObjectFrame, AudioFrame and etc.)  
    
*   3181 - Font of symbols inserted to a text could be changed after slide cloning.
*   3623, 3800 - MS PowerPoint couldn't open presentations ("PowerPoint can’t open ppt because part of the file is missing"). If target presentation was created through "new Presentation()" call then Presentation.DeleteHandout() method should be called after slide cloning.

To download: [http://www.aspose.com/Community/Files/51/aspose.slides/default.aspx][1]




[1]: http://www.aspose.com/Community/Files/51/aspose.slides/default.aspx





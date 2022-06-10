---
title: 'Aspose.Slides for .NET 2.7.0.0 Released'
date: Wed, 19 Sep 2007 13:25:00 +0000
draft: false
url: /2007/09/19/aspose-slides-for-net-2-7-0-0-released/
author: Alcrus
summary: ''
tags: []
categories: ['Aspose.Slides Product Family']
---

**What's New:**  

*   **New enhanced high speed tables engine.**
*   Aspose.Slides installer and assemblies now come signed with Authenticode.

**Fixes:**  

*   3596 - European umlaut characters (e.g. Swedish å, ä and ö) lose font after slide cloning.

**More Info:**  
From this version we change API for working with tables. We tried to make it as close as possible to previous releases but there are some differences anyway.  

*   Temporally it's not possible to delete columns and split cells.
*   CellBorder class has GetEnumerator() method instead of LineFormat property in the previous versions. GetEnumerator retirns iterator for enumerating all Line objects which compose border of a cell.
*   Cell class has new TopLeftCell and BottomRightCell properties to get coordinates of a cell. These properties are equal to each other for normal cells and different for merged cells.  
    

To download [http://www.aspose.com/Community/Files/51/aspose.slides/entry95372.aspx][1]




[1]: http://www.aspose.com/Community/Files/51/aspose.slides/entry95372.aspx





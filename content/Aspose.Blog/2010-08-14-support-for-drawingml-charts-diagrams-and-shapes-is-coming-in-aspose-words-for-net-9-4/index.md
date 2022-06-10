---
title: 'Support for DrawingML Charts, Diagrams and Shapes is coming in Aspose.Words for .NET 9.4'
date: Sat, 14 Aug 2010 12:53:00 +0000
draft: false
url: /2010/08/14/support-for-drawingml-charts-diagrams-and-shapes-is-coming-in-aspose-words-for-net-9-4/
author: Romank
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---

DrawingML is the "new" XML language for all Microsoft Office graphics. Before DrawingML office graphics was stored in VML (with Office extensions). Before VML office graphics were stored in binary "Escher" format.

*   DrawingML can describe Shapes, Pictures, Diagrams and Charts.
*   DrawingML first appeared in ECMA-376:2006.
*   MS Word 2007 supports DrawingML in a "limited way". MS Word 2010 supports DrawingML more.

**DrawingML in Aspose.Words - Before Today**

Aspose.Words today supports only small subset of DrawingML related to pictures only. We need to improve support of DrawingML in Aspose.Words and it is a big task.

*   If you open/save a DOCX document with DrawingML pictures, they will be roundtripped okay.
*   If you open a DOCX document with DrawingML pictures and save to another format or render to PDF they will be output okay.
*   If you open/save a DOCX document with DrawingML Charts, Diagrams or Shapes - these will be lost.

**DrawingML in Aspose.Words - Coming End of August 2010**

All DrawingML Charts, Diagrams (a.k.a SmartArt) and Shapes are fully roundtripped during DOCX open/save operations. This highly requested feature will be available in Aspose.Words for .NET 9.4 by the end of August.

Converting DOCX to another format or rendering remains as is. Pictures will be converted but all other DrawingML will not appear in the output.

**DrawingML in Aspose.Words - What's Next**

We are now working to implement output of DrawingML Charts, Diagrams and Shapes to all other formats. Aspose.Words will render DrawingML into raster or vector graphics on conversion to other formats. There is a lot of work because DrawingML is complex and includes rich visual effects, but we plan to release some workable features by the end of the year.









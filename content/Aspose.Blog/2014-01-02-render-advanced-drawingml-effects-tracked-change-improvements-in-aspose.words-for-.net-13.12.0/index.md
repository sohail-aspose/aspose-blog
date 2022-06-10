---
title: 'Render Advanced DrawingML Effects &amp; Tracked Change Improvements in Aspose.Words for .NET 13.12.0'
date: Thu, 02 Jan 2014 23:27:48 +0000
draft: false
url: /2014/01/02/render-advanced-drawingml-effects-tracked-change-improvements-in-aspose.words-for-.net-13.12.0/
author: Adam Skelton
summary: ''
tags: ['Bezier curve', 'Improvements to field engine', 'Shadow', 'Tracked revisions', 'WordArt support', 'change', 'curves', 'deletion', 'glow', 'insertion', 'reflection', 'rendering WordArt', 'trackmove support']
categories: ['Aspose.Words Product Family']
---

Aspose.Words 13.12.0 has been released with over 103 useful new features, enhancements and bug fixes. This version marks the first version for the 2014 year.

You can download the latest releases of Aspose.Words from the following links:

*   [Aspose.Words for .NET 13.12.0][1]
*   [Aspose.Words for Java 13.12.0][2]
*   [Aspose.Words for Android 1.5][3]

Here is a look at just a few of the biggest features in this month’s release. For a full list of bug fixes and improvements please refer to the download pages in the links above.

## Support for Rendering Curved WordArt and DrawingML Advanced Effects

DrawingML is primary language used to represent graphical objects in OOXML version of Words documents (DOCX is an OOXML format for instance). The DrawingML language is complex by nature but with each release support for this feature is improved within Aspose.Words.

With this month’s release curved WordArt is supported (the WordArt shapes fit to frames defined by Bezier curves) and advanced DrawingML effects such as glow, outer shadow and reflection are included. Keep an eye out for further DrawingML improvements coming with future versions.

The following images which demonstrate rendering of different DrawingML images are produced by Aspsoe.Words.

[![][4]](https://blog.aspose.com/wp-content/uploads/sites/2/2014/01/image1r.jpg)

[![][5]](https://blog.aspose.com/wp-content/uploads/sites/2/2014/01/image004.png)

Curved WordArt

Glow

[![][6]](https://blog.aspose.com/wp-content/uploads/sites/2/2014/01/image005.png)

[![][7]](https://blog.aspose.com/wp-content/uploads/sites/2/2014/01/image002.png)

Outer shadow

Reflection

## Support for Moved Track Revisions

When track changed are enabled, any insertions, deletions or changes in the document are identified and displayed to the user.  Along with these three standard changes, there is a special type of tracked changed which identifies when a portion of content is moved from one place to another in the document. This move is seen as one unique operation where the content moved from one position to another. Without support for this type of tracked change the move appears as two operations: a separate deletion and insertion.

Aspose.Words now support this type of tracked change and will correct identify any “moves” in the document with tracked change enabled as one operation.

_Note that at the moment this feature is only supported when loading and saving in DOCX format, however support for other formats is planned for the next few releases._



[1]: http://www.aspose.com/community/files/51/.net-components/aspose.words-for-.net/category1188.aspx
[2]: http://www.aspose.com/community/files/72/java-components/aspose.words-for-java/category1378.aspx
[3]: http://www.aspose.com/community/files/74/android-components/aspose.words-for-android/category1430.aspx
[4]: https://blog.aspose.com/wp-content/uploads/sites/2/2014/01/image1r.jpg "Curved WordArt"
[5]: https://blog.aspose.com/wp-content/uploads/sites/2/2014/01/image004.png "DrawingML Glow"
[6]: https://blog.aspose.com/wp-content/uploads/sites/2/2014/01/image005.png "DrawingML Shadow"
[7]: https://blog.aspose.com/wp-content/uploads/sites/2/2014/01/image002.png "DrawingML Reflection"





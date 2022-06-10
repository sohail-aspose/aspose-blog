---
title: 'AWesome Drawing Objects'
date: Tue, 12 Sep 2006 10:44:00 +0000
draft: false
url: /2006/09/12/56417/
author: Romank
summary: ''
tags: ['Roman Korchagin']
---

I liked the **AW**esome line started by my colleague Dmitry Vorobyev in a post about his work on RTF export and I want to carry it on to describe what we've done for drawing objects in Aspose.Words 4.0.

Drawing objects in Microsoft Word documents are images, shapes (also called auto shapes), group shapes, textboxes, diagrams, OLE objects, ActiveX controls, horizontal lines and WordArt objects.

In the binary DOC format they are sometimes called "Escher", probably an early code name from Microsoft. In WordprocessingML drawing objects are represented using VML.

In Aspose.Words documentation we will collectively call them "drawing objects" or "shapes". When we talk about "shapes" we basically talk about any kind of shape including image, textbox or an OLE object because "shape" is shorter than "drawing object".

Aspose.Words for .NET versions earlier than 4.0 dealt with drawing objects reasonably well:

*   Drawing objects in the documents were generally well-preserved during open-save cycle.
*   You were able to access the drawing objects in the document tree via the Shape and InlineShape classes and perform some limited manipulations such as change shape size, position, extract image bytes
*   You were able to insert images into a document.

However, the design that we had before 4.0 for dealing with drawing objects was not perfect, mainly because we did not understand the format of the shapes well. Here are the most notorious problems that customers had with shapes using Aspose.Words before version 4.0:

*   Textboxes in group shapes were damaged during open-save cycle.
*   Group shapes were sometimes damaged during open-save cycle.
*   Diagrams created in Microsoft Word were damaged during open-save cycle.
*   Z-order of shapes anchored to a same place in the document was lost during open-save cycle.
*   Only images and textboxes were exported to PDF and with limited formatting options.
*   Public API to access shapes was limited, no way to create shapes or modify most of their properties. No way to modify content of a group shape.

In Aspose.Words 4.0 we changed all that. All of the problems mentioned above have now been solved. Here is what we've done:

1.  Reworked code responsible for representing shapes in the document model
2.  Reworked code for reading and writing shapes to DOC files
3.  Created code for exporting shapes to RTF
4.  Created code for exporting shapes to WordML.
5.  Improved code for exporting shapes to PDF.
6.  Added a new Aspose.Words.Drawing namespace with new and rich public API for drawing objects.

The work on export/import shapes to various formats was the most important part of the support for drawing objects. This work was very hard due to poor and inconsistent documentation for shapes in all those formats. While it does not need any further comments apart from it should just work for you perfectly, I want to say a few more words about the new drawing objects API we are publishing.

All classes and enumerations related to drawing objects have been put into the new Aspose.Words.Drawing namespace.

If you look at the API Reference (you need to download Aspose.Words 4.0 Beta for that) you will see that the classes in Aspose.Words.Drawing resemble VML. This was one of the design decisions we had to make. We had two options: make drawing objects classes look  like drawing objects in Microsoft Word Automation or like VML. So far the decision we made was in favor of VML-like API. If you have a strong case against it, you are welcome to raise it since Aspose.Words 4.0 is still in Beta.

Aspose.Words 4.0 is still Beta and we are still working to finalize the API and documentation for it. There will be methods to create shapes easier than now. Also there is a decision to be made about positioning units for shapes. At the moment top-level shapes are positioned in points but shapes that are children of a group shape are positioned in the units of the group shape coordinate space.

If you have comments or requests for the drawing objects API, welcome to comment here or post in the support forums. Your input will help to shape the API.








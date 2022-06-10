---
title: 'Content Rendering and Document Object Model Navigation Improvements in Aspose.Note for .NET 1.1.0'
date: Wed, 02 Apr 2014 17:06:26 +0000
draft: false
url: /2014/04/02/content-rendering-and-document-object-model-navigation-improvements-in-aspose.note-for-.net-1.1.0/
author: Imran Rafique
summary: ''
tags: ['Imran.Rafique']
categories: ['Aspose.Note Product Family']
---

[![][1]](https://blog.aspose.com/wp-content/uploads/sites/2/2013/08/aspose-Slides-for-net_100.png)We are pleased to announce the release of Aspose.Note for .NET 1.1.0 with new features, enhancements and bug fixes. This latest version now supports rendering text with subscript or superscript layout. (Superscript and subscript is text or numbers slightly above or below the normal text level and usually in a smaller font.) In addition to that, users can easily access and manipulate bullet lists, numbered lists and paragraphs with spacing options through the Aspose.Note API. The content manipulation features now offer a bit more control.

One valuable feature is retrieving the bullet or numbered list properties, for example the font, font size, font color and format. Please see a complete example topic: Retrieve Bullet or Number List Properties

## Fixed Issues and Enhancements

Thanks to the recently fixed issues and improvements, rendering a OneNote document to other formats is now better. In this regard, we have fixed some error messages which were thrown when the page contains the only title element or the font does not support the Regular style.

Several other fixes have been made to improve the overall quality. Accuracy is the key factor. These fixes cover precise rendering of image inside the outline element, the correct measurement of text lines, size calculation of RichText elements and the indent position of outlines and outline group elements.

The Document Object Model navigation mechanism has also been improved. It is now possible to access FirstChild, LastChild, NextSibling and PreviousSibling from the current node object. Aspose.Note assembly is CLS compliant. It makes sure that the library can be used from any CLR language.

## Public API Changes

The following API changes in the new version are also worth noting:

1.  The **SpaceBefore** property has been added to the RichText class. Use it to get or set the minimum amount of space before the text line.
    
2.  The **SpaceAfter** property has been added to the RichText class. Use it get or set the minimum amount of space after the text line.
    
3.  The **LineSpacing** property has been added to the RichText class. Use it to get or set line spacing.
    
4.  The **NumberList** property has been added to the OutlineElement class. Use it to get or set the bullet or number list for outline.
    
5.  The **INotebookVisitor** interface is now a **DocumentVisitor** abstract class. It helps avoiding problems.
    
6.  A new **NumberList** class  has been added. Use it to retrieve the numbers or bullet list.
    

To view a complete list of API features and try the API at your end, please visit the following page and [download the latest version of Aspose.Note for .NET][2]. If you need any help, please feel free to ask in the [Aspose.Note forum][3]. For more details, please visit the Aspose.Note for .NET documentation.




[1]: https://blog.aspose.com/wp-content/uploads/sites/2/2014/02/AsposeNote-for-NET-100X100.png "Aspose.Slides or .NET logo"
[2]: http://www.aspose.com/community/files/51/.net-components/aspose.note-for-.net/default.aspx
[3]: http://www.aspose.com/community/forums/aspose.note-product-family/522/showforum.aspx





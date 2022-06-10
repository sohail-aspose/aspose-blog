---
title: 'Insert an Image into the OneNote Document and Saving Support in OneNote Format using Aspose.Note for .NET 1.5.0'
date: Tue, 12 May 2015 04:12:37 +0000
draft: false
url: /2015/05/12/insert-an-image-into-the-onenote-document-and-saving-support-in-onenote-format-using-aspose.note-for-.net-1.5.0/
author: Imran Rafique
summary: ''
tags: ['Imran.Rafique']
categories: ['Aspose.Note Product Family']
---

[![][1]](https://blog.aspose.com/wp-content/uploads/sites/2/2013/08/aspose-Slides-for-net_100.png)We are pleased to announce the new release version of Aspose.Note for .NET 1.5.0. This new release allows clients to also save OneNote documents in .ONE format, insert an image into the OneNote document, apply different text styles in one rich text element, parsing and exporting of different formats of numbered lists and maintain various page levels as Microsoft Office OneNote do. Besides this, our product team has also included fixes of recently reported bugs and other sort of enhancement.

## Saving a Document to Microsoft OneNote Format

We have added support to save a document to Microsoft Office OneNote format. Few of our clients were anxiously waiting for this feature support. Since we have accomplished our promise. Previously, our clients were only able to save OneNote documents in PDF and some common thumbnail formats. Please check this feature details in the following help pages: Product Overview, Specify OneNote Save Options.

## Insert an Image into the OneNote Document

The OneNote documents clients create in Microsoft Office OneNote let them collect and keep all kinds of information in one place. Aspose.Note APIs now allows developers to insert an image into the OneNote document automatically. Following help topic shows, how developers insert an image into the OneNote document: Insert an Image on a OneNote Document Page

## Set Page Title of the OneNote Document

Our clients can set the page title of the OneNote document. It is now supported. We can get or set Title property of the Page class object.

In addition to the above features, we have added support of page levels. Previously, it was saving big chunks of data in a single page and not splitting into pages as Microsoft Office OneNote do. It also allows to preserve different text styles in one rich text element during the call of OneNote export features.

The Numbered list can have various formats. Many of our clients were facing issues of missing numbered list during the export features of OneNote documents. We have added support of basic numbered list formats.

## Public API Changes

The following API changes in the new version are also worth noting:

*   A new Page.Title property has been added. It helps to set the document page title.
    
*   The new interfaces for child nodes are added, e.g. INode, ICompositeNode, IOutlineElementChildNode, IOutlineChildNode and IPageChildNode etc. Almost all composite nodes now have a more strict type of child nodes unlike the base type Node previously.
    
*   The Section and PageSeries classes are removed. All properties which correspond to the Section node were moved to the Document class (CreationTime, Color, DisplayName, Guid). The pages from the PageSeries node moved to the document's children and are accessible through the IEnumerable interface implemented by the Document type.
    
*   The CompositeNode class is converted into a generic type with an interface INode constraint of the type parameter. It increases clarity of the OneNote composite node.
    
*   IsTitleText, IsTitleDate and IsTitleTime properties of the RichText type are marked as obsolete. These objects are now accessible through TitleText, TitleDate and TitleTime properties respectively.
    
*   TableColumn.Ordinal property is marked as obsolete. To specify an order for the columns the Table.Children property should be used.
    
*   Table.Rows property is marked as obsolete. The property provides a read only list of rows. To change the rows collection AppendChild and RemoveChild methods should be used.
    
*   RichText.IsTitleText property is marked as obsolete. To set the text of the title, Title.TitleText property should be used.
    
*   RichText.IsTitleDate property is marked as obsolete. To set the date of the title, Title.TitleDate property should be used.
    
*   RichText.IsTitleTime property is marked as obsolete. To set the time of the title, Title.TitleTime property should be used.
    
*   Image.Path property is marked as obsolete. Use the constructor parameters to specify the path to the image.
    
*   Image.IsSizeSetByUser property is marked as obsolete. The property does not affect anything.
    
*   NumberList.ctor() method is marked as obsolete. Use other constructors to create a valid NumberList instance.
    
*   Image.ctor(Document document) method is marked as obsolete. Use other constructors to create a valid Image instance.
    

## Aspose.Note for .NET Resources

The resources, you may need to accomplish your tasks:

*   [Homepage for Aspose.Note for .NET API][2]
    
*   [Download Aspose.Note for .NET][3]
    
*   Aspose.Note for .NET Wiki docs - help documentation and API reference documents.
    
*   [Aspose.Note Product Family Forum][4] - post your technical questions and queries, or any other problem you faced while running Aspose.Note APIs.
    
*   [Enable Email Subscription][5] - Don't limit yourself, you can keep yourself updated with the latest news on Aspose.Note APIs and new features, fixes, plus other API related topics by subscribing to Aspose.Note blog.
    
*   [Aspose.Note for .NET Examples][6] – We have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: https://blog.aspose.com/wp-content/uploads/sites/2/2014/02/AsposeNote-for-NET-100X100.png "Aspose.Slides or .NET logo"
[2]: http://www.aspose.com/.net/onenote-component.aspx
[3]: http://www.aspose.com/community/files/51/.net-components/aspose.note-for-.net/default.aspx
[4]: http://www.aspose.com/community/forums/aspose.note-product-family/522/showforum.aspx
[5]: https://blog.aspose.com/
[6]: https://github.com/asposenote/Aspose_Note_NET





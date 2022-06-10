---
title: 'Improved OneNote Table Export and Generic Node Retrieval in Aspose.Note for .NET 1.4.0'
date: Wed, 01 Apr 2015 18:26:35 +0000
draft: false
url: /2015/04/01/improved-onenote-table-export-and-generic-node-retrieval-in-aspose.note-for-.net-1.4.0/
author: Imran Rafique
summary: ''
tags: ['Imran.Rafique']
categories: ['Aspose.Note Product Family']
---

[![][1]](https://blog.aspose.com/wp-content/uploads/sites/2/2013/08/aspose-Slides-for-net_100.png)We are pleased to announce the new version of Aspose.Note for .NET 1.4.0. In this major build, we have optimized the parsing algorithm of OneNote document, and border lines of the table can be preserved in the output PDF and thumbnail formats. We have also added a new generic approach to retrieve OneNote document nodes and the older one has been marked as obsolete. This release also includes the most recent bug fixes along with the above enhancements.

## Retrieve OneNote Document Nodes

**Old sample code (.NET, C#):**

```
// load OneNote document
Aspose.Note.Document oneFile = new Aspose.Note.Document(@"Test.one");
// retrieve RichText type nodes
IList<Node> richTextNodes = oneFile.GetChildNodes(Aspose.Note.NodeType.RichText);
// retrieve a particular node from the collection
Aspose.Note.RichText firstTextNode = (Aspose.Note.RichText)richTextNodes[0];
```

**New sample code (.NET, C#):**

```
// load OneNote document
Aspose.Note.Document oneFile = new Aspose.Note.Document(@"Test.one");
// retrieve RichText type nodes
IList<RichText> richTextNodes = oneFile.GetChildNodes<RichText>();
// retrieve a particular node from the collection
Aspose.Note.RichText firstTextNode = richTextNodes[0];
```

This release comprises a number of key fixes that help us improve accuracy, performance and rendering capabilities.

*   Fixed: OneNote to PDF conversion, can't open the output PDF file.
    
*   Fixed: OneNote to PDF conversion, some words cannot be shown.
    
*   Fixed: OneNote to PDF conversion, the table borders are not preserved.
    
*   Fixed: OneNote to PDF conversion, the date text overlaps with time.
    
*   Fixed: InvalidOperationException occurred while loading OneNote document.
    
*   Fixed: Argument Exception message while exports of OneNote to PDF format.
    
*   Fixed: Invalid data error while loading OneNote document.
    

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





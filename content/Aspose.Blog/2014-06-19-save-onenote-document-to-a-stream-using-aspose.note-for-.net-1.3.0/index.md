---
title: 'Save OneNote Document to a Stream using Aspose.Note for .NET 1.3.0'
date: Thu, 19 Jun 2014 08:10:04 +0000
draft: false
url: /2014/06/19/save-onenote-document-to-a-stream-using-aspose.note-for-.net-1.3.0/
author: Imran Rafique
summary: ''
tags: ['Imran.Rafique']
categories: ['Aspose.Note Product Family']
---

[![][1]](https://blog.aspose.com/wp-content/uploads/sites/2/2013/08/aspose-Slides-for-net_100.png)We are pleased to announce the release of [Aspose.Note for .NET][2] 1.3.0. This new build enables developers to save OneNote documents to a Stream object. Developers can now pass a stream object to the Document.Save(Stream, SaveFormat) or Document.Save(Stream, SaveOptions) method. When saving to a stream, specify the save format explicitly. Please have a look at our official documentation, the help topics: Save OneNote Document to a Stream, and Specify OneNote Save Options

## Bug Fixes & Enhancements

This new release fixes several issues, including the presence of duplicate pages in a PDF output file. We have also updated the parsing of styles based on new JCID structure. The JCID structure specifies the type of object and the type of data the object contains. Previously, the default style rich text sometimes had an incorrect value. Several other enhancements are included too, as follows:

*   Optimized the parsing algorithm of OneNote files.
*   Access to document available through any nodes.

## Public API Changes

The following API changes in the new version are also worth noting:

1.  A new Node.Document property has been added. It helps to access the document available through any nodes.
    
2.  A new Document.Save(Stream stream, SaveOptions options) method has been added. It saves the OneNote document to a stream using the specified save options.
    
3.  A new Document.Save(Stream stream, SaveFormat format) method has been added. It saves the OneNote document to a stream in the specified format.
    

To view a complete list of API features and try the API at your end, please visit the following page and [download the latest version of Aspose.Note for .NET][3]. If you need any help, please feel free to ask in the [Aspose.Note forum][4]. For more details, please visit the Aspose.Note for .NET documentation.




[1]: https://blog.aspose.com/wp-content/uploads/sites/2/2014/02/AsposeNote-for-NET-100X100.png "Aspose.Slides or .NET logo"
[2]: http://www.aspose.com/.net/onenote-component.aspx
[3]: http://www.aspose.com/community/files/51/.net-components/aspose.note-for-.net/default.aspx
[4]: http://www.aspose.com/community/forums/aspose.note-product-family/522/showforum.aspx





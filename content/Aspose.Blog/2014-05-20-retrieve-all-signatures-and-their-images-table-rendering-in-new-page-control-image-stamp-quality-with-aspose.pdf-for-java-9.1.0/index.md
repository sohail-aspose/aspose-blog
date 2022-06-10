---
title: 'Retrieve Signatures with Images, Render Table on New Page, and Control Image Stamp Quality - Aspose.PDF for Java 9.1.0'
date: Tue, 20 May 2014 05:52:10 +0000
draft: false
url: /2014/05/20/retrieve-all-signatures-and-their-images-table-rendering-in-new-page-control-image-stamp-quality-with-aspose.pdf-for-java-9.1.0/
author: Codewarior
summary: ''
tags: ['Nayyer Shahbaz', 'Control the quality of stamp images in PDF in Java', 'Get signature images from PDF in Java', 'Java PDF API']
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/aspose-Pdf-for-Java_100.png" alt="Aspose.Pdf for Java logo">}}


Ever since we published the autoported merged Aspose.PDF for Java API, we have been working hard to make this API as powerful and compelling as its sibling Aspose.PDF for .NET. With every new release, we try to port the latest features available in Aspose.PDF for .NET and introduce fixes for issues reported in earlier versions. In [Aspose.PDF for Java 9.1.0][1], we have introduced some exciting new features and enhancements which have made this API more compelling. Some of the new features introduced in this release are described below.

## Extracting Image from Signature Field

Aspose.Pdf for Java supports the feature to add, remove, and delete signatures from PDF documents. While adding a signature to a PDF file, we provide an image for the signature appearance and now Aspose.Pdf for Java offers the capability to read all signature objects and retrieve the images associated with each object. Please visit the following link for further details: [Extracting Image from Signature Field][2].

## Control Image Quality when Adding as Stamp

The feature to add an image or text as a stamp in PDF files has been supported by Aspose.Pdf for Java for a while. However, recently we received a requirement to control the image quality when adding an image as a stamp object. The following code snippet shows the steps to control image stamp quality when adding it to a PDF document. For more information, read about how to [control image quality when adding an image stamp][3].



## Bookmark Points to Start of Page

Bookmarks are one of the important elements of PDF document as they allow readers to quickly move between different pages. Aspose.Pdf for Java has supported features for [adding a bookmark][4], [getting bookmarks][5] and [deleting bookmarks][6]. Now the latest release supports editing the destination of a bookmark and points it to the start of a page. Or you can set the destination while creating a new bookmark inside a PDF document. Please visit the following link for further details: [Bookmarks should Point to Start of Page][7].

## Render Table on New Page

Tables are integral objects when displaying data inside PDF files. Aspose.Pdf for Java supports [adding tables to PDF documents.][8] By default, tables are added in a flow layout (top-left to bottom-right). Even if there is a space on the PDF page, you might need to render the table on a new page. To accomplish this requirement, the isInNewPage(..) method has been added to the BaseParagraph class. For more information, please visit [Force Table Rendering in New Page][9].

## Delete Images from PDF using ImagePlacementAbsorber

Aspose.Pdf for Java makes it possible to add text and image objects as well as extracting text and image objects from existing PDF documents. If you are certain about the index of an image inside the Images collection of a particular PDF page, you can use the following method to delete it: pdfDocument.getPages().get\_Item(1).getResources().getImages().delete(1);.

However, if you need to search all the images inside a PDF file using ImagePlacementAbsorber and then delete images, please follow the instructions in [Delete Image from PDF Resources Found by][10] [ImagePlacementAbsorber][11].

As well as the new features above, this new version includes fixes related to PDF to image conversion, saving PDF files in a particular PDF version, deleting images from PDF files, performance improvements when generating PDF files and much more. Go ahead, download and start exploring the new release of [Aspose.PDF for Java 9.1.0.][12]




[1]: https://downloads.aspose.com/pdf/java
[2]: http://docs.aspose.com/display/pdfjava/Extracting+Image+from+Signature+Field
[3]: https://docs.aspose.com/
[4]: http://docs.aspose.com/display/pdfjava/Add+a+Bookmark+to+a+PDF+Document
[5]: http://docs.aspose.com/display/pdfjava/Get+Bookmarks+from+PDF+Document
[6]: http://docs.aspose.com/display/pdfjava/Delete+Bookmarks+from+PDF+Document
[7]: http://docs.aspose.com/display/pdfjava/Bookmark+should+point+to+start+of+page
[8]: http://docs.aspose.com/display/pdfjava/Set+Border+Style%2C+Margins+and+Padding+of+Table
[9]: https://docs.aspose.com/display/pdfjava/Force+Table+Rendering+on+New+Page
[10]: https://docs.aspose.com/display/pdfjava/Home
[11]: https://docs.aspose.com/
[12]: https://downloads.aspose.com/pdf/java





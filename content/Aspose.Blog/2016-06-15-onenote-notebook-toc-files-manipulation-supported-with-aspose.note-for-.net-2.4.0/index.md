---
title: 'Manipulate OneNote Notebook TOC Files using C#'
date: Wed, 15 Jun 2016 12:28:50 +0000
draft: false
url: /2016/06/15/onenote-notebook-toc-files-manipulation-supported-with-aspose.note-for-.net-2.4.0/
author: Kashif Iqbal
summary: ''
tags: []
categories: ['Aspose.Note Product Family']
---



{{< figure align=center src="images/Aspose.Note-for-.NET_1.png" alt="">}}


We are pleased to announce the release of [Aspose.Note for .NET 2.4.0][1]. This month’s release comes with the read/write support of Microsoft OneNote notebooks (.onetoc2). It provides the capability to create and manipulate notebooks. The API lets you create, save and export notebooks to a number of different formats. It also supports adding and removing child nodes from a notebook. For a complete list of what is new and fixed, please visit the Product Release Notes of Aspose.Note for .NET 2.4.0.

## Create OneNote Notebooks using C#

As mentioned earlier, this month’s release introduces the capability of OneNote Notebook file format read/write support. You can now [create a Notebook][2] using the API’s _NoteBook_ class and save it to disc or stream using the Notebook API’s _Save_ method.

## Add and Remove Child Nodes from Notebook using C#

Aspose.Note API gives you complete capability to add and remove OneNote documents from a notebook. The [AppendChild][3] and [RemoveChild][4] methods exposed by the Notebook class can be used to add or remove documents from the Notebook document.

## Convert Notebook to PDF using C#

This month’s release also introduces a new feature of savingthe OneNote Notebook (.onetoc2) to PDF format. The _NotebookPdfSaveOptions_ class can be used to specify additional save options such as page splitting algorithm and flattening. The flattening option, if used, lets you export the Notebook child to a single directory.

## Export Notebook to Image using C#

You can also convert a complete Notebook (.onetoc2) to a number of [image formats][5] using this latest version of the API. The _NotebookImageSaveOptions_ class can be used to specify additional save options such as image resolution.

## Identify OneNote File Format using C#

Aspose.Note supports both Microsoft OneNote and OneNote online file format. However, it has certain limitations in case of OneNote online file format where it doesn’t provide support for attachments and images in the document. We are currently working to provide complete support for these as well. However, until these are supported completely, the API lets its users retrieve the file format information of the document in order to be aware of these limitations. The Document class exposes the FileFormat property that can be used for determining the file format of the document.

## Other Improvements

This month's release also fixes a number of bugs that were reported by our valued customers while working with the previous version of the API. These further aid to the overall stability of the API.

## API Resources

You can get started with Aspose.Note for .NET by making use of information available in the following.

*   **API Documentation** – Helps getting started with the API using code samples and examples
*   **[Forum Support][6]** – Post your inquiries to get help from our technical support team
*   **[Examples][7]** – Try the ready-to-use examples of the API by downloading from our GitHub repository
*   [**API Reference Guide**][8] – Provides information about all the namespaces, classes and properties of the API

We are pleased to announce the release of Aspose.Note for .NET 2.4.0. This month’s release comes with the read/write support of Microsoft OneNote notebooks (.onetoc2). It provides the capability to create and manipulate notebooks. The API lets you create, save and export notebooks to a number of different formats. It also supports adding and removing child nodes from a notebook. For a complete list of what is new and fixed, please visit the Product Release page of Aspose.Note for .NET 2.4.0.

## New Features & Enhancements

**Creating OneNote Notebooks and Saving:** As mentioned earlier, this month’s release introduces the capability of OneNote Notebook file format read/write support. You can now create a Notebook using the API’s _NoteBook_ class and save it to disc or stream using the Notebook API’s _Save_ method.

**Adding and Removing Child Nodes from Notebook:** Aspose.Note API gives you complete capability to add and remove OneNote documents from a notebook. The _AppendChild_ and _RemoveChild_ methods exposed by the Notebook class can be used to add or remove documents from the Notebook document.

**Converting Notebook to PDF:** This month’s release also introduces a new feature of savingthe OneNote Notebook (.onetoc2) to PDF format. The _NotebookPdfSaveOptions_ class can be used to specify additional save options such as page splitting algorithm and flattening. The flattening option, if used, lets you export the Notebook child to a single directory.

**Exporting Notebook to Image:** You can also convert a complete Notebook (.onetoc2) to a number of image formats using this latest version of the API. The NotebookImageSaveOptions class can be used to specify additional save options such as image resolution.

**Support for Identifying OneNote File Format:** Aspose.Note supports both Microsoft OneNote and OneNote online file format. However, it has certain limitations in case of OneNote online file format where it doesn’t provide support for attachments and images in the document. We are currently working to provide complete support for these as well. However, until these are supported completely, the API lets its users retrieve the file format information of the document in order to be aware of these limitations. The Document class exposes the FileFormat property that can be used for determining the file format of the document.




[1]: http://www.aspose.com/downloads/note/net
[2]: https://docs.aspose.com/display/notenet/Working+with+OneNote+NoteBook#WorkingwithOneNoteNoteBook-CreatingandSavingaNotebook
[3]: https://docs.aspose.com/display/notenet/Working+with+OneNote+NoteBook#WorkingwithOneNoteNoteBook-AddingaChildNodetoOneNoteNotebook
[4]: https://docs.aspose.com/display/notenet/Working+with+OneNote+NoteBook#WorkingwithOneNoteNoteBook-RemoveaChildNodeFromOneNoteNotebook
[5]: https://docs.aspose.com/display/notenet/Working+with+OneNote+NoteBook#WorkingwithOneNoteNoteBook-ConvertingNotebookDocumenttoImage
[6]: https://forum.aspose.com/c/note
[7]: https://github.com/asposenote/Aspose_Note_NET
[8]: http://www.aspose.com/api/net/note





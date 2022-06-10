---
title: 'Attach Files and Insert Table with Locked Column Width in OneNote Documents in C#'
date: Tue, 09 Jun 2015 11:05:01 +0000
draft: false
url: /2015/06/09/attach-files-in-onenote-insert-table-with-locked-column-width-using-csharp/
author: Imran Rafique
summary: ''
tags: ['Imran.Rafique']
categories: ['Aspose.Note Product Family']
---



{{< figure align=center src="images/AsposeNote-for-NET-100X100.png" alt="">}}


We are pleased to announce the new release version of [Aspose.Note for .NET][1] 1.6.0. To keep a duplicate of any file or document as a part of the notes, clients can now attach it to the OneNote document programmatically. In a recent couple of releases, we have added the table management APIs which allows clients to insert a new table, update its content, and insert a table with locked column width. We have also added support to insert text with hyperlinks in the OneNote document. We're glad to offer the most demanding feature operations.

In addition to that, we have added support to apply bullets and numbers to the text. Our rich image management APIs has also been improved. This month’s release contains many useful new features, enhancements, and bug fixes in the Aspose.Note APIs.

## Attach a Document or File to OneNote using C#

With OneNote, users can gather and keep a wide range of data in one spot, including data from different sources. Instead of retyping data or depending on links to files and documents, users can attach files directly into OneNote. Aspose.Note APIs supports this feature. Following help topic shows, how developers attach a file into the OneNote document: [Attach a File to the OneNote Document][2]

## Insert a Table in the OneNote Document

Using Aspose.Note APIs, developers can now insert a table, edit table content, and easily edit basic table structure, such as adding or deleting rows and columns. Developers can also create a table with locked column width. Following help topics show, how developers insert a table in the OneNote document: [Insert a Table in OneNote Document][3], [Create a Table with Locked Columns in the OneNote Document][4]

## Insert Hyperlinks in the OneNote Document

A hyperlink is a text or a picture client can click on, and jump to another document or URL. Aspose.Note APIs permits to include hyperlinks in the OneNote Document. Following help topic shows, how developers add hyperlinks in the OneNote document: [Add a Hyperlink to the OneNote Document][5]

## Use Note Tags to Sort OneNote Document Content

OneNote lets users tag their notes for easy searching and sorting. The real power is the ability to create your own tags specific to common tasks programmatically. Aspose.Note APIs supports adding a new text node with a tag note, add a new image node with a tag note and add a new table with a tag note. Following help topic shows, how developers can tag text, image, and table in the OneNote document: [Tag Important Notes in the OneNote Document][6]

## Apply Bullets and Numbering on the Text

Arranging texts in bullets or numbers form is a very common phenomenon. Aspose.Note for .NET APIs allows developers to arrange text items with bullets and numbers. Following help topics show, how developers apply bullet or numbers to the texts in the OneNote document: [Apply Bullets on the Text][7], Apply Numbering on the Text

In addition to the above features, we have added many other help topics for our clients with ease. Please refer to the following help topics: [Create a Hello World OneNote document Using API][8], [Create an Empty OneNote Document with a Page Title][9], [Create OneNote Document with Root and Sub Level Pages][10], [Insert an Image on a OneNote Document Page][11]

Regarding the new enhancements and fixes, we have improved OneNote to Pdf conversion performance for documents with missing fonts. We have added flexibilities in enhancing the tag element size because we noticed that the big size text is the cause of wrong tag element sizes.  We also included a fix in reference of the page title. The Page.GetChildNodes method was throwing an error when the page title was not available. It's now fixed.

## Public API Changes

The following API changes in the new version are also worth noting:

*   A new AttachedFile.IconExtension property has been added. It can be used for getting icon extension.
*   A new AttachedFile.Extension property has been added. It can be used for extension of the attached file or document.
*   The Tags property has been added in various classes. Tags property gives an ability to add tags to attach files, tables or images.
*   The new boolean LockedWidth property of the TableColumn type has been added to specify whether a table column has locked width and does not resize automatically to fit table content.

## Aspose.Note for .NET Resources

The resources, you may need to accomplish your tasks:

*   [Home page for Aspose.Note for .NET API][12]
*   [Download Aspose.Note for .NET][13]
*   [Aspose.Note for .NET Wiki docs][14] - help documentation and API reference documents.
*   [Aspose.Note Product Family Forum][15] - post your technical questions and queries, or any other problem you faced while running Aspose.Note APIs.
*   [Enable Email Subscription][16] - Don't limit yourself, you can keep yourself updated with the latest news on Aspose.Note APIs and new features, fixes, plus other API related topics by subscribing to Aspose.Note blog.
*   [Aspose.Note for .NET Examples][17] – We have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: https://products.aspose.com/note/net
[2]: https://docs.aspose.com/display/notenet/Working+with+Attachments
[3]: https://docs.aspose.com/display/notenet/Working+with+Tables#WorkingwithTables-InsertaTableinOneNoteDocument
[4]: https://docs.aspose.com/display/notenet/Working+with+Tables#WorkingwithTables-CreateaTablewithLockedColumnsintheOneNoteDocument
[5]: https://docs.aspose.com/display/notenet/Working+with+Hyperlinks
[6]: https://docs.aspose.com/display/notenet/Working+with+Tags#WorkingwithTags-TagImportantNotesintheOneNoteDocument
[7]: https://docs.aspose.com/display/notenet/Working+with+Text#WorkingwithText-ApplyBulletsontheText
[8]: https://docs.aspose.com/display/notenet/Introduction
[9]: https://docs.aspose.com/display/notenet/Working+with+OneNote+Document
[10]: https://docs.aspose.com/display/notenet/Working+with+Pages#WorkingwithPages-CreateOneNoteDocumentwithRootandSubLevelPages
[11]: https://docs.aspose.com/display/notenet/Working+with+Images#WorkingwithImages-InsertanImageonaOneNoteDocumentPage
[12]: https://products.aspose.com/note/net
[13]: https://downloads.aspose.com/note/net
[14]: http://docs.aspose.com/display/notenet/Home
[15]: http://forum.aspose.com
[16]: https://blog.aspose.com/
[17]: https://github.com/asposenote/Aspose_Note_NET





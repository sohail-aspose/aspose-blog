---
title: 'New PDF Save Options and Other Goodies in Aspose.Words 13.9.0'
date: Wed, 09 Oct 2013 11:32:20 +0000
draft: false
url: /2013/10/09/new-pdf-save-options-and-other-goodies-in-aspose.words-13.9.0/
author: Adam Skelton
summary: ''
tags: ['Fullscreen', 'Outline', 'PDF', 'Pagemode', 'Thumbs', 'blank document', 'zero byte']
categories: ['Aspose.Words Product Family']
---

We are pleased to announce the monthly release of Aspose.Words for .NET and Java 13.9.0 as well as Aspose.Words for Android 1.2.  Aspose.Words for Android 1.2 marks the third release for the newest member of the Aspose.Words product family and we are pleased to announce all three product releases contain more than 100 useful improvements.

You can download the latest release of Aspose.Words from the following links:

*   [Aspose.Words for .NET 13.9.0][1]
*   [Aspose.Words for Java 13.9.0][2]
*   [Aspose.Words for Android 1.2][3] (this version matches the Aspose.Words for Java 13.9.0 codebase)

Here is a look at just a few of the features in this month’s release. For a full list of bug fixes and improvements please refer to the download pages in the links above.

## Set Page Mode in Word to PDF

This version of Aspose.Words adds a new option to the **PdfSaveOptions** class **PageMode** that controls how the PDF should appear and what internal windows in the PDF document should be initially displayed when opened in the PDF reader.

The option provides an enumeration with the following values:

<figure class="wp-block-table"><table class=""><tbody><tr><td>**Option Value</strong></td><td><strong>Description**</td></tr><tr><td>Use None</td><td>Neither document outline nor thumbnail images are visible.</td></tr><tr><td>Use Outlines</td><td>Document outline is visible.  Note that if there're no outlines in the PDF document then outline navigation pane will not be visible anyway.</td></tr><tr><td>Use Thumbs</td><td>Thumbnail images are visible.</td></tr><tr><td>Full Screen</td><td>Full-screen mode, with no menu bar, window controls, or any other window visible.</td></tr><tr><td>Use OC</td><td>Optional content group panel is visible.</td></tr></tbody></table></figure>

Open Zero Byte Documents directly using the Document Constructor

When you create a new Microsoft Word document via the Explorer context menu (right-click and choose New Microsoft Word Document) a blank file with no content is created as a placeholder for the document. The file that is created isn't a valid Microsoft Word file yet as this only happens when the file is opened in Microsoft Word or a similar editor and the appropriate data is written.

In previous of Aspose.Words trying to open such empty documents using the Document constructor would cause an exception as the file being opened was not valid. This caused some confusion and user experience issues for customers, therefore, we have remedied this and in the latest version of Aspose.Words will detect and handle these types of files so you can now open such documents directly via the constructor.




[1]: https://downloads.aspose.com/words/net
[2]: https://downloads.aspose.com/words/java
[3]: https://downloads.aspose.com/words/androidjava





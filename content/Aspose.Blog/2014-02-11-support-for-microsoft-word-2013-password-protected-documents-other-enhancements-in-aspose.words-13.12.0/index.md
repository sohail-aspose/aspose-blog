---
title: 'Work with Microsoft Word 2013 Password-Protected Documents'
date: Tue, 11 Feb 2014 02:03:50 +0000
draft: false
url: /2014/02/11/support-for-microsoft-word-2013-password-protected-documents-other-enhancements-in-aspose.words-13.12.0/
author: Adam Skelton
summary: ''
tags: ['Android', 'DOC', 'DOCX', 'Microsoft Word 2013', 'NET', 'Revisions API', 'java', 'memory usage', 'password protection', 'performance', 'rendering', 'revision', 'revision options', 'tracked changes']
categories: ['Aspose.Words Product Family']
---

The first official release of Aspose.Words for 2014 has been released. As such the major version number of the Aspose.Words for .NET and Aspose.Words for Java releases has reset to ‘14’.

Aspose.Words 14.1.0 includes over 100 useful new features, enhancements and bug fixes.

You can download the latest releases of Aspose.Words from the following links:

*   [Aspose.Words for .NET 14.1.0][1]
*   [Aspose.Words for Java 14.1.0][2]
*   [Aspose.Words for Android 1.6][3]

Here is a look at just a few of the biggest features in this month’s release. For a full list of bug fixes and improvements please refer to the download pages in the links above.

## Support for Microsoft Word 2013 Password-Protected Documents

Aspose.Words has wide support for documents created by Microsoft Word 2013 however one there was a limitation when it came to password-protection. Documents created by Microsoft Word 2013 use a different type of encryption when compared to older versions of Microsoft Word and as such were not supported by Aspose.Words from the get go when the new format was introduced. The fix included in this month’s release fix resolves this problem and Aspose.Words can now load and save such documents without any issues.



{{< figure align=center src="images/PasswordProtectDocument.jpg" alt="MS Word 2013 Password Protection Screen" caption="The password protection screen in Microsoft Word 2013">}}


## Control how Revisions are displayed in Rendered Documents

A new class has been introduced which allows you to control how revisions are displayed when rendering documents to formats such as PDF, XPS etc. Use the members of **LayoutOptions.RevisionOptions** to fine tune how revisions appear in rendered documents_Document doc = new Document("myRevisedDocument.docx");_ _RevisionOptions ro = doc.LayoutOptions.RevisionOptions;_ _ro.InsertedTextColor = RevisionColor.ByAuthor; // For inserted revisions each author gets own color_ _ro.DeletedTextColor =  RevisionColor.NoHighlight; // Deleted revisions are not highlighted_ _ro.RevisedPropertiesColor = RevisionColor.DarkBlue; // Formatting revisions will be marked in dark blue_ _ro.RevisionBarsColor = RevisionColor.DarkYellow; // Revision Bars on the side of the page will be dark yellow_ _doc.Save("myNicelyColoredRevisedDocument.pdf");_

## Memory Usage Improvements to the Page Layout Engine

This month’s release marks further improvements to rendering performance as internal parts of the rendering process have been optimized to reduce memory usage.  This improvement will reduce the possibility of **OutOfMemory** issues and improve the rendering performance when working with extra large documents.




[1]: https://downloads.aspose.com/words/net
[2]: https://downloads.aspose.com/words/java
[3]: https://downloads.aspose.com/total/androidjava





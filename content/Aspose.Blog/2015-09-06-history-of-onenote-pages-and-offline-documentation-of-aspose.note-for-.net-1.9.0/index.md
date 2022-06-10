---
title: 'Get History of OneNote Document Pages using C# .NET'
date: Sun, 06 Sep 2015 22:59:40 +0000
draft: false
url: /2015/09/06/history-of-onenote-pages-and-offline-documentation-of-aspose.note-for-.net-1.9.0/
author: Imran Rafique
summary: ''
tags: ['Imran.Rafique']
categories: ['Aspose.Note Product Family']
---



{{< figure align=center src="images/AsposeNote-for-NET-100X100.png" alt="">}}


We're pleased to announce the new release of version 1.9.0 of the [Aspose.Note for .NET][1] APIs. Using the Aspose.Note APIs is really not as hard to use as people seem to think. We're continuously minimizing the programming efforts of our clients. To lead these goals, we have added support of load or unload the entire history of the OneNote document and improved the export of OneNote document to PDF file format. From this release version, users will also be able to use offline documentation because we have included a CHM help file. Many other bug fixes, enhancements are included based on our clients use cases.

## Load or Unload History of the Entire OneNote

OneNote document keeps a history for each page and Aspose.Note APIs allow users to manage tracking this history. It also allows users to not load OneNote document history because the off loading of the entire history can improve memory and CPU usage. Please refer to the following help topic: Get All Revisions of a Specific Page.

## CHM Help File of Aspose.Note for .NET

CHM help file has been included in this release as the part of MSI and zip packages. It only covers APIs section part. We're already maintaining articles in the online documentation.

Please check a list of newly added features, defect fixes and enhancements:

*   Fixed: Improve the performance of the PDF export.
*   Fixed: Not all pages are parsed in the sample file.
*   Fixed: Aspose.Note for .Net 1.8 isn't signed.

## Public API Changes

The following API changes in the new version are also worth noting:

*   A new Document.GetPageHistory method has been added. It can be used to obtain a history of a specific page.
*   The LoadOptions class is added. It can be set specific load options (for example, whether to load history) in theDocument type constructor.

## Aspose.Note for .NET Resources

The resources, you may need to accomplish your tasks:

*   [Home page for Aspose.Note for .NET API][2]
*   [Download Aspose.Note for .NET][3]
*   [Aspose.Note for .NET Wiki docs][4] - help documentation and API reference documents.
*   [Aspose.Note Product Family Forum][5] - post your technical questions and queries, or any other problem you faced while running Aspose.Note APIs.
*   [Enable Email Subscription][6] - Don't limit yourself, you can keep yourself updated with the latest news on Aspose.Note APIs and new features, fixes, plus other API related topics by subscribing to Aspose.Note blog.
*   [Aspose.Note for .NET Examples][7] – We have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: https://products.aspose.com/note
[2]: https://products.aspose.com/note/net
[3]: https://downloads.aspose.com/note/net
[4]: https://docs.aspose.com/note/net
[5]: http://forum.aspose.com
[6]: https://blog.aspose.com/
[7]: https://github.com/asposenote/Aspose_Note_NET





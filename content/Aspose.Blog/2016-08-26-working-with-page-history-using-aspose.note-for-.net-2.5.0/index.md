---
title: 'Working with Page History using Aspose.Note for .NET 2.5.0'
date: Fri, 26 Aug 2016 14:44:11 +0000
draft: false
url: /2016/08/26/working-with-page-history-using-aspose.note-for-.net-2.5.0/
author: Kashif Iqbal
summary: ''
tags: []
categories: ['Aspose.Note Product Family']
---

[![][1]](https://blog.aspose.com/wp-content/uploads/sites/2/2016/08/Aspose.Note-for-.NET_.png)

We are pleased to announce the release of [Aspose.Note for .NET 2.5.0][2]. This month’s release provides support for reading/writing revision information to a document’s page type. It also enhances the functionality of working with history of a document such as rolling back to previous page version, pushing current page version to history and modifying page history. For a detailed note on what is new and fixed, please visit product release notes section of API documentation.

# New Features and Enhancements

**Working with Page Revision Information:** This month’s release provides the capability of working with page revision information of a document such as recent author and last modification time. This feature lets you read as well write the page revision information to a document’s page as shown in the code sample below.

```
// Load OneNote document
Document document = new Document("Aspose.one", new LoadOptions { LoadHistory = true });
// Get first page
Page firstPage = document.FirstChild;
foreach (Page pageRevision in document.GetPageHistory(firstPage))
{
    /*Use pageRevision like a regular page.*/
    Console.WriteLine("LastModifiedTime: {0}", pageRevision.LastModifiedTime);
    Console.WriteLine("CreationTime: {0}", pageRevision.CreationTime);
    Console.WriteLine("Title: {0}", pageRevision.Title);
    Console.WriteLine("Level: {0}", pageRevision.Level);
    Console.WriteLine("Author: {0}", pageRevision.Author);
    Console.WriteLine();
} 
```

**Working with Page History:** Aspose.Note API already provides support for working with Page history in a document. This month’s release brings further enhancements to this capability by providing the facility to rolling back to previous page version, pushing current page version to page history and modifying page history.

*   **Rolling Back to Previous Page Version:** This lets the API users to roll back to a previous version of the API by getting the last version from the page’s history.
*   **Pushing Current Page Version to Page History:** The current page version of the page can be included in the history collection by using the Page.Clone method.
*   **Modifying Page History:** This feature allows modifying the information related to a page history such as title and author.

# Other Improvements

This month’s release also fixes a number of bugs related to API functionality that further improves the API stability in terms of features and quality.

# API Resources

You can get started with Aspose.Note for .NET by making use of information available in the following.

**API Documentation** – Helps getting started with the API using code samples and examples

**[Forum Support][3]** – Post your inquiries to get help from our technical support team

**[Examples][4]** – Try the ready-to-use examples of the API by downloading from our GitHub repository

**[API Reference Guide][5]** – Provides information about all the namespaces, classes and properties of the API




[1]: https://blog.aspose.com/wp-content/uploads/sites/2/2016/08/Aspose.Note-for-.NET_.png "Aspose.Note for .NET"
[2]: http://www.aspose.com/downloads/note/net
[3]: https://forum.aspose.com/c/note
[4]: https://github.com/asposenote/Aspose_Note_NET
[5]: http://www.aspose.com/api/net/note





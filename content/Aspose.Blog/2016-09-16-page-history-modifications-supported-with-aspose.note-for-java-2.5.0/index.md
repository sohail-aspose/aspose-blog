---
title: 'Page History Modifications Supported with Aspose.Note for Java 2.5.0'
date: Fri, 16 Sep 2016 04:38:41 +0000
draft: false
url: /2016/09/16/page-history-modifications-supported-with-aspose.note-for-java-2.5.0/
author: Kashif Iqbal
summary: ''
tags: []
categories: ['Aspose.Note Product Family']
---

[![][1]](http://www.aspose.com/products/note/java)

[Aspose.Note for Java 2.5.0][2] has been release. This month's release incorporates new features working with revision and history information of a page in OneNote documents. It also addresses a number of API issues related to functionality that have been fixed now. For a complete list of what is new and fixed, please visit the product release notes section of the API.

# New Features and Enhancements

**Working with Page Revision Information:** This new feature lets you working with the page revision information of a document. This feature lets you read as well write the revision information to a document’s page as shown in the code sample below.

```
String inputFile = "Sample1.one";
Path inputPath = Utils.getPath(GetAllRevisionsOfSpecificPage.class, inputFile);

LoadOptions loadOptions = new LoadOptions();
loadOptions.setLoadHistory(true);
// load OneNote document
Document document = new Document(inputPath.toString(), loadOptions);
// get first page
Page firstPage = document.getFirstChild();
for (Page pageRevision : document.getPageHistory(firstPage)) {
	// Use pageRevision like a regular page.
	System.out.println("LastModifiedTime: " + pageRevision.getLastModifiedTime());
	System.out.println("CreationTime: " + pageRevision.getCreationTime());
	System.out.println("Title: " + pageRevision.getTitle());
	System.out.println("Level: " + pageRevision.getLevel());
	System.out.println("Author: " + pageRevision.getAuthor());
	System.out.println();
} 
```

**Working with Page History:** Aspose.Note API already provides support for working with Page history in a document. This month’s release brings further enhancements to this capability by providing the facility to rolling back to previous page version, pushing current page version to page history and modifying page history.

*   **Rolling Back to Previous Page Version:** This lets the API users to roll back to a previous version of the API by getting the last version from the page’s history.
*   **Pushing Current Page Version to Page History:** The current page version of the page can be included in the history collection by using the Page.clone method.
*   **Modifying Page History:** This feature allows modifying the information related to a page history such as title and author.

# Other Improvements

This month’s release also fixes a number of bugs that were reported with the latest version of the API. This further brings stability to the API functionality.

# API Resources

*   Documentation – Visit our documentation section for getting started with the API in no time
*   [API Reference Guide][3] – Gives detailed information about all the namespaces, classes and methods of the API
*   [Forum Support][4] – Post your queries on Aspose.Note forum to get assistance from our technical support team
*   [GitHub Examples][5] – Try the ready-to-use examples of the API by downloading from our GitHub repository




[1]: https://blog.aspose.com/wp-content/uploads/sites/2/2016/09/aspose_note-for-java.png "Aspose.Note for Java"
[2]: http://www.aspose.com/downloads/note/java
[3]: http://www.aspose.com/api/java/note
[4]: https://forum.aspose.com/c/note
[5]: https://github.com/aspose-note/Aspose.Note-for-Java





---
title: 'Microsoft OneNote Notebook File Format supported with Aspose.Note for Java 2.3.0'
date: Tue, 21 Jun 2016 16:14:46 +0000
draft: false
url: /2016/06/21/microsoft-onenote-notebook-file-format-supported-with-aspose.note-for-java-2.3.0/
author: Kashif Iqbal
summary: ''
tags: []
categories: ['Aspose.Note Product Family']
---

[![][1]](https://blog.aspose.com/wp-content/uploads/sites/2/2016/06/aspose_note-for-java.png)

We are pleased to announce the release of Aspose.Note for Java 2.3.0. This month's release includes new feature of providing support for Microsoft OneNote Notebook (.onetoc2) file format. It lets you load Notebook files and retrieve the documents information from these files. For a complete list of what is new and fixed, please visit the Product Release Notes page of this month's release.

# New Features & Enhancements

Support for Microsoft OneNote Notebook: This month's release provides the capability to load OneNote notebook files and manipulate them (to some extent). Following operations can be performed on the Notebook file at present.

**Loading OneNote Netbook:** The API introduces a new class, Notebook, that represents a Microsoft OneNote Notebook document. Once loaded, a notebook object contains a collection of Documents which actually refer to the OneNote documents of the notebook and can be processed using the Document class of the API.

**Loading Notebook with Load Options:** Aspose.Note API loads the notebook's child documents lazily i.e. their loading is postponed until a direct access to a specific child is made. At the same time, it provides the option to load all the child nodes at once. The API provides the NotebookLoadOptions class to specify whether the child documents are to be loaded instantly or through the default lazy behavior.

**Retrieving Documents from Notebook:** With this month's release, you can now use the API to read the child documents of a Notebook. The getChildNodes method of Notebook class lets you access each child node of the file and process them as a normal .one document using the Document class of the API.

**Reading Rich Text Nodes from Microsoft OneNote Notebook:** You can also read the information of Rich Text Nodes from the notebook using the getChildNodes method of Notebook class and specifying the RichText class. It returns all the rich text nodes information contained in the notebook.

# Other Improvements

Besides the major new feature of supporting OneNote notebook, this month's release also fixes a number of bugs related to the API functionality. This further brings stability to the API and results in improved performance.

# API Resources

*   Documentation – Visit our documentation section for getting started with the API in no time
*   [API Reference Guide][2] – Gives detailed information about all the namespaces, classes and methods of the API
*   [Forum Support][3] – Post your queries on Aspose.Note forum to get assistance from our technical support team
*   [GitHub Examples][4] – Try the ready-to-use examples of the API by downloading from our GitHub repository

We are pleased to announce the release of [Aspose.Note for Java 2.3.0][5]. This month's release includes new feature of providing support for Microsoft OneNote Notebook (.onetoc2) file format. It lets you load Notebook files and retrieve the documents information from these files. For a complete list of what is new and fixed, please visit the Product Release Notes page of this month's release.

# New Features & Enhancements

**Support for Microsoft OneNote Notebook:** This month's release provides the capability to load OneNote notebook files and manipulate them (to some extent). Following operations can be performed on the Notebook file at present.

**Loading OneNote Netbook:** The API introduces a new class, Notebook, that represents a Microsoft OneNote Notebook document. Once loaded, a notebook object contains a collection of Documents which actually refer to the OneNote documents of the notebook and can be processed using the Document class of the API.

**Loading Notebook with Load Options:** Aspose.Note API loads the notebook's child documents lazily i.e. their loading is postponed until a direct access to a specific child is made. At the same time, it provides the option to load all the child nodes at once. The API provides the NotebookLoadOptions class to specify whether the child documents are to be loaded instantly or through the default lazy behavior.

**Retrieving Documents from Notebook:** With this month's release, you can now use the API to read the child documents of a Notebook. The getChildNodes method of Notebook class lets you access each child node of the file and process them as a normal .one document using the Document class of the API.

**Reading Rich Text Nodes from Microsoft OneNote Notebook:** You can also read the information of Rich Text Nodes from the notebook using the getChildNodes method of Notebook class and specifying the RichText class. It returns all the rich text nodes information contained in the notebook.

# Other Improvements

Besides the major new feature of supporting OneNote notebook, this month's release also fixes a number of bugs related to the API functionality. This further brings stability to the API and results in improved performance.




[1]: https://blog.aspose.com/wp-content/uploads/sites/2/2016/06/aspose_note-for-java.png "Aspose.Note for Java"
[2]: http://www.aspose.com/api/java/note
[3]: https://forum.aspose.com/c/note
[4]: https://github.com/aspose-note/Aspose.Note-for-Java
[5]: http://www.aspose.com/downloads/note/java





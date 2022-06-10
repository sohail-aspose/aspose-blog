---
title: 'Creating Password Protected Documents Supported with Aspose.Note for .NET 16.11.0'
date: Tue, 15 Nov 2016 13:29:19 +0000
draft: false
url: /2016/11/15/creating-password-protected-documents-supported-with-aspose.note-for-.net-16.11.0/
author: Kashif Iqbal
summary: ''
tags: []
categories: ['Aspose.Note Product Family']
---

[![][1]](https://blog.aspose.com/wp-content/uploads/sites/2/2016/08/Aspose.Note-for-.NET_.png)

We are pleased to announce the release of [Aspose.Note for .NET 16.11.0][2]. This month’s release introduces new features and enhancements that further enrich the API functionality. It includes new features of working with password protected OneNote documents and Notebooks. It also fixes several bugs that further stabilizes the API functionality. To get an idea about what is new and fixed, please visit our documentation section for release notes of this month’s version.

# New Features and Enhancements

**Support for Creating Password Protected OneNote Documents:** In our earlier versions, the API introduced the capability of reading password protected OneNote documents. With this month’s release, the API now provides the capability to create password protected OneNote documents. This is achieved using the _OneSaveOptions_ class by specifying the _DocumentPassword_ property as shown in the following code sample.

```
Document document = new Document();

document.Save("doc.one", new OneSaveOptions() { DocumentPassword = "pass" }); 
```

**Support for Password Protected Documents as Part of OneNote Notebooks:** This month’s release extends the feature of password protected OneNote documents to Notebooks as well. This feature allows to load and save notebook files with password protected children. This, however, needs deferred loading of the notebook file and apply the document password using the _OneSaveOptions_ class.

**Setting Background Color of Table Cell:** This month’s release also enhances the functionality of working with Table cells by providing the capability to set background color of a table’s cell. The _BackgroundColor_ property of the _TableCell_ class can be used to set the color of a table cell.

**Loading and Saving of Notebook to Stream:** This month’s release also provides the capability to load and save notebook to stream. This has been implemented by providing new constructor of _Notebook_ class and overloaded _Save_ method. The child documents of the notebook also need to be saved/loaded from child object’s stream and populated in _Document_ class.

# Other Improvements

This month’s release also fixes a number of bugs related to API functionality that further improves the API stability in terms of features and quality.

# API Resources

You can get started with Aspose.Note for .NET by making use of information available in the following.

**API Documentation** – Helps getting started with the API using code samples and examples

**[Forum Support][3]** – Post your inquiries to get help from our technical support team

**[Examples][4]** – Try the ready-to-use examples of the API by downloading from our GitHub repository

**[API Reference Guide][5]** – Provides information about all the namespaces, classes and properties of the API




[1]: https://blog.aspose.com/wp-content/uploads/sites/2/2016/11/Aspose.Note-for-.NET_.png "Aspose.Note for .NET"
[2]: http://www.aspose.com/downloads/note/net
[3]: https://forum.aspose.com/c/note
[4]: https://github.com/asposenote/Aspose_Note_NET
[5]: http://www.aspose.com/api/net/note





---
title: 'Reading Password Protected OneNote Documents with Aspose.Note for .NET 2.1.0'
date: Mon, 21 Dec 2015 13:06:33 +0000
draft: false
url: /2015/12/21/reading-password-protected-onenote-documents-with-aspose.note-for-.net-2.1.0/
author: Kashif Iqbal
summary: ''
tags: []
categories: ['Aspose.Note Product Family']
---

[![][1]](http://www.aspose.com/.net/onenote-component.aspx)

We are pleased to announce the release of Aspose.Note for .NET 2.1.0. This month’s release includes new feature, enhancement and bug fixes. The API also introduces a number of classes to handle exceptions of different types. A complete list of API changes can be found in our documentation section, Public API Changes in Aspose.Note for .NET.

# New Features and Enhancements

**Reading Password Protected Documents:** Aspose.Note for .NET API now provides the capability to read password protected OneNote documents. This can be achieved using the _DocumentPassword_ property of the _LoadOptions_ class. The overloaded constructor of the _Document_ class can be used to specify the document options for loading a password protected document as shown in the following sample code.

```
LoadOptions loadOptions = new LoadOptions
{
     DocumentPassword = "password"
};
Document doc = new Document("in.one", loadOptions); 
```

**Setting Page Splitting Algorithm:** A OneNote document may contain a number of images and other documents at locations that cannot be retained while converting the document to other formats. This can result in displacement of such content to next page, for example, if it lies on the page border. This month’s release empowers users to specify the page splitting algorithm while converting the document to other formats. It can be done using the PageSplittingAlgorithm property of PdfSaveOptions class that can be set to the following values:

*   **AlwaysSplitObjectsAlgorithm** - Splits objects into several parts at pages' bottom position.
*   **KeepPartAndCloneSolidObjectToNextPageAlgorithm** - Adds objects up to the bottom of the page and clones full object to the next page in case it doesn't fit in original page.

*   **KeepSolidObjectsAlgorithm** - Shifts full object to the next page in case it doesn't fit in original page

Our documentation article, Setting Page Splitting Algorithm, demonstrates the usage of different page splitting options.

# Other Improvements

This month’s release also includes a number of bug fixes that further improves the overall API functionality. For a complete list of what is new and fixed, please visit our [product download page][2] for release notes.

# API Resources

You can get started with Aspose.Note for .NET by making use of information available in the following.

**API Documentation** – Helps getting started with the API using code samples and examples

**[Forum Support][3]** – Post your inquiries to get help from our technical support team

**[Examples][4]** – Try the ready-to-use examples of the API by downloading from our GitHub repository

**API Reference Guide** – Provides information about all the namespaces, classes and properties of the API




[1]: https://blog.aspose.com/wp-content/uploads/sites/2/2015/12/AsposeNote-for-NET-100X100.png "AsposeNote-for-NET-100X100"
[2]: http://www.aspose.com/community/files/51/.net-components/aspose.note-for-.net/default.aspx
[3]: https://forum.aspose.com/c/note
[4]: https://github.com/asposenote/Aspose_Note_NET





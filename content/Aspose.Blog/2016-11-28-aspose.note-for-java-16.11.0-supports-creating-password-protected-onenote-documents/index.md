---
title: 'Aspose.Note for Java 16.11.0 Supports Creating Password Protected OneNote Documents'
date: Mon, 28 Nov 2016 13:45:21 +0000
draft: false
url: /2016/11/28/aspose.note-for-java-16.11.0-supports-creating-password-protected-onenote-documents/
author: Kashif Iqbal
summary: ''
tags: []
categories: ['Aspose.Note Product Family']
---

[![][1]](https://blog.aspose.com/wp-content/uploads/sites/2/2016/11/aspose_note-for-java.png)Aspose team is pleased to announce the release of [Aspose.Note for Java 16.11.0][2]. Ported from its equivalent .NET version i.e. Aspose.Note for .NET 16.11.0, this month's release includes the same new features, enhancements, and bug fixes. Major improvements include the support for creating Password protected OneNote documents and saving OneNote Notebooks to stream. Bugs fixed in this month's release brings further stability to the API functionality and usage. For a detailed note on what is new and fixed, please visit the release notes section of our documentation for this version.

# New Features & Enhancements

**Support for Password Protected OneNote Documents Creation:** Aspose.Note for Java already supports reading password protected Microsoft OneNote documents. This month’s release takes the capability of working with password protected OneNote documents one step further by providing the feature of creating OneNote documents and save them with password. The _OneSaveOptions_ class provides the method _setPassword_ for protecting a Notebook document with user defined password, as shown in the code sample below.

```
OneSaveOptions saveOptions = new OneSaveOptions();

saveOptions.setDocumentPassword("pass");

document.save("doc.one", saveOptions); 
```

**Password Protecting OneNote Documents as part of OneNote Notebooks:** This month’s release also extends the feature of password protecting OneNote documents as part of OneNote notebooks. The same OneSaveOptions can be used to specify the document password while saving the OneNote document. For loading a password protected child document of Notebook, use the LoadOptions class to specify the document password.

**Support for Loading and Saving Notebook to Stream:** This month’s release also provides the capability of loading and saving Notebook from stream.

**Setting Background Color of Table Cell:** We have also improved the functionality of working with table cells by providing the capability of setting background color of table cells. The setBackgroundColor method of the TableCell class can be used to set the color of a table cell.

# Other Improvements

This month’s release also brings several improvements to the API functionality by fixing various bugs. This also adds to the overall stability of the API.

# API Resources

*   Documentation – Visit our documentation section for getting started with the API in no time
*   [API Reference Guide][3] – Gives detailed information about all the namespaces, classes and methods of the API
*   [Forum Support][4] – Post your queries on Aspose.Note forum to get assistance from our technical support team
*   [GitHub Examples][5] – Try the ready-to-use examples of the API by downloading from our GitHub repository




[1]: https://blog.aspose.com/wp-content/uploads/sites/2/2016/11/aspose_note-for-java.png "Aspose.Note for Java"
[2]: http://downloads.aspose.com/note/java/new-releases/aspose.note-for-java-16.11.0/
[3]: http://www.aspose.com/api/java/note
[4]: https://forum.aspose.com/c/note
[5]: https://github.com/aspose-note/Aspose.Note-for-Java





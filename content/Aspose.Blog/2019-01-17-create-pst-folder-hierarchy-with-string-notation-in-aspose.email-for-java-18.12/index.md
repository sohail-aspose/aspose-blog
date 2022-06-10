---
title: 'Create PST Folder Hierarchy with String Notation using Java'
date: Thu, 17 Jan 2019 19:07:06 +0000
draft: false
url: /2019/01/17/create-pst-folder-hierarchy-with-string-notation-in-aspose.email-for-java-18.12/
author: Muhammad Ahmad
summary: ''
tags: []
categories: ['Aspose.Email Product Family']
---



{{< figure align=center src="images/aspose-Email-for-Java_100.png" alt="aspose-email-for-java">}}


We are pleased to announce the release of [Aspose.Email for Java 18.12][1]. This release provides the ability to create a folder hierarchy in PST files using string notation and other bug fixes. For a detailed note on what is new and fixed, you may visit the [release notes][2] section of API.

## Create folder hierarchy in PST file by using string notation

This release adds an overload to _**addSubFolder(string name, bool createHierarchy)**_ and **_createPredefinedFolder(string name, StandardIpmFolder defaultFolder, bool createHierarchy)_** functions that enable you to create folder hierarchy using string notation as shown below in the code example.

```
PersonalStorage personalStorage = PersonalStorage
.create("CreateFolderHierarchyUsingStringNotation.pst", 
FileFormatVersion.Unicode);

personalStorage.getRootFolder()
.addSubFolder("Inbox\\Folder1\\Folder2", true);
```

By setting the second parameter of addSubFolder() to true, you can create folder hierarchy using string notation. Backslash ("\\") is used as the path separator.

## Other Improvements

This release includes several improvements in term of bug fixes. Following is the list of improvements in this month’s release.

*   Fetching messages with ImapClient
*   Converting email message to MHTML
*   Reading Distribution Lists
*   Working with MapiContact and VCF
*   VCF to MHT conversion
*   Working with ICS
*   Working with MapiMessage attachments
*   Working with EMLX files

## API Resources

We have detailed information available online for getting started with the Aspose.Email for Java API. These are:

*   [Product Documentation][3] – Provides detailed examples of working with the API
*   [API Reference Guide][4] – Details all the packages and classes of the API
*   [GitHub Examples][5] – Provides ready to run API examples
*   [Aspose.Email Forum][6] – Feel free to contact us on Aspose.Email forum for your queries




[1]: https://repository.aspose.com/webapp/#/artifacts/browse/tree/General/repo/com/aspose/aspose-email/18.12
[2]: https://docs.aspose.com/display/emailjava/Aspose.Email+for+Java+18.12+Release+Notes
[3]: https://docs.aspose.com/display/emailjava/Home
[4]: http://www.aspose.com/api/java/email
[5]: https://github.com/aspose-email/Aspose.Email-for-Java
[6]: https://forum.aspose.com/c/email





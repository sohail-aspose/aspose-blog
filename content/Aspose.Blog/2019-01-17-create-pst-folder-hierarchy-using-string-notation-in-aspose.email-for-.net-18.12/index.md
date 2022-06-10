---
title: 'Create PST Folder Hierarchy with String Notation using C#'
date: Thu, 17 Jan 2019 19:04:05 +0000
draft: false
url: /2019/01/17/create-pst-folder-hierarchy-using-string-notation-in-aspose.email-for-.net-18.12/
author: Muhammad Ahmad
summary: ''
tags: []
categories: ['Aspose.Email Product Family']
---



{{< figure align=center src="images/Aspose.Email-for-.NET_.png" alt="">}}


We are pleased to announce the release of [Aspose.Email for .NET 18.12][1]. This release provides the ability to create a folder hierarchy in PST files using string notation and other bug fixes. For a detailed note on what is fixed, please visit the [release notes][2] section of API.

## Create Folder Hierarchy in PST using String Notation

This release adds an overload to **_AddSubFolder(string name, bool createHierarchy)_** and **_CreatePredefinedFolder(string name, StandardIpmFolder defaultFolder, bool createHierarchy)_** functions that enable you to create folder hierarchy using string notation as shown below in the code example.

```
PersonalStorage personalStorage = PersonalStorage.Create(dataDir + 
"CreateFolderHierarchyUsingStringNotation.pst", 
FileFormatVersion.Unicode);

personalStorage.RootFolder.AddSubFolder(@"Inbox\\Folder1\\Folder2", 
true);
```

By setting the second parameter of AddSubFolder() to true, you can create a folder hierarchy using string notation. A backslash ("\\") is used as the path separator.

## Other Improvements

This release includes several improvements in term of bug fixes. Following is the list of improvements in this month’s release.

*   Fetching messages with ImapClient
*   Converting email message to MHTML
*   Reading Distribution Lists
*   Working with MapiContact and VCF
*   VCF to MHT conversion
*   Working with ICS
*   Working with MapiMessage attachments
*   Working with EMLX files

## API Resources

The following API resources can be of help to you in getting started with Aspose.Email API.

*   [Product Documentation][3] – Provides detailed examples of working with the API
*   [API Reference Guide][4] – Details all the namespaces and classes of the API
*   [GitHub Examples][5] – Provides ready to run API example
*   [Support Forum][6] – Write to us if you have any query or inquiry about the API




[1]: https://www.nuget.org/packages/Aspose.Email/
[2]: https://docs.aspose.com/display/emailnet/Aspose.Email+for+.NET+18.12+Release+Notes
[3]: https://docs.aspose.com/display/emailnet/Home
[4]: https://apireference.aspose.com/net/email
[5]: https://github.com/asposeemail/Aspose_Email_NET
[6]: https://forum.aspose.com/c/email





---
title: 'Create new PST files and add/import messages with Aspose.Email for .NET'
date: Wed, 02 Nov 2011 09:46:07 +0000
draft: false
url: /2011/11/02/create-new-pst-files-and-addimport-messages/
author: Saqib Razzaq
summary: ''
tags: ['Saqib Razzaq', 'Add messages to PST in csharp', 'Create PST Files in Csharp', 'PST', 'create PST']
---



{{< figure align=center src="images/aspose.email-logo120.jpg" alt="Create PST in C#">}}


We are pleased to announce the release of Aspose.Email for .NET 1.1. In this version, we have added support for creating a new PST file and adding/importing email messages to a PST. The reading PST feature has been available for a while and we've been working on the modification feature but this is the first version with which you can create your own PST files, add new folders and messages.

The API is very simple. Here is a sample code snippet for creating a new PST and adding a new folder and message to it in C#.

```
// Create new PST
PersonalStorage pst = PersonalStorage.Create(@"d:\emails\New.pst", FileFormatVersion.Unicode);

// Add new folder "Inbox"
pst.RootFolder.AddSubFolder("Inbox");
// Select the "Inbox" folder
FolderInfo inboxFolder = pst.RootFolder.GetSubFolder("Inbox");

// Add some messages to "Inbox" folder
inboxFolder.AddMessage(MapiMessage.FromFile("d:\emails\message 1.msg"));
inboxFolder.AddMessage(MapiMessage.FromFile("d:\emails\message 2.msg"));
```

Besides these new features, we have also added some other features and fixes. For release notes and downloads, please visit [https://downloads.aspose.com/email/net][1].




[1]: https://downloads.aspose.com/email/net




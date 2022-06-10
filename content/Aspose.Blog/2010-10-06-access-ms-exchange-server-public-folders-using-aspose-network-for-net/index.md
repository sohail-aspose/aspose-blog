---
title: 'Access MS Exchange Server Public Folders using Aspose.Network for .NET'
date: Wed, 06 Oct 2010 01:10:00 +0000
draft: false
url: /2010/10/06/access-ms-exchange-server-public-folders-using-aspose-network-for-net/
author: Saqib Razzaq
summary: ''
tags: []
categories: ['Aspose.Email Product Family']
---

We are pleased to announce the release of a new version of Aspose.Network for .NET v5.7. We added support for reading Public Folders from Microsoft Exchange Server and downloading messages from folders/sub-folders. Below is the simple C# code for getting the list of all public folders: // Connect to Exchange Server.

```
NetworkCredential credential = new NetworkCredential(username, password, domain);
ExchangeWebServiceClient client = new ExchangeWebServiceClient(mailboxURI, credential);
// Get list of public folders
ExchangeFolderInfoCollection folders = client.ListPublicFolders();
// Display folder name and sub-folder count
foreach (ExchangeFolderInfo publicFolder in folders)
{
      Console.WriteLine("Name: " + publicFolder.DisplayName);
      Console.WriteLine("Subfolders count: " + publicFolder.ChildFolderCount);
} 
```

Some other new features and bug fixes are also included in this release. For release notes and download, please visit [http://www.aspose.com/community/files/51/.net-components/aspose.network-for-.net/default.aspx][1].




[1]: http://www.aspose.com/community/files/51/.net-components/aspose.network-for-.net/default.aspx





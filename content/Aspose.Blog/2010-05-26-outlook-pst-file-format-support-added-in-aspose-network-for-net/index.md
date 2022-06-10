---
title: 'Outlook PST File Format Support Added in Aspose.Network for .NET'
date: Wed, 26 May 2010 19:37:00 +0000
draft: false
url: /2010/05/26/outlook-pst-file-format-support-added-in-aspose-network-for-net/
author: Saqib Razzaq
summary: ''
tags: []
categories: ['Aspose.Email Product Family']
---

We are pleased to announce the release of new version of Aspose.Network for .NET 5.3. We added support for reading Microsoft Outlook PST file. A new namespace (Aspose.Network.Outlook.Pst) and set of classes are added for reading the PST file. You can now load Microsoft Outlook PST file from disk or stream, get folders and subfolders information, get message information e.g. subject, sender, recipient etc from message contained in any folder and also save the message from PST file in MSG format to disk or stream. Sample code to display folders and message information:

```
try
{
      Console.WriteLine(“Loading PST file….”);
      // load the Outlook PST file
      PersonalStorage pst = PersonalStorage.FromFile(@”Personal Folders.pst”);
      Console.WriteLine(“Display Name: ” + pst.DisplayName);
      // get all the folders
      FolderInfoCollection folderInfoCollection = pst.RootFolder.GetSubFolders();
      // browse through each folder to display message information
      foreach (FolderInfo folderInfo in folderInfoCollection)
      {
            Console.WriteLine(“Folder: ” + folderInfo.DisplayName);
            // get messages inside this folder
            MessageInfoCollection messageInfoCollection = folderInfo.GetContents();
            foreach (MessageInfo messageInfo in messageInfoCollection)
            {
                  // display subject of message
                  Console.WriteLine(messageInfo.Subject);
                  // save this message to disk in MSG format
                  MapiMessage message = pst.GetMessage(messageInfo);
                  message.Save(messageInfo.Subject.Replace(“:”, ” “) + “.msg”);
            }
      }
}
catch (Exception ex)
{
      Console.WriteLine(ex.Message);
}
```

For release notes and downloads, please visit: [https://products.aspose.com/email][1]




[1]: https://products.aspose.com/email





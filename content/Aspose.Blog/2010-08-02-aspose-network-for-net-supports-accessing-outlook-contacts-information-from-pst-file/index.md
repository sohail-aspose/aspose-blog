---
title: 'Aspose.Network for .NET supports accessing Outlook Contacts Information from PST file'
date: Mon, 02 Aug 2010 18:28:00 +0000
draft: false
url: /2010/08/02/aspose-network-for-net-supports-accessing-outlook-contacts-information-from-pst-file/
author: Saqib Razzaq
summary: ''
tags: []
categories: ['Aspose.Email Product Family']
---

We have recently released a new version of Aspose.Network for .NET v5.5. It now supports accessing Contacts information from PST files and saving a contact to disk in MSG format.

  

Sample code:

// load the Outlook PST file  
PersonalStorage pst = PersonalStorage.FromFile(@"Outlook-File.pst");  
// Get the Contacts folder  
FolderInfo folderInfo = pst.GetFolder("Contacts");  
// loop through all the contacts in this folder  
MessageInfoCollection messageInfoCollection = folderInfo.GetContents();  
foreach (MessageInfo messageInfo in messageInfoCollection)  
{  
      // Get the contact information  
      MapiContact contact = pst.ExtractContactInfo(messageInfo);  
      // Display some contents on screen  
      Console.WriteLine("Name: " + contact.NameInfo.DisplayName);  
      // Save to disk in MSG format  
      if (contact.NameInfo.DisplayName != null)  
      {  
            MapiMessage message = pst.ExtractMessage(messageInfo);  
            string messageName = message.Subject.Replace(":", " ").Replace("\\\\", " ").Replace("?", " ").Replace("/", " ");  
            message.Save("Contacts\\\\" + messageName + ".msg");  
      }  
}

  

Some bugs were also fixed, which were reported by our customers in forums. For release notes and download, please visit [http://www.aspose.com/community/files/51/.net-components/aspose.network-for-.net/default.aspx][1].




[1]: http://www.aspose.com/community/files/51/.net-components/aspose.network-for-.net/default.aspx





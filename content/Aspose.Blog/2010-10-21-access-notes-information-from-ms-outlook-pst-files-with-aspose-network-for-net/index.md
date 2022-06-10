---
title: 'Access Notes Information from MS Outlook PST Files with Aspose.Network for .NET'
date: Thu, 21 Oct 2010 17:54:00 +0000
draft: false
url: /2010/10/21/access-notes-information-from-ms-outlook-pst-files-with-aspose-network-for-net/
author: Saqib Razzaq
summary: ''
tags: []
categories: ['Aspose.Email Product Family']
---

We are pleased to announce the release of a new version of Aspose.Network for .NET v5.8. API for accessing Notes information from Outlook PST has been added in this version. You can get the list of notes in a collection and get subject, body, creation date, color etc of each individual note.

  

Sample code to get all notes from PST:

// load the Outlook PST file  
string strBaseFolder = @"C:\\Emails\\";  
string strPSTFile = @"PersonalFolders.pst";  
PersonalStorage pst = PersonalStorage.FromFile(strBaseFolder + strPSTFile);  
  
// get the folders and messages information  
FolderInfo folderInfo = pst.RootFolder;  
  
// Get subfolders  
if (folderInfo.HasSubFolders == true)  
{  
      foreach (FolderInfo subfolderInfo in folderInfo.GetSubFolders())  
      {  
            // We only need notes information  
            if (subfolderInfo.DisplayName == "Notes")  
            {  
                  MessageInfoCollection messageInfoCollection = subfolderInfo.GetContents();  
                  foreach (MessageInfo messageInfo in messageInfoCollection)  
                  {  
                        // get note  
                        MapiMessage message = pst.ExtractMessage(messageInfo);  
                        MapiNote note = message.ToMapiMessageItem() as MapiNote;  
                        Console.WriteLine("Subject: " + note.Subject);  
                        Console.WriteLine("Body: " + note.Body);  
                  }  
            }  
      }  
}

  

We also fixed some bugs, which were reported in forums by customers. For release notes and download, please visit [http://www.aspose.com/community/files/51/.net-components/aspose.network-for-.net/default.aspx][1].




[1]: http://www.aspose.com/community/files/51/.net-components/aspose.network-for-.net/default.aspx





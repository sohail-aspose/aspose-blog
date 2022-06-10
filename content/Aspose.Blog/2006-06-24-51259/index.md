---
title: 'Aspose.Network 2.4.4.0 Released'
date: Sat, 24 Jun 2006 06:00:00 +0000
draft: false
url: /2006/06/24/51259/
author: Iret
summary: ''
tags: ['Kyle Huang']
---

Dear Customers,

We've released Aspose.Network 2.4.4.0.

What's new features in this version:

*   Supports Imap v4 protocols, a new Aspose.Network.Imap namespace is exposed.

>    \[C#\]
> 
>    ImapClient client = new ImapClient("127.0.0.1", "user", "password");  
>    client.Connect(true);  
>      
>    Console.WriteLine("Selecting folder '{0}'...", "inbox");  
>    //select the inbox mail folder  
>    client.SelectFolder(ImapFolderInfo.Inbox);  
>      
>    ImapFolderInfo folder = client.CurrentFolder;
> 
>    // Show number of messages in the folder  
>    Console.WriteLine("{0} messages found.", folder.TotalMessageCount);  
>      
>    MessageInfoCollection list = client.GetMessageInfoList();
> 
>    // Download each message  
>    for (int i = 0; i < list.Count; i++)  
>    {  
>     ImapMessageInfo message = list\[ i \];
> 
>     // Create filename from email unique ID  
>     string filename = message.UniqueId + ".eml";  
>     if (message.Subject != null)  
>     {  
>      //get the message and save the attachments  
>       if (message.Subject.Equals("Imap Test",                                                      StringComparison.InvariantCultureIgnoreCase))  
>       {  
>       client.SaveMessage(message.UniqueId, filename);  
>       MimeMessage mime = client.GetMimeMessage(message.UniqueId);  
>       foreach (Aspose.Network.Mime.MimePart attachment in mime.GetAttachments())  
>         attachment.SaveDecodedContent(attachment.GetFileName());       
>      }  
>     }  
>       
>     //save the eml file locally  
>     client.SaveMessage(message.UniqueId, filename);  
>    }

*   Resolved x-mailer bug in SmtpClient.Merge
*   Improve the Mail Merge feature, a new event called TemplateMerge is exposed
*   Resolved some minimal issues in Calendar components.

Thanks








---
title: 'Aspose.Network 3.3.0.0 Released'
date: Sat, 17 Mar 2007 01:51:00 +0000
draft: false
url: /2007/03/17/70590/
author: Iret
summary: ''
tags: []
categories: ['Aspose.Email Product Family']
---

We have released Aspose.Network 3.3.0.0!

**What's new?**

*   This is a major release for Aspose.Network, with Microsoft Exchange Server supporting (WEBDAV).
    *   Supports fetch e-mail messages on an exchange store.
    *   Supports delete e-mail messages
    *   Supports send e-mail messages

    \[C#\]

    string mailboxUri = "http://gz.aspose.com/exchange/andrew";   
    string username = "andrew";  
    string password = "12345678";  
    string domain = "aspose";

    NetworkCredential credential = new NetworkCredential(username, password, domain);

   //create an exchangeclient  
   ExchangeClient client = new ExchangeClient(mailboxUri, credential);  
   try  
   {  
    //query mailbox  
    ExchangeMailboxInfo mailbox = client.GetMailboxInfo();  
    //list messages in the Inbox  
    ExchangeMessageInfoCollection messages = client.ListMessages(mailbox.InboxUri, false);

    foreach (ExchangeMessageInfo info in messages)  
    {  
     //save the message locally  
     client.SaveMessage(info.UniqueUri, info.Subject + ".eml");  
    }  
   }  
   catch(ExchangeException ex)  
   {  
    Console.WriteLine(ex.ToString());  
   }

*   Adding a new Windows Form control, **FileDragPanel**, which supports dragging and dropping messages from Microsoft Outlook.
*   Quick start tutorial for Aspose.Network has also been updated.
*   Fixed the bug in Pop3Client.DeleteMessage .
*   Fixed the bug in MailMessage.Load function, which may lead to a hang in parsing e-mail messages .
*   All hotfixes from 3.2.0\*.









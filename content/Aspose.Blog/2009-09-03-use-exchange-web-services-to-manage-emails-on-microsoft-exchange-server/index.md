---
title: 'Use Exchange Web Services to Manage Emails on Microsoft Exchange Server'
date: Thu, 03 Sep 2009 22:33:00 +0000
draft: false
url: /2009/09/03/use-exchange-web-services-to-manage-emails-on-microsoft-exchange-server/
author: Saqib Razzaq
summary: ''
tags: []
categories: ['Aspose.Email Product Family']
---

We have recently released a new version of Aspose.Network for .NET. In this release (Aspose.Network for .NET 4.8.0.0), we added support for Exchange Web Services to connect to Microsoft Exchange Server and manage emails. You can get the mailbox information, send and receive email messages, list messages from Inbox, delete or fetch messages from Inbox or other folders. For utilizing Exchange Web Services, we added a new class ExchangeWebServiceClient. Below is the C# sample code for getting mailbox information and list of messages from Inbox folder using Exchange Web Services:

```
// create an instance of ExchangeWebServiceClient
ExchangeWebServiceClient client = new ExchangeWebServiceClient(
    "https://exchange-server-host/ews/Exchange.asmx",
    new NetworkCredential("user", "password", "domain"));

// get mailbox information
ExchangeMailboxInfo mailbox = client.GetMailboxInfo(); 

// get list of messages from inbox folder
ExchangeMessageInfoCollection col = client.ListMessages(mailbox.InboxUri);
```

We also fixed some bugs along with the above new feature. For downloading the latest release and detailed release notes, please visit [https://downloads.aspose.com/email/net][1]




[1]: https://downloads.aspose.com/email/net





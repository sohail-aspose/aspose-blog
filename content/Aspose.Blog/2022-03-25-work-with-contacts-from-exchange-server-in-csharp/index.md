---
title: 'Add, Update and Delete Contacts from Microsoft Exchange Server in C#'
date: Fri, 25 Mar 2022 14:36:06 +0000
draft: false
url: /2022/03/25/work-with-contacts-from-exchange-server-in-csharp/
author: ''Usman Aziz''
summary: '[Microsoft Exchange Server][1] is a popular platform that provides various collaboration services like email, calendars, contacts, etc. In the [previous post][2], we have shown you how to read emails from Microsoft Exchange Server. However, you may also need to work with the contacts on the Exchange Server programmatically. In this article, you will learn **how to add, delete, or update contacts on Microsoft Exchange Server in C# .NET**.'
tags: ['Add Contacts to MS Exchange Server Csharp', 'Delete Contacts from MS Exchange Server Csharp', 'Update a Contact on MS Exchange Server Csharp']
categories: ['Aspose.Email Product Family']
---



{{< figure align=center src="images/aspose-email-exchange.png" alt="Add or Delete Contacts from Microsoft Exchange Server in C#">}}


[Microsoft Exchange Server][3] is a popular platform that provides various collaboration services like email, calendars, contacts, etc. In the [previous post][4], we have shown you how to read emails from Microsoft Exchange Server. However, you may also need to work with the contacts on the Exchange Server programmatically. In this article, you will learn **how to add, delete, or update contacts on Microsoft Exchange Server in C# .NET**.

*   [.NET API to Access Contacts on MS Exchange Server][5]
*   [Add Contacts to MS Exchange Server][6]
*   [Delete Contacts from MS Exchange Server][7]
*   [Update a Contact on MS Exchange Server][8]

## C# .NET API to Access Contacts on MS Exchange Server {#API-to-Access-Contacts-on-Exchange-Server}

To work with contacts on Microsoft Exchange Server, we will use [Aspose.Email for .NET][9]. It is a well-known API to work with different email clients from within .NET applications. You can either [download][10] the API's DLL or install it from NuGet using the following command.

```
PM> Install-Package Aspose.Email
```

## Add Contacts to MS Exchange Server in C# {#Add-Contacts-to-Exchange-Server}

The following are the steps to add contacts to Microsoft Exchange Server in C#.

*   First, create and initialize [NetworkCredential][11] object with username, password, and domain.
*   Then, initialize [IEWSClient][12] with mailbox URI and _NetworkCredential_ object.
*   Create an object of [Contact][13] class and set its properties such as name, job, gender, phone, associated persons, etc.
*   Finally, call [EWSClient.CreateContact(Contact)][14] to add contact.

The following code sample shows how to add a contact to Microsoft Exchange Server in C#.

{{< gist aspose-com-gists f4e69195ff3bf9836fbf8be1bada88d3 "add-contact.cs" >}}

## Delete Contacts from MS Exchange Server in C# {#Delete-Contacts-from-Exchange-Server}

You can also delete a contact from the MS Exchange Server. To filter the contacts, you can use the name, email, or any other suitable property. The following are the steps to delete a contact from Microsoft Exchange Server in C#.

*   First, initialize [IEWSClient][15] object.
*   Then, get contacts from MS Exchange Server using [IEWSClient.GetContacts(EWSClient.MailboxInfo.ContactsUri)][16] method.
*   Loop through the contacts and filter the required one.
*   Finally, delete a filtered contact using [IEWSClient.DeleteItem(Contact.Id.EWSId, DeletionOptions.DeletePermanently)][17] method.

The following code sample shows how to delete contacts from Microsoft Exchange Server in C#.

{{< gist aspose-com-gists f4e69195ff3bf9836fbf8be1bada88d3 "delete-contact.cs" >}}

## Update a Contact on Exchange Server in C# {#Update-a-Contact-on-Exchange-Server}

You can also update a contact on MS Exchange Server using Aspose.Email for .NET. The following are the steps to perform this operation.

*   First, create and initialize [NetworkCredential][18] object with username, password, and domain.
*   Then, initialize [IEWSClient][19] with mailbox URI and _NetworkCredential_ object.
*   Get contacts from Exchange Server using [IEWSClient.GetContacts(EWSClient.MailboxInfo.ContactsUri)][20] method.
*   After that, loop through the contacts and filter the desired contact.
*   Finally, update the contact's properties and call [IEWSClient.UpdateContact(Contact)][21] to save it.

The following code sample shows how to update a contact on MS Exchange Server in C#.

{{< gist aspose-com-gists f4e69195ff3bf9836fbf8be1bada88d3 "update-contact.cs" >}}

## Get a Free API License {#Get-a-Free-API-License}

You can get a [free temporary license][22] to use Aspose.Email for .NET without evaluation limitations.

## Conclusion

In this article, you have learned how to work with contacts on Microsoft Exchange Server in C#. We have demonstrated how to add, remove, and update contacts from the MS Exchange Server programmatically in C#. Besides, you can explore the [documentation][23] to read more about Aspose.Email for .NET. Also, you can ask your questions via our [forum][24].

## See Also

*   [Create and Send Outlook Emails using C#][25]




[1]: https://en.wikipedia.org/wiki/Microsoft_Exchange_Server
[2]: https://blog.aspose.com/2020/11/20/read-emails-from-exchange-server-using-csharp/
[3]: https://en.wikipedia.org/wiki/Microsoft_Exchange_Server
[4]: https://blog.aspose.com/2020/11/20/read-emails-from-exchange-server-using-csharp/
[5]: #API-to-Access-Contacts-on-Exchange-Server
[6]: #Add-Contacts-to-Exchange-Server
[7]: #Delete-Contacts-from-Exchange-Server
[8]: #Update-a-Contact-on-Exchange-Server
[9]: https://products.aspose.com/email/net
[10]: https://downloads.aspose.com/email/net
[11]: https://docs.microsoft.com/en-us/dotnet/api/system.net.networkcredential
[12]: https://apireference.aspose.com/email/net/aspose.email.clients.exchange.webservice/iewsclient
[13]: https://apireference.aspose.com/email/net/aspose.email.personalinfo/contact
[14]: https://apireference.aspose.com/email/net/aspose.email.clients.exchange.webservice.iewsclient/createcontact/methods/1
[15]: https://apireference.aspose.com/email/net/aspose.email.clients.exchange.webservice/iewsclient
[16]: https://apireference.aspose.com/email/net/aspose.email.clients.exchange.webservice/iewsclient/methods/getcontacts
[17]: https://apireference.aspose.com/email/net/aspose.email.clients.exchange.webservice/iewsclient/methods/deleteitem
[18]: https://docs.microsoft.com/en-us/dotnet/api/system.net.networkcredential
[19]: https://apireference.aspose.com/email/net/aspose.email.clients.exchange.webservice/iewsclient
[20]: https://apireference.aspose.com/email/net/aspose.email.clients.exchange.webservice/iewsclient/methods/getcontacts
[21]: https://apireference.aspose.com/email/net/aspose.email.clients.exchange.webservice.iewsclient/updatecontact/methods/1
[22]: https://purchase.aspose.com/temporary-license
[23]: https://docs.aspose.com/email/net/
[24]: https://forum.aspose.com/
[25]: https://blog.aspose.com/2020/01/23/create-send-outlook-email-eml-msg-csharp-net-core/





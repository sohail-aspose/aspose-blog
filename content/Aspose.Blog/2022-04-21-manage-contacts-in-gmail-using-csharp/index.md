---
title: 'Create, Update, and Delete Contacts in Gmail using C#'
seoTitle: "C# Create, Update, and Delete Contacts in Gmail | .NET Gmail API"
description: "Use .NET Gmail API to create and update contacts in a Gmail account in C#. Delete desired contacts from Gmail account programmatically in C#."
date: Thu, 21 Apr 2022 16:28:02 +0000
draft: false
url: /2022/04/21/manage-contacts-in-gmail-using-csharp/
author: Usman Aziz
summary: '[Gmail][1] is one of the popular and widely used email applications around the globe. Along with managing emails, it allows working with calendars, contacts, chats, etc. and provides other collaboration services. In the [previous article][2], you have seen how to import contacts from a Gmail account within a .NET application. In this article, we will cover **how to create, update, and delete contacts in a Gmail account using C# .NET**.'
tags: ['Create a Contact on Gmail in CSharp', 'Delete a Contact on Gmail Csharp', 'DotNet API to Manage Gmail Contacts', 'DotNet Gmail API', 'Update a Contact on Gmail in Csharp']
categories: ['Aspose.Email Product Family']
---



{{< figure align=center src="images/Create-Update-and-Delete-Gmail-Contacts.png" alt="Create, Update, and Delete Contacts in Gmail using C#">}}


[Gmail][3] is one of the popular and widely used email applications around the globe. Along with managing emails, it allows working with calendars, contacts, chats, etc. and provides other collaboration services. In the [previous article][4], you have seen how to import contacts from a Gmail account within a .NET application. In this article, we will cover **how to create, update, and delete contacts in a Gmail account using C# .NET**.

*   [C# .NET API to Manage Gmail Contacts][5]
*   [Create a Contact on Gmail][6]
*   [Update a Contact on Gmail][7]
*   [Delete a Contact on Gmail][8]

## C# .NET API to Create, Update and Delete Gmail Contacts {#API-to-Manage-Gmail-Contacts}

To create and manipulate contacts in a Gmail account, we will use [Aspose.Email for .NET][9]. It is an email processing API that lets you manipulate emails and work with popular email clients. You can either [download][10] the API’s DLL or install it from [NuGet][11] using the following command.

```
PM> Install-Package Aspose.Email
```

Before you start working, you need to create a project on the Google Developer Console, which will allow you to communicate with Gmail. To create one, you can follow [this guide][12].

To access and manipulate contacts in a Gmail account, we need to write some code to handle the user’s information and perform authentication. For the Gmail user, we will first create a class named **TestUser** and then inherit it from **GoogleUser** class. The following is the complete implementation of both of the classes.

{{< gist aspose-com-gists 66a1b4d034b3b4f72f593359c8624ddf "GoogleUser.cs" >}}

Now, we need to create a helper class that will take care of the authentication of a Gmail account. We will name this class as **GoogleOAuthHelper**. The following is the complete implementation of this class.

{{< gist aspose-com-gists 66a1b4d034b3b4f72f593359c8624ddf "GoogleOAuthHelper.cs" >}}

## Create a Contact on Gmail in C# {#Create-a-Contact-on-Gmail}

The following are the steps to create a contact on Gmail in C#.

*   First, create a Google user, get an access token, and initialize an [IGmailClient][13] object.
*   Then, create an object of the [Contact][14] class.
*   Set properties of the contact such as name, prefix, profession, etc.
*   To set the postal address, create an instance of [PostalAddress][15] and set its properties.
*   Add newly created address to the collection using the [Contact.PhysicalAddresses.Add(PostalAddress)][16] method.
*   Set phone number details using [PhoneNumber][17] class.
*   Add phone number details to collection using [Contact.PhoneNumbers.Add(PhoneNumber)][18] method.
*   Create an instance of [EmailAddress][19] class, set the email address, and assign it to the contact.
*   Finally, call [IGmailClient.CreateContact(Contact)][20] method to create Gmail contact.

The following code sample shows how to create a contact on Gmail in C#.

{{< gist aspose-com-gists 66a1b4d034b3b4f72f593359c8624ddf "create-gmail-contact.cs" >}}

## Update a Contact on Gmail in C# {#Update-a-Contact-on-Gmail}

You can also update the details of a Gmail contact after accessing it. The following are the steps to update a contact in a Gmail account in C#.

*   First, create a Google user, get an access token, and initialize an [IGmailClient][21] object.
*   Get contacts in an array using [IGmailClient.GetAllContacts()][22] method.
*   Fetch required contact from the array in a [Contact][23] object.
*   Update the details of contact and call [IGmailClient.UpdateContact(contact)][24] method.

The following code sample shows how to update a contact in Gmail in C#.

{{< gist aspose-com-gists 66a1b4d034b3b4f72f593359c8624ddf "update-gmail-contact.cs" >}}

## Delete a Contact on Gmail in C# {#Delete-a-Contact-on-Gmail}

Finally, let's see how to delete a Gmail contact using C#. The following are the steps to perform this operation.

*   First, create a Google user, get an access token, and initialize an [IGmailClient][25] object.
*   Get contacts in an array using [IGmailClient.GetAllContacts()][26] method.
*   Filter the desired contact from the array in a [Contact][27] object.
*   Finally, call [IGmailClient.DeleteContact(Contact.Id.GoogleId)][28] method to delete the contact.

The following code sample shows how to delete a contact on Gmail in C#.

{{< gist aspose-com-gists 66a1b4d034b3b4f72f593359c8624ddf "delete-gmail-contact.cs" >}}

## Get a Free API License

You can use Aspose.Email for .NET without evaluation limitations using a [free temporary license][29].

## Conclusion

In this article, you have learned how to create and update contacts in a Gmail account in C# .NET. Furthermore, you have seen how to delete a Gmail contact programmatically. Besides, you can visit the [documentation][30] to explore other features of Aspose.Email for .NET. In case you would have any questions, you can post to our [forum][31].

## See Also

*   [Read Emails from MS Exchange Server using C#][32]




[1]: https://en.wikipedia.org/wiki/Gmail
[2]: https://blog.aspose.com/2022/01/19/import-contacts-from-gmail-in-csharp-net/
[3]: https://en.wikipedia.org/wiki/Gmail
[4]: https://blog.aspose.com/2022/01/19/import-contacts-from-gmail-in-csharp-net/
[5]: #API-to-Manage-Gmail-Contacts
[6]: #Create-a-Contact-on-Gmail
[7]: #Update-a-Contact-on-Gmail
[8]: #Delete-a-Contact-on-Gmail
[9]: https://products.aspose.com/email/net/
[10]: https://downloads.aspose.com/email/net/
[11]: https://www.nuget.org/packages/Aspose.Email
[12]: https://docs.aspose.com/email/net/gmail-utility-features/#creating-project-in-google-developer-console
[13]: https://apireference.aspose.com/email/net/aspose.email.clients.google/igmailclient
[14]: https://apireference.aspose.com/email/net/aspose.email.personalinfo/contact
[15]: https://apireference.aspose.com/email/net/aspose.email.personalinfo/postaladdress
[16]: https://apireference.aspose.com/email/net/aspose.email.personalinfo/contact/properties/physicaladdresses
[17]: https://apireference.aspose.com/email/net/aspose.email.personalinfo/phonenumber
[18]: https://apireference.aspose.com/email/net/aspose.email.personalinfo/contact/properties/phonenumbers
[19]: https://apireference.aspose.com/email/net/aspose.email.personalinfo/emailaddress
[20]: https://apireference.aspose.com/email/net/aspose.email.clients.google/igmailclient/methods/createcontact/index
[21]: https://apireference.aspose.com/email/net/aspose.email.clients.google/igmailclient
[22]: https://apireference.aspose.com/email/net/aspose.email.clients.google/igmailclient/methods/getallcontacts
[23]: https://apireference.aspose.com/email/net/aspose.email.personalinfo/contact
[24]: https://apireference.aspose.com/email/net/aspose.email.clients.google/igmailclient/methods/updatecontact
[25]: https://apireference.aspose.com/email/net/aspose.email.clients.google/igmailclient
[26]: https://apireference.aspose.com/email/net/aspose.email.clients.google/igmailclient/methods/getallcontacts
[27]: https://apireference.aspose.com/email/net/aspose.email.personalinfo/contact
[28]: https://apireference.aspose.com/email/net/aspose.email.clients.google/igmailclient/methods/deletecontact
[29]: https://products.aspose.com/email
[30]: https://docs.aspose.com/email/net/
[31]: https://forum.aspose.com/
[32]: https://blog.aspose.com/2020/11/20/read-emails-from-exchange-server-using-csharp/





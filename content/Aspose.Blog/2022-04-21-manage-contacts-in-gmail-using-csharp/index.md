---
title: 'Create, Update, and Delete Contacts in Gmail using C#'
date: Thu, 21 Apr 2022 16:28:02 +0000
draft: false
url: /2022/04/21/manage-contacts-in-gmail-using-csharp/
author: 'Usman Aziz'
summary: '[Gmail](https://en.wikipedia.org/wiki/Gmail) is one of the popular and widely used email applications around the globe. Along with managing emails, it allows working with calendars, contacts, chats, etc. and provides other collaboration services. In the [previous article](https://blog.aspose.com/2022/01/19/import-contacts-from-gmail-in-csharp-net/), you have seen how to import contacts from a Gmail account within a .NET application. In this article, we will cover **how to create, update, and delete contacts in a Gmail account using C# .NET**.'
tags: ['Create a Contact on Gmail in CSharp', 'Delete a Contact on Gmail Csharp', 'DotNet API to Manage Gmail Contacts', 'DotNet Gmail API', 'Update a Contact on Gmail in Csharp']
categories: ['Aspose.Email Product Family']
---



{{< figure align=center src="images/Create-Update-and-Delete-Gmail-Contacts.png" alt="Create, Update, and Delete Contacts in Gmail using C#">}}


[Gmail](https://en.wikipedia.org/wiki/Gmail) is one of the popular and widely used email applications around the globe. Along with managing emails, it allows working with calendars, contacts, chats, etc. and provides other collaboration services. In the [previous article](https://blog.aspose.com/2022/01/19/import-contacts-from-gmail-in-csharp-net/), you have seen how to import contacts from a Gmail account within a .NET application. In this article, we will cover **how to create, update, and delete contacts in a Gmail account using C# .NET**.

*   [C# .NET API to Manage Gmail Contacts](#API-to-Manage-Gmail-Contacts)
*   [Create a Contact on Gmail](#Create-a-Contact-on-Gmail)
*   [Update a Contact on Gmail](#Update-a-Contact-on-Gmail)
*   [Delete a Contact on Gmail](#Delete-a-Contact-on-Gmail)

## C# .NET API to Create, Update and Delete Gmail Contacts {#API-to-Manage-Gmail-Contacts}

To create and manipulate contacts in a Gmail account, we will use [Aspose.Email for .NET](https://products.aspose.com/email/net/). It is an email processing API that lets you manipulate emails and work with popular email clients. You can either [download](https://downloads.aspose.com/email/net/) the API’s DLL or install it from [NuGet](https://www.nuget.org/packages/Aspose.Email) using the following command.

```
PM> Install-Package Aspose.Email
```

Before you start working, you need to create a project on the Google Developer Console, which will allow you to communicate with Gmail. To create one, you can follow [this guide](https://docs.aspose.com/email/net/gmail-utility-features/#creating-project-in-google-developer-console).

To access and manipulate contacts in a Gmail account, we need to write some code to handle the user’s information and perform authentication. For the Gmail user, we will first create a class named **TestUser** and then inherit it from **GoogleUser** class. The following is the complete implementation of both of the classes.

{{< gist aspose-com-gists 66a1b4d034b3b4f72f593359c8624ddf "GoogleUser.cs" >}}

Now, we need to create a helper class that will take care of the authentication of a Gmail account. We will name this class as **GoogleOAuthHelper**. The following is the complete implementation of this class.

{{< gist aspose-com-gists 66a1b4d034b3b4f72f593359c8624ddf "GoogleOAuthHelper.cs" >}}

## Create a Contact on Gmail in C# {#Create-a-Contact-on-Gmail}

The following are the steps to create a contact on Gmail in C#.

*   First, create a Google user, get an access token, and initialize an [IGmailClient](https://apireference.aspose.com/email/net/aspose.email.clients.google/igmailclient) object.
*   Then, create an object of the [Contact](https://apireference.aspose.com/email/net/aspose.email.personalinfo/contact) class.
*   Set properties of the contact such as name, prefix, profession, etc.
*   To set the postal address, create an instance of [PostalAddress](https://apireference.aspose.com/email/net/aspose.email.personalinfo/postaladdress) and set its properties.
*   Add newly created address to the collection using the [Contact.PhysicalAddresses.Add(PostalAddress)](https://apireference.aspose.com/email/net/aspose.email.personalinfo/contact/properties/physicaladdresses) method.
*   Set phone number details using [PhoneNumber](https://apireference.aspose.com/email/net/aspose.email.personalinfo/phonenumber) class.
*   Add phone number details to collection using [Contact.PhoneNumbers.Add(PhoneNumber)](https://apireference.aspose.com/email/net/aspose.email.personalinfo/contact/properties/phonenumbers) method.
*   Create an instance of [EmailAddress](https://apireference.aspose.com/email/net/aspose.email.personalinfo/emailaddress) class, set the email address, and assign it to the contact.
*   Finally, call [IGmailClient.CreateContact(Contact)](https://apireference.aspose.com/email/net/aspose.email.clients.google/igmailclient/methods/createcontact/index) method to create Gmail contact.

The following code sample shows how to create a contact on Gmail in C#.

{{< gist aspose-com-gists 66a1b4d034b3b4f72f593359c8624ddf "create-gmail-contact.cs" >}}

## Update a Contact on Gmail in C# {#Update-a-Contact-on-Gmail}

You can also update the details of a Gmail contact after accessing it. The following are the steps to update a contact in a Gmail account in C#.

*   First, create a Google user, get an access token, and initialize an [IGmailClient](https://apireference.aspose.com/email/net/aspose.email.clients.google/igmailclient) object.
*   Get contacts in an array using [IGmailClient.GetAllContacts()](https://apireference.aspose.com/email/net/aspose.email.clients.google/igmailclient/methods/getallcontacts) method.
*   Fetch required contact from the array in a [Contact](https://apireference.aspose.com/email/net/aspose.email.personalinfo/contact) object.
*   Update the details of contact and call [IGmailClient.UpdateContact(contact)](https://apireference.aspose.com/email/net/aspose.email.clients.google/igmailclient/methods/updatecontact) method.

The following code sample shows how to update a contact in Gmail in C#.

{{< gist aspose-com-gists 66a1b4d034b3b4f72f593359c8624ddf "update-gmail-contact.cs" >}}

## Delete a Contact on Gmail in C# {#Delete-a-Contact-on-Gmail}

Finally, let's see how to delete a Gmail contact using C#. The following are the steps to perform this operation.

*   First, create a Google user, get an access token, and initialize an [IGmailClient](https://apireference.aspose.com/email/net/aspose.email.clients.google/igmailclient) object.
*   Get contacts in an array using [IGmailClient.GetAllContacts()](https://apireference.aspose.com/email/net/aspose.email.clients.google/igmailclient/methods/getallcontacts) method.
*   Filter the desired contact from the array in a [Contact](https://apireference.aspose.com/email/net/aspose.email.personalinfo/contact) object.
*   Finally, call [IGmailClient.DeleteContact(Contact.Id.GoogleId)](https://apireference.aspose.com/email/net/aspose.email.clients.google/igmailclient/methods/deletecontact) method to delete the contact.

The following code sample shows how to delete a contact on Gmail in C#.

{{< gist aspose-com-gists 66a1b4d034b3b4f72f593359c8624ddf "delete-gmail-contact.cs" >}}

## Get a Free API License

You can use Aspose.Email for .NET without evaluation limitations using a [free temporary license](https://products.aspose.com/email).

## Conclusion

In this article, you have learned how to create and update contacts in a Gmail account in C# .NET. Furthermore, you have seen how to delete a Gmail contact programmatically. Besides, you can visit the [documentation](https://docs.aspose.com/email/net/) to explore other features of Aspose.Email for .NET. In case you would have any questions, you can post to our [forum](https://forum.aspose.com/).

## See Also

*   [Read Emails from MS Exchange Server using C#](https://blog.aspose.com/2020/11/20/read-emails-from-exchange-server-using-csharp/)





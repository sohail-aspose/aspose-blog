---
title: 'Import Gmail Contacts in C# .NET'
seoTitle: "Import Gmail Contacts in C# ASP.NET | .NET Gmail API"
description: "Use .NET email library to access and import contacts from a Gmail account in C# ASP.NET. Import contacts from a specific email group programmatically."
date: Wed, 19 Jan 2022 17:45:25 +0000
draft: false
url: /2022/01/19/import-contacts-from-gmail-in-csharp-net/
author: Usman Aziz
summary: '[Gmail][1] is a popular and widely used email service provided by Google. Along with sending and receiving emails, it offers various additional features such as auto-reply, chats, etc. As a programmer, you may come across the scenario when you need to import contacts from a particular Gmail account. To accomplish that from within .NET applications, this article covers **how to import contacts from Gmail in C# .NET**. Moreover, we will demonstrate how to fetch contacts from a specific email group.'
tags: ['Dotnet API to Import Contacts from Gmail', 'Import Contacts from Email Group in Csharp', 'Import Contacts from Gmail in Csharp']
categories: ['Aspose.Email Product Family']
---



{{< figure align=center src="images/Import-Contacts-from-Gmail-Account.png" alt="Import Contacts from Gmail in C# .NET">}}


[Gmail][2] is a popular and widely used email service provided by Google. Along with sending and receiving emails, it offers various additional features such as auto-reply, chats, etc. As a programmer, you may come across the scenario when you need to import contacts from a particular Gmail account. To accomplish that from within .NET applications, this article covers **how to import Gmail contacts in C# .NET**. Moreover, we will demonstrate how to fetch contacts from a specific email group.

*   [.NET API to Import Contacts from Gmail][3]
*   [Import Contacts from Gmail in C#][4]
    *   [Import Gmail Contacts][5]
    *   [Get Contacts from a Specific Group][6]

## C# .NET API to Import Gmail Contacts {#API-to-Import-Contacts-from-Gmail}

To import contacts from a Gmail account, we will use [Aspose.Email for .NET][7]. It is a feature-rich API that allows you to create and send emails quite easily. Moreover, it lets you manipulate various email formats including MSG and EML. You can either [download][8] the API's DLL or install it using [NuGet][9].

```
PM> Install-Package Aspose.Email
```

## Import Contacts from Gmail in C# {#Import-Contacts-from-Gmail}

To access the contacts from a Gmail account, we need to write some code to handle the user's information and to perform Gmail authentication. For the Gmail user, we will first create a class named **TestUser** and then inherit it from **GoogleUser** class. The following is the complete implementation of both of the classes.

{{< gist aspose-com-gists a466d3365e805aea2cf68f50a95b9d05 "GoogleUser.cs" >}}

Now, we need to create a helper class that will take care of the authentication of a Gmail account. We will name this class as **GoogleOAuthHelper**. The following is the complete implementation of this class.

{{< gist aspose-com-gists a466d3365e805aea2cf68f50a95b9d05 "GoogleOAuthHelper.cs" >}}

### Import Contacts from a Gmail Account {#Import-Contacts}

At this stage, we are ready to access contacts in a Gmail account. The following are the steps to import contacts from a Gmail account in C#.

*   Create an object of **GoogleUser** class and initialize it with name, email, password, client ID and client secret.
*   Create two string objects to store access token and refresh token.
*   Call **GoogleOAuthHelper.GetAccessToken(GoogleUser, out string, out string)** method to get the access and refresh tokens.
*   Get an instance of [GmailClient][10] class into an [IGmailClient][11] object.
*   Create an array of [Contact][12] and get all the contacts using [IGmailClient.GetAllContacts()][13] method.
*   Loop through array to access each contact.

The following code sample shows how to import contacts from a Gmail account in C#.

{{< gist aspose-com-gists a466d3365e805aea2cf68f50a95b9d05 "Import-Gmail-Contacts.cs" >}}

## Import Gmail Contacts from a Group {#Get-Contacts-from-a-Specific-Group}

You can also access contacts from a specific email group in Gmail. The following are the steps to perform this operation.

*   Create an object of **GoogleUser** class and initialize it with name, email, password, client ID and client secret.
*   Create two string objects to store access token and refresh token.
*   Call **GoogleOAuthHelper.GetAccessToken(GoogleUser, out string, out string)** method to get the access token.
*   Get an instance of [GmailClient][14] class into an [IGmailClient][15] object.
*   Get all email groups into a [ContactGroupCollection][16] object using [IGmailClient.GetAllGroups()][17] method.
*   Access the desired [GoogleContactGroup][18] using its name.
*   Create an array of [Contact][19] and get all the contacts from group using [IGmailClient.GetContactsFromGroup(string)][20] method.
*   Loop through array to access each contact.

The following code sample shows how to import contacts from a specific email group in C#.

{{< gist aspose-com-gists a466d3365e805aea2cf68f50a95b9d05 "Import-Gmail-Contacts-From-Group.cs" >}}

## Get a Free API License {#Get-a-Free-API-License}

You can get a [free temporary license][21] to use Aspose.Email for .NET without evaluation limitations.

## Conclusion

In this article, you have learned how to import Gmail contacts from accounts programmatically in C#. Moreover, you have seen how to access contacts from a particular email group in Gmail. Besides, you can explore other features of Aspose.Email for .NET using the [documentation][22]. Also, you can ask your questions via our [forum][23].

## See Also

*   [Create and Send Outlook Emails using C#][24]




[1]: https://www.google.com/gmail/about/
[2]: https://www.google.com/gmail/about/
[3]: #API-to-Import-Contacts-from-Gmail
[4]: #Import-Contacts-from-Gmail
[5]: #Import-Contacts
[6]: #Get-Contacts-from-a-Specific-Group
[7]: https://products.aspose.com/email/net/
[8]: https://downloads.aspose.com/email/net/
[9]: https://www.nuget.org/packages/Aspose.Email
[10]: https://apireference.aspose.com/email/net/aspose.email.clients.google/gmailclient
[11]: https://apireference.aspose.com/email/net/aspose.email.clients.google/igmailclient
[12]: https://apireference.aspose.com/email/net/aspose.email.personalinfo/contact
[13]: https://apireference.aspose.com/email/net/aspose.email.clients.google/igmailclient/methods/getallcontacts
[14]: https://apireference.aspose.com/email/net/aspose.email.clients.google/gmailclient
[15]: https://apireference.aspose.com/email/net/aspose.email.clients.google/igmailclient
[16]: https://apireference.aspose.com/email/net/aspose.email.clients.google/contactgroupcollection
[17]: https://apireference.aspose.com/email/net/aspose.email.clients.google/igmailclient/methods/getallgroups
[18]: https://apireference.aspose.com/email/net/aspose.email.clients.google/googlecontactgroup
[19]: https://apireference.aspose.com/email/net/aspose.email.personalinfo/contact
[20]: https://apireference.aspose.com/email/net/aspose.email.clients.google/igmailclient/methods/getcontactsfromgroup
[21]: https://purchase.aspose.com/temporary-license
[22]: https://docs.aspose.com/email/net/
[23]: https://forum.aspose.com/
[24]: https://blog.aspose.com/2020/01/23/create-send-outlook-email-eml-msg-csharp-net-core/





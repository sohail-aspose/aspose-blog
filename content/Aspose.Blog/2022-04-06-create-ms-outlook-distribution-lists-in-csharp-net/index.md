---
title: 'Create and Read MS Outlook Distribution Lists in C#'
seoTitle: "Create MS Outlook Distribution Lists in C# | .NET MS Outlook Library"
description: "Use .NET Outlook library to create distribution lists in MS Outlook in C#. Create and save distribution lists in PST format programmatically in C#."
date: Wed, 06 Apr 2022 14:39:00 +0000
draft: false
url: /2022/04/06/create-ms-outlook-distribution-lists-in-csharp-net/
author: Usman Aziz
summary: "Email distribution lists make it easier to send a single email to a group of people without writing their individual email IDs. You can create as many lists as required based on the circles you have, such as official, social, etc. [MS Outlook][1] also allows you to make the distribution lists and often you may need to create such lists programmatically. So let's see **how to create and read MS Outlook distribution lists in C# .NET**."
tags: ['Create a Distribution List in MS Outlook in Csharp', 'Csharp Dotnet API to Create MS Outlook Distribution Lists', 'Read an MS Outlook Distribution List in Csharp']
categories: ['Aspose.Email Product Family']
---



{{< figure align=center src="images/Users.png" alt="Create Outlook Distribution Lists in C#">}}


Email distribution lists make it easier to send a single email to a group of people without writing their individual email IDs. You can create as many lists as required based on the circles you have, such as official, social, etc. [MS Outlook][2] also allows you to make the distribution lists and often you may need to create such lists programmatically. So let's see **how to create and read MS Outlook distribution lists in C# .NET**.

*   [.NET API to Create MS Outlook Distribution Lists][3]
*   [Create a Distribution List in MS Outlook][4]
*   [Read an MS Outlook Distribution List][5]

## C# .NET API to Create MS Outlook Distribution Lists {#API-to-Create-MS-Outlook-Distribution-Lists}

[Aspose.Email for .NET][6] is a feature-rich API to create, send, and process emails. Furthermore, it allows you to work with different email clients including MS Outlook. We will use this API to create and read the Outlook distribution lists. You can either [download][7] the API’s DLL or install it from [NuGet][8] using the following command.

```
PM> Install-Package Aspose.Email
```

## Create a Distribution List in MS Outlook in C# {#Create-a-Distribution-List-in-MS-Outlook}

MS Outlook uses [PST][9] format to store the information about the distribution lists. Let's see how to create an Outlook distribution list in C# using Aspose.Email for .NET.

*   First, create string objects to store details of the members.
*   Then, create a PST file using the [PersonalStorage.Create()][10] method to store the distribution list.
*   After that, make a new folder in PST using [PersonalStorage.CreatePredefinedFolder()][11] method and set its name.
*   Then, create a [MapiDistributionListMember][12] object for each member and initialize it.
*   Create a new [MapiDistributionListMemberCollection][13] object and add members to it.
*   Assign the collection to a [MapiDistributionList][14] object.
*   Finally, add a distribution list to the folder of PST using the [FolderInfo.AddMapiMessageItem()][15] method.

The following code sample shows how to create an MS Outlook distribution list in C#.

{{< gist aspose-com-gists 736ed7a3971410f00d272e3e04e606f1 "create-outlook-distribution-list.cs" >}}

## Read an MS Outlook Distribution List in C# {#Read-an-MS-Outlook-Distribution-List}

You can also read an Outlook distribution list and fetch the contacts' information. The following steps show how to perform this operation.

*   Load the distribution list from the PST file using [MapiMessage.Load()][16] method.
*   Fetch the list using [MapiMessage.ToMapiMessageItem()][17] method and cast it to [MapiDistributionList][18].
*   Read the contacts from the _MapiDistributionList_ object.

The following code sample shows how to read an MS Outlook distribution list in C#.

{{< gist aspose-com-gists 736ed7a3971410f00d272e3e04e606f1 "read-outlook-distribution-list.cs" >}}

## Get a Free API License

You can use Aspose.Email for .NET without evaluation limitations by getting a [free temporary license][19].

## Conclusion

A distribution list in MS Outlook lets you send an email to a group of people. In this article, you have learned how to create MS Outlook distribution lists in C#. Furthermore, you have seen how to read the Outlook distribution lists programmatically. Besides, you can explore more about .NET email API using the [documentation][20]. Also, you can post your questions or queries on our [forum][21].

## See Also

*   [Create, Update, and Delete Contacts in Gmail using C#][22]




[1]: https://en.wikipedia.org/wiki/Microsoft_Outlook
[2]: https://en.wikipedia.org/wiki/Microsoft_Outlook
[3]: #API-to-Create-MS-Outlook-Distribution-Lists
[4]: #Create-a-Distribution-List-in-MS-Outlook
[5]: #Read-an-MS-Outlook-Distribution-List
[6]: https://products.aspose.com/email/net/
[7]: https://downloads.aspose.com/email/net/
[8]: https://www.nuget.org/packages/Aspose.Email
[9]: https://docs.fileformat.com/email/pst/
[10]: https://apireference.aspose.com/email/net/aspose.email.storage.pst.personalstorage/create/methods/4
[11]: https://apireference.aspose.com/email/net/aspose.email.storage.pst/personalstorage/methods/createpredefinedfolder
[12]: https://apireference.aspose.com/email/net/aspose.email.mapi/mapidistributionlistmember
[13]: https://apireference.aspose.com/email/net/aspose.email.mapi/mapidistributionlistmembercollection
[14]: https://apireference.aspose.com/email/net/aspose.email.mapi/mapidistributionlist
[15]: https://apireference.aspose.com/email/net/aspose.email.storage.pst/folderinfo/methods/addmapimessageitem
[16]: https://apireference.aspose.com/email/net/aspose.email.mapi.mapimessage/load/methods/2
[17]: https://apireference.aspose.com/email/net/aspose.email.mapi/mapimessage/methods/tomapimessageitem
[18]: https://apireference.aspose.com/email/net/aspose.email.mapi/mapidistributionlist
[19]: https://products.aspose.com/email
[20]: https://docs.aspose.com/email/net/
[21]: https://forum.aspose.com/
[22]: https://blog.aspose.com/2022/04/21/manage-contacts-in-gmail-using-csharp/





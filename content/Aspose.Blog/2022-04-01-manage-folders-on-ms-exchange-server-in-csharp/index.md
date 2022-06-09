---
title: 'Create and Delete Folders on MS Exchange Server in C#'
seoTitle: "C# Create and Delete Folders with EWS on Exchange Server | .NET API"
description: "Use .NET EWS API to work with folders on MS Exchange Server in C#. Create and delete the folders using the EWS client on MS Exchange Server."
date: Fri, 01 Apr 2022 14:37:22 +0000
draft: false
url: /2022/04/01/manage-folders-on-ms-exchange-server-in-csharp/
author: Usman Aziz
summary: 'In [Microsoft Exchange Server][1], emails are organized in different folders such as inbox, outbox, etc. Also, you can create your own folders or subfolders based on your needs. While working with MS Exchange Server, you may need to create custom folders programmatically. In this article, you will learn **how to create folders or subfolders with EWS on MS Exchange Server in C# .NET**. Also, we will cover how to delete a folder on Exchange Server.'
tags: ['Create a Folder on MS Exchange Server Csharp', 'Create a Subfolder on MS Exchange Server Csharp', 'Delete a Folder on MS Exchange Server CSharp', 'DotNet EWS Exchange Server API']
categories: ['Aspose.Email Product Family']
---



{{< figure align=center src="images/aspose-email-exchange.png" alt="Create and Delete Folders on MS Exchange Server in C#">}}


In [Microsoft Exchange Server][2], emails are organized in different folders such as inbox, outbox, etc. Also, you can create your own folders or subfolders based on your needs. While working with MS Exchange Server, you may need to create custom folders programmatically. In this article, you will learn **how to create folders or subfolders with EWS on MS Exchange Server in C# .NET**. Also, we will cover how to delete a folder on Exchange Server.

*   [.NET API to Create Folders with EWS on MS Exchange Server][3]
*   [Create a Folder on MS Exchange Server][4]
*   [Create a Subfolder on MS Exchange Server][5]
*   [Delete a Folder on MS Exchange Server][6]

## C# .NET API to Create Folders on MS Exchange Server {#API-to-Create-Folders-in-MS-Exchange-Server}

To manage folders with EWS on MS Exchange Server, we will utilize [Aspose.Email for .NET][7]. The API makes it quite easier to work with the Exchange Server's services from within .NET applications. You can either [download][8] the API’s DLL or install it from [NuGet][9] using the following command.

```
PM> Install-Package Aspose.Email
```

## Create a Folder on MS Exchange Server in C# {#Create-a-Folder-on-MS-Exchange-Server}

The following are the steps to create a folder on MS Exchange Server in C#.

*   Connect to MS Exchange Server and get the EWS client object in [IEWSClient][10].
*   Specify the name of the root folder and the folder you want to create.
*   Create folder using [IEWSClient.CreateFolder(string, string)][11] method.

The following code sample shows how to create a folder on MS Exchange Server with EWS in C#.

{{< gist aspose-com-gists 2e3d275b59a45593fe99667e3c651e6c "create-folder.cs" >}}

## Create a Subfolder on MS Exchange Server in C# {#Create-a-Subfolder-on-MS-Exchange-Server}

To create a subfolder, you would first need to check if the parent folder exists or not. If it does, simply create the subfolder, else create the parent folder first. The following steps demonstrate how to create a subfolder on MS Exchange Server in C#.

*   Connect to MS Exchange Server and get the EWS client object in [IEWSClient][12].
*   Specify the name of the root folder and subfolder.
*   Check if the parent folder exists using [IEWSClient.FolderExists(string, string, ExchangeFolderInfo)][13] method. If not, create one.
*   Create subfolder using [IEWSClient.CreateFolder(string, string)][14] method.

The following code sample shows how to create a subfolder on MS Exchange Server in C#.

{{< gist aspose-com-gists 2e3d275b59a45593fe99667e3c651e6c "create-subfolder.cs" >}}

## Delete a Folder on MS Exchange Server in C# {#Delete-a-Folder-on-MS-Exchange-Server}

The following are the steps to delete a folder on MS Exchange Server in C#.

*   Connect to MS Exchange Server and get the EWS client object in [IEWSClient][15].
*   Check if the folder exists using [IEWSClient.FolderExists(string, string, ExchangeFolderInfo)][16] method.
*   Delete folder using [IEWSClient.DeleteFolder(string, bool)][17] method.

The following code sample shows how to delete a folder on MS Exchange Server in C#.

{{< gist aspose-com-gists 2e3d275b59a45593fe99667e3c651e6c "delete-folder.cs" >}}

## Get a Free API License {#Get-a-Free-API-License}

You can get a [free temporary license][18] to use Aspose.Email for .NET without evaluation limitations.

## Conclusion

In this article, you have learned how to work with folders on Microsoft Exchange Server with EWS in C#. With the help of code samples, you have seen how to create and delete a particular folder on MS Exchange Server programmatically in C#. Besides, you can explore the [documentation][19] to read more about Aspose.Email for .NET. Also, you can ask your questions via our [forum][20].

## See Also

*   [Read Emails from MS Exchange Server using C#][21]




[1]: https://en.wikipedia.org/wiki/Microsoft_Exchange_Server
[2]: https://en.wikipedia.org/wiki/Microsoft_Exchange_Server
[3]: #API-to-Create-Folders-in-MS-Exchange-Server
[4]: #Create-a-Folder-on-MS-Exchange-Server
[5]: #Create-a-Subfolder-on-MS-Exchange-Server
[6]: #Delete-a-Folder-on-MS-Exchange-Server
[7]: https://products.aspose.com/email/net/
[8]: https://downloads.aspose.com/email/net
[9]: https://www.nuget.org/packages/Aspose.Email/
[10]: https://apireference.aspose.com/email/net/aspose.email.clients.exchange.webservice/iewsclient
[11]: https://apireference.aspose.com/email/net/aspose.email.clients.exchange.webservice.iewsclient/createfolder/methods/2
[12]: https://apireference.aspose.com/email/net/aspose.email.clients.exchange.webservice/iewsclient
[13]: https://apireference.aspose.com/email/net/aspose.email.clients.exchange.webservice.iewsclient/folderexists/methods/1
[14]: https://apireference.aspose.com/email/net/aspose.email.clients.exchange.webservice.iewsclient/createfolder/methods/2
[15]: https://apireference.aspose.com/email/net/aspose.email.clients.exchange.webservice/iewsclient
[16]: https://apireference.aspose.com/email/net/aspose.email.clients.exchange.webservice.iewsclient/folderexists/methods/1
[17]: https://apireference.aspose.com/email/net/aspose.email.clients.exchange.webservice.iewsclient/deletefolder/methods/1
[18]: https://purchase.aspose.com/temporary-license
[19]: https://docs.aspose.com/email/net/
[20]: https://forum.aspose.com/
[21]: https://blog.aspose.com/2020/11/20/read-emails-from-exchange-server-using-csharp/





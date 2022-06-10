---
title: 'Listing Tasks from Exchange Server using C#'
date: Wed, 25 Jan 2017 10:19:04 +0000
draft: false
url: /2017/01/25/listing-tasks-exchange-server-supported-aspose.email-.net-17.1.0/
author: Kashif Iqbal
summary: ''
tags: []
categories: ['Aspose.Email Product Family']
---



{{< figure align=center src="images/Aspose.Email-for-.NET_-1.png" alt="">}}


We are pleased to announce the release of [Aspose.Email for .NET 17.1.0][1]. This month’s release brings several improvements to the API functional areas including Exchange Web Service (EWS) API, Linked Resources of a message, and MIME message processing. It also fixes several bugs that were reported with last month’s version of the API. For a complete list of what is new and fixed, please visit the [](http://www.aspose.com/products/email/net) release notes section of API documentation.

## Listing Tasks from Exchange Server using EWS

Aspose.Email API lets you list messages from exchange server mailbox using the ListMessages method. Similarly, appointments can be retrieved using the ListAppointments method of the IEWSClient API. This month’s release implements the functionality of listing tasks from Exchange Server mailbox using the ListTasks method. Not only tasks can be listed from the mailbox, these can be filtered as well by using the ExchangeQueryBuilder – a feature that was introduced in our last month’s [release][2]. Sample code for listing tasks from Exchange is as listed below.

```
// Set mailboxURI, Username, password, domain information
string mailboxUri = "https://ex2010/ews/exchange.asmx";
string username = "test.exchange";
string password = "pwd";
string domain = "ex2010.local";
NetworkCredential credentials = new NetworkCredential(username, password, domain);
IEWSClient client = EWSClient.GetEWSClient(mailboxUri, credentials);

//Listing Tasks from Server
client.TimezoneId = "Central Europe Standard Time";
TaskCollection taskCollection = client.ListTasks(client.MailboxInfo.TasksUri);

//print retrieved tasks' details
foreach (ExchangeTask task in taskCollection)
{
    Console.WriteLine(task.TimezoneId);
    Console.WriteLine(task.Subject);
    Console.WriteLine(task.StartDate);
    Console.WriteLine(task.DueDate);
} 
```

## Additional Properties for Exchange Contact

The IEWSClient already supports creating contacts on Exchange Server. The use of Contact class, however, had limitations as it was lacking certain properties. This month’s release enhances this functionality by providing additional properties including:

*   Title
*   FileUnder
*   Html
*   Gender
*   Location
*   OrganizationalIdNumber
*   ManagerName
*   OfficeLocation
*   Email1
*   Email2
*   Email3
*   OtherTelephoneNumber
*   Business2TelephoneNumber

Of these, the following are collections:

*   Urls
*   AssociatedPersons
*   PhoneNumbers
*   EmailAddresses

## Removing Linked Resources’ Traces from Message Body

This month’s release also provides the capability to remove Linked Resource’s traces from message’s body if it is removed from the message. The overloaded method of LinkedResourceCollection.RemoveAt method removes all traces of the resource from message body along with the resource.

## Preserving Embedded EML format during Conversion to MSG

The API converts embedded EML attachments to MSG during conversion to MSG format using MapiMessage.FromMailMessage. However, there could be occurrences where the requirement is to retain/preserve embedded EML format during this conversion. This month’s release provides the capability to preserve the embedded EML format using the MapiConversionOptions.PreserveEmbeddedMessageFormat.

## Have you switched to Aspose.Email for .NET Revamped API?

We shared the news of [Revamped Aspose.Email for .NET][3] API with you a month ago, and mentioned that the legacy version of API will be published for three consecutive months alongside the revamped API. After this, we’ll stop publishing the legacy API and any non-modified codes in your application will break after upgrading to the revamped version. Therefore, we strongly recommend you to update your applications as per the Revamped API with improved namespace structure.

## API Resources

The following API resources can be of help to you in getting started with Aspose.Email API.

*   [Product Documentation][4] – Provides detailed examples of working with the API
*   [API Reference Guide][5] – Details all the namespaces and classes of the API
*   [GitHub Examples][6] – Provides ready to run API example
*   [Support Forum][7] – Write to us if you have any query or inquiry about the API




[1]: https://products.aspose.com/email/net
[2]: https://blog.aspose.com/2016/12/26/filtering-tasks-status-supported-aspose.email-.net-16.12.0/
[3]: https://blog.aspose.com/2016/12/26/aspose.email-.net-improved-namespace-structure-available-now/
[4]: https://products.aspose.com/email/net
[5]: https://apireference.aspose.com/email/net
[6]: https://github.com/asposeemail/Aspose_Email_NET
[7]: https://forum.aspose.com/c/email





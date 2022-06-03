---
title: 'Create, Update or Delete Google Calendar in C#'
date: Sun, 10 Apr 2022 15:16:00 +0000
draft: false
url: /2022/04/10/create-update-or-delete-google-calendar-in-csharp-net/
author: 'Usman Aziz'
summary: '[Google Calendar][1] is a scheduling service that lets you create and keep track of the events such as meetings. You can log the events on the calendar and get reminders about the upcoming ones. Google also allows you to use its calendaring service programmatically. Thus, you can manage your events using Google Calendars from within your applications. In this article, you will learn **how to create, update, and delete Google Calendar programmatically in C#**.'
tags: ['Create a Google Calendar in CSharp', 'Delete a Google Calendar in CSharp', 'DotNet API to Create and Manipulate Google Calendar', 'Update a Google Calendar in CSharp']
categories: ['Aspose.Email Product Family']
---



{{< figure align=center src="images/Create-and-Update-Google-Calendar.png" alt="Create, Update or Delete Google Calendar in C#">}}


[Google Calendar][2] is a scheduling service that lets you create and keep track of the events such as meetings. You can log the events on the calendar and get reminders about the upcoming ones. Google also allows you to use its calendaring service programmatically. Thus, you can manage your events using Google Calendars from within your applications. In this article, you will learn **how to create, update, and delete Google Calendar programmatically in C#**.

*   [.NET API to Create and Manipulate Google Calendar][3]
*   [Create a Google Calendar in C#][4]
*   [Update a Google Calendar in C#][5]
*   [Delete a Google Calendar in C#][6]

## C# .NET API to Create and Manipulate Google Calendar {#Java-API-to-Create-and-Manipulate-Google-Calendar}

In order to work with the Google Calendar service, we will use [Aspose.Email for .NET][7]. It is a powerful API that provides a range of features for processing emails, working with email clients, and using Google's collaboration services. You can either [download][8] the API’s DLL or install it from [NuGet][9] using the following command.

```
PM> Install-Package Aspose.Email
```

Before you start working, you need to create a project on the Google Developer Console, which will allow your application to communicate with Google services. To create one, you can follow [this guide][10].

To access and manipulate Google Calendar, we need to write some code to handle the user’s information and perform authentication. For the Google user, we will first create a class named **TestUser** and then inherit it from **GoogleUser** class. The following is the complete implementation of both of the classes.

{{< gist aspose-com-gists 66a1b4d034b3b4f72f593359c8624ddf "GoogleUser.cs" >}}

Now, we need to create a helper class that will take care of the authentication of a Google account. We will name this class as **GoogleOAuthHelper**. The following is the complete implementation of this class.

{{< gist aspose-com-gists 66a1b4d034b3b4f72f593359c8624ddf "GoogleOAuthHelper.cs" >}}

## Create a Google Calendar in C# {#Create-a-Google-Calendar}

Once you have done the above configuration, you can proceed to work with the Google Calendar service. The following are the steps to create and update a Google Calendar in C#.

*   Get an instance of [GmailClient][11] class into an [IGmailClient][12]  object using [GmailClient.GetInstance(String, String)][13] method.
*   Create an instance of the [Calendar][14] class and initialize it with name, description, and other properties.
*   Call [IGmailClient.CreateCalendar(Calendar)][15] method to create the Google Calendar.
*   Get the returned ID of the calendar.

The following code sample shows how to create a Google Calendar in C#.

{{< gist aspose-com-gists 14d2e416098408b95b73aff572531e84 "create-google-calendar.cs" >}}

## Update a Google Calendar in C# {#Update-a-Google-Calendar}

The following are the steps to update a Google Calendar programmatically in C#.

*   Get an instance of [GmailClient][16] class into an [IGmailClient][17]  object using [GmailClient.GetInstance(String, String)][18] method.
*   Use [IGmailClient.FetchCalendar(String)][19] method to fetch the calendar instance using its ID.
*   Update the properties of the calendar and call [IGmailClient.UpdateCalendar(Calendar)][20] method to update the calendar.

The following code sample shows how to update a Google Calendar in C#.

{{< gist aspose-com-gists 14d2e416098408b95b73aff572531e84 "update-google-calendar.cs" >}}

## Delete a Google Calendar in C# {#Delete-a-Google-Calendar}

You can also delete a particular calendar using Aspose.Email for .NET. The following are the steps to perform this operation.

*   Get an instance of [GmailClient][21] class into an [IGmailClient][22]  object using [GmailClient.GetInstance(String, String)][23] method.
*   Get list of calendars using [IGmailClient.ListCalendars()][24] method.
*   Loop through the list and filter the desired one.
*   Delete calendar using [IGmailClient.DeleteCalendar(Calendar.Id)][25] method.

The following code sample shows how to delete a Google Calendar in C#.

{{< gist aspose-com-gists 14d2e416098408b95b73aff572531e84 "delete-google-calendar.cs" >}}

## Get a Free API License {#Get-a-Free-API-License}

You can get a [free temporary license][26] to use Aspose.Email for .NET without evaluation limitations.

## Conclusion

In this article, you have learned how to create Google Calendar programmatically in C#. Moreover, you have seen how to update and delete a particular Google Calendar in C#. Besides, you can explore the [documentation][27] to read more about Aspose.Email for .NET. Also, you can ask your questions via our [forum][28].

## See Also

*   [Read Emails from MS Exchange Server using C#][29]




[1]: https://en.wikipedia.org/wiki/Google_Calendar
[2]: https://en.wikipedia.org/wiki/Google_Calendar
[3]: #Java-API-to-Create-and-Manipulate-Google-Calendar
[4]: #Create-a-Google-Calendar
[5]: #Update-a-Google-Calendar
[6]: #Delete-a-Google-Calendar
[7]: https://products.aspose.com/email/net/
[8]: https://downloads.aspose.com/email/net/
[9]: https://www.nuget.org/packages/Aspose.Email
[10]: https://docs.aspose.com/email/net/gmail-utility-features/#creating-project-in-google-developer-console
[11]: https://apireference.aspose.com/email/net/aspose.email.clients.google/gmailclient
[12]: https://apireference.aspose.com/email/net/aspose.email.clients.google/igmailclient
[13]: https://apireference.aspose.com/email/net/aspose.email.clients.google.gmailclient/getinstance/methods/1
[14]: https://apireference.aspose.com/email/net/aspose.email.clients.google/calendar
[15]: https://apireference.aspose.com/email/net/aspose.email.clients.google/igmailclient/methods/createcalendar
[16]: https://apireference.aspose.com/email/net/aspose.email.clients.google/gmailclient
[17]: https://apireference.aspose.com/email/net/aspose.email.clients.google/igmailclient
[18]: https://apireference.aspose.com/email/net/aspose.email.clients.google.gmailclient/getinstance/methods/1
[19]: https://apireference.aspose.com/email/net/aspose.email.clients.google/igmailclient/methods/fetchcalendar
[20]: https://apireference.aspose.com/email/net/aspose.email.clients.google/igmailclient/methods/updatecalendar
[21]: https://apireference.aspose.com/email/net/aspose.email.clients.google/gmailclient
[22]: https://apireference.aspose.com/email/net/aspose.email.clients.google/igmailclient
[23]: https://apireference.aspose.com/email/net/aspose.email.clients.google.gmailclient/getinstance/methods/1
[24]: https://apireference.aspose.com/email/net/aspose.email.clients.google/igmailclient/methods/listcalendars
[25]: https://apireference.aspose.com/email/net/aspose.email.clients.google/igmailclient/methods/deletecalendar
[26]: https://purchase.aspose.com/temporary-license
[27]: https://docs.aspose.com/email/net/
[28]: https://forum.aspose.com/
[29]: https://blog.aspose.com/2020/11/20/read-emails-from-exchange-server-using-csharp/





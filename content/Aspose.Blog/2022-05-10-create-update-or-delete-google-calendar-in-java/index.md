---
title: 'Create, Update or Delete Google Calendar in Java'
seoTitle: "Create or Update Google Calendar in Java | Delete Calendar | Java API"
description: "Use Java email API to create and update Google Calendar programmatically in Java. Delete a particular Google Calendar from within your Java application."
date: Tue, 10 May 2022 07:03:40 +0000
draft: false
url: /2022/05/10/create-update-or-delete-google-calendar-in-java/
author: Usman Aziz
summary: '[Google Calendar][1] is a scheduling service that lets you create and keep track of the events such as meetings. You can log the events on the calendar and get reminders about the upcoming ones. Google also allows you to use its calendaring service programmatically. Thus, you can manage your events using Google Calendars from within your applications. In this article, you will learn **how to create, update, and delete Google Calendar programmatically in Java**.'
tags: ['Create a Google Calendar in Java', 'Delete a Google Calendar in Java', 'Java API to Create and Manipulate Google Calendar', 'Update a Google Calendar in Java']
categories: ['Aspose.Email Product Family']
---



{{< figure align=center src="images/Create-and-Update-Google-Calendar.png" alt="Create, Update or Delete Google Calendar in Java">}}


[Google Calendar][2] is a scheduling service that lets you create and keep track of the events such as meetings. You can log the events on the calendar and get reminders about the upcoming ones. Google also allows you to use its calendaring service programmatically. Thus, you can manage your events using Google Calendars from within your applications. In this article, you will learn **how to create, update, and delete Google Calendar programmatically in Java**.

*   [Java API to Create and Manipulate Google Calendar][3]
*   [Create a Google Calendar in Java][4]
*   [Update a Google Calendar in Java][5]
*   [Delete a Google Calendar in Java][6]

## Java API to Create and Manipulate Google Calendar {#Java-API-to-Create-and-Manipulate-Google-Calendar}

In order to work with the Google Calendar service, we will use [Aspose.Email for Java][7]. It is a powerful API that provides a range of features for processing emails, working with email clients, and using Google's collaboration services. You can either [download][8] the API or install it using the following Maven configurations.

```
**Repository:**
<repository>
    <id>AsposeJavaAPI</id>
    <name>Aspose Java API</name>
    <url>http://repository.aspose.com/repo/</url>
</repository>

**Dependency:**
<dependency>
    <groupId>com.aspose</groupId>
    <artifactId>aspose-email</artifactId>
    <version>22.3</version>
    <classifier>jdk16</classifier>
</dependency>
```

## Create a Google Calendar in Java {#Create-a-Google-Calendar-in-Java}

Before you start, you need to create a project on the Google Developer Console for your application to communicate with Google's services. To create one, you can follow [this guide][9].

Now, create a helper class named **GoogleOAuthHelper** to take care of the authentication of a Google account. Also, create a class named **OAuthUser **to store user information. The following is the complete implementation of both classes.

{{< gist aspose-com-gists 4f01b0affc2beaa1c63b58c4716d67a2 "OAuthUser.java" >}}

{{< gist aspose-com-gists 4f01b0affc2beaa1c63b58c4716d67a2 "GoogleOAuthHelper.java" >}}

Once you have done the above configuration, you can proceed to work with Google Calendar service. The following are the steps to create and update a Google Calendar in Java.

*   Get an instance of [GmailClient][10] class into an [IGmailClient][11]  object using [GmailClient.getInstance(String, String)][12] method.
*   Create an instance of [Calendar][13] class and initialize it with name, description and other properties.
*   Call [IGmailClient.createCalendar(Calendar)][14] method to create the Google Calendar.
*   Get the returned ID of the calendar.

The following code sample shows how to create a Google Calendar in Java.

{{< gist aspose-com-gists b0078a63655cbe08b7295b671a06d014 "create-google-calendar.java" >}}

## Update a Google Calendar in Java {#Update-a-Google-Calendar-in-Java}

The following are the steps to update a Google Calendar programmatically in Java.

*   Get an instance of [GmailClient][15] class into an [IGmailClient][16]  object using [GmailClient.getInstance(String, String)][17] method.
*   Use [IGmailClient.fetchCalendar(String)][18] method to fetch the calendar instance using its ID.
*   Update the properties of calendar and call [IGmailClient.updateCalendar(Calendar)][19] method to update the calendar.

The following code sample shows how to update a Google calendar in Java.

{{< gist aspose-com-gists b0078a63655cbe08b7295b671a06d014 "update-google-calendar.java" >}}

## Delete a Google Calendar in Java {#Delete-a-Google-Calendar-in-Java}

You can also delete a particular calendar using Aspose.Email for Java. The following are the steps to perform this operation.

*   Get an instance of [GmailClient][20] class into an [IGmailClient][21]  object using [GmailClient.getInstance(String, String)][22] method.
*   Get list of calendars using [IGmailClient.listCalendars()][23] method.
*   Loop through the list and filter the desired one.
*   Delete calendar using [IGmailClient.deleteCalendar(Calendar.getId())][24] method.

The following code sample shows how to delete a Google Calendar in Java.

{{< gist aspose-com-gists b0078a63655cbe08b7295b671a06d014 "delete-google-calendar.java" >}}

## Get a Free API License {#Get-a-Free-API-License}

You can get a [free temporary license][25] to use Aspose.Email for Java without evaluation limitations.

## Conclusion

In this article, you have learned how to create Google Calendar programmatically in Java. Moreover, you have seen how to update and delete a particular Google Calendar in Java. Besides, you can explore the [documentation][26] to read more about Aspose.Email for Java. Also, you can ask your questions via our [forum][27].

## See Also

*   [Read Emails from MS Exchange Server using Java][28]
*   [Create and Send Outlook Email Messages using Java][29]




[1]: https://en.wikipedia.org/wiki/Google_Calendar
[2]: https://en.wikipedia.org/wiki/Google_Calendar
[3]: #Java-API-to-Create-and-Manipulate-Google-Calendar
[4]: #Create-a-Google-Calendar-in-Java
[5]: #Update-a-Google-Calendar-in-Java
[6]: #Delete-a-Google-Calendar-in-Java
[7]: https://products.aspose.com/email/java/
[8]: https://downloads.aspose.com/email/java/
[9]: https://docs.aspose.com/email/net/gmail-utility-features/#creating-project-in-google-developer-console
[10]: https://apireference.aspose.com/email/java/com.aspose.email/GmailClient
[11]: https://apireference.aspose.com/email/java/com.aspose.email/IGmailClient
[12]: https://apireference.aspose.com/email/java/com.aspose.email/GmailClient#getInstance(java.lang.String,%20java.lang.String)
[13]: https://apireference.aspose.com/email/java/com.aspose.email/Calendar
[14]: https://apireference.aspose.com/email/java/com.aspose.email/IGmailClient#createCalendar(com.aspose.email.Calendar)
[15]: https://apireference.aspose.com/email/java/com.aspose.email/GmailClient
[16]: https://apireference.aspose.com/email/java/com.aspose.email/IGmailClient
[17]: https://apireference.aspose.com/email/java/com.aspose.email/GmailClient#getInstance(java.lang.String,%20java.lang.String)
[18]: https://apireference.aspose.com/email/java/com.aspose.email/IGmailClient#fetchCalendar(java.lang.String)
[19]: https://apireference.aspose.com/email/java/com.aspose.email/IGmailClient#updateCalendar(com.aspose.email.Calendar)
[20]: https://apireference.aspose.com/email/java/com.aspose.email/GmailClient
[21]: https://apireference.aspose.com/email/java/com.aspose.email/IGmailClient
[22]: https://apireference.aspose.com/email/java/com.aspose.email/GmailClient#getInstance(java.lang.String,%20java.lang.String)
[23]: https://apireference.aspose.com/email/java/com.aspose.email/IGmailClient#listCalendars()
[24]: https://apireference.aspose.com/email/java/com.aspose.email/IGmailClient#deleteCalendar(java.lang.String)
[25]: https://purchase.aspose.com/temporary-license
[26]: https://docs.aspose.com/email/java/
[27]: https://forum.aspose.com/
[28]: https://blog.aspose.com/2021/03/22/read-emails-from-ms-exchange-server-using-java/
[29]: https://blog.aspose.com/2020/05/20/create-and-send-outlook-email-messages-asynchronously-using-java/





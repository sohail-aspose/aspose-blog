---
title: 'List Tasks from Exchange Server using  Java'
date: Mon, 30 Jan 2017 15:08:10 +0000
draft: false
url: /2017/01/30/support-listing-tasks-exchange-server-using-aspose.email-java-17.1.0/
author: Kashif Iqbal
summary: ''
tags: []
categories: ['Aspose.Email Product Family']
---



{{< figure align=center src="images/aspose-Email-for-Java_100.png" alt="List Tasks from Exchange Server">}}


[Aspose.Email for Java 17.1.0][1] has been released. Ported from its equivalent .NET version, this month’s release includes several enhancements and bug fixes that further improve API functionality and performance. Specifically, it improves the functionality of working with Tasks on Microsoft Exchange server using the API’s Exchange Web Service (EWS) client. It also enhances Contact’s class for working with contacts on Exchange server. For a complete list of what is new and fixed, please visit the release notes section of Aspose.Email for Java documentation.

## **Listing Messages from Exchange Server**

This month’s release provides a feature enhancement for listing Exchange Tasks from sever using the Exchange Web Service (EWS) client of the API. The listTasks method exposed by IEWSClient provides this capability of listing tasks from Exchange’s Tasks folder. In addition, it also supports filtering tasks from Exchange server using the ExchangeQueryBuilder class. The following sample code gives an illustration of this new feature introduced by the API.

```
String mailboxUri = "https://ex2010/ews/exchange.asmx";
String username = "test.exchange";
String password = "pwd";
String domain = "ex2010.local";
NetworkCredential credentials = new NetworkCredential(username, password, domain);
IEWSClient client = EWSClient.getEWSClient(mailboxUri, credentials);

//Listing Tasks from Server
client.setTimezoneId("Central Europe Standard Time");
TaskCollection taskCollection = client.listTasks(client.getMailboxInfo().getTasksUri());

//print retrieved tasks' details
int iTasksCount = taskCollection.size();
for (int i = 0; i < iTasksCount; i++) {
    ExchangeTask task = (ExchangeTask) taskCollection.get\_Item(i);
    System.out.println(task.getTimezoneId());
    System.out.println(task.getSubject());
    System.out.println(task.getStartDate());
    System.out.println(task.getDueDate());
}

//Listing Tasks from server based on Query - Completed and In-Progress
Integer\[\] selectedStatuses = new Integer\[\]
        {
                ExchangeTaskStatus.Completed,
                ExchangeTaskStatus.InProgress
        };
ExchangeQueryBuilder queryBuilder = new ExchangeQueryBuilder();
queryBuilder.getTaskStatus().in(Arrays.asList(selectedStatuses));
MailQuery query = queryBuilder.getQuery();

taskCollection = client.listTasks(client.getMailboxInfo().getTasksUri(), query);

//print retrieved tasks' details
iTasksCount = taskCollection.size();
for (int i = 0; i < iTasksCount; i++) {
    ExchangeTask task = (ExchangeTask) taskCollection.get\_Item(i);
    System.out.println(task.getTimezoneId());
    System.out.println(task.getSubject());
    System.out.println(task.getStartDate());
    System.out.println(task.getDueDate());
}

```

## **Support for Additional Contact Properties**

We have also enhanced the functionality of working with Contacts on Exchange server. This month’s release provides additional properties for Contact class for retrieving the information in totality from Exchange server. These additional properties include:

*   Title
*   FileUnder
*   Gender
*   Html
*   Location
*   OrganizationalIdNumber
*   ManagerName
*   OfficeLocation
*   Email1, Email2, Email3
*   OtherTelephoneNumber
*   Business2TelephoneNumber

## **Clearing Traces of Embedded Objects from Message Body**

Embedded objects, represented by LinkedResourcesCollection, can be removed from email message using Aspose.Email API. This, however, leaves traces of these embedded objects in message body. This month’s release provides the capability to remove traces of such embedded objects from message body. The overloaded version of LinkedResourceCollection.RemoveAt can be used to remove all traces of an embedded object from email message.

## **Preserving Embedded EML format during Conversion to MSG**

Aspose.Email API till yet converted embedded EML messages to MSG format while converting EML to MSG. This month’s release enhances the functionality of EML to MSG conversion by providing the capability to preserve embedded EML message format.

## **Rendering Recurrence and Organizer Information to MTHML**

This month’s release also enhances the functionality of EML to MHTML conversion by providing the capability of rendering recurrence and organizer information to output MHTML. This can now be achieved using the MhtMessageFormatter of the API.

## Other Improvements

This month’s release also fixes several bugs that were either resolved in .NET equivalent API or were directly reported in the Java API. This further adds stability to the overall functionality of the API.

## API Resources

We have detailed information available online for getting started with the Aspose.Email for Java API. These are:

*   Product Documentation – Provides detailed examples of working with the API
*   [API Reference Guide][2] – Details all the packages and classes of the API
*   [GitHub Examples][3] – Provides ready to run API examples
*   [Aspose.Email Forum][4] – Feel free to contact us on Aspose.Email forum for your queries




[1]: http://www.aspose.com/downloads/email/java
[2]: http://www.aspose.com/api/java/email
[3]: https://github.com/aspose-email/Aspose.Email-for-Java
[4]: https://forum.aspose.com/c/email





---
title: 'Filter Email Messages by Message Size using Java Email API'
date: Sat, 20 May 2017 09:19:25 +0000
draft: false
url: /2017/05/20/filtering-messages-message-size-using-aspose.email-java-17.5.0/
author: Kashif Iqbal
summary: ''
tags: []
categories: ['Aspose.Email Product Family']
---

[Aspose.Email for Java 17.5.0][1] has been released. Ported from its equivalent .NET version, this month’s release includes the same set of new features, enhancements and bug fixes. Specifically, it allows to modify or delete occurrences from a recurrence pattern, filter messages from Exchange server based on message size, identify folder and message types retrieved from Exchange server, and others. For a complete list of what is new and fixed, please visit the [release notes][2] section of Aspose.Email for Java documentation.

## Modify or Delete Occurrences from Recurrence Pattern

This month’s release provides a new feature of [modifying or deleting a specific occurrence][3] from an event’s recurrence pattern. This is achieved using the MapiCalendarExceptionInfo class as illustrated in code sample below.

```
Date startDate = addHours(new Date(), 12);

MapiCalendarEventRecurrence recurrence = new MapiCalendarEventRecurrence();
recurrence.setRecurrencePattern(new MapiCalendarDailyRecurrencePattern());
		
MapiCalendarRecurrencePattern pattern = recurrence.getRecurrencePattern();
pattern.setPatternType(MapiCalendarRecurrencePatternType.Day);
pattern.setPeriod(1);
pattern.setEndType(MapiCalendarRecurrenceEndType.NeverEnd);

Date exceptionDate = addDays(startDate, 1);

// adding one exception
MapiCalendarExceptionInfo exceptionInfo = new MapiCalendarExceptionInfo();
exceptionInfo.setLocation("London");
exceptionInfo.setSubject("Subj");
exceptionInfo.setOriginalStartDate(exceptionDate);
exceptionInfo.setStartDateTime(exceptionDate);
exceptionInfo.setEndDateTime(addHours(exceptionDate, 5));
pattern.getExceptions().addItem(exceptionInfo);
pattern.getModifiedInstanceDates().addItem(exceptionDate);
		
// every modified instance also has to have an entry in the DeletedInstanceDates field with the original instance date.
pattern.getDeletedInstanceDates().addItem(exceptionDate);

// adding one deleted instance
pattern.getDeletedInstanceDates().addItem(addHours(exceptionDate, 2));

MapiRecipientCollection recColl = new MapiRecipientCollection();
recColl.add("recepient@gmail.com", "R1", MapiRecipientType.MAPI_TO);
		
MapiCalendar newCal = new MapiCalendar(
    "This is Location",
    "This is Summary",
    "This is recurrence test",
    startDate,
    addHours(startDate, 3),
    "organizer@domain.com",
    recColl);
newCal.setRecurrence(recurrence);

ByteArrayOutputStream memory = new ByteArrayOutputStream();
try {
    PersonalStorage pst = PersonalStorage.create(memory, FileFormatVersion.Unicode);
    
    FolderInfo calendarFolder = pst.createPredefinedFolder("Calendar", StandardIpmFolder.Appointments);
    
    calendarFolder.addMapiMessageItem(newCal);
}
finally {
    memory.close();
} 
```

## Getting Message Class Information using EWS

Retrieving items from Exchange server folder, such as Deleted Items, can include items of different types. User’s logic is prone to error if items are fetched with the wrong API method. This month’s release provides the capability to [get the item type][4] from ExchangeMessageInfo, the summary information about an item, and use the appropriate method to fetch the message from the server as shown in the code sample below.

```
IEWSClient client = EWSClient.getEWSClient("https://outlook.office365.com/exchange/ews.asmx", "username", "password");
		
ExchangeMessageInfoCollection list = client.listMessages(client.getMailboxInfo().getDeletedItemsUri());
		
System.out.println(list.get_Item(0).getMessageInfoType());
```

## Identifying Folder Type using EWS

This month’s release also provides the capability to get [folder type information][5] from FolderInfo, the summary information about a folder. This is achieved using the getFolderType method of FolderInfo, which returns the following possible options:

*   Appointment
*   Contact
*   Note
*   Task
*   StickyNote
*   Journal

## Filtering Messages from Exchange Server using Message Size

We have also enhanced the functionality of filtering messages from Exchange Server by providing additional option of [filtering messages by message size][6]. You can now specify a message size to retrieve only those messages that meet the message size criterion.

## Sending Messages without using MailMessage

EML files, that have well defined structure, can now be sent out using the [API’s SMTP client][7] without first loading in MailMessage. This helps in situations where there are limited memory resources in a system and addition loading of large messages by MailMessage can lead to out of memory issues.

## Other Improvements

This month’s release also fixes several bugs that were either reported with the Java version of the API or with the equivalent .NET API. This further adds to the performance and stability of the API.

## API Resources

We have detailed information available online for getting started with the Aspose.Email for Java API. These are:

*   [Product Documentation][8] – Provides detailed examples of working with the API
*   [API Reference Guide][9] – Details all the packages and classes of the API
*   [GitHub Examples][10] – Provides ready to run API examples
*   [Aspose.Email Forum][11] – Feel free to contact us on Aspose.Email forum for your queries




[1]: https://downloads.aspose.com/email/java
[2]: https://docs.aspose.com/display/emailjava/Aspose.Email+for+Java+17.5.0+Release+Notes
[3]: https://docs.aspose.com/email/java/working-with-calendar-items-in-pst-file/#WorkingwithCalendarItemsinPSTFile-Modify/DeleteOccurrencesfromRecurrences
[4]: https://docs.aspose.com/email/java/working-with-exchange-mailbox-and-messages/#WorkingwithExchangeMailboxandMessages-GettingMessageClassInformationfromExchangeMessageInfo
[5]: https://docs.aspose.com/email/java/working-with-folders-on-exchange-server/#WorkingwithFoldersonExchangeServer-GettingFolderTypeInformationusingEWS
[6]: https://docs.aspose.com/email/java/filter-messages-from-exchange-mailbox/#FilterMessagesfromExchangeMailbox-CodeSamples:ByMessageSize
[7]: https://docs.aspose.com/email/java/sending-and-forwarding-messages/#SendingandForwardingMessages-ForwardingEmailWithoutLoadingusingMailMessage
[8]: https://docs.aspose.com/email/java/
[9]: http://www.aspose.com/api/java/email
[10]: https://github.com/aspose-email/Aspose.Email-for-Java
[11]: https://forum.aspose.com/c/email





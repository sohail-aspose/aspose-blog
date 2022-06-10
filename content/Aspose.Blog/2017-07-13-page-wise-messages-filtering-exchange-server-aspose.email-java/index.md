---
title: 'Page Wise Messages Filtering from Exchange Server using Java'
date: Thu, 13 Jul 2017 13:04:33 +0000
draft: false
url: /2017/07/13/page-wise-messages-filtering-exchange-server-aspose.email-java/
author: Kashif Iqbal
summary: ''
tags: []
categories: ['Aspose.Email Product Family']
---



{{< figure align=center src="images/aspose-Email-for-Java_100.png" alt="">}}


[](https://downloads.aspose.com/email/java)[Aspose.Email for Java 17.7][1] has been released. Ported from its equivalent .NET version, this month’s release includes the same enhancements and bug fixes that improve the API functionality. These enhancements to various functional areas of API enrich the API features and add to the value of the API. For a complete list of what is new and fixed, please visit the [release notes][2] page of Aspose.Email for Java 17.7.

## Read Multiple Events from ICS Files

Aspose.Email for Java API now supports reading multiple events from iCalendar (ICS) files. The CalendarReader class introduced in this month’s release allows reading all events from such an ICS file. It also provides the capability to read events from a specific index in the ICS file as shown in the code sample below.

```
String dataDir = Utils.getSharedDataDir(DisplayEmailInformation.class) + "email/";
List appointments = new ArrayList();
CalendarReader reader = new CalendarReader(dataDir + "US-Holidays.ics");
while (reader.nextEvent())
{
    appointments.add(reader.getCurrent());
}
		
System.out.println("Number of events read: " + appointments.size());
//Process appointments loaded from events

//Reading events from a specific index
appointments = new ArrayList();
AppointmentLoadOptions options = new AppointmentLoadOptions();
options.setEventIndex(4);
reader = new CalendarReader(dataDir + "US-Holidays.ics", options);
//start reading from 4th appointment...
while (reader.nextEvent())
{
    appointments.add(reader.getCurrent());
} 
```

## Filter Messages from Exchange with Paging Support

The API already supports criterion-based messages filtering from the Exchange server mailbox. However, this can result in a large number of messages if lots of emails meet this criterion. To cater to this, we have enhanced the functionality to filter messages from the Exchange server with [Paging support][3].

## Preserve Embedded Messages Format in EML

[Embedded messages][4] format in EML files can now be preserved during loading with EMLLoadOptions class. This can help identify the original format of attachment in an email.

## Read Message Size from MBox File

We have also enhanced the functionality of working with MBox files by providing the facility of reading message size during message extraction.

## API Resources

We have detailed information available online for getting started with the Aspose.Email for Java API. These are:

*   [Product Documentation][5]– Provides detailed examples of working with the API
*   [API Reference Guide][6]– Details all the packages and classes of the API
*   [GitHub Examples][7]– Provides ready to run API examples
*   [Aspose.Email Forum][8]– Feel free to contact us on Aspose.Email forum for your queries




[1]: https://products.aspose.com/email/java
[2]: https://docs.aspose.com/email/java/aspose-email-for-java-17-7-release-notes/
[3]: https://docs.aspose.com/email/java/filter-messages-from-exchange-mailbox/#FilterMessagesfromExchangeMailbox-FilteringMessageswithPagingSupport
[4]: https://docs.aspose.com/email/java/loading-and-saving-message/#preserving-embedded-message-format-during-loading
[5]: https://docs.aspose.com/email/java/
[6]: https://apireference.aspose.com/email/java
[7]: https://github.com/aspose-email/Aspose.Email-for-Java
[8]: https://forum.aspose.com/c/email





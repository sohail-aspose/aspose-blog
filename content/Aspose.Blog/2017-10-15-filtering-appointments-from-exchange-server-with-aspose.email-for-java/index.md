---
title: 'Filter Appointments from Exchange Server using Java'
date: Sun, 15 Oct 2017 14:03:30 +0000
draft: false
url: /2017/10/15/filtering-appointments-from-exchange-server-with-aspose.email-for-java/
author: Kashif Iqbal
summary: ''
tags: []
categories: ['Aspose.Email Product Family']
---



{{< figure align=center src="images/aspose-Email-for-Java_100.png" alt="aspose-email-for-java">}}


[Aspose.Email for Java 17.10][1] has been released. Ported from its equivalent .NET version, this month’s release includes enhancement of filtering appointments from Exchange Server using EWS client of the API. It also includes several bug fixes which further improve the overall API functionality. For a detailed note on what is new and fixed, please visit the [release notes][2] section of Aspose.Email for Java 17.10.

## Filter Appointments from Exchange Server using EWS

This release of Aspose.Email for Java introduces the capability of [filtering appointments from Exchange Sever][3] using its IEWSClient. Appointments can be filtered from Exchange server using the IEWSClient of the API with the help of ExchangeQueryBuilder. Appointments can be filtered from server by:

*   Date
*   Recurrence

The following code snippets show filtering appointments from Exchange server using this new feature.

## Filter Appointments by Date```
IEWSClient client = EWSClient.getEWSClient(mailboxUri, username, password, domain);

SimpleDateFormat sdf = new SimpleDateFormat("dd/MM/yyyy HH:mm:ss");
		
ExchangeQueryBuilder builder = new ExchangeQueryBuilder();
builder.getAppointment().getStart().since(sdf.parse("10/05/2016 10:00:00"));
builder.getAppointment().getEnd().beforeOrEqual(sdf.parse("10/15/2016 10:00:00"));
MailQuery query = builder.getQuery();
Appointment[] appointments = client.listAppointments(query); 
```

## Filter Appointments by Recurrence```
builder = new ExchangeQueryBuilder();
builder.getAppointment().isRecurring().equals(false);
MailQuery query = builder.getQuery();
Appointment[]appointments = client.listAppointments(query);
```

## Other Improvements

This month’s release also includes several bug fixes that further add to the overall stability of the API. In addition, since the API is ported from its equivalent .NET version, it also includes all those fixes which were part of the .NET version. Detailed information about the fixes can be found in the release notes section of the API documentation.

## API Resources

We have detailed information available online for getting started with the Aspose.Email for Java API. These are:

*   [Product Documentation][4] – Provides detailed examples of working with the API
*   [API Reference Guide][5] – Details all the packages and classes of the API
*   [GitHub Examples][6] – Provides ready to run API examples
*   [Aspose.Email Forum][7] – Feel free to contact us on Aspose.Email forum for your queries




[1]: https://downloads.aspose.com/email/java
[2]: https://downloads.aspose.com/email/java/new-releases/aspose.email-for-java-17.10/
[3]: https://docs.aspose.com/display/emailjava/Filter+Appointments+from+Exchange+Server
[4]: https://docs.aspose.com/display/emailjava/Home
[5]: http://www.aspose.com/api/java/email
[6]: https://github.com/aspose-email/Aspose.Email-for-Java
[7]: https://forum.aspose.com/c/email





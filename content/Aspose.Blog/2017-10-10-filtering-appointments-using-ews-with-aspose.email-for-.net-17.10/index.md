---
title: 'Filter Appointments using EWS in C# with Aspose.Email for .NET 17.10'
date: Tue, 10 Oct 2017 13:24:56 +0000
draft: false
url: /2017/10/10/filtering-appointments-using-ews-with-aspose.email-for-.net-17.10/
author: Kashif Iqbal
summary: ''
tags: []
categories: ['Aspose.Email Product Family']
---



{{< figure align=center src="images/Aspose.Email-for-.NET_-1.png" alt="aspose-email-for-.NET">}}


We are pleased to announce the release of [Aspose.Email for .NET 17.10][1]. This release includes enhancement for filtering appointments from Exchange server using Exchange Web Service (EWS) client of the API. It also includes improvements in terms of bug fixes which further add to the overall functionality of the API. For a detailed note on what is new and fixed, please visit the [release notes][2] section of API documentation.

## Filter Appointments using EWS Client using C#

The EWS client of the API already provides the capability of filtering messages from the Exchange server. This month’s release further enhances the functionality of searching items on the Exchange server. You can now [filter appointments][3] from Exchange server mailbox based on:

*   Date and Time
*   Recurrence

The ExchangeQueryBuilder class is the user interface in this case. The following code samples show filtering appointments from the Exchange server using the IEWSClient of the API.

### Filtering Appointments by Date Time```
IEWSClient client = EWSClient.GetEWSClient(mailboxUri, username, password, domain);
DateTime startTime = new DateTime(2017,09, 15);
DateTime endTime = new DateTime(2017, 10, 10);
ExchangeQueryBuilder builder = new ExchangeQueryBuilder();
builder.Appointment.Start.Since(startTime);
builder.Appointment.End.BeforeOrEqual(endTime);
MailQuery query = builder.GetQuery();
Appointment[] appointments = client.ListAppointments(query);
```

### Filtering Appointments by Recurrence```
builder = new ExchangeQueryBuilder();
builder.Appointment.IsRecurring.Equals(false);
query = builder.GetQuery();
appointments = client.ListAppointments(query); 
```

## Other Improvements

In addition to enhancement mentioned above, this month’s release also includes several bug fixes that add to the overall stability of the API in terms of expected output. Details about the fixed issues can be found in the release notes section of the API.

## API Resources

The following API resources can be of help to you in getting started with Aspose.Email API.

*   [Product Documentation][4] – Provides detailed examples of working with the API
*   [API Reference Guide][5] – Details all the namespaces and classes of the API
*   [GitHub Examples][6] – Provides ready to run API example
*   [Support Forum][7] – Write to us if you have any query or inquiry about the API




[1]: https://downloads.aspose.com/email/net
[2]: https://docs.aspose.com/display/emailnet/Aspose.Email+for+.NET+17.10+Release+Notes
[3]: https://docs.aspose.com/display/emailnet/Filter+Appointments+from+Exchange+Server#FilterAppointmentsfromExchangeServer-FilteringAppointmentswithEWS
[4]: https://docs.aspose.com/display/emailnet/Home
[5]: https://www.aspose.com/api/net/email
[6]: https://github.com/asposeemail/Aspose_Email_NET
[7]: https://forum.aspose.com/c/email





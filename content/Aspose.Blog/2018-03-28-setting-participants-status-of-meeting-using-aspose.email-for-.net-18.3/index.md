---
title: 'Setting Participants Status of Meeting using C#'
date: Wed, 28 Mar 2018 16:28:08 +0000
draft: false
url: /2018/03/28/setting-participants-status-of-meeting-using-aspose.email-for-.net-18.3/
author: Kashif Iqbal
summary: ''
tags: []
categories: ['Aspose.Email Product Family']
---



{{< figure align=center src="images/Aspose.Email-for-.NET_.png" alt="">}}


We are pleased to announce the release of [Aspose.Email for .NET 18.3][1]. This release introduces the capability of setting the participant status of a meeting which was not supported earlier. It also brings several improvements to the API in terms of bug fixes. For a complete list of what is new and fixed, please visit the [release notes][2] information of API documentation.

## Setting Participant Status for Meeting

This release of Aspose.Email API lets you set the [participation status of attendees][3] of a meeting. This lets you add the same information to the output ICS file in the form of PARTSTAT property. Status can be set to accepted as well as declined as per user’s requirements. This is as demonstrated by the following code sample.

```
string location = "Room 5";
DateTime startDate = new DateTime(2011, 12, 10, 10, 12, 11),
         endDate = new DateTime(2012, 11, 13, 13, 11, 12);
MailAddress organizer = new MailAddress("aaa@amail.com", "Organizer");
MailAddressCollection attendees = new MailAddressCollection();
MailAddress attendee1 = new MailAddress("bbb@bmail.com", "First attendee");
MailAddress attendee2 = new MailAddress("ccc@cmail.com", "Second attendee");

attendee1.ParticipationStatus = ParticipationStatus.Accepted;
attendee2.ParticipationStatus = ParticipationStatus.Declined;
attendees.Add(attendee1);
attendees.Add(attendee2);

Appointment target = new Appointment(location, startDate, endDate, organizer, attendees); 
```

## API Resources

The following API resources can be of help to you in getting started with Aspose.Email API.

*   [Product Documentation][4]– Provides detailed examples of working with the API
*   [API Reference Guide][5]– Details all the namespaces and classes of the API
*   [GitHub Examples][6]– Provides ready to run API example
*   [Support Forum][7]– Write to us if you have any query or inquiry about the API




[1]: https://www.nuget.org/packages/Aspose.Email/
[2]: https://docs.aspose.com/email/net/aspose-email-for-net-18-3-release-notes/
[3]: https://docs.aspose.com/email/net/working-with-appointments/#WorkingwithAppointments-SetParticipantsStatusofAppointmentAttendees
[4]: https://docs.aspose.com/email/net/
[5]: https://apireference.aspose.com/net/email
[6]: https://github.com/asposeemail/Aspose_Email_NET
[7]: https://forum.aspose.com/c/email





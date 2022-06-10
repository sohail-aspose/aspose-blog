---
title: 'Aspose.Network 2.4.0.0 Released'
date: Sat, 27 May 2006 02:59:00 +0000
draft: false
url: /2006/05/27/48969/
author: Iret
summary: ''
tags: ['Kyle Huang']
---

Dear Customers,

We've released Aspose.Network 2.4.0.0.

New features in this version:

*   Support iCalendar features in Mail component, which will enable developer send the meetings or schedules in the email.

          A new class named CalendarMessageBuilder (Aspose.Network.Mail.CalendarMessageBuilder) is exposed, for creating the iCalendar standard compliant email messages. It is the major entry to use the iCalendar features.

         \[C#\]

         MailMessage msg = new MailMessage("[guangzhou@aspose.com][1]", "[kyle.huang@aspose.com][2]");

         msg.Subject = "Release Meeting";

         CalendarMessageBuilder cmb = msg.GetCalendarBuilder();//Get the CalendarMessageBuilder

         cmb.BuildCalendarMessage("Building A Room 504", "Release Meeting", "We will discuss the release for Aspose.Network",  
                                                                                                  new DateTime(2006, 5, 27, 13, 0, 0), new DateTime(2006, 5, 27, 14, 0, 0));//Creating Meeting Calendar

         msg.Send(new SmtpConnection("smtp.yourdomain.com"));

         \[VB.NET\]

         Dim msg As new MailMessage("[guangzhou@aspose.com][3]", "[kyle.huang@aspose.com][4]")

         msg.Subject = "Release Meeting"

         Dim cmb As CalendarMessageBuilder

         cmb = msg.GetCalendarBuilder();//Get the CalendarMessageBuilder

         cmb.BuildCalendarMessage("Building A Room 504", "Release Meeting", "We will discuss the release for Aspose.Network",  
                                                                                                  new DateTime(2006, 5, 27, 13, 0, 0), new DateTime(2006, 5, 27, 14, 0, 0)) 'Creating Meeting Calendar

         msg.Send(new SmtpConnection("smtp.yourdomain.com"))

*   Fixed the bug in BulkSend, which may lead to some email cannot be sent.
*   All fixes from 2.3.\*.\*

Thanks




[1]: mailto:guangzhou@aspose.com
[2]: mailto:kyle.huang@aspose.com
[3]: mailto:guangzhou@aspose.com
[4]: mailto:kyle.huang@aspose.com




---
title: 'PST Password Protection and Exchange Client Logging with .NET Email API'
date: Tue, 11 Aug 2015 17:55:24 +0000
draft: false
url: /2015/08/11/pst-password-protection-and-exchange-client-logging-supported-with-aspose.email-for-.net-5.6.0/
author: Kashif Iqbal
summary: ''
tags: []
categories: ['Aspose.Total Product Family', 'Aspose.Email Product Family']
---



{{< figure align=center src="images/aspose-Email-for-net_100.png" alt="">}}


We are pleased to announce the release of [Aspose.Email for .NET][1] 5.6.0. This month’s release includes new feature, enhancements and other functional improvements as result of a number of bug fixes. The API now provides support for logging in Exchange clients. For a complete list of what is new and fixed, please visit our [product download page][2]. You can also visit our documentation article, Public API Changes, to have complete details about the overall changes in the API.

## Logging in Exchange Clients

Aspose.Email API now provides the capability to log Exchange events in both WebDav and Exchange Web Service clients. This can be achieved by configuring the App.Config file of the application. With this feature, users can now have the facility to log exchange client events for monitoring and errors. More Info

## Rendering Calendar Events to MTHML

Aspose.Email API already provides the capability to convert email and calendar items to MHTML. This month’s release further enriches the conversion feature by allowing calendar events to render to the output MHTML. The MhtFormatOptions enumeration provides RenderCalendarEvent value to achieve this. This is as illustrated in the following code sample.

```
var appointment = Appointment.Load(fileName);

var outlookMsg = new MailMessage();

outlookMsg.AddAlternateView(appointment.RequestApointment());

MhtSaveOptions opt = SaveOptions.DefaultMhtml;

opt.MhtFormatOptions = opt.MhtFormatOptions | MhtFormatOptions.RenderCalendarEvent;

outlookMsg.Save(mhtfileName, opt); 
```

## Setting/Changing PST Password

This month’s release of Aspose.Email API provides the capability to set or change password on a PST file. The _ChangePassword_ method of PST store allows changing or removing the PST password. The following code sample demonstrates the usage of the API for achieving this.

```
using (PersonalStorage pst = PersonalStorage.Create(filename, FileFormatVersion.Unicode))
{
     // set the password
     string password = "qgHgjdLcv63";
     pst.Store.ChangePassword(password);
     // remove the password
     pst.Store.ChangePassword(null);
}
```

## Retrieving Content-Description from Attachment

With this month’s release, the API introduces an enhancement of retrieving attachment’s content description from its headers. The Headers collection exposed by the Attachment class provides all the headers information. More Info

## Bug Fixes

This month’s release fixes a number of bugs that further improves the overall API functionality. These include:

*   Loss of headers during message conversion
*   Wrong start date of recurrence rule
*   Missing inline images from loaded HTML content
*   Issues related to retrieving singed and encrypted messages using POP3 client of the API
*   Formatting issues raised during MHT to MSG
*   Problems related to ICS categories and IMAP Clients
*   Exceptions while assigning task request to MailMessage

## API Documentation and Resources

We offer rich documentation and API examples to get you started with the API in no time. You may visit:

*   Aspose.Email documentation to have knowledge about the API’s functionality
*   [GitHub examples][3] repository to download and try the example in no time
*   API Reference Guide to have an idea about the API classes, methods and properties

If you have any query relate to Aspose.Email API usage, please feel free to write to us over [Aspose.Email forum][4]. We’ll be glad to assist you to the best of our knowledge.




[1]: https://products.aspose.com/email/net
[2]: https://downloads.aspose.com/email/net
[3]: https://github.com/asposeemail/Aspose_Email_NET
[4]: http://www.aspose.com/community/forums/aspose.email-product-family/188/showforum.aspx





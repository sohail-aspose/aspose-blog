---
title: 'Metered Licensing support with Aspose.Email for .NET 18.2'
date: Thu, 22 Feb 2018 14:10:41 +0000
draft: false
url: /2018/02/22/metered-licensing-support-with-aspose.email-for-.net-18.2/
author: Kashif Iqbal
summary: ''
tags: []
categories: ['Aspose.Email Product Family']
---



{{< figure align=center src="images/Aspose.Email-for-.NET_.png" alt="">}}


We are pleased to announce the release of [Aspose.Email for .NET 18.2][1]. This month’s release introduces the capability of Metered Licensing in the API. In addition, it also brings improvements to the API in terms of bug fixes which further add to the overall stability of the API. For a detailed note on what is new and fixed, please visit the [release notes][2] section of the API.

## Metered License with Aspose.Email for .NET 18.2

We are glad to share the support for Metered Licensing in Aspose.Email API. For those who are new to the term “Metered Licensing”, it is a form of consumptive licensing for which you pay royalties for the use of product every month. You can also visit the [Metered Licensing FAQs][3] section to know more about this type of licensing.

## Using the Metered Licensing in API

Usage of Metered Licensing scheme is simple and can be used along with existing licensing method. The new licensing mechanism will be used along with existing licensing method. Those customers who want to be billed based on the usage of the API features can use the metered licensing. 

```
Aspose.Email.Metered metered = new Aspose.Email.Metered();
// Access the SetMeteredKey property and pass public and private keys as parameters
metered.SetMeteredKey("*****", "*****");

// The path to the documents directory. 
string dataDir = RunExamples.GetDataDir_Email();

// Load the message from file system
MailMessage eml = MailMessage.Load(dataDir + "Message.eml");
//Get the subject of Email
Console.WriteLine(eml.Subject); 
```

## API Resources

The following API resources can be of help to you in getting started with Aspose.Email API.

*   [Product Documentation][4] – Provides detailed examples of working with the API
*   [API Reference Guide][5] – Details all the namespaces and classes of the API
*   [GitHub Examples][6] – Provides ready to run API example
*   [Support Forum][7] – Write to us if you have any query or inquiry about the API




[1]: https://www.nuget.org/packages/Aspose.Email/18.2.0
[2]: https://docs.aspose.com/display/emailnet/Aspose.Email+for+.NET+18.2+Release+Notes
[3]: https://purchase.aspose.com/faqs/licensing/metered
[4]: https://docs.aspose.com/display/emailnet/Home
[5]: https://apireference.aspose.com/net/email
[6]: https://github.com/asposeemail/Aspose_Email_NET
[7]: https://forum.aspose.com/c/email





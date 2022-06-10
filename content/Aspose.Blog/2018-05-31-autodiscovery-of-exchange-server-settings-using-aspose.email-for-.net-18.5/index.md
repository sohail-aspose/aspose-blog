---
title: 'Auto Discovery of Exchange Server in C# using Aspose.Email for .NET 18.5'
date: Thu, 31 May 2018 13:05:02 +0000
draft: false
url: /2018/05/31/autodiscovery-of-exchange-server-settings-using-aspose.email-for-.net-18.5/
author: Kashif Iqbal
summary: ''
tags: []
categories: ['Aspose.Email Product Family']
---



{{< figure align=center src="images/Aspose.Email-for-.NET_-1.png" alt="aspose-email-for-.NET">}}


We are pleased to announce the release of [Aspose.Email for .NET 18.5][1]. This month’s release introduces several new features related to various API functionality. It also enhances the API by fixing several bugs that were reported by our valued customers with the previous version of the API. For a detailed note on what is new and fixed, please visit the [release notes][2] section of Aspose.Email API.

## Auto Discover Exchange Server in C#

This release introduces a new feature of [auto-discovery of Exchange server settings][3] using the account’s user name and password. The AutoDiscoverService introduced by the API gets this information from the exchange server using the username and password specified by the application user. In addition to other settings returned by the API, you can get the server’s EWS Url as well using this feature.

{{< gist aspose-email 9e8fbeb51a8cbc4129dc71ca8cd55f0b "Examples-CSharp-Exchange_EWS-AutoDiscoverUsingEWS-AutoDiscoverUsingEWS.cs" >}}

## Abort PST to Exchange Server Operation

PST restore feature of the Aspose.Email API lets you restore the contents of a PST file to Exchange server. The feature is useful in a variety of ways. There is the possibility that operation may take a long time due to the large size of the PST file. This new release of API lets you [abort PST restoration process][4] to the Exchange server based on defined time. This allows users to abort the PST restore operation in case it is taking too long to complete the operation.

{{< gist aspose-email 9e8fbeb51a8cbc4129dc71ca8cd55f0b "Examples-CSharp-Exchange_EWS-AbortPSTToExchangeServerOperation-AbortPSTToExchangeServerOperation.cs" >}}

## Writing Multiple Events to ICS

Aspose.Email already lets you read multiple events from ICS file. This new release of API lets you [write multiple calendar events][5] to a single ICS file as shown in the following code sample.

{{< gist aspose-com-gists 6e5185a63aec6fd70d83098e82b06a32 "Examples-CSharp-Exchange_EWS-WriteMultipleEventsToICS-WriteMultipleEventsToICS.cs" >}}

## API Resources

The following API resources can be of help to you in getting started with Aspose.Email API.

*   [Product Documentation][6] – Provides detailed examples of working with the API
*   [API Reference Guide][7] – Details all the namespaces and classes of the API
*   [GitHub Examples][8] – Provides ready to run API example
*   [Support Forum][9] – Write to us if you have any query or inquiry about the API




[1]: https://www.nuget.org/packages/Aspose.Email/
[2]: https://docs.aspose.com/display/emailnet/Aspose.Email+for+.NET+18.5+Release+Notes
[3]: https://docs.aspose.com/display/emailnet/Utility+Features#UtilityFeatures-AutoDiscoverFeatureusingEWS
[4]: https://docs.aspose.com/display/emailnet/Utility+Features#UtilityFeatures-AbortPSTRestoretoExchangeServerOperation
[5]: https://docs.aspose.com/display/emailnet/Working+with++Appointments#WorkingwithAppointments-WriteMultipleEventstoICSFile
[6]: https://docs.aspose.com/display/emailnet/Home
[7]: https://apireference.aspose.com/net/email
[8]: https://github.com/asposeemail/Aspose_Email_NET
[9]: https://forum.aspose.com/c/email





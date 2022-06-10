---
title: 'Aspose.Email for .NET with Improved Namespace Structure'
date: Mon, 26 Dec 2016 10:29:35 +0000
draft: false
url: /2016/12/26/aspose.email-.net-improved-namespace-structure-available-now/
author: Kashif Iqbal
summary: ''
tags: []
categories: ['Aspose.Email Product Family']
---



{{< figure align=center src="images/Aspose.Email-for-.NET_-1.png" alt="Aspose.Email for .NET">}}


We recently shared with our valued users/customers that [Aspose.Email for .NET][1] is under the process of improvement in terms of [API Namespace restructuring][2]. We are pleased to announce that this revamped version with improved namespace structure is available for [download][3] now. API with old namespace structure, hereafter called as legacy API, is still available for download from the [product download section][4].

## Why Namespace Restructuring?

To understand the need for the API namespace restructuring, let’s have a look at few namespaces of the legacy version of Aspose.Email for .NET.

*   Email
*   Email.Mime
*   Email.AntiSpam
*   Email.Imap
*   Email.Pop3
*   Email.Mail.Smtp
*   Email.Mail
*   Email.Mapi
*   Email.Outlook

These are some of the API namespaces beside others. Now if looked carefully, one can see that although the API provides all the published functionality, there exists a lack in the logical organization between the functional elements of the API. For example, it is difficult to choose between the Mapi and Outlook namespaces for working with Personal Storage (PST) files. The same is true for Aspose.Email, Mail, and Mime namespaces for working with a MIME email message.

## Revamped API with Improved Namespace Structure

Keeping in view the afore-mentioned observations, we found more space for improvement in the Namespace structure of the API in terms of relevance between the API functional elements. This is the reason that has led us to a revamped version of the API with a logical grouping of the functionality.

## About New Namespace Structure

Following is the new namespace structure of the improved API.

*   **Aspose.Email**
*   **Aspose.Email.AntiSpam**
*   **Aspose.Email.Bounce**
*   **Aspose.Email.Calendar**
    *   Aspose.Email.Calendar.Recurrences
*   **Aspose.Email.Clients**
    *   Aspose.Email.Clients.ActiveSync
    *   Aspose.Email.Clients.Exchange
    *   Aspose.Email.Clients.Exchange.Dav
    *   Aspose.Email.Clients.Exchange.WebService
    *   Aspose.Email.Clients.Google
    *   Aspose.Email.Clients.Imap
    *   Aspose.Email.Clients.Pop3
    *   Aspose.Email.Clients.Smtp
*   **Aspose.Email.DKIM**
*   **Aspose.Email.Mapi**
    *   Aspose.Email.Mapi.Msg
*   **Aspose.Email.Mime**
*   **Aspose.Email.PersonalInfo**
    *   Aspose.Email.PersonalInfo.VCard
*   **Aspose.Email.Printing**
*   **Aspose.Email.Storage**
    *   Aspose.Email.Storage.Mbox
    *   Aspose.Email.Storage.Pst
*   **Aspose.Email.Tools**
    *   Aspose.Email.Tools.Logging
    *   Aspose.Email.Tools.Verifications
    *   Aspose.Email.Tools.Merging
    *   Aspose.Email.Tools.Search
*   **Aspose.Email.Windows**
    *   Aspose.Email.Windows.Forms
    *   Aspose.Email.Windows.WPF

As can be seen, this new Namespace structure of the API has a much better organization of API’s functional elements. For example, all the communication clients such as IMAP, POP3, SMTP, and Exchange clients have been grouped under Aspose.Email.Clients namespace. Similarly, working with storage elements like PST and Mbox have been grouped under the Aspose.Email.Storage namespace so as to be more meaningful and easy to locate.

## What will happen to my applications built on legacy API?

As a user of the legacy API, your concerns are right. Since the revamped API has a difference in namespace structure, the old codes won’t work in almost all the cases. However, we will keep publishing the legacy as well as the improved version in parallel for three consecutive months. We’ll address the bug reports in the legacy API for these versions. Any new features, as well as bug fixes, will be part of the legacy as well as the newest implementation.

## Which version will be available on NuGet?

Till three parallel releases of the legacy as well as the revamped version, the legacy version will be available on NuGet. After this period, the new version will be available on NuGet. This is to ensure that this transition doesn’t break the customer’s production systems.

## How to get started with migration?

As such, there is no functionality implementation change. The logical organization of the namespaces has been rearranged that will only need you to update your “using” statements in applications and fully qualified calls to API. For a guide about addressing the proper namespace, please visit the release notes section of the improved version of the API. It provides a complete guide for migrating your codes to this improved version of the API.

## Where can I find the new API documentation?

At present, the API documentation and API reference guide of Aspose.Email for .NET is based on the legacy API. However, our code samples in documentation pages are independent of this change as they don’t refer to the “using” statements of a project. These can be readily used with the improved version of the API as well.

# Are there any revamped examples Available?

Since our Github examples are configured to work with the available version from Nuget, our Github examples are still based on the legacy API. We’ll update them once we are done with the three parallel releases of both the APIs. For now, we have prepared an offline version of the examples which are based on the revamped API.

# Got queries?

As always, we are here to answer your queries related to this change in addition to our continual routine support for the API. Feel free to post us with your questions in [Aspose.Email forum][5]. We’ll be more than happy to assist you in this regard.




[1]: https://products.aspose.com/email/net
[2]: https://blog.aspose.com/2016/12/08/improvements-in-namespace-structure-of-aspose.email-for-.net/
[3]: http://downloads.aspose.com/email/net/new-releases/aspose.email-for-.net-16.12.0---revamped/
[4]: http://downloads.aspose.com/email/net
[5]: https://forum.aspose.com/c/email





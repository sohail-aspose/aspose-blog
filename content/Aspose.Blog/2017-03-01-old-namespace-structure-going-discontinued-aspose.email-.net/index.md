---
title: 'Old namespace structure is going to be discontinued - Aspose.Email for .NET'
date: Wed, 01 Mar 2017 12:54:22 +0000
draft: false
url: /2017/03/01/old-namespace-structure-going-discontinued-aspose.email-.net/
author: Kashif Iqbal
summary: ''
tags: []
categories: ['Aspose.Email Product Family']
---

We shared earlier with our valued customers about the [improved namespace structure][1] API of Aspose.Email for .NET.  We have been publishing this revamped API in parallel to the API with old namespace structure for three consecutive months now. However, we won’t be publishing any further releases of the legacy API and only the revamped version of the API will be published hereafter.

## Revamped API with Improved Namespace Structure

We found more space for improvement in Namespace structure of the API in terms of relevance between the API functional elements. This is the reason that has lead us to a revamped version of the API with logical grouping of the functionality.

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

As can be seen, this new Namespace structure of the API has much better organization of API’s functional elements. For example, all the communication clients such as IMAP, POP3, SMTP and Exchange clients have been grouped under Aspose.Email.Clients namespace. Similarly, working with storage elements like PST and Mbox have been grouped under the Aspose.Email.Storage namespace so as to be more meaningful and easy to locate.

## What if I don't update to the revamped version?

Well, if you are a regular user of the API and want to avail all the features offered by the latest version of the API, you'll have to update to the revamped version of the API. As mentioned, we won't be publishing any further releases of the legacy API. This will break your codes in production server if you will update from Nuget or you will have to live with the last legacy version of the API which won't benefit you for long.

## How to get started with migrating existing code?

As such, there is no functionality implementation change. The logical organization of the namespaces has been rearranged that will only need you to update your “using” statements in applications and fully qualified calls to API. For a guide about addressing the proper namespace, please visit the release notes section of the improved version of the API. It provides a complete guide for migrating your codes to this improved version of the API. You can download the latest version of the Revamped Aspose.Email for .NET API from [downloads section][2] of Aspose.Email for .NET API.

## Are there any revamped examples available?

We'll update our GitHub examples repositories for Aspose.Email for .NET with the new version of the API once we start publishing this improved version to Nuget. However, we have modified these as an offline version and can be downloaded from this link for experimenting with the new API.

## Got queries?

As always, we are here to answer your queries related to this change in addition to our continual routine support for the API. Feel free to post us with your questions in [Aspose.Email forum][3]. We’ll be more than happy to assist you in this regard.




[1]: https://blog.aspose.com/2016/12/26/aspose.email-.net-improved-namespace-structure-available-now/
[2]: https://downloads.aspose.com/email/net/new-releases/aspose.email-for-.net-17.2.0---revamped/
[3]: https://forum.aspose.com/c/email





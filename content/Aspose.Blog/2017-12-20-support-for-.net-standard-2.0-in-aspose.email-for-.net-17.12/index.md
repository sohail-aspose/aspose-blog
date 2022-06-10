---
title: 'Support for .NET Standard 2.0 in Aspose.Email for .NET 17.12'
date: Wed, 20 Dec 2017 14:38:01 +0000
draft: false
url: /2017/12/20/support-for-.net-standard-2.0-in-aspose.email-for-.net-17.12/
author: Kashif Iqbal
summary: ''
tags: ['Email API for .NET Core', 'Email API for .NET Standard', 'Send Emails in .NET Core', 'Send Emails in .NET Standard']
categories: ['Aspose.Email Product Family']
---



{{< figure align=center src="images/Aspose.Email-for-.NET_-1.png" alt="aspose-email-for-.NET">}}


We are pleased to announce the release of [Aspose.Email for .NET 17.12][1]. This release brings exciting feature of support for .NET Standard 2.0 (.NET Core) for our users. We have also merged Aspose.Email APIs for Xamarin platform in this month’s release. For a detailed note on what is new and fixed, please visit the [release notes section][2] of API documentation for Aspose.Email for .NET.

# Support for .NET Standard 2.0

Starting from 17.12 release, the API now includes .NET Standard 2.0 (.NET Core). It has full functionality of standard .NET Framework except the following limitations:

*   Email.Clients.ActiveSync.TransportLayer namespace is not available
*   Email.Windows namespace is not available
*   Email.Printing namespace is not available
*   Linked images into message body in both RTF as well as HTML format are not supported
*   It also has no functionality of Signing or Encrypting/Decrypting messages
*   Email under .NET Core will work only with servers that implement at least TLS 1.0. Some servers (like Gmail) support both SSL and TLS. Aspose.Email can force them to use TLS.

# Merged Xamarin APIs

Starting from this release, Aspose.Email for Android via Xamarin, Aspose.Email for iOS via Xamarin and Aspose.Email for Mac via Xamarin have become part of Aspose.Email for .NET. There are no breaking changes.

# Improvements

This release also includes several improvements in terms of bug fixes which further add to the overall stability of the API. These are related to various API functionality and include:

*   Processing of encrypted messages
*   Email messages to MHTML
*   Rendering of hyperlinks to HTML during conversion
*   Timezone changes during conversion of EML to MSG
*   Exceptions while converting messages to MSG and ICS
*   Loss of formatting during messages conversion to XPS

# API Resources

The following API resources can be of help to you in getting started with Aspose.Email API.

*   [Product Documentation][3] – Provides detailed examples of working with the API
*   [API Reference Guide][4] – Details all the namespaces and classes of the API
*   [GitHub Examples][5] – Provides ready to run API example
*   [Support Forum][6] – Write to us if you have any query or inquiry about the API




[1]: https://www.nuget.org/packages/Aspose.Email/17.12.0
[2]: https://docs.aspose.com/display/emailnet/Aspose.Email+for+.NET+17.12+Release+Notes
[3]: https://docs.aspose.com/display/emailnet/Home
[4]: https://apireference.aspose.com/net/email
[5]: https://github.com/asposeemail/Aspose_Email_NET
[6]: https://forum.aspose.com/c/email





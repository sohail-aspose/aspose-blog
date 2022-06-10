---
title: 'Add Custom Flags to Email Messages using C# with Aspose.Email for .NET'
date: Fri, 09 Jun 2017 18:43:57 +0000
draft: false
url: /2017/06/09/add-custom-flags-messages-using-aspose.email-.net-17.6/
author: Kashif Iqbal
summary: ''
tags: []
categories: ['Aspose.Email Product Family']
---



{{< figure align=center src="images/Aspose.Email-for-.NET_-1.png" alt="">}}


We are pleased to announce the release of [Aspose.Email for .NET 17.6][1]. It includes new features and enhancements related to various functional areas of the API. Specifically, the enhancements are related to the API’s IMAP, EWS client and rendering of messages to MHTML. The API also fixes several bugs that further improve the performance and functionality of the API. For a complete list of what is new and fixed, please visit the [release notes section][2] of API documentation.

## Add Custom Flag to Messages using IMAP in C#

This month’s release introduces a new feature of [adding custom flags][3] to a message on the server using the API’s ImapClient. Custom flags can be added to a message using the AddMessageFlags method using the ImageMessageFlags. This is illustrated in the code sample below.

{{< gist aspose-com-gists 6e5185a63aec6fd70d83098e82b06a32 "Examples-CSharp-IMAP-SetCustomFlag-SetCustomFlag.cs" >}}

## Filter Messages based on Custom Flags using C#

Not only you can add custom flags to messages on server using the API’s ImapClient, but you can also filter messages by specifying custom flags. The ImapQueryBuilder’s HasFlags and HasNoFlags can be used for this purpose as shown in the code sample below.

{{< gist aspose-com-gists 6e5185a63aec6fd70d83098e82b06a32 "Examples-CSharp-IMAP-GetMessagesWithSpecificCriteria-GetMessagesWithCustomFlags.cs" >}}

## Skip Inline Images during Email Conversion

Email messages with multiple or large size images embedded in them can take considerable time and system resources during conversion to MHTML format. This month’s release provides the capability to [skip inline images][4] from including in output MHTML using the MhtSaveOptions class’s SkipInlineImages property. Setting this flag avoids writing inline images from the message body to output MHTML.

{{< gist aspose-com-gists 6e5185a63aec6fd70d83098e82b06a32 "Examples-CSharp-Email-ConvertMHTMLWithOptionalSettings-ConvertToMHTMLWithoutInlineImages.cs" >}}

## API Resources

The following API resources can be of help to you in getting started with Aspose.Email API.

*   [Product Documentation][5] – Provides detailed examples of working with the API
*   [API Reference Guide][6] – Details all the namespaces and classes of the API
*   [GitHub Examples][7] – Provides ready to run API example
*   [Support Forum][8] – Write to us if you have any query or inquiry about the API




[1]: https://downloads.aspose.com/email/net/new-releases/aspose.email-for-.net-17.5.0/
[2]: https://docs.aspose.com/display/emailnet/Aspose.Email+for+.NET+17.6+Release+Notes
[3]: https://docs.aspose.com/display/emailnet/Working+with+Message+Flags+on+Server#WorkingwithMessageFlagsonServer-SettingCustomFlags
[4]: https://docs.aspose.com/display/emailnet/Loading+and+Saving+Message#LoadingandSavingMessage-ExportingEmailtoMHTwithoutInlineImages
[5]: https://docs.aspose.com/display/emailnet/Home
[6]: https://www.aspose.com/api/net/email
[7]: https://github.com/asposeemail/Aspose_Email_NET
[8]: https://forum.aspose.com/c/email





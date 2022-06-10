---
title: 'Render Outlook VCard Contact to MHTML using C#'
date: Wed, 29 Mar 2017 17:37:06 +0000
draft: false
url: /2017/03/29/rendering-outlook-vcard-contact-mhtml-aspose.email-.net-17.3.0/
author: Kashif Iqbal
summary: ''
tags: []
categories: ['Aspose.Email Product Family']
---



{{< figure align=center src="images/Aspose.Email-for-.NET_.png" alt="">}}


We are pleased to announce the release of [Aspose.Email for .NET 17.3.0][1]. This month’s release includes enhancements and bug fixes that enriches the API functionality and adds stability to the API behavior. As mentioned [earlier][2], we have also stopped publishing the legacy version of the API and the revamped version with improved namespace will be published from now onwards. For a detailed note on what is new and fixed, please visit the [release notes section][3] of Aspose.Email for .NET documentation.

## Render VCard Information to MHTML using C#

This month’s release provides the capability to render Microsoft Outlook [VCard contact][4] information to MHTML. This can be achieved with MhtFormatOptions.RenderVCardInfo enumerator while saving the message to MHTML. Previously, only headers information was rendered to output while rendering the respective values was not supported. The following code sample gives an illustration of how to use this feature.

```
//Load VCF Contact and convert to MailMessage for rendering to MHTML
MapiContact contact = MapiContact.FromVCard(dataDir + "Contact.vcf");

MemoryStream ms = new MemoryStream();
contact.Save(ms, ContactSaveFormat.Msg);
ms.Position = 0;
MapiMessage msg = MapiMessage.FromStream(ms);
MailConversionOptions op = new MailConversionOptions();
MailMessage eml = msg.ToMailMessage(op);

//Prepare the MHT format options
MhtSaveOptions mhtSaveOptions = new MhtSaveOptions();
mhtSaveOptions.CheckBodyContentEncoding = true;
mhtSaveOptions.PreserveOriginalBoundaries = true;
MhtFormatOptions formatOp = MhtFormatOptions.WriteHeader | MhtFormatOptions.HideExtraPrintHeader | MhtFormatOptions.RenderVCardInfo;
mhtSaveOptions.MhtFormatOptions = formatOp;
eml.Save(dataDir + "ContactMhtml.mhtml", mhtSaveOptions);
```

## Support for Email Threading

Aspose.Email API already supported creating reply and forwarding messages using the MailMessage class. However, this didn’t support creating a thread between the original and replied email. This month’s release provides the capability to [create threading][5] among the original emails and the replies sent out using Aspose.Email API.

## Other Improvements

Like always, we have also fixed several bugs in this month’s release that were reported by our valued customers with different API functionality. This further adds stability to the API functionality and makes the output predictable.

## API Resources

The following API resources can be of help to you in getting started with Aspose.Email API.

*   [Product Documentation][6] – Provides detailed examples of working with the API
*   [API Reference Guide][7] – Details all the namespaces and classes of the API
*   [GitHub Examples][8] – Provides ready to run API example
*   [Support Forum][9] – Write to us if you have any query or inquiry about the API




[1]: https://downloads.aspose.com/email/net
[2]: https://blog.aspose.com/2017/03/01/old-namespace-structure-going-discontinued-aspose.email-.net/
[3]: https://docs.aspose.com/display/emailnet/Aspose.Email+for+.NET+17.3.0+Release+Notes
[4]: https://docs.aspose.com/display/emailnet/Working+with+Outlook+Contacts#WorkingwithOutlookContacts-RenderingContactInformationtoMHTML
[5]: https://docs.aspose.com/display/emailnet/Managing+Message+Files+with+Aspose.Email.Outlook#ManagingMessageFileswithAspose.Email.Outlook-CreatingReplyMessage
[6]: https://docs.aspose.com/display/emailnet/Home
[7]: https://www.aspose.com/api/net/email
[8]: https://github.com/asposeemail/Aspose_Email_NET
[9]: https://forum.aspose.com/c/email





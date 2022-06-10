---
title: 'Convert Outlook VCard Contacts to MHTML using Aspose.Email for Java'
date: Mon, 03 Apr 2017 14:45:46 +0000
draft: false
url: /2017/04/03/convert-outlook-vcard-contacts-mhtml-using-aspose.email-java/
author: Kashif Iqbal
summary: ''
tags: []
categories: ['Aspose.Email Product Family']
---

![](http://blog.aspose.com/wp-content/uploads/sites/2/2016/11/aspose-Email-for-Java_100.png)

[Aspose.Email for Java 17.3.0][1] has been released. Ported from its equivalent .NET version, it contains the same enhancements and bug fixes that were part of the equivalent .NET version. It now provides support for email threading and conversion of Outlook VCard contact to MHTML. For a detailed list of what is new and fixed, please visit the [release notes section][2] of our documentation.

# New Features and Enhancements

**Support for Email Threading:** We have enhanced the functionality of replying messages using the API in this month’s release which results in generating [email threads][3] for the original and replied email. This leads to the display of email as conversation threads. There hasn’t been any public API reference change from user’s perspective as the changes are internal to the reply email functionality already supported by the API.

**Support for converting VCard contact to MHTML:** This month’s release also supports conversion of Outlook VCard contact to MHTML. The MhtFormatOptions.RenderVCardInfo enumerator provides the user interface for specifying the [rendering of VCard][4] information to MHTML. This is as illustrated in the following code sample.

```
//Load VCF Contact and convert to MailMessage for rendering to MHTML
MapiContact contact = MapiContact.fromVCard("VCard Contact.vcf");

ByteArrayOutputStream os = new ByteArrayOutputStream();

contact.save(os, ContactSaveFormat.Msg);

MapiMessage msg = MapiMessage.fromStream(new ByteArrayInputStream(os.toByteArray()));
MailConversionOptions op = new MailConversionOptions();
MailMessage eml = msg.toMailMessage(op);

//Prepare the MHT format options
MhtSaveOptions mhtSaveOptions = new MhtSaveOptions();
mhtSaveOptions.setCheckBodyContentEncoding(true);
mhtSaveOptions.setPreserveOriginalBoundaries(true);
int formatOp = (int)(MhtFormatOptions.WriteHeader | MhtFormatOptions.HideExtraPrintHeader | MhtFormatOptions.RenderVCardInfo);
mhtSaveOptions.setMhtFormatOptions(formatOp);
  
eml.save("ContactsSaqib Razzaq_out.mhtml", mhtSaveOptions); 
```

# Other Improvements

This month’s release also includes several bug fixes that were reported by our users with the previous release. Details about these can be found in the release notes section of this month's release.  
  

# API Resources

We have detailed information available online for getting started with the Aspose.Email for Java API. These are:

*   [Product Documentation][5] – Provides detailed examples of working with the API
*   [API Reference Guide][6] – Details all the packages and classes of the API
*   [GitHub Examples][7] – Provides ready to run API examples
*   [Aspose.Email Forum][8] – Feel free to contact us on Aspose.Email forum for your queries




[1]: https://downloads.aspose.com/email/java
[2]: https://docs.aspose.com/display/emailjava/Aspose.Email+for+Java+17.3.0+Release+Notes
[3]: https://docs.aspose.com/display/emailjava/Managing+Message+Files+with+Aspose.Email.Outlook#ManagingMessageFileswithAspose.Email.Outlook-CreateReplyMessage
[4]: https://docs.aspose.com/display/emailjava/Working+with+Outlook+Contacts#WorkingwithOutlookContacts-RenderingContactInformationtoMHTML
[5]: https://docs.aspose.com/display/emailjava/Home
[6]: http://www.aspose.com/api/java/email
[7]: https://github.com/aspose-email/Aspose.Email-for-Java
[8]: https://forum.aspose.com/c/email





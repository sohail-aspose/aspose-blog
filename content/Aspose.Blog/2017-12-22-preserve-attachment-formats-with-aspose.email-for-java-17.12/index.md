---
title: 'Preserve Attachment Formats with Aspose.Email for Java 17.12'
date: Fri, 22 Dec 2017 17:42:19 +0000
draft: false
url: /2017/12/22/preserve-attachment-formats-with-aspose.email-for-java-17.12/
author: Kashif Iqbal
summary: ''
tags: ['Preserve attachment format in the emails']
categories: ['Aspose.Email Product Family']
---



{{< figure align=center src="images/aspose-Email-for-Java_100.png" alt="aspose-email-for-java">}}


We are pleased to announce the release of [Aspose.Email for Java 17.12][1]. This release brings the same improvements that are part of equivalent Aspose.Email for .NET version. Specifically, it provides the capability to preserve attachment format while extracting Contacts and Tasks from the PST file. For a detailed note on what is new and fixed, please visit the [release notes][2] section of API documentation.

# Preserving Attachments Format During Conversion

This release introduces the capability to save Outlook item’s attachment format during saving to disc. Attachment MSG formats can now be preserved while exporting Outlook Contacts and Tasks from PST file. This can be achieved using the setPreserveEmbeddedMessageFormat method of EmlSaveOptions to true.

```
EmlSaveOptions saveOptions = new EmlSaveOptions(MailMessageSaveType.getEmlFormat());
saveOptions.setPreserveEmbeddedMessageFormat(true);
message.save("output.eml", saveOptions);
```

# Other Improvements

This release also includes several improvements in terms of bug fixes. These include issues related to:

*   Processing of encrypted messages
*   Email messages to MHTML
*   Rendering of hyperlinks to HTML during conversion
*   Timezone changes during the conversion of EML to MSG
*   Exceptions while converting messages to MSG and ICS
*   Loss of formatting during messages conversion to XPS

# API Resources

We have detailed information available online for getting started with the Aspose.Email for Java API. These are:

*   [Product Documentation][3] – Provides detailed examples of working with the API
*   [API Reference Guide][4] – Details all the packages and classes of the API
*   [GitHub Examples][5] – Provides ready to run API examples
*   [Aspose.Email Forum][6] – Feel free to contact us on Aspose.Email forum for your queries




[1]: http://maven.aspose.com/repository/simple/ext-release-local/com/aspose/aspose-email/17.12/
[2]: https://docs.aspose.com/display/emailjava/Aspose.Email+for+Java+17.12+Release+Notes
[3]: https://docs.aspose.com/display/emailjava/Home
[4]: https://apireference.aspose.com/java/email
[5]: https://github.com/aspose-email/Aspose.Email-for-Java
[6]: https://forum.aspose.com/c/email





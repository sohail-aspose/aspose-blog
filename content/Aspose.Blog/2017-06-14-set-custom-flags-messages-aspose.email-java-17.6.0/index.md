---
title: 'Set Custom Flags on Messages with Aspose.Email for Java 17.6.0'
date: Wed, 14 Jun 2017 10:42:53 +0000
draft: false
url: /2017/06/14/set-custom-flags-messages-aspose.email-java-17.6.0/
author: Kashif Iqbal
summary: ''
tags: []
categories: ['Aspose.Email Product Family']
---

[![][1]](https://www.aspose.com/products/email/java)We are pleased to announce the release of [Aspose.Email for Java 17.6][2]. This month’s release includes a new feature of adding custom flag to a message using IMAP. It also enhances several API functionality by adding to the existing features of the API and fixes bugs. For a detail note on what is new and fixed, please visit the [release notes][3] section of Aspose.Email for Java 17.6.

# New Features and Enhancements

**Adding Custom Flag to Messages using IMAP:** This month’s release provides the capability to add [custom flag to a message][4] using the API’s ImapClient. Custom flags can be added to a message using the addMessageFlags method using the ImageMessageFlags as shown in the following code sample.

```
// Create a message
MailMessage message = new MailMessage("user@domain1.com", "user@domain2.com", "subject", "message");

ImapClient client = new ImapClient("host.domain.com", 587, "username", "password");
		
//Append the message to mailbox
String uid = client.appendMessage(ImapFolderInfo.IN_BOX, message);

//Add custom flags to the added message
client.addMessageFlags(uid, ImapMessageFlags.op_BitwiseOr(
        ImapMessageFlags.keyword("custom1")
        ,ImapMessageFlags.keyword("custom1_0")));

//Retrieve the messages for checking the presence of custom flag
client.selectFolder(ImapFolderInfo.IN_BOX);

ImapMessageInfoCollection messageInfos = client.listMessages();
for (ImapMessageInfo inf: messageInfos)
{
    ImapMessageFlags[] flags = inf.getFlags().split();

    if (inf.containsKeyword("custom1"))
        System.out.println("Keyword found");
} 
```

**Filtering messages based on Custom Flag:** The API also now supports filtering messages based on custom flags from the message. The ImapQueryBuilder can be used to achieve this as shown in the following code sample.

```
ImapQueryBuilder queryBuilder = new ImapQueryBuilder();

queryBuilder.hasFlags(ImapMessageFlags.keyword("custom1"));

queryBuilder.hasNoFlags(ImapMessageFlags.keyword("custom2")); 
```

 **Skipping Inline Images during Email Conversion to MHT:** We have also incorporated the functionality of [skipping inline images][5] from email messages while converting to MHTML format. This helps in improved performance while converting email messages that have large size inline images in message body.

```
MailMessage eml = MailMessage.load(dataDir + "Message.msg", new MsgLoadOptions());
		
MhtSaveOptions mhtSaveOptions = new MhtSaveOptions();
		
mhtSaveOptions.setSkipInlineImages(true);

eml.save(dataDir + "EmlToMhtmlWithoutInlineImages_out.mht", mhtSaveOptions); 
```

# API Resources

We have detailed information available online for getting started with the Aspose.Email for Java API. These are:

*   [Product Documentation][6] – Provides detailed examples of working with the API
*   [API Reference Guide][7] – Details all the packages and classes of the API
*   [GitHub Examples][8] – Provides ready to run API examples
*   [Aspose.Email Forum][9] – Feel free to contact us on Aspose.Email forum for your queries




[1]: http://blog.aspose.com/wp-content/uploads/sites/2/2016/11/aspose-Email-for-Java_100.png
[2]: https://downloads.aspose.com/email/java
[3]: https://docs.aspose.com/display/emailjava/Aspose.Email+for+Java+17.6+Release+Notes
[4]: https://docs.aspose.com/display/emailjava/Aspose.Email+for+Java+17.6+Release+Notes
[5]: https://docs.aspose.com/display/emailjava/Loading+and+Saving+Message#LoadingandSavingMessage-ExportingEmailtoMHTwithoutInlineImages
[6]: https://docs.aspose.com/display/emailjava/Home
[7]: http://www.aspose.com/api/java/email
[8]: https://github.com/aspose-email/Aspose.Email-for-Java
[9]: https://forum.aspose.com/c/email





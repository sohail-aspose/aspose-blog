---
title: 'Aspose.Email for Java 6.1.0 supports Extracting Attachments from PST Messages'
date: Thu, 14 Jan 2016 15:34:11 +0000
draft: false
url: /2016/01/14/aspose.email-for-java-6.1.0-supports-extracting-attachments-from-pst-messages/
author: Kashif Iqbal
summary: ''
tags: []
categories: ['Aspose.Email Product Family']
---

![](https://blog.aspose.com/wp-content/uploads/sites/2/2016/01/aspose-Email-for-Java_100.png "Aspose.Email for Java")

[Aspose.Email for Java 6.1.0][1] has been released. This month’s release brings enhancements to various functional areas of the API. Specifically, the enhancements are related to the Exchange Web Service (EWS) client and Personal Storage (PST) files. It also fixes a number of bugs that were reported with our last month’s release. Please visit our documentation section, Public API changes, to get complete information about the changes included in this month’s release.

# Enhancements

**Extracting Attachments from PST file:** This month’s release implements the functionality of extracting attachments from PST messages without extracting complete message first. The API now provides a new method, _extractAttachments_, which can be used to extract attachments from the message using either the message summary information or message entry id.

**Getting Parent Folder Information of a Message:** The API also provides an enhancement feature of getting parent folder information from a message’s entry id or summary information in a PST. This gives users the power of getting information about a message’s parent folder for storing as meta-data. It can also help in getting other messages from the parent folder if required.

**Provision of Including Special Characters in Folder Names:** Aspose.Email’s Exchange Web Service (EWS) API already provides the capability of creating folders and sub-folders in an Exchange Mailbox. However, the API had an issue while creating a folder name with “/” in it. It resulted in creating sub-folder after the “/”. This month’s release now provides IEWSClient. setUseSlashAsFolderSeparator folder to treat slash as folder separator and create sub-folder in mailbox.

# Other Improvements

As Aspose.Email for Java is ported from its equivalent .NET version, it includes the same bug fixes that were part of the .NET version. Details about these can be found in the [API’s download section][2].

# API Resources

We have detailed information available online for getting started with the Aspose.Email for Java API. These are:

*   Product Documentation – Provides detailed examples of working with the API
*   API Reference Guide – Details all the packages and classes of the API
*   [GitHub Examples][3] – Provides ready to run API examples
*   [Aspose.Email Forum][4] – Feel free to contact us on Aspose.Email forum for your queries




[1]: http://www.aspose.com/community/files/72/java-components/aspose.email-for-java/default.aspx
[2]: http://www.aspose.com/community/files/72/java-components/aspose.email-for-java/default.aspx
[3]: https://github.com/aspose-email/Aspose.Email-for-Java
[4]: http://www.aspose.com/community/forums/aspose.email-product-family/188/showforum.aspx





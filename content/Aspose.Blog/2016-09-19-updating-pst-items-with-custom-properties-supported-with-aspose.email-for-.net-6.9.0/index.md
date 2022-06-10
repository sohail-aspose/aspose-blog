---
title: 'Updating PST Items with Custom Properties supported with Aspose.Email for .NET 6.9.0'
date: Mon, 19 Sep 2016 14:39:39 +0000
draft: false
url: /2016/09/19/updating-pst-items-with-custom-properties-supported-with-aspose.email-for-.net-6.9.0/
author: Kashif Iqbal
summary: ''
tags: []
categories: ['Aspose.Email Product Family']
---

[![][1]](http://www.aspose.com/products/email/net)

We are pleased to announce the release of [Aspose.Email for .NET 6.9.0][2]. It includes new feature of marking items in-place in a PST file. It also includes enhancement for syncing Exchange server’s folder information and detecting embedded message type using the _MailMessage_ API. In addition, it includes a number of bug fixes that brings further stability to the API functionality. For a complete list of what is new and fixed, please visit our Product documentation section for Release Notes.

# New Features and Enhancements

**Updating Messages In-Place in a PST:** This new feature provides the capability to update certain properties in a message file that could be lateral used to determine the marked messages. This can be achieved with the help of custom properties set on message files. The _ChangeMessages_ and _ChangeMessage_ introduced respectively by the _FolderInfo_ and _PersonalStorage_ classes can be used to achieve this. Our documentation article, Updating Custom Properties on Messages in PST file, demonstrates the usage of this new feature.

```
using (PersonalStorage pst = PersonalStorage.FromFile(@"test.pst"))
{
    FolderInfo testFolder = pst.RootFolder.GetSubFolder("test");

    // Create the collection of message properties for adding or updating
    MapiPropertyCollection newProperties = new MapiPropertyCollection();

    // Normal property
    MapiProperty property = new MapiProperty(
        MapiPropertyTag.PR_ORG_EMAIL_ADDR_W,
        Encoding.Unicode.GetBytes("test_address@org.com"));

    // Custom named property
    MapiProperty namedProperty1 = new MapiNamedProperty(
        GenerateNamedPropertyTag(0, MapiPropertyType.PT_LONG),
        "ITEM_ID",
        Guid.NewGuid(),
        BitConverter.GetBytes(123));

    // PidLidLogFlags named property
    MapiProperty namedProperty2 = new MapiNamedProperty(
        GenerateNamedPropertyTag(1, MapiPropertyType.PT_LONG),
        0x0000870C,
        new Guid("0006200A-0000-0000-C000-000000000046"),
        BitConverter.GetBytes(0));

    newProperties.Add(namedProperty1.Tag, namedProperty1);
    newProperties.Add(namedProperty2.Tag, namedProperty2);
    newProperties.Add(property.Tag, property);

    testFolder.ChangeMessages(testFolder.EnumerateMessagesEntryId(), newProperties);
} 
```

**Detecting Embedded Message in a MIME message:** This month’s release also includes a new feature of detecting an attachment for embedded message in a MIME message. The IsEmbeddedMessage property of the Attachment class provides the capability to achieve this.

**Support for Synching Folder Information on Exchange Server:** This month’s release further enhances the functionality of synching folder items on Exchange server. The feature of synching folder contents was supported earlier. However, this month’s release further enhances the functionality by synching the folder name and properties as well.

# Other Improvements

This month’s release also fixes a number of bugs that were reported with the earlier version of the API. Fixing of these issues further enhances the quality of API functionality.

# API Resources

The following API resources can be of help to you in getting started with Aspose.Email API.

*   Product Documentation – Provides detailed examples of working with the API
*   API Reference Guide – Details all the namespaces and classes of the API
*   [GitHub Examples][3] – Provides ready to run API example
*   [Support Forum][4] – Write to us if you have any query or inquiry about the API




[1]: https://blog.aspose.com/wp-content/uploads/sites/2/2016/09/Aspose.Email-for-.NET_.png "Aspose.Email for .NET"
[2]: http://www.aspose.com/downloads/email/net
[3]: https://github.com/asposeemail/Aspose_Email_NET
[4]: http://www.aspose.com/community/forums/aspose.email-product-family/188/showforum.aspx





---
title: 'Update PST Items without Extraction using Aspose.Email for Java'
date: Tue, 20 Sep 2016 16:39:28 +0000
draft: false
url: /2016/09/20/update-pst-items-without-extraction-using-aspose.email-for-java-6.9.0/
author: Kashif Iqbal
summary: ''
tags: []
categories: ['Aspose.Email Product Family']
---



{{< figure align=center src="images/aspose-Email-for-Java_100.png" alt="">}}


[Aspose.Email for Java 6.9.0][1] has been released. This month’s release includes the same new features as were part of the equivalent .NET version of the API. Specifically, it provides the capability to mark items in-place in a PST file and detect if an attachment of a message is an embedded message. It also contains a number of bug fixes that further improve the API functionality. For a complete list of what is new and fixed, please visit the release notes section of Aspose.Email for Java documentation.

## Mark PST Items using Custom Properties in Java

This month’s release enhances the capability of updating PST Items in-place using custom properties. The API, earlier, supported updating common properties of PST items such as subject, recipients, senders, etc. With this enhancements, an item in a PST can be attached a custom property for marking it with specific information. The feature doesn’t require to extract the complete item first. Instead, the items can be marked in-place using the _FolderInfo_ and _PersonalStorage_ classes as shown in the code sample below.

```
PersonalStorage pst = PersonalStorage.fromFile("test.pst");
try {
        FolderInfo testFolder = pst.getRootFolder().getSubFolder("test");

        // Create the collection of message properties for adding or updating
        MapiPropertyCollection newProperties = new MapiPropertyCollection();

        // Normal property
        MapiProperty property = new MapiProperty(
                MapiPropertyTag.PR_ORG_EMAIL_ADDR_W,
                "test_address@org.com".getBytes("UTF-8"));

        // Custom named property
        MapiProperty namedProperty1 = new MapiNamedProperty(
                generateNamedPropertyTag((long)0, MapiPropertyType.PT_LONG),
                "ITEM_ID",
                UUID.randomUUID(),
                new byte[] {123, 0, 0, 0});

        // PidLidLogFlags named property
        MapiProperty namedProperty2 = new MapiNamedProperty(
                generateNamedPropertyTag((long)1, MapiPropertyType.PT_LONG),
                (long)0x0000870C,
                UUID.fromString("0006200A-0000-0000-C000-000000000046"),
                new byte[] {0, 0, 0, 0});

        newProperties.add(namedProperty1.getTag(), namedProperty1);
        newProperties.add(namedProperty2.getTag(), namedProperty2);
        newProperties.add(property.getTag(), property);

        testFolder.changeMessages(testFolder.enumerateMessagesEntryId(), newProperties);
} 
finally {
        pst.dispose();
} 
```

## Identify Embedded Message Attachment

This month’s release also enhances the Attachment class by providing the capability to identify attachment as embedded message. The _isEmbeddedMessage_ method returns true if the embedded attachment is another message file.

## Other Improvements

We have also fixed a number of bugs in this month’s release. This further brings stability to the API functionality and surety of the expected behavior in these cases.

## API Resources

We have detailed information available online for getting started with the Aspose.Email for Java API. These are:

*   [Product Documentation][2] – Provides detailed examples of working with the API
*   [API Reference Guide][3] – Details all the packages and classes of the API
*   [GitHub Examples][4] – Provides ready to run API examples
*   [Aspose.Email Forum][5] – Feel free to contact us on Aspose.Email forum for your queries




[1]: https://products.aspose.com/email/java
[2]: https://docs.aspose.com/email/java
[3]: http://www.aspose.com/api/java/email
[4]: https://github.com/aspose-email/Aspose.Email-for-Java
[5]: http://www.aspose.com/community/forums/aspose.email-product-family/188/showforum.aspx





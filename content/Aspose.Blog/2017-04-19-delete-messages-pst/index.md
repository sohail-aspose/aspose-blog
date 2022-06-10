---
title: 'Delete Messages Permanently from PST'
date: Wed, 19 Apr 2017 15:02:31 +0000
draft: false
url: /2017/04/19/delete-messages-pst/
author: Kashif Iqbal
summary: ''
tags: ['delete me', 'delete message from PST', 'message in PST']
categories: ['Aspose.Email Product Family']
---



{{< figure align=center src="images/aspose-Email-for-Java_100.png" alt="Delete messages from PST">}}


[Aspose.Email for Java 17.4.0][1] has been released. This month’s release provides the capability to permanently delete messages from Outlook PST file. It also supports new MAPI property in addition to the already set of supported properties. Other than these exciting new features, the API also fixes several bugs reported with the last version by our valued customers. For a complete list of what is new and fixed, please visit the [release notes][2] section of Aspose.Email for Java 17.4.0.

## **Permanently Delete Messages from PST**

This month’s release enhances the functionality of [deleting messages from PST][3] file such that deleted messages won’t be recoverable from the file anymore. In situations, where the PST file needs to be handed over to another party after extracting desired messages, this is helpful in the sense that deleted messages are no more recoverable by any forensic tool. There are no public API changes to incorporate this functionality in your applications and upgrading to this latest version will do the needful.

## **Support for PT\_FLOAT Mapi Property**

Aspose.Email is rich in features while working with Outlook MSG files. It's support for reading and setting wide range of MAPI properties for Outlook MSG file makes it favorite for manipulating such type of messages. This months’ release further enhances the capability of [working with MAPI properties][4] by providing support for a new property i.e. PT\_FLOAT. This further enriches the set of properties supported by the API. Following code illustrates how to set this property for a MSG file using Aspose.Email API.

```
float floatValue = 123.456F;
MapiMessage newMsg = new MapiMessage();
long floatTag = newMsg.getNamedPropertyMapping().getNextAvailablePropertyId(MapiPropertyType.PT\_FLOAT);
UUID guid = UUID.randomUUID();
MapiProperty newMapiProperty = new MapiProperty(floatTag, BitConverter.getBytesSingle(floatValue));
newMsg.getNamedPropertyMapping().addNamedPropertyMapping(newMapiProperty,(long) 12, guid);
newMsg.setProperty(newMapiProperty);

boolean propertyIsOk = false;
for (MapiNamedProperty prop : (Iterable) newMsg.getNamedProperties().getValues())
{
    if (prop.getGuid().equals(guid))
    {
        float val = prop.getFloat();
        propertyIsOk = val == floatValue;
    }
}
```

## Other Improvements

This month’s release also includes several bug fixes that were reported by our users with the previous release. Details about these can be found in the release notes section of this month’s release.

## API Resources

We have detailed information available online for getting started with the Aspose.Email for Java API. These are:

*   [Product Documentation][5] – Provides detailed examples of working with the API
*   [API Reference Guide][6] – Details all the packages and classes of the API
*   [GitHub Examples][7] – Provides ready to run API examples
*   [Aspose.Email Forum][8] – Feel free to contact us on Aspose.Email forum for your queries




[1]: http://www.aspose.com/downloads/email/java
[2]: https://docs.aspose.com/display/emailjava/Aspose.Email+for+Java+17.4.0+Release+Notes
[3]: https://docs.aspose.com/display/emailjava/Working+with+Messages+in+a+PST+File#WorkingwithMessagesinaPSTFile-DeleteMessagesfromPST
[4]: https://docs.aspose.com/display/emailjava/Working+with+MAPI+Properties#WorkingwithMAPIProperties-SetAdditionalProperties
[5]: https://docs.aspose.com/display/emailjava/Home
[6]: http://www.aspose.com/api/java/email
[7]: https://github.com/aspose-email/Aspose.Email-for-Java
[8]: https://forum.aspose.com/c/email





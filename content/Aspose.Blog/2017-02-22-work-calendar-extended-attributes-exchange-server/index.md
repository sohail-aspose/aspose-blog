---
title: 'Work with Calendar''s Extended Attributes on Exchange Server using Java'
date: Wed, 22 Feb 2017 17:28:36 +0000
draft: false
url: /2017/02/22/work-calendar-extended-attributes-exchange-server/
author: Kashif Iqbal
summary: ''
tags: []
categories: ['Aspose.Email Product Family']
---



{{< figure align=center src="images/aspose-Email-for-Java_100.png" alt="">}}


Aspose.Email for Java 17.2.0 is available for [download now][1]. This month’s release includes new features and enhancements. It also fixes a number of issues reported with the last version of the API. It also inherits the fixes from its equivalent .NET version. For a detailed list of what is new and fixed, please visit the [release notes section][2] of product documentation.

## Working with Extended Attributes on Exchange Server

This month’s release introduces the API’s capability to [retrieve extended attributes information for calendar items on the][3] Exchange server using the Exchange Web Service (EWS) client. This feature is limited to Calendar items only and support for other Exchange items such as Notes, Tasks, and Contacts is planned to be available in subsequent versions of the API. The availability of this new feature empowers the API to provide support of MAPI properties for Exchange server items.

## Total Number of Items from MBox File

This month’s release also provides support for getting total number of items from MBox storage files. This can help developers show progress of MBox file processing using the total count of items in such type of storage files.

## Improved Conversion of Messages to MHTML

We have enhanced the conversion of [messages to MHTML][4] in this month’s release. Specifically, this feature has been improved with the following two main changes.

*   Exclusion of public MhtFormatter class – use the MhtSaveOptions instead to specify the desired output format
*   Auto-rendering of message headers – uses message properties to determine which message headers to render to output MHTML

Earlier, you required to specify options to specify information such as email address and/or display name to output MHTML. This improvement makes you free of specifying these options and automatically renders the required fields to output MHTML.

## API Resources

We have detailed information available online for getting started with the Aspose.Email for Java API. These are:

*   [Product Documentation][5] – Provides detailed examples of working with the API
*   [API Reference Guide][6] – Details all the packages and classes of the API
*   [GitHub Examples][7] – Provides ready to run API examples
*   [Aspose.Email Forum][8] – Feel free to contact us on Aspose.Email forum for your queries




[1]: https://downloads.aspose.com/email/java
[2]: https://docs.aspose.com/display/emailjava/Aspose.Email+for+Java+17.2.0+Release+Notes
[3]: https://docs.aspose.com/email/java/working-with-calendar-items-on-exchange-server/#working-with-calendar-items-using-ews
[4]: https://docs.aspose.com/email/java/loading-and-saving-message/#rendering-calendar-events-while-converting-to-mhtml
[5]: https://docs.aspose.com/email/java/
[6]: https://apireference.aspose.com/email/java/
[7]: https://github.com/aspose-email/Aspose.Email-for-Java
[8]: https://forum.aspose.com/c/email





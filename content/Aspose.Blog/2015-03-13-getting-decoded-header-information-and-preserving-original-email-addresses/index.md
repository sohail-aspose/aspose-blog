---
title: 'Decode Header Information and Preserve Original Email Addresses with Aspose.Email for .NET 5.1.0'
date: Fri, 13 Mar 2015 16:05:51 +0000
draft: false
url: /2015/03/13/getting-decoded-header-information-and-preserving-original-email-addresses/
author: Muhammad Waqas
summary: ''
tags: ['Decode Email Header in Csharp', 'Get textual information from emails', 'Parse HTML Body of Email']
categories: ['Aspose.Email Product Family']
---



{{< figure align=center src="images/aspose-Email-for-net_100.png" alt="">}}


Aspose.Email for .NET 5.1.0 has been released. This month’s release includes a number of enhancements that improve the overall functionality and performance of the API. You can download this latest version from Aspose.Email’s [product download][1] page.

# Getting Textual Information from Message’s HTML Body

There might be cases where the message body is not correct due to any reason. In such cases, certain characters may not be returned properly while accessing the message body such as hyphens converted to “?”. When this is the case, getting the HTML contained information from the message’s HTML body is helpful. This month's release provides an enhancement where this information can be obtained in plain text format from the message’s Html body using the _HtmlBodyText_ property.

```
MailMessagemsg = MailMessage.Load(filename);
String textFromHtml = msg.HtmlBodyText;
```

# Getting Decoded Information from Message Headers

Message headers contain encoded information that is almost useless in the majority of the cases as these are accompanied by coded characters. If you want to get the decoded value of the header, you can use the latest version of Aspose.Email for .NET to achieve this. The HeaderCollection’s _GetDecodedValue_ method provides the decoded value of the encoded header as shown in the code sample below.

```
MailMessage msg = MailMessage.Load(filename);
String decodedValue = mail.Headers.GetDecodedValue(“Thread-Topic”);
```

# Preserving Original Email Address

It is often possible that the email address of a message may contain invalid characters such as a backslash (\\) character. Microsoft Exchange provides an Exchange service address format that is one example of such an address. In addition, it might be required to preserve such an email address while adding them to a Personal Storage (PST) file. Thus, it required the API to accommodate such invalid/malformed headers where necessary. In order to cater to this requirement, the MapiConversionOptions class now introduces a new property, named PreserveOriginalAddresses. If set to true, the address fields allow setting email addresses such as "a\\xasadf@xam.com”. You can have more information about the sample code by visiting our documentation article.

# Other Improvements

As can be seen from the product release notes, the API includes further improvements by fixing a number of functionality bugs and exceptions. These include, but not limited to:

*   Issues related to Exchange Web Service when creating voting buttons, loss of Notes information while fetch and save Outlook Contacts, and missing information while resolving contacts from Exchange server
*   Problems with message subject, message formatting and dynamic tags during mail merge
*   Issues related to PST such as message sender name visibility in PST preview pane, corrupted meeting body and reminder value, invalid Task body and exceptions while extracting messages
*   Other exceptions related to message conversion, parsing message headers and loading certain EML files.

In order to get further information about the API changes, please visit our documentation section, Public API changes in [Aspose.Email for .NET 5.1.0][2]. If you have any query about the API, please feel free to write to us on [Aspose.Email forum][3]. We shall be glad to answer your inquiries.




[1]: https://downloads.aspose.com/email/net
[2]: http://docs.aspose.com/display/emailnet/Public+API+Changes+in+Aspose.Email+5.1.0
[3]: http://forum.aspose.com





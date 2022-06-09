---
title: 'Get Contacts List from Microsoft Exchange Server in Java'
seoTitle: "Get Contacts List from Microsoft Exchange Server in Java | Java API"
description: "Get contacts list from Microsoft Exchange Server programmatically in Java. Retrieve a particular contact from MS Exchange Server using ID."
date: Mon, 28 Feb 2022 05:55:00 +0000
draft: false
url: /2022/02/28/get-contacts-list-from-ms-exchange-server-in-java/
author: Usman Aziz
summary: 'While working with [Microsoft Exchange Server][1] programmatically, you may need to access the contacts from it. For example, to export the contacts, manipulate them, or use them for other purposes. In this article, you will learn **how to get the contacts list from Microsoft Exchange Server in Java**.'
tags: ['Get Contacts List from MS Exchange Server in Java', 'Get a Contact using ID from Exchanger Server in Java', 'Java API to Retrieve Contacts from MS Exchange Server']
categories: ['Aspose.Email Product Family']
---



{{< figure align=center src="images/aspose-email-exchange.png" alt="Get Contacts List from Microsoft Exchange Server in Java">}}


While working with [Microsoft Exchange Server][2] programmatically, you may need to access the contacts from it. For example, to export the contacts, manipulate them, or use them for other purposes. In this article, you will learn **how to get the contacts list from Microsoft Exchange Server in Java**.

*   [API to Retrieve Contacts from MS Exchange Server][3]
*   [Get Contacts List from MS Exchange Server][4]
*   [Get a Contact using ID][5]

## Java API to Get Contacts List from MS Exchange Server {#API-to-Access-Contacts-on-Exchange-Server}

To retrieve the contacts, we will use [Aspose.Email for Java][6]. The API is designed to implement the email clients from within the Java applications. It also lets you connect to MS Exchange Server and perform various operations programmatically. You can either [download][7] the API's JAR or install it from Maven using the following Maven configurations.

```
**Repository:**
<repository>
    <id>AsposeJavaAPI</id>
    <name>Aspose Java API</name>
    <url>http://repository.aspose.com/repo/</url>
</repository>

**Dependency:**
<dependency>
    <groupId>com.aspose</groupId>
    <artifactId>aspose-email</artifactId>
    <version>22.2</version>
    <classifier>jdk16</classifier>
</dependency>
```

## Retrieve Contacts List from MS Exchange Server in Java {#Get-Contacts-List-from-MS-Exchange-Server}

The following are the steps to get the contacts list from Microsoft Exchange Server in Java.

*   First, initialize [IEWSClient][8] object using username, password, domain, and mailbox URI.
*   Then, call [IEWSClient.getContacts(EWSClient.getMailboxInfo().getContactsUri())][9] method to get contacts in an array.
*   Loop through each contact in array and fetch its details.

The following code sample shows how to retrieve the contacts from Microsoft Exchange Server.

{{< gist aspose-com-gists 5b337b0a4efe8fe90f471f6063f489a4 "get-contacts-list.java" >}}

## Get a Contact from MS Exchange Server by ID {#Get-a-Contact-using-ID}

You can also retrieve a contact from MS Exchange Server using its ID. The following are the steps to perform this operation.

*   First, initialize [IEWSClient][10] object using username, password, domain, and mailbox URI.
*   Then, call [IEWSClient.getContact(String)][11] method and get contact in a [Contact][12] object.
*   Use or manipulate the contact as required.

The following code sample shows how to retrieve a particular contact from Microsoft Exchange Server in Java.

{{< gist aspose-com-gists 5b337b0a4efe8fe90f471f6063f489a4 "get-contact.java" >}}

## Get a Free API License {#Get-a-Free-API-License}

Get a [free temporary license][13] and use Aspose.Email for Java without evaluation limitations.

## Conclusion

In this article, you have learned how to get the contacts list from Microsoft Exchange Server in Java. Furthermore, you have seen how to retrieve a contact by its ID programmatically. In addition to that, you can read more about Aspose.Email for Java using the [documentation][14]. Also, in case you would have any questions, you can post to our [forum][15].

## See Also

*   [Read Emails from MS Exchange Server in Java][16]




[1]: https://en.wikipedia.org/wiki/Microsoft_Exchange_Server
[2]: https://en.wikipedia.org/wiki/Microsoft_Exchange_Server
[3]: #API-to-Access-Contacts-on-Exchange-Server
[4]: #Get-Contacts-List-from-MS-Exchange-Server
[5]: #Get-a-Contact-using-ID
[6]: https://products.aspose.com/email/java/
[7]: https://downloads.aspose.com/email/java/
[8]: https://apireference.aspose.com/email/java/com.aspose.email/IEWSClient
[9]: https://apireference.aspose.com/email/java/com.aspose.email/IEWSClient#getContacts(java.lang.String)
[10]: https://apireference.aspose.com/email/java/com.aspose.email/IEWSClient
[11]: https://apireference.aspose.com/email/java/com.aspose.email/IEWSClient#getContact(java.lang.String)
[12]: https://apireference.aspose.com/email/java/com.aspose.email/Contact
[13]: https://purchase.aspose.com/temporary-license
[14]: https://docs.aspose.com/email/java/
[15]: https://forum.aspose.com/
[16]: https://blog.aspose.com/2021/03/22/read-emails-from-ms-exchange-server-using-java/





---
title: 'Add and Remove Members in MS Exchange Distribution Lists in Java'
seoTitle: "Java Add and Remove Members in MS Exchange Distribution List | EWS"
description: "Use Java EWS API to work with members in MS Exchange distribution list in Java. Add or remove members from distribution lists programmatically."
date: Mon, 07 Mar 2022 09:57:00 +0000
draft: false
url: /2022/03/07/manage-members-in-exchange-distribution-lists-in-java/
author: Usman Aziz
summary: '[MS Exchange Server][1] allows you to create distribution lists to send emails to a group of people. In the [previous article][2], we have covered how to create or fetch Exchange distribution lists in Java. In this article, you will learn **how to add or remove members in MS Exchange distribution lists in Java**.'
tags: ['Add Members to MS Exchange Distribution Lists Java', 'Java API to Manage Members of Exchange Distribution Lists', 'Java EWS API', 'Remove Members from MS Exchange Distribution Lists Java']
categories: ['Aspose.Email Product Family']
---



{{< figure align=center src="images/aspose-email-exchange.png" alt="Add and Remove Members in MS Exchange Distribution Lists in Java">}}


[MS Exchange Server][3] allows you to create distribution lists to send emails to a group of people. In the [previous article][4], we have covered how to create or fetch Exchange distribution lists in Java. In this article, you will learn **how to add or remove members in MS Exchange distribution lists in Java**.

*   [Java API to Manage Members of Exchange Distribution Lists][5]
*   [Add Members to MS Exchange Distribution Lists][6]
*   [Remove Members from MS Exchange Distribution Lists][7]

## Java API to Manage Members of Exchange Distribution Lists {#API-to-Manage-Members-of-Exchange-Distribution-Lists}

To work with members of distribution lists on MS Exchange Server, we will use [Aspose.Email for Java][8]. It is a powerful API that allows you to work with MS Exchange Server seamlessly. You can either [download][9] the API or install it using the following Maven configurations.

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
    <version>22.3</version>
    <classifier>jdk16</classifier>
</dependency>
```

## Add Members to MS Exchange Distribution Lists in Java {#Add-Members-to-MS-Exchange-Distribution-Lists}

The following are the steps to add members to MS Exchange distribution list in Java.

*   First, connect to Exchange Server and get the instance of the EWS client into an [IEWSClient][10] object.
*   Then, get distribution lists into an [ExchangeDistributionList][11] array using [IEWSClient.listDistributionLists()][12] method.
*   After that, create an instance of [MailAddressCollection][13] class and add members to the collection.
*   Finally, add members to the specific distribution list using [IEWSClient.addToDistributionList(ExchangeDistributionList, MailAddressCollection)][14] method.

The following code sample shows how to add members to an Exchange distribution list in Java.

{{< gist aspose-com-gists 32ba9a85096bf605d5f239a882cf057b "add-members-to-list.java" >}}

## Remove Members from MS Exchange Distribution Lists in Java {#Remove-Members-from-MS-Exchange-Distribution-Lists}

The following are the steps to remove members from MS Exchange distribution list using Java.

*   First, connect to Exchange Server and get the instance of the EWS client into an [IEWSClient][15] object.
*   Then, get distribution lists into an [ExchangeDistributionList][16] array using [IEWSClient.listDistributionLists()][17] method.
*   After that, get the reference of a particular list using [IEWSClient.fetchDistributionList(ExchangeDistributionList)][18] method.
*   Then, create an instance of [MailAddressCollection][19] class and add members to be deleted.
*   Finally, delete members from distribution list using [IEWSClient.deleteFromDistributionList(ExchangeDistributionList, MailAddressCollection)][20] method.

The following code sample shows how to delete members from Exchange distribution lists in Java.

{{< gist aspose-com-gists 32ba9a85096bf605d5f239a882cf057b "remove-members-from-list.java" >}}

## Get a Free API License {#Get-a-Free-API-License}

You can get a [free temporary license][21] to use Aspose.Email for Java without evaluation limitations.

## Conclusion

In this article, we have covered how to manipulate members in MS Exchange distribution lists programmatically. With the help of code samples, you have seen how to add or remove members from an Exchange distribution list in Java. Alongside, you can explore the [documentation][22] to read more about Aspose.Email for Java. Also, you can ask your questions via our [forum][23].

## See Also

*   [Read Emails from MS Exchange Server in Java][24]




[1]: https://en.wikipedia.org/wiki/Microsoft_Exchange_Server
[2]: https://blog.aspose.com/2022/04/07/create-exchange-distribution-list-in-java/
[3]: https://en.wikipedia.org/wiki/Microsoft_Exchange_Server
[4]: https://blog.aspose.com/2022/04/07/create-exchange-distribution-list-in-java/
[5]: #API-to-Manage-Members-of-Exchange-Distribution-Lists
[6]: #Add-Members-to-MS-Exchange-Distribution-Lists
[7]: #Remove-Members-from-MS-Exchange-Distribution-Lists
[8]: https://products.aspose.com/email/java/
[9]: https://downloads.aspose.com/email/java/
[10]: https://apireference.aspose.com/email/java/com.aspose.email/IEWSClient
[11]: https://apireference.aspose.com/email/java/com.aspose.email/ExchangeDistributionList
[12]: https://apireference.aspose.com/email/java/com.aspose.email/IEWSClient#listDistributionLists()
[13]: https://apireference.aspose.com/email/java/com.aspose.email/MailAddressCollection
[14]: https://apireference.aspose.com/email/java/com.aspose.email/IEWSClient#addToDistributionList(com.aspose.email.ExchangeDistributionList,%20com.aspose.email.MailAddressCollection)
[15]: https://apireference.aspose.com/email/java/com.aspose.email/IEWSClient
[16]: https://apireference.aspose.com/email/java/com.aspose.email/ExchangeDistributionList
[17]: https://apireference.aspose.com/email/java/com.aspose.email/IEWSClient#listDistributionLists()
[18]: https://apireference.aspose.com/email/java/com.aspose.email/IEWSClient#fetchDistributionList(com.aspose.email.ExchangeDistributionList)
[19]: https://apireference.aspose.com/email/java/com.aspose.email/MailAddressCollection
[20]: https://apireference.aspose.com/email/java/com.aspose.email/IEWSClient#deleteFromDistributionList(com.aspose.email.ExchangeDistributionList,%20com.aspose.email.MailAddressCollection)
[21]: https://purchase.aspose.com/temporary-license
[22]: https://docs.aspose.com/email/java/
[23]: https://forum.aspose.com/
[24]: https://blog.aspose.com/2021/03/22/read-emails-from-ms-exchange-server-using-java/





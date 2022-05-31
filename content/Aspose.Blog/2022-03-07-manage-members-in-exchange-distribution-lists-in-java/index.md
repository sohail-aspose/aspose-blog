---
title: 'Add and Remove Members in MS Exchange Distribution Lists in Java'
date: Mon, 07 Mar 2022 09:57:00 +0000
draft: false
url: /2022/03/07/manage-members-in-exchange-distribution-lists-in-java/
author: 'Usman Aziz'
summary: '[MS Exchange Server](https://en.wikipedia.org/wiki/Microsoft_Exchange_Server) allows you to create distribution lists to send emails to a group of people. In the [previous article](https://blog.aspose.com/2022/04/07/create-exchange-distribution-list-in-java/), we have covered how to create or fetch Exchange distribution lists in Java. In this article, you will learn **how to add or remove members in MS Exchange distribution lists in Java**.'
tags: ['Add Members to MS Exchange Distribution Lists Java', 'Java API to Manage Members of Exchange Distribution Lists', 'Java EWS API', 'Remove Members from MS Exchange Distribution Lists Java']
categories: ['Aspose.Email Product Family']
---



{{< figure align=center src="images/aspose-email-exchange.png" alt="Add and Remove Members in MS Exchange Distribution Lists in Java">}}


[MS Exchange Server](https://en.wikipedia.org/wiki/Microsoft_Exchange_Server) allows you to create distribution lists to send emails to a group of people. In the [previous article](https://blog.aspose.com/2022/04/07/create-exchange-distribution-list-in-java/), we have covered how to create or fetch Exchange distribution lists in Java. In this article, you will learn **how to add or remove members in MS Exchange distribution lists in Java**.

*   [Java API to Manage Members of Exchange Distribution Lists](#API-to-Manage-Members-of-Exchange-Distribution-Lists)
*   [Add Members to MS Exchange Distribution Lists](#Add-Members-to-MS-Exchange-Distribution-Lists)
*   [Remove Members from MS Exchange Distribution Lists](#Remove-Members-from-MS-Exchange-Distribution-Lists)

## Java API to Manage Members of Exchange Distribution Lists {#API-to-Manage-Members-of-Exchange-Distribution-Lists}

To work with members of distribution lists on MS Exchange Server, we will use [Aspose.Email for Java](https://products.aspose.com/email/java/). It is a powerful API that allows you to work with MS Exchange Server seamlessly. You can either [download](https://downloads.aspose.com/email/java/) the API or install it using the following Maven configurations.

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

*   First, connect to Exchange Server and get the instance of the EWS client into an [IEWSClient](https://apireference.aspose.com/email/java/com.aspose.email/IEWSClient) object.
*   Then, get distribution lists into an [ExchangeDistributionList](https://apireference.aspose.com/email/java/com.aspose.email/ExchangeDistributionList) array using [IEWSClient.listDistributionLists()](https://apireference.aspose.com/email/java/com.aspose.email/IEWSClient#listDistributionLists()) method.
*   After that, create an instance of [MailAddressCollection](https://apireference.aspose.com/email/java/com.aspose.email/MailAddressCollection) class and add members to the collection.
*   Finally, add members to the specific distribution list using [IEWSClient.addToDistributionList(ExchangeDistributionList, MailAddressCollection)](https://apireference.aspose.com/email/java/com.aspose.email/IEWSClient#addToDistributionList(com.aspose.email.ExchangeDistributionList,%20com.aspose.email.MailAddressCollection)) method.

The following code sample shows how to add members to an Exchange distribution list in Java.

{{< gist aspose-com-gists 32ba9a85096bf605d5f239a882cf057b "add-members-to-list.java" >}}

## Remove Members from MS Exchange Distribution Lists in Java {#Remove-Members-from-MS-Exchange-Distribution-Lists}

The following are the steps to remove members from MS Exchange distribution list using Java.

*   First, connect to Exchange Server and get the instance of the EWS client into an [IEWSClient](https://apireference.aspose.com/email/java/com.aspose.email/IEWSClient) object.
*   Then, get distribution lists into an [ExchangeDistributionList](https://apireference.aspose.com/email/java/com.aspose.email/ExchangeDistributionList) array using [IEWSClient.listDistributionLists()](https://apireference.aspose.com/email/java/com.aspose.email/IEWSClient#listDistributionLists()) method.
*   After that, get the reference of a particular list using [IEWSClient.fetchDistributionList(ExchangeDistributionList)](https://apireference.aspose.com/email/java/com.aspose.email/IEWSClient#fetchDistributionList(com.aspose.email.ExchangeDistributionList)) method.
*   Then, create an instance of [MailAddressCollection](https://apireference.aspose.com/email/java/com.aspose.email/MailAddressCollection) class and add members to be deleted.
*   Finally, delete members from distribution list using [IEWSClient.deleteFromDistributionList(ExchangeDistributionList, MailAddressCollection)](https://apireference.aspose.com/email/java/com.aspose.email/IEWSClient#deleteFromDistributionList(com.aspose.email.ExchangeDistributionList,%20com.aspose.email.MailAddressCollection)) method.

The following code sample shows how to delete members from Exchange distribution lists in Java.

{{< gist aspose-com-gists 32ba9a85096bf605d5f239a882cf057b "remove-members-from-list.java" >}}

## Get a Free API License {#Get-a-Free-API-License}

You can get a [free temporary license](https://purchase.aspose.com/temporary-license) to use Aspose.Email for Java without evaluation limitations.

## Conclusion

In this article, we have covered how to manipulate members in MS Exchange distribution lists programmatically. With the help of code samples, you have seen how to add or remove members from an Exchange distribution list in Java. Alongside, you can explore the [documentation](https://docs.aspose.com/email/java/) to read more about Aspose.Email for Java. Also, you can ask your questions via our [forum](https://forum.aspose.com/).

## See Also

*   [Read Emails from MS Exchange Server in Java](https://blog.aspose.com/2021/03/22/read-emails-from-ms-exchange-server-using-java/)





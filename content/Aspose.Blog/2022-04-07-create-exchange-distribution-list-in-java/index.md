---
title: 'Create Exchange Distribution List in Java'
date: Thu, 07 Apr 2022 09:46:37 +0000
draft: false
url: /2022/04/07/create-exchange-distribution-list-in-java/
author: 'Usman Aziz'
summary: '[MS Exchange Server][1] allows you to create email distribution lists that can be used to send emails to a group of people without entering individual email addresses. To create such lists programmatically, this article covers **how to create a distribution list on MS Exchange Server in Java**. Furthermore, it shows how to fetch a distribution list programmatically.'
tags: ['Create an MS Exchange Distribution List in Java', 'Fetch a Distribution List from MS Exchange Server in Java', 'Java API to Create Distribution List on MS Exchange Server']
categories: ['Aspose.Email Product Family']
---



{{< figure align=center src="images/aspose-email-exchange.png" alt="Create Exchange Distribution List in Java">}}


[MS Exchange Server][2] allows you to create email distribution lists that can be used to send emails to a group of people without entering individual email addresses. To create such lists programmatically, this article covers **how to create a distribution list on MS Exchange Server in Java**. Furthermore, it shows how to fetch a distribution list programmatically.

*   [API to Create Distribution List on MS Exchange Server][3]
*   [Create an MS Exchange Distribution List][4]
*   [Fetch a Distribution List from MS Exchange Server][5]

## Java API to Create Distribution List on MS Exchange Server {#API-to-Create-Distribution-List-on-MS-Exchange-Server}

To create the distribution lists on MS Exchange Server, we will use [Aspose.Email for Java][6]. The API is designed to create, send, and process emails from within Java applications. Alongside, it supports working with MS Outlook and Exchange Server without writing complex code. You can either [download][7] the API or install it using the following Maven configurations.

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

## Create an MS Exchange Distribution List in Java {#Create-an-MS-Exchange-Distribution-List}

The following are the steps to create a distribution list on MS Exchange Server in Java.

*   First, connect to Exchange Server and get the instance of the EWS client into an [IEWSClient][8] object.
*   After that, create an instance of [ExchangeDistributionList][9] class.
*   Set display name of list using [ExchangeDistributionList.setDisplayName()][10] method.
*   Create an instance of [MailAddressCollection][11] class and add members to the collection.
*   Finally, create distribution list using [IEWSClient.createDistributionList(ExchangeDistributionList, MailAddressCollection)][12] method.

The following code sample shows how to create an MS Exchange distribution list in Java.

{{< gist aspose-com-gists 04e417c8cb38ba69570b164e89b1bbe5 "create-distribution-list.java" >}}

## Fetch a Distribution List from MS Exchange Server in Java {#Fetch-a-Distribution-List-from-MS-Exchange-Server}

Now, let's see how to fetch a distribution list from MS Exchange Server programmatically in Java.

*   First, connect to Exchange Server and get the instance of the EWS client into an [IEWSClient][13] object.
*   After that, get distribution list into an [ExchangeDistributionList][14] array using [IEWSClient.listDistributionLists()][15] method.
*   Loop through each distribution list in the array.
*   Finally, use [IEWSClient.fetchDistributionList(ExchangeDistributionList)][16] method to fetch the members of the distribution list.

The following code sample shows how to fetch distribution lists from MS Exchange Server in Java.

{{< gist aspose-com-gists 04e417c8cb38ba69570b164e89b1bbe5 "fetch-distribution-list.java" >}}

## Get a Free API License {#Get-a-Free-API-License}

You can get a [free temporary license][17] to use Aspose.Email for Java without evaluation limitations.

## Conclusion

In this article, you have learned how to create distribution lists on MS Exchange Server in Java. Furthermore, you have seen how to fetch MS Exchange distribution lists programmatically. In addition, you can explore the [documentation][18] to read more about Aspose.Email for Java. Also, you can post your queries to our [forum][19].

## See Also

*   [Read Emails from MS Exchange Server in Java][20]




[1]: https://en.wikipedia.org/wiki/Microsoft_Exchange_Server
[2]: https://en.wikipedia.org/wiki/Microsoft_Exchange_Server
[3]: #API-to-Create-Distribution-List-on-MS-Exchange-Server
[4]: #Create-an-MS-Exchange-Distribution-List
[5]: #Fetch-a-Distribution-List-from-MS-Exchange-Server
[6]: https://products.aspose.com/email/java/
[7]: https://downloads.aspose.com/email/java/
[8]: https://apireference.aspose.com/email/java/com.aspose.email/IEWSClient
[9]: https://apireference.aspose.com/email/java/com.aspose.email/ExchangeDistributionList
[10]: https://apireference.aspose.com/email/java/com.aspose.email/ExchangeDistributionList#setDisplayName(java.lang.String)
[11]: https://apireference.aspose.com/email/java/com.aspose.email/MailAddressCollection
[12]: https://apireference.aspose.com/email/java/com.aspose.email/IEWSClient#createDistributionList(com.aspose.email.ExchangeDistributionList,%20com.aspose.email.MailAddressCollection)
[13]: https://apireference.aspose.com/email/java/com.aspose.email/IEWSClient
[14]: https://apireference.aspose.com/email/java/com.aspose.email/ExchangeDistributionList
[15]: https://apireference.aspose.com/email/java/com.aspose.email/IEWSClient#listDistributionLists()
[16]: https://apireference.aspose.com/email/java/com.aspose.email/IEWSClient#fetchDistributionList(com.aspose.email.ExchangeDistributionList)
[17]: https://purchase.aspose.com/temporary-license
[18]: https://docs.aspose.com/email/java/
[19]: https://forum.aspose.com/
[20]: https://blog.aspose.com/2021/03/22/read-emails-from-ms-exchange-server-using-java/





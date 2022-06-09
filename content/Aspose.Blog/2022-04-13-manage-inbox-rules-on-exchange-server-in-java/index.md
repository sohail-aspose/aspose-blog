---
title: 'Manage Inbox Rules on Exchange Server in Java'
seoTitle: "Java Create and Update Inbox Rules with EWS on Exchange Server"
description: "Use Java EWS API to manage inbox rules on Exchange Server using Java. Create and update inbox rules with EWS on Exchange Server programmatically."
date: Wed, 13 Apr 2022 06:22:00 +0000
draft: false
url: /2022/04/13/manage-inbox-rules-on-exchange-server-in-java/
author: Usman Aziz
summary: 'While using [Microsoft Exchange Server][1] services, you may need to define different rules for the inbox folder. These rules are applied to the messages such as moving a message to a folder, deleting a message, etc. An inbox rule is comprised of conditions and the actions to be performed when the conditions are met. In this article, you will learn **how to create and update inbox rules on MS Exchange Server in Java**.'
tags: ['Create Inbox Rules on Exchange Server in Java', 'Java API to Manage Inbox Rules on Exchange Server', 'Java EWS API', 'Update Inbox Rules on Exchange Server in Java']
categories: ['Aspose.Email Product Family']
---



{{< figure align=center src="images/aspose-email-exchange.png" alt="Manage Inbox Rules on Exchange Server in Java">}}


While using [Microsoft Exchange Server][2]'s services, you may need to define different rules for the inbox folder. These rules are applied to the messages such as moving a message to a folder, deleting a message, etc. An inbox rule is comprised of conditions and the actions to be performed when the conditions are met. In this article, you will learn **how to create and update inbox rules on MS Exchange Server in Java**.

*   [API to Manage Inbox Rules on Exchange Server][3]
*   [Create Inbox Rules on Exchange Server][4]
*   [Update Inbox Rules on Exchange Server][5]

## Java API to Manage Inbox Rules on Exchange Server {#API-to-Manage-Inbox-Rules-on-Exchange-Server}

To work with inbox rules on MS Exchange Server, we will use [Aspose.Email for Java][6]. The API is designed to seamlessly work with MS Exchange Server and manage its services. You can either [download][7] the API or install it using the following Maven configurations.

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

## Create an Inbox Rule on Exchange Server in Java {#Create-Inbox-Rules-on-Exchange-Server}

Aspose.Email for Java uses Exchange Web Services (EWS) to work with inbox rules on Exchange Server. The following are the steps to create an inbox rule on Exchange Server in Java.

*   First, connect to Exchange Server and get the instance of the EWS client into an [IEWSClient][8] object.
*   Then, create an object of [InboxRule][9] class.
*   Set rule's name using [InboxRule.setDisplayName()][10] method.
*   Create an instance of [RulePredicates][11] class and specify the conditions.
*   Assign _RulePredicates_ instance using [InboxRule.setConditions()][12] method.
*   Create an instance of [RuleActions][13] class and set actions.
*   Assign _RuleAction_ instance using [InboxRule.setActions()][14] method.
*   Finally, call [IEWSClient.createInboxRule(InboxRule)][15] to create the rule.

The following code sample shows how to create an inbox rule on Exchange Server in Java.

{{< gist aspose-com-gists 654fcbd7a3342d45b4c993acc50ff036 "create-inbox-rule.java" >}}

## Update an Inbox Rule on Exchange Server in Java {#Update-Inbox-Rules-on-Exchange-Server}

The following are the steps to fetch and update an existing inbox rule on Exchange Server in Java.

*   First, connect to Exchange Server and get the instance of the EWS client into an [IEWSClient][16] object.
*   Then, call the [IEWSClient.getInboxRules()][17] method to get all the rules in an [InboxRule][18] array.
*   Loop through each _InboxRule_ in the array.
*   Filter the required rules based on some conditions.
*   Update the rule's conditions or actions.
*   Finally, call [IEWSClient.updateInboxRule(InboxRule)][19] method to update the inbox rule.

The following code sample shows how to update an inbox rule on MS Exchange Server in Java.

{{< gist aspose-com-gists 654fcbd7a3342d45b4c993acc50ff036 "update-inbox-rule.java" >}}

## Get a Free API License {#Get-a-Free-API-License}

You can get a [free temporary license][20] to use Aspose.Email for Java without evaluation limitations.

## Conclusion

In this article, you have learned how to work with inbox rules on Microsoft Exchange Server from within Java applications. You have seen how to add or update an inbox rule on Exchange Server in Java. In addition, you can explore the features of Aspose.Email for Java using the [documentation][21]. Also, in case you would have any questions, you can post to our [forum][22].

## See Also

*   [Read Emails from MS Exchange Server in Java][23]




[1]: https://en.wikipedia.org/wiki/Microsoft_Exchange_Server
[2]: https://en.wikipedia.org/wiki/Microsoft_Exchange_Server
[3]: #API-to-Manage-Inbox-Rules-on-Exchange-Server
[4]: #Create-Inbox-Rules-on-Exchange-Server
[5]: #Update-Inbox-Rules-on-Exchange-Server
[6]: https://products.aspose.com/email/java/
[7]: https://downloads.aspose.com/email/java/
[8]: https://apireference.aspose.com/email/java/com.aspose.email/IEWSClient
[9]: https://apireference.aspose.com/email/java/com.aspose.email/InboxRule
[10]: https://apireference.aspose.com/email/java/com.aspose.email/InboxRule#setDisplayName(java.lang.String)
[11]: https://apireference.aspose.com/email/java/com.aspose.email/RulePredicates
[12]: https://apireference.aspose.com/email/java/com.aspose.email/InboxRule#setConditions(com.aspose.email.RulePredicates)
[13]: https://apireference.aspose.com/email/java/com.aspose.email/RuleActions
[14]: https://apireference.aspose.com/email/java/com.aspose.email/InboxRule#setActions(com.aspose.email.RuleActions)
[15]: https://apireference.aspose.com/email/java/com.aspose.email/IEWSClient#createInboxRule(com.aspose.email.InboxRule)
[16]: https://apireference.aspose.com/email/java/com.aspose.email/IEWSClient
[17]: https://apireference.aspose.com/email/java/com.aspose.email/IEWSClient#getInboxRules()
[18]: https://apireference.aspose.com/email/java/com.aspose.email/InboxRule
[19]: https://apireference.aspose.com/email/java/com.aspose.email/IEWSClient#updateInboxRule(com.aspose.email.InboxRule)
[20]: https://purchase.aspose.com/temporary-license
[21]: https://docs.aspose.com/email/java/
[22]: https://forum.aspose.com/
[23]: https://blog.aspose.com/2021/03/22/read-emails-from-ms-exchange-server-using-java/





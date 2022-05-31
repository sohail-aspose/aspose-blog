---
title: 'Manage Inbox Rules on Exchange Server in Java'
date: Wed, 13 Apr 2022 06:22:00 +0000
draft: false
url: /2022/04/13/manage-inbox-rules-on-exchange-server-in-java/
author: 'Usman Aziz'
summary: 'While using [Microsoft Exchange Server](https://en.wikipedia.org/wiki/Microsoft_Exchange_Server) services, you may need to define different rules for the inbox folder. These rules are applied to the messages such as moving a message to a folder, deleting a message, etc. An inbox rule is comprised of conditions and the actions to be performed when the conditions are met. In this article, you will learn **how to create and update inbox rules on MS Exchange Server in Java**.'
tags: ['Create Inbox Rules on Exchange Server in Java', 'Java API to Manage Inbox Rules on Exchange Server', 'Java EWS API', 'Update Inbox Rules on Exchange Server in Java']
categories: ['Aspose.Email Product Family']
---



{{< figure align=center src="images/aspose-email-exchange.png" alt="Manage Inbox Rules on Exchange Server in Java">}}


While using [Microsoft Exchange Server](https://en.wikipedia.org/wiki/Microsoft_Exchange_Server)'s services, you may need to define different rules for the inbox folder. These rules are applied to the messages such as moving a message to a folder, deleting a message, etc. An inbox rule is comprised of conditions and the actions to be performed when the conditions are met. In this article, you will learn **how to create and update inbox rules on MS Exchange Server in Java**.

*   [API to Manage Inbox Rules on Exchange Server](#API-to-Manage-Inbox-Rules-on-Exchange-Server)
*   [Create Inbox Rules on Exchange Server](#Create-Inbox-Rules-on-Exchange-Server)
*   [Update Inbox Rules on Exchange Server](#Update-Inbox-Rules-on-Exchange-Server)

## Java API to Manage Inbox Rules on Exchange Server {#API-to-Manage-Inbox-Rules-on-Exchange-Server}

To work with inbox rules on MS Exchange Server, we will use [Aspose.Email for Java](https://products.aspose.com/email/java/). The API is designed to seamlessly work with MS Exchange Server and manage its services. You can either [download](https://downloads.aspose.com/email/java/) the API or install it using the following Maven configurations.

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

*   First, connect to Exchange Server and get the instance of the EWS client into an [IEWSClient](https://apireference.aspose.com/email/java/com.aspose.email/IEWSClient) object.
*   Then, create an object of [InboxRule](https://apireference.aspose.com/email/java/com.aspose.email/InboxRule) class.
*   Set rule's name using [InboxRule.setDisplayName()](https://apireference.aspose.com/email/java/com.aspose.email/InboxRule#setDisplayName(java.lang.String)) method.
*   Create an instance of [RulePredicates](https://apireference.aspose.com/email/java/com.aspose.email/RulePredicates) class and specify the conditions.
*   Assign _RulePredicates_ instance using [InboxRule.setConditions()](https://apireference.aspose.com/email/java/com.aspose.email/InboxRule#setConditions(com.aspose.email.RulePredicates)) method.
*   Create an instance of [RuleActions](https://apireference.aspose.com/email/java/com.aspose.email/RuleActions) class and set actions.
*   Assign _RuleAction_ instance using [InboxRule.setActions()](https://apireference.aspose.com/email/java/com.aspose.email/InboxRule#setActions(com.aspose.email.RuleActions)) method.
*   Finally, call [IEWSClient.createInboxRule(InboxRule)](https://apireference.aspose.com/email/java/com.aspose.email/IEWSClient#createInboxRule(com.aspose.email.InboxRule)) to create the rule.

The following code sample shows how to create an inbox rule on Exchange Server in Java.

\[gist id="654fcbd7a3342d45b4c993acc50ff036" file="create-inbox-rule.java"\]

## Update an Inbox Rule on Exchange Server in Java {#Update-Inbox-Rules-on-Exchange-Server}

The following are the steps to fetch and update an existing inbox rule on Exchange Server in Java.

*   First, connect to Exchange Server and get the instance of the EWS client into an [IEWSClient](https://apireference.aspose.com/email/java/com.aspose.email/IEWSClient) object.
*   Then, call the [IEWSClient.getInboxRules()](https://apireference.aspose.com/email/java/com.aspose.email/IEWSClient#getInboxRules()) method to get all the rules in an [InboxRule](https://apireference.aspose.com/email/java/com.aspose.email/InboxRule) array.
*   Loop through each _InboxRule_ in the array.
*   Filter the required rules based on some conditions.
*   Update the rule's conditions or actions.
*   Finally, call [IEWSClient.updateInboxRule(InboxRule)](https://apireference.aspose.com/email/java/com.aspose.email/IEWSClient#updateInboxRule(com.aspose.email.InboxRule)) method to update the inbox rule.

The following code sample shows how to update an inbox rule on MS Exchange Server in Java.

\[gist id="654fcbd7a3342d45b4c993acc50ff036" file="update-inbox-rule.java"\]

## Get a Free API License {#Get-a-Free-API-License}

You can get a [free temporary license](https://purchase.aspose.com/temporary-license) to use Aspose.Email for Java without evaluation limitations.

## Conclusion

In this article, you have learned how to work with inbox rules on Microsoft Exchange Server from within Java applications. You have seen how to add or update an inbox rule on Exchange Server in Java. In addition, you can explore the features of Aspose.Email for Java using the [documentation](https://docs.aspose.com/email/java/). Also, in case you would have any questions, you can post to our [forum](https://forum.aspose.com/).

## See Also

*   [Read Emails from MS Exchange Server in Java](https://blog.aspose.com/2021/03/22/read-emails-from-ms-exchange-server-using-java/)




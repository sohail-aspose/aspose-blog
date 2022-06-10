---
title: 'Aspose.Email for Java 6.0.0 supports Working with Distribution Lists on Exchange Server'
date: Tue, 15 Dec 2015 15:03:00 +0000
draft: false
url: /2015/12/15/aspose.email-for-java-6.0.0-supports-working-with-distribution-lists-on-exchange-server/
author: Kashif Iqbal
summary: ''
tags: []
categories: ['Aspose.Email Product Family']
---

![](https://blog.aspose.com/wp-content/uploads/sites/2/2015/12/aspose-Email-for-Java_100.png "aspose-Email-for-Java_100")

We are pleased to announce the release of [Aspose.Email for Java 6.0.0][1]. This month’s release includes the same new features, enhancements and bug fixes that were part of its equivalent .NET version i.e. Aspose.Email for .NET 6.0.0. It includes improvements to the Exchange Server API, CPU utilization and the Outlook MSG type. A detailed list of changes can be found in our API documentation section, Public API Changes in Aspsoe.Email API.

# New Features

**Support for Distribution Lists on Exchange Server:** Distribution lists are one of the key features provided by Microsoft Exchange Server where users can define groups having contacts of interest. Email address can be defined for this group and messages can be sent to the group, thus reaching all the members of the group.

This month’s release of Aspose.Email for Java introduces the new feature of working with Distribution Lists using the Exchange Web Service (EWS) API. It provides the capability of:

*   Create private distribution list
*   Fetch distribution list
*   Add members to the list
*   Delete members from the list
*   Send message to the distribution list
*   Create Mail address from distribution lit

**Support for Creating and Formatting Response Messages:** Aspose.Email for Java API now provides the feature of creating and formatting response messages i.e. message Reply and Forward messages. The OriginalMessageAdditionalMode enumerator specifies the information to be included in the response message. This enumerator has the following options for including information to the response message:

*   **OriginalMessageAdditionMode.None** - The original message is not included in response message.
*   **OriginalMessageAdditionMode.Attachment** - The original message is included as attachment in response message
*   **OriginalMessageAdditionMode.Textpart** - The original message is included as text in body of response message

# Enhancements

**Getting Message Summary Information using Message URI:** In all systems that keep/save meta-data of messages for lateral referencing, it is a common method to store the message URI. This information is laterally used to retrieve message information from Exchange Server such as fetching the message. This month’s release of Aspose.Email for Java provides the capability to retrieve message summary information, represented by ExchangeMessageInfo, using the overloaded method of listMessages. It returns the ExchangeMessageInfoCollection for the list of provided ids.

**Improvement in CPU Utilization with MailMessage API:** Our last month’s version of Aspose.Email for .NET was identified to have some CPU utilization issues while using the _MailMessage_ API. The behavior was inherited in the Java API as well due to the conversion from its .NET version. It has been fixed in both the .NET and Java versions of the API.

# Other Improvements

In addition to new features and enhancements, this month’s release also includes a number of bug fixes. For a complete list of bug fixes, please visit the product download page.

# API Resources

We have detailed information available online for getting started with the Aspose.Email for Java API. These are:

*   Product Documentation – Provides detailed examples of working with the API
*   API Reference Guide – Details all the packages and classes of the API
*   [GitHub Examples][2] – Provides ready to run API examples
*   [Aspose.Email Forum][3] – Feel free to contact us on Aspose.Email forum for your queries




[1]: http://www.aspose.com/community/files/72/java-components/aspose.email-for-java/default.aspx
[2]: https://github.com/aspose-email/Aspose.Email-for-Java
[3]: http://www.aspose.com/community/forums/aspose.email-product-family/188/showforum.aspx





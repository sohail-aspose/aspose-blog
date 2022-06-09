---
title: 'Add, Update and Delete Contacts from Microsoft Exchange Server in Java'
seoTitle: "Java: Add, Update, Delete Contacts from Microsoft Exchange Server"
description: "Use Java email API to work with contacts on Microsoft Exchange Server in Java. Add, delete or update contacts from Exchange Server in Java."
date: Fri, 25 Feb 2022 08:07:00 +0000
draft: false
url: /2022/02/25/work-with-contacts-from-exchange-server-in-java/
author: Usman Aziz
summary: '[Microsoft Exchange Server][1] is an email and calendaring server that provides different collaboration services like email, calendars, contacts management, etc. In [one of my posts][2], I have shown you how to access and read emails from Microsoft Exchange Server programmatically in Java. However, we often need the contact list that we have on the MS Exchange Server. So in this article, you will learn **how to add, delete, or update contacts on Microsoft Exchange Server in Java**.'
tags: ['Add Contacts to MS Exchange Server in Java', 'Delete Contacts from MS Exchange Server in Java', 'Java API to Access Contacts on MS Exchange Server', 'Update a Contact on MS Exchange Server in Java']
categories: ['Aspose.Email Product Family']
---



{{< figure align=center src="images/aspose-email-exchange.png" alt="Add or Delete Contacts from Microsoft Exchange Server in Java">}}


[Microsoft Exchange Server][3] is an email and calendaring server that provides different collaboration services like email, calendars, contacts management, etc. In [one of my posts][4], I have shown you how to access and read emails from Microsoft Exchange Server programmatically in Java. However, we often need the contact list that we have on the MS Exchange Server. So in this article, you will learn **how to add, delete, or update contacts on Microsoft Exchange Server in Java**.

*   [Java API to Access Contacts on MS Exchange Server][5]
*   [Add Contacts to MS Exchange Server][6]
*   [Delete Contacts from MS Exchange Server][7]
*   [Update a Contact on MS Exchange Server][8]

## Java API to Access Contacts on MS Exchange Server {#API-to-Access-Contacts-on-Exchange-Server}

[Aspose.Email for Java][9] is a popular API to implement email client applications in Java. Moreover, it allows you to work with MS Exchange Server and manipulate the contacts, emails, and conversation items. We will use this API to add, update, and delete contacts on Exchange Server. You can either [download][10] the API's JAR or install it using the following Maven configurations.

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

## Add Contacts to MS Exchange Server in Java {#Add-Contacts-to-Exchange-Server}

The following are the steps to add contacts to Microsoft Exchange Server in Java.

*   First, create and initialize **NetworkCredential** object with username, password, and domain.
*   Then, initialize [IEWSClient][11] with mailbox URI and _NetworkCredential_ object.
*   Create an object of [Contact][12] class and set its properties such as name, job, gender, phone, associated persons, etc.
*   Finally, call [EWSClient.createContact(Contact)][13] method to add contact.

The following code sample shows how to add a contact to Microsoft Exchange Server in Java.

{{< gist aspose-com-gists 76cb1fc386756b5098e9a44e6e6b0c6d "add-contact.java" >}}

## Delete Contacts from MS Exchange Server in Java {#Delete-Contacts-from-Exchange-Server}

You can also delete a contact from the MS Exchange Server. To filter the contacts, you can use the name, email, or any other suitable property. The following are the steps to delete a contact from Microsoft Exchange Server in Java.

*   First, create and initialize [IEWSClient][14] object.
*   Then, get all the contacts from MS Exchange Server using [IEWSClient.getContacts(EWSClient.getMailboxInfo().getContactsUri())][15] method.
*   Loop through the contacts and filter the required one(s).
*   At the end, delete the contact using [IEWSClient.deleteItem(Contact.getId().getEWSId(), DeletionOptions.getDeletePermanently())][16] method.

The following code sample shows how to delete contacts from Microsoft Exchange Server in Java.

{{< gist aspose-com-gists 76cb1fc386756b5098e9a44e6e6b0c6d "delete-contact.java" >}}

## Update a Contact on Exchange Server in Java {#Update-a-Contact-on-Exchange-Server}

Aspose.Email for Java also allows you to update a contact on MS Exchange Server. The following are the steps to perform this operation.

*   First, create and initialize **NetworkCredential** object with username, password, and domain.
*   Then, initialize [IEWSClient][17] with mailbox URI and _NetworkCredential_ object.
*   Get contacts from Exchange Server using [IEWSClient.getContacts(EWSClient.getMailboxInfo().getContactsUri())][18] method.
*   After that, loop through the contacts and filter the desired contact.
*   Finally, update the contact's properties and call [IEWSClient.updateContact(Contact)][19] to save it.

The following code sample shows how to update a contact on MS Exchange Server in Java.

{{< gist aspose-com-gists 76cb1fc386756b5098e9a44e6e6b0c6d "update-contact.java" >}}

## Get a Free API License {#Get-a-Free-API-License}

You can get a [free temporary license][20] to use Aspose.Email for Java without evaluation limitations.

## Conclusion

In this article, you have learned how to work with contacts on Microsoft Exchange Server in Java. We have demonstrated how to add, remove, and update contacts from the MS Exchange Server in Java. Besides, you can explore the [documentation][21] to read more about Aspose.Email for Java. Also, you can post your queries on our [forum][22].

## See Also

*   [Read Emails from MS Exchange Server in Java][23]




[1]: https://en.wikipedia.org/wiki/Microsoft_Exchange_Server
[2]: https://blog.aspose.com/2021/03/22/read-emails-from-ms-exchange-server-using-java/
[3]: https://en.wikipedia.org/wiki/Microsoft_Exchange_Server
[4]: https://blog.aspose.com/2021/03/22/read-emails-from-ms-exchange-server-using-java/
[5]: #API-to-Access-Contacts-on-Exchange-Server
[6]: #Add-Contacts-to-Exchange-Server
[7]: #Delete-Contacts-from-Exchange-Server
[8]: #Update-a-Contact-on-Exchange-Server
[9]: https://products.aspose.com/email/java
[10]: https://downloads.aspose.com/email/java
[11]: https://apireference.aspose.com/email/java/com.aspose.email/IEWSClient
[12]: https://apireference.aspose.com/email/java/com.aspose.email/Contact
[13]: https://apireference.aspose.com/email/java/com.aspose.email/IEWSClient#createContact(com.aspose.email.Contact)
[14]: https://apireference.aspose.com/email/java/com.aspose.email/IEWSClient
[15]: https://apireference.aspose.com/email/java/com.aspose.email/IEWSClient#getContacts(java.lang.String)
[16]: https://apireference.aspose.com/email/java/com.aspose.email/IEWSClient#deleteItem(java.lang.String,%20com.aspose.email.DeletionOptions)
[17]: https://apireference.aspose.com/email/java/com.aspose.email/IEWSClient
[18]: https://apireference.aspose.com/email/java/com.aspose.email/IEWSClient#getContacts(java.lang.String)
[19]: https://apireference.aspose.com/email/java/com.aspose.email/IEWSClient#updateContact(com.aspose.email.Contact)
[20]: https://purchase.aspose.com/temporary-license
[21]: https://docs.aspose.com/email/java/
[22]: https://forum.aspose.com/
[23]: https://blog.aspose.com/2021/03/22/read-emails-from-ms-exchange-server-using-java/





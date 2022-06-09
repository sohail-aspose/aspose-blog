---
title: 'Create, Update, and Delete Contacts in Gmail using Java'
seoTitle: "Java: Create, Update, and Delete Contacts in Gmail | Java Gmail API"
description: "Use Java Gmail API to create and update contacts in a Gmail account in Java. Delete desired contacts from Gmail account programmatically in Java."
date: Tue, 22 Mar 2022 22:19:00 +0000
draft: false
url: /2022/03/22/create-update-and-delete-contacts-in-gmail-using-java/
author: Usman Aziz
summary: '[Gmail][1] is one of the commonly used online applications for sending and receiving emails. In addition, it allows working with calendars, contacts, chats, etc., and provides various other collaboration services. Recently, in [an article][2], we have covered how to import contacts from a Gmail account. Today, you will learn **how to create, update, and delete contacts in a Gmail account using Java**.'
tags: ['Create a Contact on Gmail in Java', 'Delete a Contact on Gmail in Java', 'Java API to Manage Gmail Contacts', 'Java Gmail API', 'Update a Contact on Gmail in Java']
categories: ['Aspose.Email Product Family']
---



{{< figure align=center src="images/Create-Update-and-Delete-Gmail-Contacts.png" alt="Create, Update, and Delete Contacts in Gmail using Java">}}


[Gmail][3] is one of the commonly used online applications for sending and receiving emails. In addition, it allows working with calendars, contacts, chats, etc., and provides various other collaboration services. Recently, in [an article][4], we have covered how to import contacts from a Gmail account. Today, you will learn **how to create, update, and delete contacts in a Gmail account using Java**.

*   [Java API to Manage Gmail Contacts][5]
*   [Create a Contact on Gmail][6]
*   [Update a Contact on Gmail][7]
*   [Delete a Contact on Gmail][8]

## Java API to Create, Update and Delete Gmail Contacts {#API-to-Manage-Gmail-Contacts}

To create and manipulate contacts in a Gmail account, we will use [Aspose.Email for Java][9]. It is a feature-rich API that lets you create and send emails and work with popular email clients. You can either [download][10] the API or install it using the following Maven configurations.

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

After installing the API, you need to create a project on the Google Developer Console, which will allow you to communicate with Gmail. To create one, you can follow [this guide][11].

Now, create a helper class named **GoogleOAuthHelper** to take care of the authentication of a Gmail account. Also, create a class named **OAuthUser** to store user information. The following is the complete implementation of both classes.

{{< gist aspose-com-gists 80635cdce7ba63ea8689fb71f05bb577 "OAuthUser.java" >}}

{{< gist aspose-com-gists 80635cdce7ba63ea8689fb71f05bb577 "GoogleOAuthHelper.java" >}}

## Create a Contact on Gmail in Java {#Create-a-Contact-on-Gmail}

The following are the steps to create a contact on Gmail in Java.

*   First, create a Google user, get an access token, and initialize an [IGmailClient][12] object.
*   Then, create an object of the [Contact][13] class.
*   Set properties of the contact such as name, prefix, profession, etc.
*   To set the postal address, create an instance of [PostalAddress][14] and set its properties.
*   Add newly created address to the collection using the [Contact.getPhysicalAddresses().add(PostalAddress)][15] method.
*   Set phone number details using [PhoneNumber][16] class.
*   Add phone number details to collection using [Contact.getPhoneNumbers().add(PhoneNumber)][17] method.
*   Create an instance of [EmailAddress][18] class, set the email address, and assign it to the contact.
*   Finally, call [IGmailClient.createContact(Contact)][19] method to create Gmail contact.

The following code sample shows how to create a contact on Gmail in Java.

{{< gist aspose-com-gists 80635cdce7ba63ea8689fb71f05bb577 "create-gmail-contact.java" >}}

## Update a Contact on Gmail in Java {#Update-a-Contact-on-Gmail}

You can also update the details of a Gmail contact after accessing it. The following are the steps to update a contact in a Gmail account in Java.

*   First, create a Google user, get an access token, and initialize an [IGmailClient][20] object.
*   Then, get contacts in an array using [IGmailClient.getAllContacts()][21] method.
*   After that, fetch the required contact from the array in a [Contact][22] object.
*   Finally, update the details of contact and call [IGmailClient.updateContact(contact)][23] method.

The following code sample shows how to update a contact in Gmail in Java.

{{< gist aspose-com-gists 80635cdce7ba63ea8689fb71f05bb577 "update-gmail-contact.java" >}}

## Delete a Contact on Gmail in Java {#Delete-a-Contact-on-Gmail}

Finally, let's see how to delete a Gmail contact using Java. The following are the steps to perform this operation.

*   First, create a Google user, get an access token, and initialize an [IGmailClient][24] object.
*   Then, get contacts in an array using [IGmailClient.getAllContacts()][25] method.
*   Filter the desired contact from the array in a [Contact][26] object.
*   Finally, call [IGmailClient.deleteContact(Contact.Id.GoogleId)][27] method to delete the contact.

The following code sample shows how to delete a contact on Gmail in Java.

{{< gist aspose-com-gists 80635cdce7ba63ea8689fb71f05bb577 "delete-gmail-contact.java" >}}

## Get a Free API License

You can use Aspose.Email for Java without evaluation limitations using a [free temporary license][28].

## Conclusion

In this article, you have learned how to create and update contacts in a Gmail account in Java. Furthermore, you have seen how to delete a Gmail contact programmatically. Besides, you can visit the [documentation][29] to explore other features of Aspose.Email for Java. In case you would have any questions, you can post to our [forum][30].

## See Also

*   [Read Emails from MS Exchange Server using Java][31]
*   [Create and Send Outlook Email Messages using Java][32]




[1]: https://en.wikipedia.org/wiki/Gmail
[2]: https://blog.aspose.com/2022/03/24/import-gmail-contacts-in-java/
[3]: https://en.wikipedia.org/wiki/Gmail
[4]: https://blog.aspose.com/2022/03/24/import-gmail-contacts-in-java/
[5]: #API-to-Manage-Gmail-Contacts
[6]: #Create-a-Contact-on-Gmail
[7]: #Update-a-Contact-on-Gmail
[8]: #Delete-a-Contact-on-Gmail
[9]: https://products.aspose.com/email/java/
[10]: https://downloads.aspose.com/email/java/
[11]: https://docs.aspose.com/email/net/gmail-utility-features/#creating-project-in-google-developer-console
[12]: https://apireference.aspose.com/email/java/com.aspose.email/IGmailClient
[13]: https://apireference.aspose.com/email/java/com.aspose.email/Contact
[14]: https://apireference.aspose.com/email/java/com.aspose.email/PostalAddress
[15]: https://apireference.aspose.com/email/java/com.aspose.email/Contact#getPhysicalAddresses()
[16]: https://apireference.aspose.com/email/java/com.aspose.email/PhoneNumber
[17]: https://apireference.aspose.com/email/java/com.aspose.email/Contact#getPhoneNumbers()
[18]: https://apireference.aspose.com/email/java/com.aspose.email/EmailAddress
[19]: https://apireference.aspose.com/email/java/com.aspose.email/IGmailClient#createContact(com.aspose.email.Contact)
[20]: https://apireference.aspose.com/email/java/com.aspose.email/IGmailClient
[21]: https://apireference.aspose.com/email/java/com.aspose.email/IGmailClient#getAllContacts()
[22]: https://apireference.aspose.com/email/java/com.aspose.email/Contact
[23]: https://apireference.aspose.com/email/java/com.aspose.email/IGmailClient#updateContact(com.aspose.email.Contact)
[24]: https://apireference.aspose.com/email/java/com.aspose.email/IGmailClient
[25]: https://apireference.aspose.com/email/java/com.aspose.email/IGmailClient#getAllContacts()
[26]: https://apireference.aspose.com/email/java/com.aspose.email/Contact
[27]: https://apireference.aspose.com/email/java/com.aspose.email/IGmailClient#deleteContact(java.lang.String)
[28]: https://products.aspose.com/email
[29]: https://docs.aspose.com/email/java/
[30]: https://forum.aspose.com/
[31]: https://blog.aspose.com/2021/03/22/read-emails-from-ms-exchange-server-using-java/
[32]: https://blog.aspose.com/2020/05/20/create-and-send-outlook-email-messages-asynchronously-using-java/





---
title: 'Import Gmail Contacts Programmatically in Java'
date: Thu, 24 Mar 2022 15:04:57 +0000
draft: false
url: /2022/03/24/import-gmail-contacts-in-java/
author: ''Usman Aziz''
summary: "Google's [Gmail][1] is among the most popular and commonly used email services. Gmail provides a range of features along with just sending and receiving emails, such as calendars, chats, etc. In certain cases, you may need to connect to Gmail and import contacts programmatically from within your applications. To achieve that, this article shows **how to import Gmail contacts using Java**. Also, we will cover how to access contacts in a specific email group."
tags: ['Import Contacts from Gmail in Java', 'Import Contacts from a Specific Gmail Group in Java', 'Java API to Import Contacts from Gmail']
categories: ['Aspose.Email Product Family']
---



{{< figure align=center src="images/Import-Contacts-from-Gmail-Account.png" alt="Import Gmail Contact Programmatically in Java">}}


Google's [Gmail][2] is among the most popular and commonly used email services. Gmail provides a range of features along with just sending and receiving emails, such as calendars, chats, etc. In certain cases, you may need to connect to Gmail and import contacts programmatically from within your applications. To achieve that, this article shows **how to import Gmail contacts using Java**. Also, we will cover how to access contacts in a specific email group.

*   [API to Import Contacts from Gmail][3]
*   [Import Contacts from Gmail][4]
    *   [Import Gmail Contacts][5]
    *   [Get Contacts from a Specific Group][6]

## Java API to Import Gmail Contacts {#API-to-Import-Contacts-from-Gmail}

[Aspose.Email for Java][7] is a powerful API to create email client applications. Moreover, it supports working with Gmail such as accessing contacts, calendars, appointments, etc. We will use this API to access and import contacts from Gmail accounts. You can either [download][8] the API or install it using the following Maven configurations.

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

## Import Contacts from Gmail in Java {#Import-Contacts-from-Gmail}

Before you start, you need to create a project on the Google Developer Console, which will allow you to execute the code. To create one, you can follow [this guide][9].

Now, create a helper class named **GoogleOAuthHelper** to take care of the authentication of a Gmail account. Also, create a class named **OAuthUser** to store user information. The following is the complete implementation of both classes.

{{< gist aspose-com-gists 4f01b0affc2beaa1c63b58c4716d67a2 "OAuthUser.java" >}}

{{< gist aspose-com-gists 4f01b0affc2beaa1c63b58c4716d67a2 "GoogleOAuthHelper.java" >}}

### Import Contacts from a Gmail Account {#Import-Contacts}

The following are the steps to import contacts from a Gmail account in Java.

*   Create an object of **OAuthUser** class and initialize it with email, client ID and client secret.
*   Create two string objects to store authorization code and code verifier.
*   Get refresh token and access token.
*   Get an instance of **GmailClient** class into an **IGmailClient** object using **GmailClient.getInstance(String, String)** method.
*   Read contacts into an array using **IGmailClient.getAllContacts()** method.
*   Loop through array to access each contact.

The following code sample shows how to import Gmail contacts from an account in Java.

{{< gist aspose-com-gists 4f01b0affc2beaa1c63b58c4716d67a2 "Import-Gmail-Contacts.java" >}}

## Import Gmail Contacts from a Group {#Get-Contacts-from-a-Specific-Group}

You can also access contacts from a specific email group in Gmail following the steps below.

*   Follow the steps mentioned in previous section to initialize the **IGmailClient**.
*   Call **IGmailClient.getAllGroups()** to get groups into a **ContactGroupCollection** object.
*   Filter the required group(s) based on the title.
*   Access contacts from a group using **IGmailClient.getContactsFromGroup(String)** method.
*   Loop through array to access each contact.

The following code sample shows how to import contacts from a specific Gmail group in Java.

{{< gist aspose-com-gists 4f01b0affc2beaa1c63b58c4716d67a2 "Import-Gmail-Contacts-From-Group.java" >}}

## Get a Free API License {#Get-a-Free-API-License}

You can get a [free temporary license][10] to use Aspose.Email for Java without evaluation limitations.

## Conclusion

In this article, you have learned how to import Gmail contacts from an account programmatically in Java. Moreover, you have seen how to access contacts from a particular email group in Gmail. Apart from that, you can explore the [documentation][11] to read more about Aspose.Email for Java. Also, you can ask your questions via our [forum][12].

## See Also

*   [Read Emails from MS Exchange Server using Java][13]
*   [Create and Send Outlook Email Messages using Java][14]




[1]: https://www.google.com/gmail/about/
[2]: https://www.google.com/gmail/about/
[3]: #API-to-Import-Contacts-from-Gmail
[4]: #Import-Contacts-from-Gmail
[5]: #Import-Contacts
[6]: #Get-Contacts-from-a-Specific-Group
[7]: https://products.aspose.com/email/java/
[8]: https://downloads.aspose.com/email/java/
[9]: https://docs.aspose.com/email/net/gmail-utility-features/#creating-project-in-google-developer-console
[10]: https://purchase.aspose.com/temporary-license
[11]: https://docs.aspose.com/email/java/
[12]: https://forum.aspose.com/
[13]: https://blog.aspose.com/2021/03/22/read-emails-from-ms-exchange-server-using-java/
[14]: https://blog.aspose.com/2020/05/20/create-and-send-outlook-email-messages-asynchronously-using-java/





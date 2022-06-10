---
title: 'Move Emails using IMAP Client using Java with Aspose.Email for Java 6.4.0'
date: Tue, 19 Apr 2016 13:57:12 +0000
draft: false
url: /2016/04/19/improved-paging-implementation-and-moving-emails-using-imap-client-supported-with-aspose.email-for-java-6.4.0/
author: Kashif Iqbal
summary: ''
tags: []
categories: ['Aspose.Email Product Family']
---



{{< figure align=center src="images/aspose-Email-for-Java_100.png" alt="Aspose.Email for Java">}}


[Aspose.Email for Java 6.4.0][1] has been released. Ported from its equivalent .NET version, the API has been enriched with new features and enhancements. These include enhancements to the EML, MSG, IMAP, and EWS APIs of the library. In addition, it also contains a number of bug fixes that were reported with the Java version of the API or fixed in the equivalent .NET version.

## Send Calendar Invitations using EWS

This month’s release provides a new feature of sending calendar invitations using the API’s Exchange Web Service client, similar to Microsoft Exchange’s behavior. This functionality requires the access delegation to the invitee. In addition, the invitation needs to be sent as TNEF EML by converting the MSG using the _MailMessageInterpretor_ as shown in the code sample below:

```
final IEWSClient client = EWSClient.getClient("exchange.domain.com", "username", "password");
try
{
    // delegate calendar permission
    ExchangeDelegateUser delegateUser = new ExchangeDelegateUser(sharingTo.EMail, ExchangeDelegateFolderPermissionLevel.NotSpecified);
    delegateUser.getFolderPermissions().setCalendarFolderPermissionLevel(ExchangeDelegateFolderPermissionLevel.Reviewer);
    //client.DelegateAccess(delegateUser, sharingFrom.EMail);

    // create invitation
    MapiMessage mapiMessage = client.createCalendarSharingInvitationMessage(sharingTo.EMail);

    // send invitation
    MailMessageInterpretor messageInterpretor = MailMessageInterpretorFactory.getInstance().getIntepretor(mapiMessage.getMessageClass());
    MailMessage mailMessage = messageInterpretor.interpretAsTnef(mapiMessage);
    client.send(mailMessage);
}
finally { if (client != null) ((IDisposable)client).dispose(); } 
```

## Move Message using IMAP

With this month’s release, we have enhanced the IMAP client to support moving messages from one folder to another. The IMAP client now offers the moveMessage method that uses the message’s unique Id or sequence number to [move a message][2] across folders.

## Support for Listing Searched Messages with Paging

This month’s release also enhances the IMAP client by providing paging support for listing searched messages. The _listMessagesByPage_ method can be used to specify [the search criterion and number of messages][3] per page for retrieving the messages.

## Save Messages as Outlook Template (OFT) File

Aspose.Email for Java already supports reading Outlook Template (OFT) files. This month’s release further enhances this functionality by providing support for saving messages to OFT format. The API supports saving [EML][4] as well as [MSG][5] file types to OFT formats.

## Improvement in Paging Support Implementation

With this month’s release, we have improved the implementation of methods for listing items with paging support using the API clients. Specifically, the implementation has been implemented in separate classes for each of the communication clients.

## Set Timezone Context for Exchange Server

This month’s release also provides the capability of setting time zone defaults for the Exchange server using the EWS client. The setTimezoneId method can be used to achieve this as shown in the code sample below:

```
final IEWSClient client = TestUtil.createEwsClient(server.getUser1());
try
{
    client.setTimezoneId("Central Europe Standard Time");
    // .....
}
finally { if (client != null) ((IDisposable)client).dispose(); }
```

## Other Improvements

This month’s release also fixes a number of bugs that were reported with the last version of the API. It also contains bug fixes as a result of porting from its equivalent .NET version. For further information about the fixed issues, please visit the [release notes][6] page of Aspose.Email for Java 6.4.0.

## API Resources

We have detailed information available online for getting started with the Aspose.Email for Java API. These are:

*   [Product Documentation][7] – Provides detailed examples of working with the API
*   [API Reference Guide][8] – Details all the packages and classes of the API
*   [GitHub Examples][9] – Provides ready to run API examples
*   [Aspose.Email Forum][10] – Feel free to contact us on Aspose.Email forum for your queries




[1]: https://downloads.aspose.com/email/java
[2]: https://docs.aspose.com/display/emailjava/Working+with+Folders+on+IMAP+Server#WorkingwithFoldersonIMAPServer-MoveMessagestoAnotherMailboxFolder
[3]: https://docs.aspose.com/display/emailjava/Working+with+Messages+from+IMAP+Server#WorkingwithMessagesfromIMAPServer-FilteringMessagesBasedonSender,RecipientorDate
[4]: https://docs.aspose.com/display/emailjava/Creating+and+Setting+Contents+of+Emails#CreatingandSettingContentsofEmails-CreateNewEmailMessage
[5]: https://docs.aspose.com/display/emailjava/Creating+and+Saving+MSG+files
[6]: https://docs.aspose.com/display/emailjava/Aspose.Email+for+Java+6.4.0+Release+Notes
[7]: http://docs.aspose.com/display/EmailJava/Home
[8]: https://apireference.aspose.com/email/java
[9]: https://github.com/aspose-email/Aspose.Email-for-Java
[10]: http://forum.aspose.com





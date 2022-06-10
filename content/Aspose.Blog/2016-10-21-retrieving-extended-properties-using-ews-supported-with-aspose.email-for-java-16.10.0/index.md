---
title: 'List Messages with Extended Properties using EWS - Aspose.Email for Java 16.10.0'
date: Fri, 21 Oct 2016 14:39:45 +0000
draft: false
url: /2016/10/21/retrieving-extended-properties-using-ews-supported-with-aspose.email-for-java-16.10.0/
author: Kashif Iqbal
summary: ''
tags: ['Java API for Exchange Server', 'Retrieve messages from exchange server in Java']
categories: ['Aspose.Email Product Family']
---



{{< figure align=center src="images/aspose-Email-for-Java_100.png" alt="Aspose.Email for Java">}}


[Aspose.Email for Java 16.10.0][1] has been received. Ported from its equivalent .NET version, this month’s release includes the same enhancements as were present in the .NET version of the API. It also improves the API functionality by fixing a number of bugs reported by users. For further information about the enhancements, bug fixes, and public API changes, please visit the [release notes][2] section of our documentation.

# Enhancements

**Listing Messages by Extended Properties using EWS:** This month’s release provides enhancement where messages can be retrieved along with [extended properties][3] from the Exchange server. The overloaded method of listMessages can be used to specify the extended properties to be fetched from the Exchange server. The following code sample shows an example usage of this new feature of the API.

{{< gist aspose-com-gists 709d733586ce50505c3bca3f6e8bd18d "Examples-src-main-java-com-aspose-email-examples-exchange-FetchMessagesFromAnExchangeServerMailbox-FetchMessagesFromAnExchangeServerMailboxUsingEWS.java" >}}

**Retrieving Extra Parameters as Summary Information using IMAP:** IMAP protocol supports retrieving information from email servers with custom commands. This month’s release enhances the API functionality to retrieve these extra parameters using the _listMessages_ method of the API. This retrieves the message’s summary information, _ImapMessageInfo_, along with the specified extra parameters, as shown in the code sample below.

```
ImapClient client = new ImapClient("host.domain.com", "username", "password");
{
    try
    {
        MailMessage message = new MailMessage(
                "from@domain.com",
                "to@doman.com",
                "EMAILNET-38466 - Retrieve Extra Parameters as Summary Info." ,
                "EMAILNET-38466 Add extra parameters for UID FETCH command");

        //append the message to the server
        String uid = client.appendMessage(message);

        //wait for the message to be appended
        Thread.sleep(5000);

        //Define properties to be fetched from server along with the message
        List messageExtraFields = new List();
        messageExtraFields.add("X-GM-MSGID");
        messageExtraFields.add("X-GM-THRID");
        //retreive the message summary information using it's UID
        ImapMessageInfo messageInfoUID = client.listMessage(uid, messageExtraFields);

        //retreive the message summary information using it's sequence number
        ImapMessageInfo messageInfoSeqNum = client.listMessage(1, messageExtraFields);

        //List messages in general from the server based on the defined properties
        ImapMessageInfoCollection messageInfoCol = client.listMessages(messageExtraFields);

        ImapMessageInfo messageInfoFromList = messageInfoCol.get_Item(0);

        //verify that the parameters are fetched in the summary information

        for (String paramName:messageExtraFields)
        {
            System.out.println(messageInfoFromList.getExtraParameters().containsKey(paramName));

            System.out.println(messageInfoUID.getExtraParameters().containsKey(paramName));

            System.out.println(messageInfoSeqNum.getExtraParameters().containsKey(paramName));
        }
    }
    finally
    {
    }
} 
```

# Other Improvements

This month’s release also contains several bug fixes that were either reported with the .NET version of the API or directly faced with our Java API. Fixing these further adds stability to the API functionality.

# API Resources

We have detailed information available online for getting started with the Aspose.Email for Java API. These are:

*   [Product Documentation][4] – Provides detailed examples of working with the API
*   [API Reference Guide][5] – Details all the packages and classes of the API
*   [GitHub Examples][6] – Provides ready to run API examples
*   [Aspose.Email Forum][7] – Feel free to contact us on Aspose.Email forum for your queries




[1]: http://www.aspose.com/downloads/email/java
[2]: https://docs.aspose.com/display/emailjava/Aspose.Email+for+Java+16.10.0+Release+Notes
[3]: https://docs.aspose.com/display/emailjava/Fetch+Messages+from+an+Exchange+Server+Mailbox
[4]: http://docs.aspose.com/display/EmailJava/Home
[5]: https://apireference.aspose.com/java/email
[6]: https://github.com/aspose-email/Aspose.Email-for-Java
[7]: http://forum.aspose.com





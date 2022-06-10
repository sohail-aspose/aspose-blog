---
title: 'Aspose.Network 3.5 beta2 supports parsing Microsoft outlook message files'
date: Sun, 13 May 2007 03:39:00 +0000
draft: false
url: /2007/05/13/aspose-network-parse-microsoft-outlook-message-files/
author: Iret
summary: ''
tags: []
categories: ['Aspose.Email Product Family']
---

Dear Customers,

We have completed the Aspose.Network 3.5 beta2 development. In this release, we provide fully supporting for parsing Microsoft Outlook Message documents (\*.msg files).

By using Aspose.Network.Outlook.MapiMessage class, you can access all the information in the message files. Moreover, we also support getting the property by Mapi property tags, message body decoding, attachment saving and etc.

Please download the beta2 release, share your idea to us. We will make an official release coming weeks.

Download Link

http://www.aspose.com/Community/forums/storage/188/76302/Aspose.Network%20bet2.zip

\[C#\]

            using Aspose.Network.Outlook;

            MapiMessage message;  
            //parse the outlook message into a MapiMessage instance.  
            using (MapiMessageReader mr = new MapiMessageReader(attachment\_case1\_msg))  
            {  
                message = mr.ReadMessage();  
            }  
            //access the property in the message  
            Console.WriteLine("Subject:" + message.Subject);  
            Console.WriteLine("From:" + message.SenderEmailAddress);  
            Console.WriteLine("Body"+ message.Body);  
            //save the attachments locally.  
            foreach (MapiAttachment att in message.Attachments)  
            {  
                att.Save(att.LongFileName);  
            }

\[VB\]

            Imports Aspose.Network.Outlook

            Dim message As MapiMessage  
            'parse the outlook message into a MapiMessage instance.  
            Imports (MapiMessageReader mr = New MapiMessageReader(attachment\_case1\_msg))  
            {  
                message = mr.ReadMessage()  
            }  
            'access the property in the message  
            Console.WriteLine("Subject:" + message.Subject)  
            Console.WriteLine("From:" + message.SenderEmailAddress)  
            Console.WriteLine("Body"+ message.Body)  
            'save the attachments locally.  
            Dim att As MapiAttachment  
            For Each att In message.Attachments  
                att.Save(att.LongFileName)  
            Next









---
title: 'How to access Mapi propertes in a Microsoft Outlook Message files'
date: Sun, 13 May 2007 14:03:00 +0000
draft: false
url: /2007/05/13/aspose-network-access-mapi-property-by-mapi-property-tags/
author: Iret
summary: ''
tags: []
categories: ['Aspose.Email Product Family']
---

In this article, we will demonstrate how to access mapi propertes in a Microsoft outlook message files (\*.msg files), using Aspose.Network.

\[VB\]

            Dim message As MapiMessage  
   
            'load and parse the Microsoft Outlook Message files  
            Imports (MapiMessageReader mr = New MapiMessageReader("c:\\sample.msg"))  
            {  
                message = mr.ReadMessage()  
            }  
   
            'read subject property. Or you can use MapiMessage.Subject too.  
            Dim subject As String =  message.GetPropertyString(MapiPropertyTag.PR\_SUBJECT)  
   
            'read body property. Or you can use MapiMessage.Body too.  
            Dim body As String =  message.GetPropertyString(MapiPropertyTag.PR\_BODY)  
   
            Console.WriteLine("subject:"+subject)  
            Console.WriteLine("Body:" + body)  
   
            'read internet code page property.  
            Dim prop As MapiProperty =  message.Properties(MapiPropertyTag.PR\_INTERNET\_CPID) as MapiProperty  
            If Not prop Is Nothing Then  
                Console.WriteLine("CodePage:" + prop.GetLong())  
            End If  
\[C#\]

          MapiMessage message;  
   
            //load and parse the Microsoft Outlook Message files  
            using (MapiMessageReader mr = new MapiMessageReader(@"c:\\sample.msg"))  
            {  
                message = mr.ReadMessage();  
            }  
   
            //read subject property. Or you can use MapiMessage.Subject too.  
            string subject =  message.GetPropertyString(MapiPropertyTag.PR\_SUBJECT);  
             
            //read body property. Or you can use MapiMessage.Body too.  
            string body = message.GetPropertyString(MapiPropertyTag.PR\_BODY);  
             
            Console.WriteLine("subject:"+subject);  
            Console.WriteLine("Body:" + body);  
              
            //read internet code page property.  
            MapiProperty prop =  
                message.Properties\[MapiPropertyTag.PR\_INTERNET\_CPID\] as MapiProperty;  
            if (prop  != null)  
            {  
                Console.WriteLine("CodePage:" + prop.GetLong());  
            }









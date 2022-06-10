---
title: 'Aspose.Network v3.8.2.0 with Dns Mail'
date: Tue, 13 May 2008 22:09:00 +0000
draft: false
url: /2008/05/13/aspose-network-v3-8-2-0-with-dns-mail/
author: Iret
summary: ''
tags: []
categories: ['Aspose.Email Product Family']
---

We have released a new version of Aspose.Network. The majore feature of this release is Dns mail -- we now support sending email message with mail exchange servers if you don't have any smtp servers.

Here is the code sample for C#:

            MailMessage msg = new MailMessage();  
            msg.From = "[sender@mail.com][1]";  
            msg.To = "[use1@mail.com;user2@mail.com][2]";  
            msg.Subject = "dns sending";  
            msg.Body = "it is a test.";  
            DnsMailClient client = new DnsMailClient();  
            client.Send(msg);

By using the DnsMailClient class, you can send out an email message according to the mail exchange servers of the mail address itself. You don't need to have a valid smtp server now.

However, it will also have some performance drop for Dns mail. Because in case of no smtp server, we need to talk to all of the different mail domains(if any) in order to send an email to all recipients. Let's say, if your email has two recipients in different mail host/domain, A is [A@maildomain1.com][3], B is [B@maildomain2.com][4]. DnsMailClient will talk to maildomain1 and maildomain2 to send out emails.

Therefore, Dns mail may be slow than the smtp mail, if you have lots of recipients in different mail domain.

Here is the download page of Aspose.Network, Please check it out.

[http://www.aspose.com/community/files/54/utility-components/aspose.network/category1102.aspx][5]




[1]: mailto:sender@mail.com
[2]: mailto:use1@mail.com;user2@mail.com
[3]: mailto:A@maildomain1.com
[4]: mailto:B@maildomain2.com
[5]: http://www.aspose.com/community/files/54/utility-components/aspose.network/category1102.aspx





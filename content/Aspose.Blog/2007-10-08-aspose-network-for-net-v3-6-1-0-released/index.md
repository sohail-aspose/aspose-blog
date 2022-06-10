---
title: 'Aspose.Network for .NET v3.6.1.0 Released'
date: Mon, 08 Oct 2007 12:04:00 +0000
draft: false
url: /2007/10/08/aspose-network-for-net-v3-6-1-0-released/
author: Iret
summary: ''
tags: []
categories: ['Aspose.Email Product Family']
---

**What's New**

*   Provide format template for customizing the file format convertion from msg files to mht files. More format templates are supported in MhtMessageFormatter class, which will provide more flexibility for .NET developers to customize the output of mht format files.

        Sample:

            MailMessage mail = MailMessage.Load(file, MessageFormat.Msg);  
            MhtMessageFormatter f = new MhtMessageFormatter();  
            f.FormFormat = "FROM:{0}<br>";  
            f.SentFormat = "SENT:{0}<br>";  
            f.SubjectFormat = "SUBJECT:{0}<br>";  
            f.ToFormat = "TO:{0}<br>";  
            f.CcFormat= "CC:{0}<br>";  
            f.AttachmentFormat = "ATT:{0}<br>";  
            mail.Save(@"D:\\codestore\\Aspose.network\\phone2.mht", MessageFormat.Mht, f);

**Fixes**

*   3871 - Cannot extract alternative views in some EML files.
*   3869 - From address lost when convert to mht format files.









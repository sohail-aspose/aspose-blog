---
title: 'Aspose.Network  Hotfix Released'
date: Tue, 07 Nov 2006 00:07:00 +0000
draft: false
url: /2006/11/07/60675/
author: Iret
summary: ''
tags: []
categories: ['Aspose.Email Product Family']
---

Dear Customers,

We have released a new hotfix for Aspose.Network.

What's new in this release:

*   Fixed the bug in parsing Eml file, which will throw out a MimeException if the Eml contains invalid header for Return-Path. Now we will just ignore it.
*   Fixed the bug in parsing Empty ReplyTo header in Eml file.
*   Changed the behaviors for Pop3Client.SaveMessage function, which will not invoke Mime parsing function for validation. Therefore, the performance for the function will be improved also.
*   All other updates from 3.1.0.0 .

How to get the hotfix:

*   http://www.aspose.com/Downloads/Aspose.Network/3.1.1106.0/Default.aspx









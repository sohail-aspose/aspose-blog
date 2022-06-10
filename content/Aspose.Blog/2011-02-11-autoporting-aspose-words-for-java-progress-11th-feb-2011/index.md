---
title: 'Autoporting Aspose.Words for Java Progress - 11th Feb 2011'
date: Fri, 11 Feb 2011 00:12:00 +0000
draft: false
url: /2011/02/11/autoporting-aspose-words-for-java-progress-11th-feb-2011/
author: Romank
summary: ''
tags: ['Codeporting']
categories: ['Aspose.Words Product Family']
---

**Previous Stats** _Aspose.Words consists of 2744 source files._ _Running 311 unit tests on Aspose.Foundation for Java pass all._ _Running 8813 unit tests on Aspose.Words - 437 fail._  
**Today Stats** Aspose.Words consists of **2800** files. Aspose.Foundation **398** unit tests all pass. Aspose.Words **8868** unit tests - **376** fail.  
**Comments** You can see some great signs: 1. Aspose.Words codebase grows as the number of files and the number of tests shows. 2. All newly added code is autoportable and it is easy to maintain it autoportable. Over the past month actually more than 800 source files had changes in them and all that is autoportable too. (We use CodePorting to speed up the porting process. It ports each line in the source code to Java, quickly and efficiently.)  3. The number of Aspose.Words failing unit tests has further reduced. The nature of work right now is still resolving remaining unit tests and unfortunately it requires architectural or policy decisions. This work is best done by RK as a team leader. But when RK has to attend planning or reviewing a .NET release, then work on Java is delayed. So I am back on guiding the Java unit tests resolutions right now and hopefully we can get them all sorted this time.









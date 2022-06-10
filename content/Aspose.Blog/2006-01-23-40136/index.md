---
title: 'Backing Up Aspose.Word Files'
date: Mon, 23 Jan 2006 20:54:00 +0000
draft: false
url: /2006/01/23/40136/
author: Romank
summary: ''
tags: ['Roman Korchagin']
---

I've been trying to find a good backup utility for our development environment for long time. I wanted to backup to DVD because it is great in terms of storage space, price and availability. I was trying various programs found by googling, but all to unsatisfactory results. Some were crashing, some did not handle many files well, took hours just counting the files. Some were full of adware.

Today is a great day because I ended up using Firestreamer-RM (Removable Media) from Cristalink [http://www.cristalink.com/][1]

It allowed me to backup 103K files taking 4.2Gb onto a DVD+R in under 30 minutes. This included source code repositories of Aspose.Word, Aspose.Chart, Aspose.iCalendar and Aspose.Spell, my local working copy of these components, all my work related documents, my outlook data file and our defects tracking database. The worst was the local working copy of the source files because SVN creates thousands of small files and that resulted in so many files to backup (100K+).

Firestreamer-RM installed and worked without a hitch. It is great in that it is not a full backup software of its own, but just some sort of a driver that makes it possible for various removable media (DVD, CD, Iomega, HDD and flash) to look like a tape drive to the standard NT Backup utility. You just use the Backup Utility for Windows included with your installation of Microsoft Windows to create and schedule the backup. I also enjoyed Crystalink's website and Firestreamer user documentation. It is all nice and easy to understand, answered all the questions I had.

Firestreamer is a must for any small business or a professional who has some valuable information. I'm just thinking about developers, ISVs, accountants, lawyers, designers, writers and so on. Highly recommended.




[1]: http://www.cristalink.com/




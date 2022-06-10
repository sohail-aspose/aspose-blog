---
title: 'Yet Another 64-bit Surprise'
date: Sat, 14 Jul 2007 02:34:00 +0000
draft: false
url: /2007/07/14/yet-another-64-bit-surprise/
author: Romank
summary: ''
tags: ['Roman Korchagin']
---

Some of the Aspose.Words (and other components) demo projects and unit tests retrieve data from a Microsoft Access .mdb database. I've been trying to get everything working on Windows Vista 64-bit and was getting "Microsoft.Jet.OLEDB.4.0 not registered" error.

According to various articles this is due to the fact my project is compiled for the AnyCPU platform and runs as a 64-bit application, but there are no Microsoft Access database drivers for 64-bit.

The recommendation I found in the MSDN forum is switch the platform to x86 so the application is compiled and runs as 32-bit. The articles also say that Microsoft does not plan releasing 64-bit drivers for Microsoft Access Jet... That is there is no way to use Microsoft Access databases from a 64-bit application.

Ever since I switched to Vista 64-bit I had so many development related problems. I've been meaning to say that for long time - I became disappointed in Microsoft. The whole 64-bit and especially in combination with Vista is an awfull experience for developers on the Microsoft platform. I'm not sure why, but Microsoft has definitely lost it at some point. It became very frustrating to be a .NET developer. One more bumpy and rushed switch to new platform or new OS like this and I promise I'll go Java or change the career altogether. I hope Microsoft takes note.

One more thing: I see a whole new business opportunity here. Develop 64-bit applications that Microsoft has no plans of developing. What would you say if Aspose developed Microsoft Access Jet drivers for 64-bit and sold them for $899 a piece?








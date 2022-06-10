---
title: 'Aspose.Words for Reporting Services Runs on Katmai'
date: Tue, 10 Jul 2007 01:55:00 +0000
draft: false
url: /2007/07/10/aspose-words-for-reporting-services-runs-on-katmai/
author: DmitryV
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---

We're making huge strides :) Two weeks ago we used our corporate time machine to get back to 2000 and recently we had a trip to 2008… Well probably I'm not an expert in literary techniques so let me simply announce that we have just released Aspose.Words for Reporting Services 1.3.0 and it now supports Microsoft SQL Server 2008 code name Katmai! We tested it on the recently published CTP 3 available to download [here][1]. So now the product is fully compatible with all modern versions of Microsoft SQL Server - 2000, 2005 and 2008 CTP.

Apart of that, we have great news for the people who need exporting reports to Microsoft Word documents on the x64 platform. We've conquered some weird issues that occurred when running Aspose.Words for Reporting Services in 64-bit environment and now it perfectly works on both x86 and x64 operating systems. This is a very important improvement that actually made us publish a full-scale release instead of a hotfix.

Now it's time to sum up the results. Here is a table that incorporates all versions and platforms the product supports starting with the latest version 1.3.0:

Microsoft SQL Server version

.NET Framework version

Platform

Assembly path in ZIP package\*

Microsoft SQL Server 2000

1.1

x86

Bin\\SSRS2000\\Aspose.Words.ReportingServices.dll

Microsoft SQL Server 2005

2.0

x86 and x64

Bin\\SSRS2005\\Aspose.Words.ReportingServices.dll

Microsoft SQL Server 2008 code name Katmai CTP 3

2.0

x86 and x64

Bin\\SSRS2008\\Aspose.Words.ReportingServices.dll

\*The MSI installer will simply ask what version to install.




[1]: https://connect.microsoft.com/SQLServer/content/content.aspx?ContentID=5395





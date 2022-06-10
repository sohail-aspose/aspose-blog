---
title: 'Aspose.Words for Reporting Services 1.3.0 Released'
date: Tue, 10 Jul 2007 00:47:00 +0000
draft: false
url: /2007/07/10/aspose-words-for-reporting-services-1-3-0-released/
author: DmitryV
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---

This is a full-scale release that can be particularly useful for the people who needs exporting reports to the DOC, RTF or WordML formats on the 64-bit edition of Microsoft SQL Server Reporting Services. Also, we have added a separate assembly that supports Microsoft SQL Server 2008 code name Katmai.

**What's new:**

*   **Added the support of Microsoft SQL Server 2008 "Katmai" Reporting Services. We have tested the product on the CTP 3.**
*   The MSI installer's behaviour was slightly changed. Now it installs the rendering extension to **all** detected instances of Microsoft SQL Server 2005 Reporting Services. Until now it only installed the product to the default instance that might confuse the users who had named instances and no default instance installed on their machine.
*   Performance optimizations.

**What's fixed:**

*   Running the export in 64-bit environment occasionally caused issues such as the weird "Attempted to read or write protected memory" exception. **Now the export works equally perfect on both x86 and x64 platforms.**
*   The MSI installer failed to detect Reporting Services instances on 64-bit operating systems.
*   Some kind of matrices threw the "Index was out of range" exception.

To download visit [http://www.aspose.com/Downloads/Aspose.Words.Reporting.Services/Default.aspx][1]




[1]: https://docs.aspose.com/display/diagramjava/How+to+Convert+a+Visio+Diagram





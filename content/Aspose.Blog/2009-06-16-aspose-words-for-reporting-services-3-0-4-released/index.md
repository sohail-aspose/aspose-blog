---
title: 'Aspose.Words for Reporting Services 3.0.4 Released'
date: Tue, 16 Jun 2009 23:06:00 +0000
draft: false
url: /2009/06/16/aspose-words-for-reporting-services-3-0-4-released/
author: DmitryV
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---

We have released a new hotfix of Aspose.Words for Reporting Services. It addresses a number of issues and also introduces the new **SpacingFactor** configuration setting.

What is the new setting for? Imagine you have a report that you export to a Microsoft Word document via Aspose.Words. The default layout mode is flow mode that means the docuemnt consists of "normal" paragraphs and tables. Alas, this mode has a trade-off: we cannot set coordinates of document items explicitly, so we only may assume page contents will actually fit the page. Sometimes the contents may "flow" off the page and push the ending page break to the subsequent page, causing excessive (usually blank) pages to appear.

If you notice this happens in your case, try setting **SpacingFactor** to a value less than 1.0, say to 0.9 or 0.75. It will reduce spacing between report (document) items thus making page contents more compact. Decrease the value until you confirm there are no more excessive pages in the resulting document.

To download the hotfix, please visit

[http://www.aspose.com/community/files/52/ssrs-rendering-extensions/aspose.words-for-reporting-services/default.aspx][1]




[1]: http://www.aspose.com/community/files/52/ssrs-rendering-extensions/aspose.words-for-reporting-services/default.aspx





---
title: 'Configure Individual Reports with Aspose.Words for Reporting Services 3.3.0'
date: Tue, 10 Nov 2009 03:30:00 +0000
draft: false
url: /2009/11/10/configure-individual-reports-with-aspose-words-for-reporting-services-3-3-0/
author: DmitryV
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---

When exporting RDL reports to Microsoft Word documents, you can configure the export by specifying different configuration settings. You can control document layout, page breaks, page orientation, and so on.

There is one noticeable drawback, though. You can only configure the export at a Reporting Services instance level. That means you modify the rsreportserver.config file and it affects all the reports processed by the instance. But what if you have a single report that, for example, contains a text on top of an image and you want to export this report in positioned layout mode, while the rest should derive default settings?

This was impossible until Aspose.Words for Reporting Services 3.3.0. Now you can specify configuration XML right in the report which will affect this report only. To know more, please read the **Report level configuration** section in the following documentation topic:

http://www.aspose.com/documentation/ssrs-rendering-extensions/aspose.words-for-reporting-services/configuration-explained.html

To download Aspose.Words for Reporting Services 3.3.0, please visit

[http://www.aspose.com/community/files/52/ssrs-rendering-extensions/aspose.words-for-reporting-services/default.aspx][1]




[1]: http://www.aspose.com/community/files/52/ssrs-rendering-extensions/aspose.words-for-reporting-services/default.aspx





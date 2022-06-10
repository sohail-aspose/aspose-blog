---
title: 'How to Report Aspose.Words for Reporting Services Issues Efficiently'
date: Wed, 25 Apr 2007 01:44:00 +0000
draft: false
url: /2007/04/25/74263/
author: DmitryV
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---

[Aspose.Words for Reporting Services][1] is not a typical component such as [Aspose.Words][2] or other products from the Aspose family. It is a rendering extension for Microsoft SQL Server 2005 Reporting Services and it does not provide public API types except those required for intercommunication with SQL Server. Apart of this fact, there is another important peculiarity that affects the way of reporting and addressing technical issues, so let me cover this point.

In order to quickly resolve an issue reported by the users, the developer should be able to reproduce it first. This allows to detect the exact place where error retains and make appropriate changes in the code. That's why we often ask to attach original documents, for example, in Aspose.Words support forum. (I must admit many of you do attach documents to reproduce without the need to remind, thank you for that!). Having customers' input as the base for numerous regression tests makes sure the product becomes better and better without getting back to old flaws.

But in Aspose.Words for Reporting Services the situation is different. The problem is that the RDL reports (which are the source to be rendered) are not stand-alone documents. Each report refers to a data source used to retrieve the data that populates the report. Moreover, the report may not contain an SQL query used to fetch the data but simply involve a stored procedure instead. This basically means that the report depends on the corresponding data source and ideally they should be supplied together when reporting issues. This would allow us to reproduce the problem exactly as it occurs on your side and guarantee we will fix it shortly.

However, we do realize that providing a data source together with the report is not always easy and sometimes is not feasible. The reasons that may make the task hard are:

*   The database may contain sensitive data and you will be forced to replace it with dummy values.
*   The database may be huge.
*   Supplying both .rdl report and the corresponding data source requires some additional steps such as exporting the database, zipping the files etc.

That is why we thought that we would be able to replicate most of the issues without having the data sources on hand. We have decided to avoid requesting the data source from you unless the error cannot be reproduced without having the report filled with exact data values. So the algorithm of efficient reporting of the product issues is:

1.  Attach the .rdl report(s) that cause the issue(s) to your post in the [Aspose.Words support forum][3]. You can also attach the resulting Microsoft Word documents produced by the rendering extension, but this is not a requirement. Describe the problem; specify what error you get, what document formatting is incorrect etc.
2.  We will try to replicate the issue and tell you the result (fixed, logged etc) or, if we fail to recreate it on our side, request your data source. The details of sending the data source may be different depending on the particular situation. A neat way of extracting a database to send is backing it up to a single disk file.

Of course, if you are able to provide the data source without any problems at once - we will certainly appreciate it as it maximizes the chance to get rid of the issue immediately; but otherwise just send us your .rdl files and that's it. Anyway, whenever you experience an issue caused by Aspose.Words for Reporting Services, just report it and we will eliminate it shortly. Each reported issue makes the product better… and you are who help us in it. Thank you for that!




[1]: https://blog.aspose.com/
[2]: https://www.aspose.cloud/templates/aspose/App_Themes/V3/images/total/272x272/aspose_total-for-net-min.png
[3]: https://forum.aspose.com/





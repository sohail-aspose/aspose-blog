---
title: 'Changes in Aspose.Cells for Reporting Services V1.1.1'
date: Thu, 27 Mar 2008 23:34:00 +0000
draft: false
url: /2008/03/27/changes-in-aspose-cells-for-reporting-services-v1-1-1/
author: Laurence
summary: ''
tags: []
categories: ['Aspose.Cells Product Family']
---

In Aspose.Cells for Reporting Service v1.1, we provide a client tool to enable users to design reports in MS Excel. This tool is an Excel addin and we developed it totally with C#.

Because we develop the tool in C#, we have to use Excel interop to manipulate files. Some users found problems when using the client tool in their MS Excel. After investigating their problems, we found most of problem are caused by MS Office, Office PIA, .NET Framework or others. When they installed corresponding MS' patches, problems are solved.

However, this does bring troubles for installation and deployment. So in v1.1.1, we use VBA to make UI of client tool and use C# to develop other features. That removes dependency on Excel PIA. We think that can make installation and deployment more easy.

Some users may ask: why don't you make a .NET tool totally independent of Excel? We think MS Excel is an excellent desktop application for daily use. Using it as a design tool can save user's efforts for learning.









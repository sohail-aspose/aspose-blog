---
title: 'Improved Project Data Rendering using Aspose.Tasks for .NET 6.7.0'
date: Fri, 30 May 2014 18:12:40 +0000
draft: false
url: /2014/05/30/improved-project-data-rendering-using-aspose.tasks-for-.net-6.7.0/
author: Kashif Iqbal
summary: ''
tags: []
categories: ['Aspose.Tasks Product Family']
---

[![][1]](https://blog.aspose.com/wp-content/uploads/sites/2/2014/05/aspose-Tasks-for-net_100.png)We are pleased to announce the release of Aspose.Tasks for .NET 6.7.0. As a result of our continuous efforts to bring further improvements to the API, this month’s release includes a number of bug fixes and enhancements that further adds to the value of the API. To get further details about what is new and fixed, you can visit the Aspose.Tasks [download page][2] and refer to the release notes. You'll find a summary of some of the improvements below.

# Controlling Sub-Tasks Printing During Rendering

Summary tasks are common in Microsoft Project documents where a number of child tasks are grouped together under a parent task. While printing such a document, Microsoft Project retains the existing state of the sub-tasks, that is they are printed to output if the parent summary tasks are expanded in document as well. The Aspose.Tasks API allows retrieving this state using a task’s IsExpanded property. This month’s release mimics Microsoft Project’s behavior while rendering project task data using this property which determines whether summary sub-tasks are to be rendered to output or not. If set to true, the summary sub-tasks are rendered to the output, if false, they are not. In addition, to render a project's root task, the project level property ShowProjectSummaryTask has been added to the Project class in this month’s release.

# Bug Fixes and Other Improvements

This month's release also includes a number of fixes to issues reported by our customers using the previous version. This includes issues related to wrong split task count reading, project calendar reading and work type resources. This further improves the overall functionality of the API.

If you want to share any feedback with respect to Aspose.Tasks, please feel free to write to us on [Aspose.Tasks forum][3]. We’ll be glad to address your concerns and assist you.




[1]: https://blog.aspose.com/wp-content/uploads/sites/2/2014/05/aspose-Tasks-for-net_100.png "aspose-Tasks-for-net_100"
[2]: http://www.aspose.com/community/files/51/.net-components/aspose.tasks-for-.net/category1112.aspx
[3]: https://forum.aspose.com/c/tasks





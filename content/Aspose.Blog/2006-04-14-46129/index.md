---
title: 'Aspose.Workflow 1.1.6.0 HotFix Released'
date: Fri, 14 Apr 2006 02:14:00 +0000
draft: false
url: /2006/04/14/46129/
author: Stonewell
summary: ''
tags: ['Stone Well']
---

Dear Customers,  
    We have released Aspose.Workflow 1.1.6.0, it contains:

1.  Several small bugs are fixed in designer.
2.  Added a new feature called "DynamicJoin", it must use with "DynamicFork" feature at the same time.  
     when add the "AssignmentType.DynamicJoin" extended attribute to an activity, the value of the extened attribute will change the behavior of how to finish current activity and go to next activity. The value of "AssignmentType.DynamicJoin" can be one of belows:
    *   "AND": only when all "DynamicFork" tasks finished, the current activity will be finished, and Aspose.Workflow engine will go to next activity.
    *   "XOR": when one of the "DynamicFork" tasks finsihed, all other "DynamicFork" tasks will be aborted. Aspose.Workflow engine will finish current activity and go to next activity.
    *   "StandAlone": when One of the "DynamicFork" tasks finsihed, Aspose.Workflow will run into next activity, but all other tasks are leave there, current activity finshed only when all tasks have been finished.

If an activity has the "AssignmentType.DynamicFork" but doesn't have the "AssignmentType.DynamicJoin", it will use "StandAlone" by default.

The new release can be downloaded here [http://www.aspose.com/Downloads/Aspose.Workflow/Default.aspx][1]

Regards,  
Stone




[1]: http://www.aspose.com/Downloads/Aspose.Workflow/Default.aspx




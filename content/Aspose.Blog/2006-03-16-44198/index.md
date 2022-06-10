---
title: 'Aspose.Workflow 1.1.4.0 HotFix Released!'
date: Thu, 16 Mar 2006 23:12:00 +0000
draft: false
url: /2006/03/16/44198/
author: Stonewell
summary: ''
tags: ['Stone Well']
---

Dear Customers,

     We have released Aspose.Workflow 1.1.4.0 hotfix, it contains

*   Some SQL execution is not prepared, it take long time to finish, now it is fixed
*   Add new API in IPackageAdmin interface, RemoveAllUnusedPackage(),  it used to remove all packages from the repository, which didn't have any running process instance or there are no any other package refernece the package.
*   Add new feature to the Activity whose join type is "XOR", when add a extended attribute "JoinType.EndTaskOnOtherTransition" to the activity whose join type is "XOR", when the activity started, Aspose.Workflow will end all other tasks on other transitions connected to the current "Join" activity, this feature is request by customer.
*   Add "Dynamic Fork" feature, when add a extended attribute "AssignmentType.DynamicFork" to an activity, Aspose.Workflow will create a task for each performers instead of create single task for all performers. this feature is also request by customer
*   Some small graph/editing bugs fixed in Designer

Please goto http://www.aspose.com/Community/Downloads/ to get the newest version

Regards,

Stone








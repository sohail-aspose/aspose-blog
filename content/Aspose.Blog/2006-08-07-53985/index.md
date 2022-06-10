---
title: 'Aspose.Workflow Hotfix 1.2.4.0 Released!'
date: Mon, 07 Aug 2006 06:35:00 +0000
draft: false
url: /2006/08/07/53985/
author: Stonewell
summary: ''
tags: ['Stone Well']
---

Dear Customers,

   We have released the Aspose.Workflow Hotfix 1.2.4.0, it contains:

Feature Added:

*   New API IWorklist2.GetAllTasks(params string\[\] ids), get other user's tasks and API to get all tasks of users in one group
*   New Method in EngineManager, EngineManager.GetNewInstance(), Return a new instance of EngineManager, user can use this new instance to connect to other database or use different configuration in one OS-process.

Bug Fixed:

*   Update the IQueryService document
*   Remove no needed transaction creation to avoid dead lock.
*   Caching the compiled script assembly to increase performance.
*   Obsolete some APIs.

Database Changes

*   Add Workflow\_GetProcessVariables and Workflow\_GetActivityVariables for SQLServer Only.
*   Add a set of script for SQLServer to create all varchar fields using nvarchar.

Please go to http://www.aspose.com/Downloads/Aspose.Workflow/Default.aspx to get the newest version

Regards,

Stone








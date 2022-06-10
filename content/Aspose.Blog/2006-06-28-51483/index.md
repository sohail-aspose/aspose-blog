---
title: 'Aspose.Workflow 1.2.1.0 Hotfix Released'
date: Wed, 28 Jun 2006 02:28:00 +0000
draft: false
url: /2006/06/28/51483/
author: Stonewell
summary: ''
tags: ['Stone Well']
---

Dear customers,

   We have released Aspose.Workflow 1.2.1.0, It contains

Feature added:

*   Designer can access the external reference package now.
*   Recent file list add to Designer
*   New APIs to update the variables directly IProcessInstance.UpdateVariable, IProcessInstance.UpdateVarabiles.
*   New API to test if a process instance is a subflow, IProcessInstance.IsSubflow
*   New API IWorklist2.CompleteTaskEx2 with a IRuntimeCallback parameter to let user can decide performer and next activity at runtime.
*   Add an API to return package/Process level variables  
      IPackage.GetAllVariableIdNameMap IProcess.GetAllVariableIdNameMap
*   Add an API to return latest version of packages. IPackageAdmin.GetAllPackagesLatestVersion
*   Add an API add to IPackge to return all versions. IPackage.AvailableVersions
*   Add an API to return instance for all versions package  
      GetProcessInstanceListForAllVersion GetPackageProcessInstanceListForAllVersion
*   Add ProcessInstance.Cache.Size to configuration file, set Process.Cache.Size to 0 will disable cache.
*   Query API for filter datafields, change the database table to plain table. Add IQueryService API.
*   New API to return all user's history task, IHistoryAdmin.GetTaskHistoriesByUser

Bug Fixed:

*   Join/fork node with no transition connected will not show correctly in designer, now it fixed
*   Two packages with applcations which has same Id, then SetApplicationMapping didn't work. now it fixed.
*   IHistoryAGetInstanceTaskHistories return Tasks in non-correct order, now it fixed to return in desc order,which means the newest tasks placed at index 0.
*   Update database scripts for SQLServer 2005
*   RemoveUserFromGroup doesn't work, now it is fixed
*   IPackage.GetAllPackages will return duplicated IPackage object, now it fixed.
*   When engine start, Aspose.Workflow will always update the processstate and activitystate table using default value, now it fixed to only use default value when the states not exists.

Please goto http://www.aspose.com/Downloads/Aspose.Workflow/Default.aspx to get the latest version

Regards,

Stone








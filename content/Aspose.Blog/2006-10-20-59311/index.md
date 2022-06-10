---
title: 'Aspose.Workflow HotFix 1.2.8.0 Released!'
date: Fri, 20 Oct 2006 07:41:00 +0000
draft: false
url: /2006/10/20/59311/
author: Stonewell
summary: ''
tags: ['Stone Well']
---

Dear Customers,

   We have released Aspose.Workflow HotFix 1.2.8.0,  it contains:

Database Changes:

*   Updated store-procedure for SQLServer
    *   Workflow\_DeleteProcess.sql
*   Newly added store-procedure for SQLServer
    *   Workflow\_GetPackage\_D\_Proc.sql
    *   Workflow\_GetPackage\_DR\_Proc.sql
    *   Workflow\_GetPackage\_DRV\_Proc.sql
    *   Workflow\_GetPackage\_DV\_Proc.sql
    *   Workflow\_GetProcess\_D\_Proc.sql
    *   Workflow\_GetProcess\_DR\_Proc.sql
    *   Workflow\_GetProcess\_DRV\_Proc.sql
    *   Workflow\_GetProcess\_DV\_Proc.sql
    *   Workflow\_GetAll\_DR\_Proc.sql
    *   Workflow\_GetAllForProcess.sql
    *   Workflow\_GetAllForPackage.sql
    *   Workflow\_GetAll\_R\_Proc.sql
    *   Workflow\_GetProcess.sql
    *   Workflow\_GetAllProcess.sql
    *   Workflow\_GetPackage\_S\_Proc.sql
    *   Workflow\_GetProcess\_SV\_Proc.sql
    *   Workflow\_GetPackage\_SV\_Proc.sql
    *   Workflow\_GetProcess\_S\_Proc.sql
    *   Workflow\_GetAll\_D\_Proc.sql
    *   Workflow\_GetProcess\_Act.sql
    *   Workflow\_GetProcess\_A\_Act.sql
    *   Workflow\_GetActivity.sql  
        

Feature Added:

*   Add new APIs for query delayed process instance in IInstanceAdmin:
    *   IProcessInstance\[\] GetAllDelayedProcessInstanceList(bool runningOnly);
    *   IProcessInstance\[\] GetPackageDelayedProcessInstanceList(string packageId, string packageVersion, bool includeAllVersion, bool runningOnly);
    *   IProcessInstance\[\] GetProcessDelayedProcessInstanceList(string packageId, string packageVersion, string processId, bool includeAllVersion, bool runningOnly);  
        

*   Add new property ActivationTime on ITask and ITaskHistory interface  
    
*   Add a new interface IAssignmentsManagerEx, using this interface just same as IAssignmentsManager, but it can replace single user with multipal replacement users.

Bug Fixed:

*   Deisnger doesn't allow connect two activity with multipal transitions, now it fixed.

Please get the newest version from http://www.aspose.com/Downloads/Aspose.Workflow/Default.aspx

Regards,

Stone








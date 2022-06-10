---
title: 'Aspose.Workflow Hotfix 1.2.2.0 Released!'
date: Wed, 12 Jul 2006 06:10:00 +0000
draft: false
url: /2006/07/12/52382/
author: Stonewell
summary: ''
tags: ['Stone Well']
---

Dear Customers,

   We have released Aspose.Workflow 1.2.2.0, it contains:

Feature Added:

*    Add PackageAdmin.DoesPackageExists method
*   Add ITaskHistory.ReservedBy
*   Add LastTaskId LastTaskPerformer ProcessVariables to the IRuntimeArgs
*   Add customized IAssignmentsManager to let user customize the assignments, Add a property in the configuration file to let the Aspose.Workflow using customized AssignmentManager.

          AssignmentsManager.Implementation.Type= Customer.CustomizedAssignmentManager

         the Customer.CustomeizedAssignmentManager must implements Aspose.Workflow.Engine.IAssignmentsManager interface

*   Access DataField's Extended Attributes IProcess.GetVariableExtendedAttributes
*   Add PackageId PackageVersion ProcessId To ITaskHistory
*   Add DoesProcessInstanceExist to IInstanceAdmin  
    

Bug Fixed:

*   When using QueryServices under MS Access database, the query will fail, now it fixed.

Please goto http://www.aspose.com/Downloads/Aspose.Workflow/Default.aspx to get the newest version.

Regards,

Stone








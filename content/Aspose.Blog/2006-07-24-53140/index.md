---
title: 'Aspose.Workflow HotFix 1.2.3.0 Released!'
date: Mon, 24 Jul 2006 09:07:00 +0000
draft: false
url: /2006/07/24/53140/
author: Stonewell
summary: ''
tags: ['Stone Well']
---

Dear Customers:

    We have released the Aspose.Workflow Hotfix 1.2.3.0, it contains,

Feature Added:

*   Wait Activity

               When the activity has an extended attribute called "Activity.Wait.Condition", Aspose.Workflow will treat the value of extended attribute as a condition expression, which written in VB.Net, and the engine will automatically start the Task when the condition expression evaluated to be true.

Bug Fixed:

*   Save the process definition name in the processdefinition table
*   When the data fields' name has some invalid characters, such as "-", "+", "\*", the engine will report error, now it fixed, user have to use AsposeWorkflow\_DataFields("DataField\_Name") to access the datafield in condition or expression instead of directly put the data field name in the XPDL.
*    Add a flag in activities table to see if it is delayed.  
     Add ITask.Delayed,ITaskHistory.Delayed to indicate if the task has exceed its deadline.
*   Add delayed to process process\_history  
    Add IProcessInstance.Delayed IProcessInstanceHistory.Delayed
*   When there are invalid processid in the database, the lock will fail, now it fixed.
*   When Property return empty string instead of null in the IEngineConfiguration interface, the InitCaches method will fail. now it fixed.

Database Changes:

*   Database Table Change:

1.  Add delayed CHAR(1) To activities table
2.  Add delayed CHAR(1) To activities\_history table
3.  Add processdefinitionname VARCHAR(255) to processdefinitions table
4.  Add delayed CHAR(1) To processes table
5.  Add delayed CHAR(1) To processes\_history table

*   Store Procedure Change, Update the following store procedures:

1.  Workflow\_DeleteProcess
2.  Workflow\_SaveProcess
3.  Workflow\_SaveProcessDefinition
4.  Workflow\_SaveActivity

Please goto http://www.aspose.com/downloads to get the newest version

Regards,

Stone








---
title: 'Aspose.Workflow 1.2.0.0 Released'
date: Mon, 05 Jun 2006 02:29:00 +0000
draft: false
url: /2006/06/05/49637/
author: Stonewell
summary: ''
tags: ['Stone Well']
---

Dear Customers,

   We have released the Aspose.Workflow 1.2.0.0, it contains

Feature Added:

*   PackageAdmin/InstanceAdmin now can work on different package versions. Please refer to the APIs of IPackageAdmin and IInstanceAdmin
*   User now can configure the Aspose.Workflow database table name, please refer to the wiki page. http://www.aspose.com/Wiki/default.aspx/Aspose.Workflow/CustomizedDatabaseTableNameQA.html
*   Table struct change of Application Mapping and Participant mapping, to reflect on the new feature of Package version

Changes made:

*   GetProcessInstanceList didn't accept processId and PackageId with null. not it fixed, when both parameter is null return all instance in current system. if process id is null, return package instance list.
*   obsolete some APIs, because add new API can operate on different package version.
*   Change Demo ContractWorkflow, the table "Contacts" to "Contracts"
*   Add API to IPackageAdmin, now UploadPackage accept parameter "System.io.Stream" or a string conains the package's content.
*   Add new API Using application config section to configure Aspose.Workflow, http://www.aspose.com/Community/Forums/48658/ShowPost.aspx
*   Package.Participants will not return the participant with same id but in different process, not it is fixed
*   Actual parameter is not displayed correct Designer, now it fixed
*   Update the document of ITask.Status, list the avaliable values.








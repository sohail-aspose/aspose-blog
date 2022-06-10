---
title: 'Aspose.Workflow HotFix 1.2.7.0 Released!'
date: Fri, 29 Sep 2006 08:55:00 +0000
draft: false
url: /2006/09/29/57806/
author: Stonewell
summary: ''
tags: ['Stone Well']
---

Dear Customers,

   We have released Aspose.Workflow HotFix 1.2.7.0,  it contains:

Behavior Changes:

*   All Activity whoes start mode set to "Automatic" will be treated as "automatic" execute activity. The old implementation has different behavior based on if the activity has ToolAgent defined.

Feature Added:

*   Designer panel now has scroll bars.
*   Add a cache for the IActivity object.
*   Add IPackgeAdmin.ReplacePackage API,  This api will replace the existing version package using the new XPDL, and UpdatePackage API will always create a new version.

Bug Fixed:

*   Fixed a bug, when automatically running process end with exception, if the state already change to completed, don't change to terminate.
*   Update the process context when load the already existing process. 

Please get the newest version from http://www.aspose.com/Downloads/Aspose.Workflow/Default.aspx

Regards,

Stone[](/)








---
title: 'Aspose.Workflow HotFix 1.2.10.0 Released!'
date: Mon, 27 Nov 2006 05:23:00 +0000
draft: false
url: /2006/11/27/62107/
author: Stonewell
summary: ''
tags: ['Stone Well']
---

Dear Customers,

   We have released Aspose.Workflow 1.2.10.0, it contains

Bug Fixed:

*   When using CompleteTaskEx to set "Next" activity id, user can only to set "Next" activity which in the same activity block. now it fixed to

*   "Next" activity is in same activity block
*   "Next" activity who is not in the same activity block but in the Process activities.
*   "Next" activity is in other activity block which is not same as current block.  To set "Next" activity in other block, user have to provide a "path" to the target activity. and the first element of the parameter array must be the EngineManager.JUMP\_PATH\_ACTIVITY\_ID, and other elements should be the path to target activity. for example, if want to set "Next" activity to the activity A which in Block B1, and Block B1 is in Block B2, and block B2 is in process activities. the array should look like: new string\[\] { EngineManager.JUMP\_PATH\_ACTIVITY\_ID, "B2", "B1", "A" }

Regards,

Stone








---
title: 'Aspose.Tasks for Java 6.7.0 Provides Improved Rendering Capabilities'
date: Mon, 02 Jun 2014 09:16:29 +0000
draft: false
url: /2014/06/02/aspose.tasks-for-java-6.7.0-provides-improved-rendering-capabilities/
author: Kashif Iqbal
summary: ''
tags: []
categories: ['Aspose.Tasks Product Family']
---

[![][1]](https://blog.aspose.com/wp-content/uploads/sites/2/2014/06/aspose-Tasks-for-Java_100.png)We are pleased to announce the release of Aspose.Tasks for Java 6.7.0 that includes enhancement and bug fixes as ported from its equivalent .NET version.  This month’s release provides users with the capability to render sub-tasks based on the parent summary task. To get further details about what is new and fixed, please reference to our [product download][2] page. If you have any feedback, you are more than welcome to write to us over Aspose.Tasks forum. We’ll be glad to address these and assist you.

## Printing Sub-Tasks During Rendering

The last version of Aspose.Tasks for Java 6.6.0 had the capability to read the “IsExpanded” property of a Summary task but this information was never used to determine the rendering of sub-tasks to output when rendering a Project document. Microsoft Project, however, retains the information available in this property and renders the sub-tasks only when the parent task is in expanded form. With this month’s release, Aspose.Tasks Java API now takes into account this information and renders the sub-tasks to output only if the parent summary task is in expanded form. If the IsExpanded property is set to true, the sub-tasks will be rendered to output and vice versa.

## Bug Fixes and Improvements

This month’s release also fixes a number of issues that were found and reported with the previous version of Aspose.Tasks. These include issues related to wrong split task count reading, project’s calendar reading and Work Type resources. This further aids to the value of the API and brings improvement to the overall functionality.




[1]: https://blog.aspose.com/wp-content/uploads/sites/2/2014/06/aspose-Tasks-for-Java_100.png "aspose-Tasks-for-Java_100"
[2]: http://www.aspose.com/community/files/72/java-components/aspose.tasks-for-java/default.aspx





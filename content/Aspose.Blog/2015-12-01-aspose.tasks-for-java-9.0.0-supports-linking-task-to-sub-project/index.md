---
title: 'Aspose.Tasks for Java 9.0.0 supports Linking Task to Sub-Project'
date: Tue, 01 Dec 2015 15:40:38 +0000
draft: false
url: /2015/12/01/aspose.tasks-for-java-9.0.0-supports-linking-task-to-sub-project/
author: Muhammad Waqas
summary: ''
tags: []
categories: ['Aspose.Tasks Product Family']
---

[![][1]](http://www.aspose.com/java/project-management-component.aspx)

We are pleased to announce the release of Aspose.Tasks for Java 9.0.0. Ported from its equivalent .NET version, this month’s release includes the same enhancements as well as bug fixes that improve the overall API functionality. For a complete list of what is new and fixed, please visit our [product release page][2].

Enhancements and bug fixes included in this month’s release are detailed as follow.

**Linking Task to Sub-Project:** This month’s release includes the capability of linking a task to a sub-project. The earlier versions of API were able to read this information using the Tsk.SubProjectName property, but linking a task to sub-project was not supported earlier. The following code snippet shows how to link a task to a sub-project.

```
Project project = new Project("New Project 2010.mpp");

Task task = project.getRootTask().getChildren().add("Task 1");

//setting new subproject link
task.set(Tsk.SubprojectName, "Z:\\NewProductDev.mpp");

project.save("Link.mpp", SaveFileFormat.MPP); 
```

**Other Improvements:** This month’s release also includes the same bug fixes as the .NET version. Specifically, the issues fixed are related to:

*   Exception while adding resource assignments for a zero-duration task
*   Loss of calendar exception while loading saved MPP files
*   Lag in Timephased data for certain project files
*   Wrong Timephased data read against the holidays

# API Resources

*   Product Documentation – Provides complete information about system requirements, installation, Programmer’s Guide, Technical articles and API Changes
*   API Reference Guide – Provides information about the product namespaces, classes and methods
*   [GitHub Examples][3] – Ready to download and execute examples of the API
*   [Forum Support][4] – Post your queries/inquiries on Aspose.Tasks forum to get support from our technical support team.




[1]: https://blog.aspose.com/wp-content/uploads/sites/2/2015/12/aspose-Tasks-for-Java_100.png "aspose-Tasks-for-Java_100"
[2]: http://www.aspose.com/community/files/72/java-components/aspose.tasks-for-java/default.aspx
[3]: https://github.com/asposetasks/Aspose_TASKS_Java
[4]: http://www.aspose.com/community/forums/aspose.tasks-product-family/96/showforum.aspx





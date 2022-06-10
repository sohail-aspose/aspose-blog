---
title: 'Read Project IDs and Task Duration as Text with Aspose.Tasks for Java 9.1.0'
date: Wed, 30 Dec 2015 16:27:34 +0000
draft: false
url: /2015/12/30/read-project-ids-and-task-duration-as-text-with-aspose.tasks-for-java-9.1.0/
author: Kashif Iqbal
summary: ''
tags: []
categories: ['Aspose.Tasks Product Family']
---

[![][1]](http://www.aspose.com/java/project-management-component.aspx)After the release of Aspose.Tasks for .NET 9.1.0, we are pleased to announce the release of [Aspose.Tasks for Java 9.1.0][2]. This month’s release includes enhancements related to the API’s Project class for loading Primavera files from stream and reading the entire project IDs from Primavera XML files. For a complete list of API changes, please visit our Product documentation section, Public API changes.

# New Features & Enhancements

**Reading All Project IDs from Primavera Document:** A Primavera project document may contain more than one project where each project is identified by its own unique identifier (UID). Aspose.Tasks for Java now supports reading all the project ids from such a Primavera document that can then be used to access and retrieve individual project from such a file. The following sample code shows how to retrieve all project IDs from multi-project Primavera XML file.

```
PrimaveraXmlReader reader = new PrimaveraXmlReader("primaveraXml.xml");

List<Integer> listOpProjectUids = reader.GetProjectUids(); 
```

**Reading Task Duration as Text:** This month’s release also includes a new property to the Tsk class for retrieving task duration as text. This can be retrieved using the Tsk.DURATION\_TEXT property. If this field returns null, the Duration filed can be used to get the task duration as shown in the following code sample.

```
Project project = new Project("Project1.mpp");
ChildTasksCollector collector = new ChildTasksCollector();

// Collect all the tasks from RootTask using TaskUtils
TaskUtils.apply(project.getRootTask(), collector, 0);

for (Task task : collector.getTasks())
{
    String durationText = task.get(Tsk.DURATION_TEXT);
    if (durationText != null)
        System.out.prinltn(durationText);
    else 
        System.out.prinltn(task.Get(Tsk.DURATION));
} 
```

# Bug Fixes

Ported from its equivalent .NET version, Aspose.Tasks for Java includes the same bug fixes as were part of its equivalent .NET version. For details about the issues fixed in this month’s release, please visit our [product download page][3].

# API Resources

*   Product Documentation – Provides complete information about system requirements, installation, Programmer’s Guide, Technical articles and API Changes
*   API Reference Guide – Provides information about the product namespaces, classes and methods
*   [GitHub Examples][4] – Ready to download and execute examples of the API
*   [Forum Support][5] – Post your queries/inquiries on Aspose.Tasks forum to get support from our technical support team.




[1]: https://blog.aspose.com/wp-content/uploads/sites/2/2015/12/aspose-Tasks-for-Java_1001.png "aspose-Tasks-for-Java_100"
[2]: http://www.aspose.com/community/files/72/java-components/aspose.tasks-for-java/default.aspx
[3]: http://www.aspose.com/community/files/72/java-components/aspose.tasks-for-java/default.aspx
[4]: https://github.com/asposetasks/Aspose_TASKS_Java
[5]: https://forum.aspose.com/c/tasks





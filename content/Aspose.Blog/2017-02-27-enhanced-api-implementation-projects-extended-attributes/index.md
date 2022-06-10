---
title: 'Enhanced API Implementation for Project''s Extended Attributes'
date: Mon, 27 Feb 2017 15:14:13 +0000
draft: false
url: /2017/02/27/enhanced-api-implementation-projects-extended-attributes/
author: Kashif Iqbal
summary: ''
tags: []
categories: ['Aspose.Tasks Product Family']
---



{{< figure align=center src="images/Aspose.Tasks-for-Java.png" alt="">}}


We are pleased to announce the release of [Aspose.Tasks for Java 17.1.0][1]. This month’s release improves the Extended Attributes implementation of a task. The modification makes it easy to add lookup extended attributes to a task. It also fixes a number of resources reported by our valued customers with the last month’s version of the API. For a detailed note on what is new and fixed, please visit the [release notes section][2] of Aspose.Tasks for Java documentation.

## Improved Public API for Working with Custom Fields

This month’s release improves the implementation of [adding Extended attributes][3] to a task and resource. The new implementation makes it easy to create plain as well as Lookup custom fields to a project’s tasks and resources.  The following static methods of ExtendedAttributeDefinition class are provided under this new implementation.

*   CreateTaskDefinition
*   CreateResourceDefinition
*   CreateLookupTaskDefinition
*   CreationLookupResourceDefinition

The following code sample illustrates the usage of these new methods exposed by the API.

```
// Create new project
Project project = new Project(dataDir + "project.mpp");

//Create an Extended Attribute Definition of Text1 type
ExtendedAttributeDefinition taskExtendedAttributeText1Definition = ExtendedAttributeDefinition.createTaskDefinition(CustomFieldType.Text, ExtendedAttributeTask.Text1, "Task City Name");

//Add it to the project's Extended Attributes collection
project.getExtendedAttributes().add(taskExtendedAttributeText1Definition);

//Add a task to the project
Task task = project.getRootTask().getChildren().add("Task 1");

//Create an Extended Attribute from the Attribute Definition
ExtendedAttribute taskExtendedAttributeText1 = taskExtendedAttributeText1Definition.createExtendedAttribute();

//Assign a value to the generated Extended Attribute
taskExtendedAttributeText1.setValue("London");

//Add the Extended Attribute to task
task.getExtendedAttributes().add(taskExtendedAttributeText1);

project.save(dataDir + "PlainTextExtendedAttribute_out.mpp", SaveFileFormat.MPP); 
```

## Other Improvements

In addition to the improvements, this month’s release also fixes several bugs related to the API functionality. These include:

*   Working with Extended Attributes of the API
*   Lookup values error while assigning to task
*   Large file size after creating task baseline
*   Saving Extended Task Attributes to output MPP

## API Resources

*   [Product Documentation][4] – Provides complete information about system requirements, installation, Programmer’s Guide, Technical articles and API Changes
*   API Reference Guide – Provides information about the product namespaces, classes and methods
*   [GitHub Examples][5] – Ready to download and execute examples of the API
*   [Forum Support][6] – Post your queries/inquiries on Aspose.Tasks forum to get support from our technical support team.




[1]: https://downloads.aspose.com/tasks/java
[2]: https://docs.aspose.com/display/tasksjava/Aspose.Tasks+for+Java+17.1.0+Release+Notes
[3]: https://docs.aspose.com/display/tasksjava/Extended+Task+Attributes#ExtendedTaskAttributes-AddingExtendedAttributeInformationforaTask
[4]: https://docs.aspose.com/display/tasksjava/Home
[5]: https://github.com/asposetasks/Aspose_TASKS_Java
[6]: http://www.aspose.com/community/forums/aspose.tasks-product-family/96/showforum.aspx





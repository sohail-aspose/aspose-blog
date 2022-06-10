---
title: 'Improved Extended Attributes Implementation with Aspose.Tasks for .NET 17.1.0'
date: Thu, 02 Feb 2017 14:32:47 +0000
draft: false
url: /2017/02/02/improved-extended-attributes-implementation-aspose.tasks-.net-17.1.0/
author: Kashif Iqbal
summary: ''
tags: []
categories: ['Aspose.Tasks Product Family']
---



{{< figure align=center src="images/Aspose.Tasks-for-.NET_.png" alt="">}}


We are pleased to announce the release of [Aspose.Tasks for .NET 17.1.0][1]. This month’s release brings improvement to the public API for working with custom fields of a project. The new implementation makes it simple for creating extended attributes. This release also fixes a number of bugs reported with earlier version of the API. For a complete list of what is new and fixed with this release of version, please visit the [release notes section][2] of Aspose.Tasks for .NET documentation.

## Enhancements

**Improved Public API for working with Custom Fields:** Yes, we have improved the public API for working with custom fields i.e. Tasks as well as Resources. The improved version of this API simplifies adding an extended attribute definition to project and create extended attribute from this definition. The new implementation provides individual implementations for working with plain and lookup custom fields. The following static methods of [ExtendedAttributeDefinition][3] class allow the creation of each type of extended attribute.

*   [Create Task Definition][4]
*   [CreationResourceDefinition][5]
*   [CreateLookupTaskDefinition][6]
*   [CreateLookupResourceDefinition][7]

The sample below shows a basic illustration of this improved implementation for creating a Task lookup extended attribute. Code sample, for working with plain task and resource as well as resource lookup extended attribute can be referred to in our [documentation article][8].

```
Project project1 = new Project(dataDir + "Blank2010.mpp");

//Create an Extended Attribute Definition of Text2 type
var taskExtendedAttributeText2Definition = ExtendedAttributeDefinition.CreateLookupTaskDefinition(CustomFieldType.Text, ExtendedAttributeTask.Text2, "Task Towns Name");

//Add lookup values for the extended attribute definition
taskExtendedAttributeText2Definition.AddLookupValue(new Value { Id = 1, StringValue = "Town1", Description = "This is Town1" });
taskExtendedAttributeText2Definition.AddLookupValue(new Value { Id = 2, StringValue = "Town2", Description = "This is Town2" });

//Add it to the porject's Extended Attributes collection
project1.ExtendedAttributes.Add(taskExtendedAttributeText2Definition);

//Add a task to the project
var task2 = project1.RootTask.Children.Add("Task 2");

//Crate an Extended Attribute from the Text2 Lookup Definition for Id 1
var taskExtendedAttributeText2 = taskExtendedAttributeText2Definition.CreateExtendedAttribute(taskExtendedAttributeText2Definition.ValueList[1]);

//Add the Extended Attribute to task
task2.ExtendedAttributes.Add(taskExtendedAttributeText2);

project1.Save(dataDir + "TextExtendedAttributeWithLookup_out.mpp", SaveFileFormat.MPP); 
```

## Other Improvements

This month’s release also fixes several bugs that improves the overall API functionality. These touch different functional areas of the API, including:

*   Working with Extended Attributes of the API
*   Lookup values error while assigning to task
*   Large file size after creating task baseline
*   Saving Extended Task Attributes to output MPP

## API Resources

You may visit the following API resources for getting started and working with the API.

*   [Product Documentation][9] – Detailed API documentation with code examples and details about API functional areas
*   [API Reference Guide][10] – Detailed information about the API namespaces and classes
*   [GitHub Examples][11] – Ready to run code samples in downloadable form
*   [Aspose.Tasks Forum][12] – Our online support forum where we address your queries and inquiries




[1]: https://downloads.aspose.com/tasks/net
[2]: https://docs.aspose.com/display/tasksnet/Aspose.Tasks+for+.NET+17.1.0++Release+Notes
[3]: https://www.aspose.com/api/net/tasks/aspose.tasks/extendedattributedefinition
[4]: https://www.aspose.com/api/net/tasks/aspose.tasks/extendedattributedefinition/methods/createtaskdefinition
[5]: https://www.aspose.com/api/net/tasks/aspose.tasks/extendedattributedefinition/methods/createresourcedefinition
[6]: https://www.aspose.com/api/net/tasks/aspose.tasks/extendedattributedefinition/methods/createlookuptaskdefinition
[7]: https://www.aspose.com/api/net/tasks/aspose.tasks/extendedattributedefinition/methods/createlookupresourcedefinition
[8]: http://docs.aspose.com/display/tasksnet/Working+with+Extended+Task+Attributes#WorkingwithExtendedTaskAttributes-AddingExtendedAttributeInformationforaTask
[9]: https://docs.aspose.com/display/tasksnet/Home
[10]: http://www.aspose.com/api/net/tasks
[11]: https://github.com/asposetasks/Aspose_Tasks_NET
[12]: https://forum.aspose.com/c/tasks





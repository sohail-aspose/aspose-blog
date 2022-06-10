---
title: 'Adding Extended Attributes to Resource Assignments using Aspose.Tasks for .NET 18.6'
date: Tue, 19 Jun 2018 04:35:13 +0000
draft: false
url: /2018/06/19/adding-extended-attributes-to-resource-assignments-using-aspose.tasks-for-.net-18.6/
author: Kashif Iqbal
summary: ''
tags: []
categories: ['Aspose.Tasks Product Family']
---



{{< figure align=center src="images/Aspose.Tasks-for-.NET_.png" alt="">}}


We are pleased to announce the release of [Aspose.Tasks for .NET 18.6][1]. This release introduces a new feature of writing extended attributes information to resource assignments similar to tasks and resources. It also improves the overall API functionality by fixing issues reported with the previous version of the API. For a detailed note on what is new and fixed, please visit the [release notes][2] section of API documentation.

## Adding Extended Attributes to Resource Assignments

Aspose.Tasks API already had the capability to add extended attributes to tasks and resources in a project. This month’s release introduces the capability to add extended attributes information to resource assignments as well. Extended Attributes can be added to resource assignments as [plain][3] as well as [lookup][4] values. The ollowing examples show adding these two type of extended attributes to the project.

### Adding Extended Attribute```
Project project = new Project(dataDir + "Blank2010.mpp");

// Add new task and resource
Task task1 = project.RootTask.Children.Add("Task");
Resource rsc1 = project.Resources.Add("Rsc");

// Assign the resource desired task
ResourceAssignment assn = project.ResourceAssignments.Add(task1, rsc1);

var assignment = project.ResourceAssignments.First();

// Custom attributes which is visible in "Resource Usage" view can be created with ExtendedAttributeDefinition.CreateResourceDefinition method.
{
    ExtendedAttributeDefinition resCostAttr = ExtendedAttributeDefinition.CreateResourceDefinition(
        CustomFieldType.Cost,
        ExtendedAttributeResource.Cost5,
        "My cost");

    project.ExtendedAttributes.Add(resCostAttr);

    var value = resCostAttr.CreateExtendedAttribute();
    value.Value = "1500";

    assignment.ExtendedAttributes.Add(value);
}

// Custom attributes which is visible in "Task Usage" view can be created with ExtendedAttributeDefinition.CreateTaskDefinition method
{
    ExtendedAttributeDefinition resCostAttr2 = ExtendedAttributeDefinition.CreateTaskDefinition(
        CustomFieldType.Cost,
        ExtendedAttributeTask.Cost5,
        "My cost for task");

    project.ExtendedAttributes.Add(resCostAttr2);

    var value = resCostAttr2.CreateExtendedAttribute();
    value.Value = "2300";

    assignment.ExtendedAttributes.Add(value);
}

project.Save(dataDir + "AddExtendedAttributesToResourceAssignment_out.mpp", SaveFileFormat.MPP); 
```

### Adding Extended Attribute as Lookup Value```
Project project = new Project(dataDir + "Blank2010.mpp");

var assignment = project.ResourceAssignments.First();

{
    ExtendedAttributeDefinition resCostAttr = ExtendedAttributeDefinition.CreateLookupResourceDefinition(
        CustomFieldType.Cost,
        ExtendedAttributeResource.Cost5,
        "My lookup cost");

    var value1 = new Value { NumberValue = 1500, Description = "Val 1", Id = 1, Val = "1500" };

    resCostAttr.AddLookupValue(value1);

    resCostAttr.AddLookupValue(new Value
    {
        NumberValue = 2500,
        Description = "Val 2",
        Id = 2
    });

    project.ExtendedAttributes.Add(resCostAttr);

    var value = resCostAttr.CreateExtendedAttribute(value1);
    value.Value = "1500";
    project.Save(dataDir + "AddExtendedAttributesToRAWithLookUp_out.mpp", SaveFileFormat.MPP); 
```

## API Resources

You may visit the following API resources for getting started and working with the API.

*   [Product Documentation][5] – Detailed API documentation with code examples and details about API functional areas
*   [API Reference Guide][6] – Detailed information about the API namespaces and classes
*   [GitHub Examples][7] – Ready to run code samples in downloadable form
*   [Aspose.Tasks Forum][8] – Our online support forum where we address your queries and inquiries




[1]: https://www.nuget.org/packages/Aspose.Tasks/
[2]: https://docs.aspose.com/display/tasksnet/Aspose.Tasks+for+.NET+18.6+Release+Notes
[3]: https://docs.aspose.com/display/tasksnet/Adding+Extended+Attributes+to+Resource+Assignments#AddingExtendedAttributestoResourceAssignments-AddingExtendedAttributestoResourceAssignment
[4]: https://docs.aspose.com/display/tasksnet/Adding+Extended+Attributes+to+Resource+Assignments#AddingExtendedAttributestoResourceAssignments-AddingLookupExtendedAttributestoResourceAssignment
[5]: https://docs.aspose.com/display/tasksnet/Home
[6]: http://www.aspose.com/api/net/tasks
[7]: https://github.com/asposetasks/Aspose_Tasks_NET
[8]: https://forum.aspose.com/c/tasks





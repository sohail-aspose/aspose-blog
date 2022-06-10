---
title: 'Create MS Project Files Programmatically in C# or VB.NET'
seoTitle: "Create MS Project Files (.mpp) in C# | Add Tasks, Resources, or Calenders"
description: "C# examples to create MS Project's MPP, MPT and XML files programmatically. Add tasks and resources to projects using C# in ASP.NET. MS Project Library."
date: Tue, 05 May 2020 15:17:04 +0000
draft: false
url: /2020/05/05/create-ms-project-files-programmatically-add-tasks-and-resources-in-csharp-asp.net/
author: Usman Aziz
summary: ''
tags: ['add calendar in ms project in csharp', 'add resources in ms project in csharp', 'add tasks in ms project in csharp', 'create mpp files programmatically using csharp', 'create ms project files using csharp']
categories: ['Aspose.Tasks Product Family']
---



{{< figure align=center src="images/aspose_tasks-min-gray-1.png" alt="">}}


[Microsoft Project][1] is a popular project management software that makes it easier for project managers to efficiently manage the projects. It lets the managers create tasks and resources, assign tasks to resources, track the project's progress, manage the budget, and perform other project-related operations. In order to create and manage MS Project files programmatically, Microsoft provides MS Office Automation. However, along with [other deficiencies][2], it requires you to install MS Office. To fill this gap, Aspose jumps in to provide you with an MS Project automation solution for .NET applications as [Aspose.Tasks for .NET][3].

Aspose.Tasks for .NET is a feature-rich API that lets you create MS Project files (.mpp/.xml) programmatically using C# or VB.NET. In addition, it offers various features to work with tasks, resources, and calendars. In this article, I'll show you how to use Aspose.Tasks for .NET to create MS Project files and work with tasks and resources using C#. The rest of the article is divided into the following sections.

*   [Create an MS Project file from scratch using C#][4]
*   [Add tasks to a Project][5]
*   [Add resources to a Project][6]
*   [Assign tasks to resources in a Project][7]
*   [Add calendars to a Project][8]

## Create MS Project Files using C# {#Create-an-MS-Project-file-from-scratch-using-Csharp}

[MPP][9] is the proprietary file format of Microsoft which is used for MS Project files. However, you can also keep project data in [XML][10] files for sharing it among different applications. Creating a new project from scratch is a simple task and can be done using the following steps:

*   Create an instance of [Project][11] class.
*   Save the file using [Project.Save(string, SaveFileFormat)][12] method.

The following code samples show how to create MS Project files using C#.

### Save MS Project Files as MPP

{{< gist aspose-com-gists 03f5fe501a33bd09b09fb5dc9210aa2f "create-mpp-file.cs" >}}

### Save MS Project Files as XML

{{< gist aspose-com-gists 03f5fe501a33bd09b09fb5dc9210aa2f "create-xml-file.cs" >}}

## Add Tasks to MS Project Files using C# {#Add-tasks-to-an-MS-Project-file-using-Csharp}

The empty MS Project file is useless without tasks and resources. So let's see how to create and add tasks to a project. A task could be a single task or summary task containing a group of subtasks in it. The following are the steps to add tasks to an MS Project file.

*   Create and initialize the [Project][13] object.
*   Add a new summary task to the project's [Tasks][14] collection using _Project.RootTask.Children.Add(string)_ method.
*   Add a subtask to the summary task using _Task.Children.Add(string)_ method.
*   Save the project using [Project.Save()][15] method.

The following code sample shows how to create and add tasks to MS Project files using C#.

{{< gist aspose-com-gists 03f5fe501a33bd09b09fb5dc9210aa2f "create-tasks.cs" >}}

The following code sample shows how to set different properties of the tasks such as duration, start date/time, etc.

{{< gist aspose-com-gists 03f5fe501a33bd09b09fb5dc9210aa2f "add-task-properties.cs" >}}

## Add Resources to MS Project Files using C# {#Add-resources-to-a-Project-file-using-Csharp}

Resources are the entities that are supposed to perform the tasks in a project. Hence, a project would not be possible without the resources to work on it. So let's check out how to create and add resources to a project. The following are the steps to add resources to an MS Project file.

*   Create a new project using the [Project][16] class.
*   Add a new resource to the project's [Resources][17] collection using _Project.Resources.Add(string)_ method.
*   Save the project using [Project.Save()][18] method.

The following code sample shows how to add resources to an MS Project file using C#.

{{< gist aspose-com-gists 03f5fe501a33bd09b09fb5dc9210aa2f "add-resources.cs" >}}

The following code sample sets the properties of a resource such as a start date/time, type, etc.

{{< gist aspose-com-gists 03f5fe501a33bd09b09fb5dc9210aa2f "set-resource-properties.cs" >}}

## Assign Tasks to Resource in a Project using C# {#Assign-Tasks-to-Resource-in-MS-Project-using-Csharp}

Once you have completed adding tasks and resources in the project, you can specify which task is to be performed by which resource. Thus, you will assign the task(s) to each resource. The following are the steps to assign tasks to resources in a Project.

*   Create or load a project using [Project][19] class.
*   Add new resources to the project and set their properties such as date format, start date, etc.
*   Add new tasks to the project and set their properties such as start date/time, duration, and etc.
*   Perform tasks assignment by adding the task and its respective resource to [Project.ResourceAssignments][20] collection.
*   Save the project using [Project.Save()][21] method.

The following is the complete code sample of how to create and assign tasks to resources in an MS Project file.

{{< gist aspose-com-gists 03f5fe501a33bd09b09fb5dc9210aa2f "assign-tasks-to-resources.cs" >}}

## Add Calendar to a Project using C# {#Add-Calendar-to-a-Project-using-Csharp}

The calendars are also one of the main entities of the projects which are used to define the project's schedule. The calendar makes it possible for the project managers to create a timeline for a project. The following are the steps to add a calendar to a project.

*   Create or load a project using [Project][22] class.
*   Add new [Calendar][23] to [Project.Calendars][24] collection.
*   Create the schedule using the _Calendar_ object.
*   Save the project.

The following code sample shows how to add a calendar to a Project using C#.

{{< gist aspose-com-gists 03f5fe501a33bd09b09fb5dc9210aa2f "add-calendar-in-project.cs" >}}

## Download or Install

You can [download][25] Aspose.Tasks for .NET DLL or install it in your project using [NuGet][26].

## Try Aspose.Tasks for .NET for Free

Aspose offers a free temporary license to try its products without trial limitations. You can get one from [here][27].

## See Also

*   [Read or Create Projects on Project Server and Project Online using C#][28]




[1]: https://en.wikipedia.org/wiki/Microsoft_Project
[2]: https://docs.aspose.com/display/tasksnet/Why+Not+Automation#WhyNotAutomation-WhyNotAutomation
[3]: https://products.aspose.com/tasks/net
[4]: #Create-an-MS-Project-file-from-scratch-using-Csharp
[5]: #Add-tasks-to-an-MS-Project-file-using-Csharp
[6]: #Add-resources-to-a-Project-file-using-Csharp
[7]: #Assign-Tasks-to-Resource-in-MS-Project-using-Csharp
[8]: #Add-Calendar-to-a-Project-using-Csharp
[9]: https://wiki.fileformat.com/project-management/mpp/
[10]: https://wiki.fileformat.com/web/xml/
[11]: https://apireference.aspose.com/tasks/net/aspose.tasks/project
[12]: https://apireference.aspose.com/tasks/net/aspose.tasks.project/save/methods/1
[13]: https://apireference.aspose.com/tasks/net/aspose.tasks/project
[14]: https://apireference.aspose.com/tasks/net/aspose.tasks/project/properties/roottask
[15]: https://apireference.aspose.com/tasks/net/aspose.tasks.project/save/methods/1
[16]: https://apireference.aspose.com/tasks/net/aspose.tasks/project
[17]: https://apireference.aspose.com/tasks/net/aspose.tasks/project/properties/resources
[18]: https://apireference.aspose.com/tasks/net/aspose.tasks.project/save/methods/1
[19]: https://apireference.aspose.com/tasks/net/aspose.tasks/project
[20]: https://apireference.aspose.com/tasks/net/aspose.tasks/project/properties/resourceassignments
[21]: https://apireference.aspose.com/tasks/net/aspose.tasks.project/save/methods/1
[22]: https://apireference.aspose.com/tasks/net/aspose.tasks/project
[23]: https://apireference.aspose.com/tasks/net/aspose.tasks/calendar
[24]: https://apireference.aspose.com/tasks/net/aspose.tasks/project/properties/calendars
[25]: http://downloads.aspose.com/tasks/net
[26]: http://nuget.org/packages/Aspose.Tasks
[27]: https://purchase.aspose.com/temporary-license
[28]: https://blog.aspose.com/2020/03/20/create-read-projects-on-project-server-and-project-online-in-csharp-asp-net/






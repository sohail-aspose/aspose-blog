---
title: 'Create MS Project Files using C++ - Add Tasks, Resources, or Calenders to Projects'
seoTitle: "Create MS Project Files mpp/xml in C++ | Add Tasks, Resources, Calender"
description: "Create MS Project files (.mpp/.xml) using C++. Learn how to add tasks, resources, calendars and resource assignments in MS Project files using C++."
date: Tue, 08 Sep 2020 22:57:00 +0000
draft: false
url: /2020/09/08/create-ms-project-mpp-xml-files-using-cpp/
author: Usman Aziz
summary: 'MS Project is a widely used project management software that helps the managers in managing their projects efficiently. It helps to create the tasks, add resources, allocate tasks to resources, monitor the progress, and manage budget-related operations. In this article, you will learn how to embed the project management activities within your applications without MS Project. With the help of code samples, you will learn how to create MS Project files (.mpp), add tasks, resources, and calendars programmatically using C++. Furthermore, the assignment of tasks to resources in a project will also be demonstrated.'
tags: ['Add Calendars in Project using Cpp', 'Add Resources to Project using Cpp', 'Add Tasks to Project using Cpp', 'Assign Projects Task to Resource using Cpp', 'Create MS Project Files (.mpp) from Scratch using Cpp']
categories: ['Aspose.Tasks Product Family']
---



{{< figure align=center src="images/aspose_tasks-min-gray-1-300x234.png" alt="Create MS Project Files in C++">}}


[MS Project][1] is a widely used project management software that helps the managers in managing their projects efficiently. It allows to create the tasks, add resources, allocate tasks to resources, monitor the progress, and manage budget-related operations. In this article, you will learn how to embed the project management activities within your C++ applications without MS Project. With the help of code samples, you will learn **how to create MS Project files (.mpp/.xml), add tasks, resources, and calendars programmatically using C++**. Furthermore, the assignment of tasks to resources in a project will also be demonstrated.

*   [C++ MS Project File Manipulation API][2]
*   [Create MS Project Files from Scratch using C++][3]
*   [Add Tasks to Project using C++][4]
*   [Add Resources to Project using C++][5]
*   [Assign Project's Task to Resource using C++][6]
*   [Add Calendars in Project using C++][7]

## C++ MS Project File Manipulation API {#C++-MS-Project-File-Manipulation-API}

[Aspose.Tasks for C++][8] is a C++ project management API that lets you create, manipulate, export, and convert MS Project files programmatically. The API provides you a complete set of features to create projects, tasks, resources, calendars, and perform other project management activities without MS Project. You can download the complete package of the API from [here][9] or install it using [NuGet][10].

## Create MS Project Files (.mpp) using C++ {#Create-MS-Project-Files-mpp-using-C++}

Lets first start by creating an empty project. The following are the steps to create an MS Project (.mpp) file from scratch using Aspose.Tasks for C++.

*   Create an object of the [Project][11] class.
*   Set the project's properties.
*   Save the project as .mpp file using [Project->Save(u"project.mpp", Aspose::Tasks::Saving::SaveFileFormat::MPP)][12] method.

The following code sample shows how to create an MS Project's _.mpp_ file using C++.

{{< gist aspose-com-gists 6a638b84f0305b6f20f1e5c176774bf8 "create-project.cpp" >}}

## Add Tasks to Project using C++ {#Add-Tasks-to-Project-using-C++}

Once you have created a project, you can proceed to add tasks to it. You can either create a new project or load an existing MS Project file to add the tasks. The following are the steps to create and add tasks or subtasks to a project.

*   Create a new project or load it from _.mpp_ file using [Project][13] class.
*   Add task to project using [Project->get\_RootTask()->get\_Children()->Add(u"Summary1")][14] method and store the newly created task into a [Task][15] object.
*   (Optional) Add a subtask to the newly created task using [Task->get\_Children()->Add(u"Subtask1")][16] method.
*   Save the project as .mpp file using [Project->Save(u"project.mpp", Aspose::Tasks::Saving::SaveFileFormat::MPP)][17] method.

The following code sample shows how to create and add tasks to a project using C++.

{{< gist aspose-com-gists 6a638b84f0305b6f20f1e5c176774bf8 "add-task-to-project.cpp" >}}

[Read more][18] about extended features related to tasks.

## Add Resources to Project using C++ {#Add-Resources-to-Project-using-C++}

Resources are the entities that are supposed to complete the project. Usually, people are referred to as the resources of a project. The following are the steps to create and add resources to a project.

*   Create a new project or load it from a _.mpp_ file using [Project][19] class.
*   Add a new resource using [Project->get\_Resources()->Add(u"Rsc")][20] method.
*   Save the project using [Project->Save(u"project.mpp", Aspose::Tasks::Saving::SaveFileFormat::MPP)][21] method.

The following code sample shows how to add a resource in a project using C++.

{{< gist aspose-com-gists 6a638b84f0305b6f20f1e5c176774bf8 "add-resource-to-project.cpp" >}}

[Read more][22] about extended features related to resources.

## Assign Project's Task to Resource using C++ {#Assign-Project's-Task-to-Resource-using-C++}

Once you have created the tasks and resources, the next step is to assign each task to a resource that is responsible for its completion. The following are the steps to assign a task to a resource.

*   Create a new project or load it from a _.mpp_ file using [Project][23] class.
*   Add new tasks and resources if the project is empty.
*   Access the desired task and resource into [Task][24] and [Resource][25] object respectively.
*   Assign task to resource using [Project->get\_ResourceAssignments()->Add(Task, Resource)][26] method.
*   Save the project using [Project.Save()][27] method.

The following code sample shows how to assign a task to a resource in a project using C++.

{{< gist aspose-com-gists 6a638b84f0305b6f20f1e5c176774bf8 "assign-task-to-resource.cpp" >}}

## Add Calendars in Project using C++ {#Add-Calendars-in-Project-using-C++}

Calendars are used to create a schedule for the project within the MS Project. Aspose.Tasks for C++ has made it very simple to create a calendar for a project. The following are the steps to create a calendar, add weekdays, and specify the working time.

*   Create a new project or load it from a _.mpp_ file using [Project][28] class.
*   Add a calendar to project using [Project->get\_Calendars()->Add(u"Calendar1")][29] and store the returned value in [Calendar][30] object.
*   Add working days to the calendar using [Calendar->get\_WeekDays()->Add()][31] method.
*   Save the project.

You can also set the working time for a weekday in the calendar. For this, you can follow the below steps after adding the working days.

*   Create an object of [WeekDay][32] class.
*   Create an object of [WorkingTime][33] class.
*   Set timing using [WorkingTime->set\_FromTime()][34] and [WorkingTime->set\_ToTime()][35] methods.
*   Add working time to the weekday using [WeekDay->get\_WorkingTimes()->Add(WorkingTime)][36] method.
*   Add weekday to the calendar using [Calendar->get\_WeekDays()->Add(WeekDay)][37] method.
*   Save the project.

The following code sample shows how to create a calendar in a project using C++.

{{< gist aspose-com-gists 6a638b84f0305b6f20f1e5c176774bf8 "add-calendar-in-project.cpp" >}}

[Read more][38] about extended features related to calendars.

## Conclusion

In this article, you have learned how to create MS Project files and save them as _.mpp_ or _.xml_ using C++. Furthermore, you have learned how to add tasks, resources, resource assignments, and calendars within a project programmatically. You can also explore the [documentation][39] for the extended features of Aspose.Tasks for C++ to further enhance the project management capabilities within your applications.

## See Also

*   [Read or Create Projects on Project Server and Project Online using C# .NET][40]




[1]: https://en.wikipedia.org/wiki/Microsoft_Project
[2]: #C++-MS-Project-File-Manipulation-API
[3]: #Create-MS-Project-Files-mpp-using-C++
[4]: #Add-Tasks-to-Project-using-C++
[5]: #Add-Resources-to-Project-using-C++
[6]: #Assign-Project's-Task-to-Resource-using-C++
[7]: #Add-Calendars-in-Project-using-C++
[8]: https://products.aspose.com/tasks/cpp
[9]: https://downloads.aspose.com/tasks/cpp
[10]: http://nuget.org/packages/Aspose.tasks.cpp
[11]: https://apireference.aspose.com/tasks/cpp/class/aspose.tasks.project
[12]: https://apireference.aspose.com/tasks/cpp/class/aspose.tasks.project#aead823ff59911efa62c42622cddca7f7
[13]: https://apireference.aspose.com/tasks/cpp/class/aspose.tasks.project
[14]: https://apireference.aspose.com/tasks/cpp/class/aspose.tasks.project#ae16f6d399bf3a49cd82b9e16fcfd4a93
[15]: https://apireference.aspose.com/tasks/cpp/class/aspose.tasks.task
[16]: https://apireference.aspose.com/tasks/cpp/class/aspose.tasks.task#a6479d01d5813eb0f52d4ea9762bc2966
[17]: https://apireference.aspose.com/tasks/cpp/class/aspose.tasks.project#aead823ff59911efa62c42622cddca7f7
[18]: https://docs.aspose.com/tasks/cpp/working-with-tasks/
[19]: https://apireference.aspose.com/tasks/cpp/class/aspose.tasks.project
[20]: https://apireference.aspose.com/tasks/cpp/class/aspose.tasks.project#a03b29c892643ad4178fab4b264fa0f4c
[21]: https://apireference.aspose.com/tasks/cpp/class/aspose.tasks.project#aead823ff59911efa62c42622cddca7f7
[22]: https://docs.aspose.com/tasks/cpp/working-with-resources/
[23]: https://apireference.aspose.com/tasks/cpp/class/aspose.tasks.project
[24]: https://apireference.aspose.com/tasks/cpp/class/aspose.tasks.task
[25]: https://apireference.aspose.com/tasks/cpp/class/aspose.tasks.resource
[26]: https://apireference.aspose.com/tasks/cpp/class/aspose.tasks.project#ad07cebbf6165527307aff66d732d3b1d
[27]: https://apireference.aspose.com/tasks/cpp/class/aspose.tasks.project#aead823ff59911efa62c42622cddca7f7
[28]: https://apireference.aspose.com/tasks/cpp/class/aspose.tasks.project
[29]: https://apireference.aspose.com/tasks/cpp/class/aspose.tasks.project#abaab4524f269303da99e26360a72aa3e
[30]: https://apireference.aspose.com/tasks/cpp/class/aspose.tasks.calendar
[31]: https://apireference.aspose.com/tasks/cpp/class/aspose.tasks.calendar#a9dbe2751e96744d3723568c3169c2470
[32]: https://apireference.aspose.com/tasks/cpp/class/aspose.tasks.week_day
[33]: https://apireference.aspose.com/tasks/cpp/class/aspose.tasks.working_time
[34]: https://apireference.aspose.com/tasks/cpp/class/aspose.tasks.working_time#abaecd71a0196a26663e3d3f91b1ce541
[35]: https://apireference.aspose.com/tasks/cpp/class/aspose.tasks.working_time#ab868d8fcb7433926a49e41b67d47fb59
[36]: https://apireference.aspose.com/tasks/cpp/class/aspose.tasks.week_day#ab27036d1671291950e1c86181e19e522
[37]: https://apireference.aspose.com/tasks/cpp/class/aspose.tasks.calendar#a9dbe2751e96744d3723568c3169c2470
[38]: https://docs.aspose.com/tasks/cpp/working-with-calendars/
[39]: https://docs.aspose.com/tasks/cpp/getting-started/
[40]: https://blog.aspose.com/2020/03/20/create-read-projects-on-project-server-and-project-online-in-csharp-asp-net/






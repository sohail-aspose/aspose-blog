---
title: 'Create MS Project Files Programmatically using Java'
seoTitle: "Create MS Project Files (.mpp) in Java | Add Tasks, Resources, Calenders"
description: "Examples to create MS Project MPP, MPT, and XML files programmatically in Java. Add tasks and resources to projects using Java. MS Project Library."
date: Wed, 06 Jan 2021 11:20:00 +0000
draft: false
url: /2021/01/06/create-ms-project-files-programmatically-using-java/
author: Usman Aziz
summary: '[MS Project][1] is a well-known project management application that makes it easier for managers to perform project management activities efficiently. The project managers can create tasks, add resources, and assign tasks to the resources within a particular project. Furthermore, they can define the timeline as well as perform budget management operations. However, there could be various scenarios when managers need to customize project management operations. Also, an organization may need to automate project management within web or desktop applications.'
tags: ['Create MS Project Files in Java', 'add calendar in project in java', 'add resource assignments in java', 'add resources to project in java', 'add tasks to projects in java']
categories: ['Aspose.Tasks Product Family']
---



{{< figure align=center src="images/Create-Project-Files-in-Java-1.png.jpg" alt="Create MS Project Files in Java">}}


[MS Project][2] is a well-known project management application that makes it easier for managers to perform project management activities efficiently. The project managers can create tasks, add resources, and assign tasks to the resources within a particular project. Furthermore, they can define the timeline as well as perform budget management operations. However, there could be various scenarios when managers need to customize project management operations. Also, an organization may need to automate project management within web or desktop applications.

For such cases, this article covers how to perform the basic project management operations programmatically. Particularly, you will learn **how to create projects from scratch, add tasks and resources, and work with resource assignments and calendars using Java**.

*   [Java Project Management API][3]
*   [Create an MS Project File from Scratch using Java][4]
*   [Add Tasks to a Project][5]
*   [Add Resources to a Project][6]
*   [Assign Tasks to Resources in a Project][7]
*   [Add Calendars to a Project][8]
*   [Get Free License][9]

## Java Project Management API {#Java-Project-Management-API}

[Aspose.Tasks for Java][10] is a project management API that lets you create MS Project files from scratch. Furthermore, you can manipulate an existing project in order to add some modifications. The API lets you perform basic as well as advanced project management operations seamlessly. Aspose.Tasks for Java can be downloaded as [JAR][11] or installed within Maven-based applications using the following configurations.

```
<repository>
    <id>AsposeJavaAPI</id>
    <name>Aspose Java API</name>
    <url>http://repository.aspose.com/repo/</url>
</repository>
```
```
<dependency>
    <groupId>com.aspose</groupId>
    <artifactId>aspose-tasks</artifactId>
    <version>20.12</version>
    <classifier>jdk18</classifier>
</dependency>
```

## Create an MS Project File using Java {#Create-an-MS-Project-File-from-Scratch-using-Java}

MS Project allows you to save the project-related data in either [MPP][12] or [XML][13] format. So let's start with creating an empty project file by following the below steps.

*   Create an instance of [Project][14] class.
*   Save the file using [Project.save(String, SaveFileFormat)][15] method.

The following code samples show how to create an MS Project (.mpp and .xml) file using Java.

### Save MS Project Files as MPP

{{< gist aspose-com-gists dce94bfad4682f8d9278014f7e02828b "create-mpp-file.java" >}}

### Save MS Project Files as XML

{{< gist aspose-com-gists dce94bfad4682f8d9278014f7e02828b "create-xml-file.java" >}}

Learn more about the project manipulation features: [Working with Projects][16]

## Add Tasks to a Project using Java {#Add-Tasks-to-a-Project-using-Java}

After creating the project file, you can start adding the tasks to it. The following are the steps to create and add tasks to a project file.

*   Create an instance of [Project][17] class.
*   Add a new summary task to the project’s tasks collection using [Project.getRootTask().getChildren().add(string)][18] method.
*   Add a subtask to the summary task using [Task.getChildren.add(string)][19] method.
*   Save the project file using [Project.save(String, SaveFileFormat)][20] method.

The following code sample shows how to add tasks to a project using C#.

{{< gist aspose-com-gists dce94bfad4682f8d9278014f7e02828b "add-task.java" >}}

Learn more about task manipulation features: [Working with Tasks][21]

## Add Resources to a Project using Java {#Add-Resources-to-a-Project}

The next important thing in a project is the resources that will be assigned to perform the tasks. So in this section, we'll add some resources to the project. The following are the steps to add resources to the project.

*   Create a new project or load an existing one using [Project][22] class.
*   Add resource using [Project.getResources().add(String)][23] method.
*   Save the project file using [Project.save(String, SaveFileFormat)][24] method.

The following code sample shows how to add resources in a project using Java.

{{< gist aspose-com-gists dce94bfad4682f8d9278014f7e02828b "add-resource.java" >}}

Learn more about resource manipulation features: [Working with Resources][25]

## Assign Tasks to Resources in a Project using Java {#Assign-Tasks-to-Resources-in-a-Project}

Once you have added the tasks and resources, the next thing is to assign the tasks to the relevant resources. The following are the steps to perform resource assignments in a project.

*   Create a new project or load an existing one using [Project][26] class.
*   Add tasks and resources in the same way you have added in the previous sections.
*   Get references to the task and resource in a [Task][27] and [Resource][28] object respectively.
*   Create a resource assignment using [Project.getResourceAssignments().add(Task, Resource)][29] method.
*   Save the project file using [Project.save(String, SaveFileFormat)][30] method.

The following code sample shows how to create resource assignments in a project using Java.

{{< gist aspose-com-gists dce94bfad4682f8d9278014f7e02828b "add-resource-assignment.java" >}}

Learn more about resource assignment features: [Working with Resource Assignments][31]

## Add Calendars to a Project using Java {#Add-Calendars-to-a-Project-using-Java}

Calendars are another important entity that is used to define the timeline of a project. Using the calendar, you can create a complete schedule for a project. In order to create a calendar, you can follow the below steps:

*   Create a new project or load an existing one using [Project][32] class.
*   Create a new calendar using [Project.getCalendars().add(String)][33] method and get its reference in [Calendar][34] object.
*   Use [Calendar.getWeekDays().add(WeekDay)][35] method to specify the weekdays.
*   Set working times in the calendar.
*   Save the project file using [Project.save(String, SaveFileFormat)][36] method.

The following code sample shows how to create calendar in a project using Java.

{{< gist aspose-com-gists dce94bfad4682f8d9278014f7e02828b "add-calendar.java" >}}

Learn more about calendar features: [Working with Calendars][37]

## Get a Free License {#Get-Free-License}

You can [get a free temporary license][38] in order to try the API without evaluation limitations.

## Conclusion

In this article, you have learned some basic features of how to create MS Project files from scratch using Java. Particularly, you have seen how to add tasks, resources, resource assignments, and calendars in a project. You can explore more about the Java MS Project API using [documentation][39].

## See Also

*   [Write Metadata and Formulas in MS Project Files][40]




[1]: https://en.wikipedia.org/wiki/Microsoft_Project
[2]: https://en.wikipedia.org/wiki/Microsoft_Project
[3]: #Java-Project-Management-API
[4]: #Create-an-MS-Project-File-from-Scratch-using-Java
[5]: #Add-Tasks-to-a-Project-using-Java
[6]: #Add-Resources-to-a-Project
[7]: #Assign-Tasks-to-Resources-in-a-Project
[8]: #Add-Calendars-to-a-Project-using-Java
[9]: #Get-Free-License
[10]: https://products.aspose.com/tasks/java
[11]: https://downloads.aspose.com/tasks/java
[12]: https://docs.fileformat.com/project-management/mpp/
[13]: https://docs.fileformat.com/web/xml/
[14]: https://apireference.aspose.com/tasks/java/com.aspose.tasks/Project
[15]: https://apireference.aspose.com/tasks/java/com.aspose.tasks/Project#save-java.lang.String-int-
[16]: https://docs.aspose.com/tasks/java/working-with-projects/
[17]: https://apireference.aspose.com/tasks/java/com.aspose.tasks/Project
[18]: https://apireference.aspose.com/tasks/java/com.aspose.tasks/TaskCollection#add-java.lang.String-
[19]: https://apireference.aspose.com/tasks/java/com.aspose.tasks/TaskCollection#add-java.lang.String-
[20]: https://apireference.aspose.com/tasks/java/com.aspose.tasks/Project#save-java.lang.String-int-
[21]: https://docs.aspose.com/tasks/java/working-with-tasks/
[22]: https://apireference.aspose.com/tasks/java/com.aspose.tasks/Project
[23]: https://apireference.aspose.com/tasks/java/com.aspose.tasks/ResourceCollection#add-java.lang.String-
[24]: https://apireference.aspose.com/tasks/java/com.aspose.tasks/Project#save-java.lang.String-int-
[25]: https://docs.aspose.com/tasks/java/working-with-resources/
[26]: https://apireference.aspose.com/tasks/java/com.aspose.tasks/Project
[27]: https://apireference.aspose.com/tasks/java/com.aspose.tasks/Task
[28]: https://apireference.aspose.com/tasks/java/com.aspose.tasks/Resource
[29]: https://apireference.aspose.com/tasks/java/com.aspose.tasks/ResourceAssignmentCollection#add-com.aspose.tasks.Task-com.aspose.tasks.Resource-
[30]: https://apireference.aspose.com/tasks/java/com.aspose.tasks/Project#save-java.lang.String-int-
[31]: https://docs.aspose.com/tasks/java/working-with-resource-assignments/
[32]: https://apireference.aspose.com/tasks/java/com.aspose.tasks/Project
[33]: https://apireference.aspose.com/tasks/java/com.aspose.tasks/CalendarCollection#add-java.lang.String-
[34]: https://apireference.aspose.com/tasks/java/com.aspose.tasks/Calendar
[35]: https://apireference.aspose.com/tasks/java/com.aspose.tasks/WeekDayCollection#add-com.aspose.tasks.WeekDay-
[36]: https://apireference.aspose.com/tasks/java/com.aspose.tasks/Project#save-java.lang.String-int-
[37]: https://docs.aspose.com/tasks/java/working-with-calendars/
[38]: https://purchase.aspose.com/temporary-license
[39]: https://docs.aspose.com/tasks/java/getting-started/
[40]: https://blog.aspose.com/2019/08/26/metadata-and-formulas-writing-support-in-aspose.tasks/






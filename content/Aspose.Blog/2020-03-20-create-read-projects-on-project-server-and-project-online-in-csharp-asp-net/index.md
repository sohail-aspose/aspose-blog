---
title: 'Read or Create Projects on Project Server and Project Online using C# .NET'
seoTitle: "Create or Read Projects on Project Server or Project Online | C# ASP.NET"
description: ".NET API to connect to Project Server or Project Online. Read or create projects in C#, ASP.NET or .NET Core application. Project Server/Online API for C#."
date: Fri, 20 Mar 2020 15:56:35 +0000
draft: false
url: /2020/03/20/create-read-projects-on-project-server-and-project-online-in-csharp-asp-net/
author: Usman Aziz
summary: ''
tags: ['Access Project Online in ASP.NET', 'Access Project Server in ASP.NET']
categories: ['Aspose.Tasks Product Family']
---



{{< figure align=center src="images/aspose_tasks-min.png" alt="Project Server and Project Online in C# ASP.NET">}}


The **Project Online** and **Project Server** are the feature-rich project and portfolio management solutions provided by Microsoft. Both the solutions offer almost a similar range of features for creating and managing projects, however, they differ based on which solution fits well with your requirements. For example, if you want the on-premise solution with more control over the hardware and software then you may opt Project Server. On the other hand, Project Online serves as a cloud-based instance of Project Server without requiring your own infrastructure.

There might be the case when to need to access the information of the projects from Project Server/Online from within your applications. In order to deal with such cases, in this article, I'll show you how to **create/read the projects on/from Project Server or Project Online** within your .NET applications (ASP.NET, etc.) or web services using C#.

## C# API for Project Server/Online

For creating the new projects and reading the existing ones from Project Server/Online, we'll use [Aspose.Tasks for .NET][1]. It is a cross-platform class library for reading and writing MS Project files programmatically in .NET Standard or .NET Core applications. The API is hosted on [NuGet][2] as well as available as an MSI package and zipped DLL in the [Downloads][3] section.

## Working with Project Server

In this section, I'll show you how to connect to the Project Server and read or create the projects. In order to connect to the Project Server, you need to know the following details:

*   Project Server's URL i.e. https://contoso.sharepoint.com
*   Domain i.e. contoso.com
*   Username
*   Password

### Read Projects from Project Server in C#

The following are the steps to connect to Project Server and retrieve the projects list from it.

*   Instantiate [NetworkCredential][4] class and initialize it with credentials.
*   Create an object of [ProjectServerCredentials][5] class and initialize it with the project server's URL and _NetworkCredential_ object.
*   Create an object of [ProjectServerManager][6] class and get a list of the projects using [ProjectServerManager.GetProjectList()][7] method.

The following code sample shows how to read projects from Project Server in C#.

{{< gist aspose-com-gists 10d4de13018b7279cf03bab28ed78aeb "Examples-CSharp-WorkingWithProjects-CreatingReadingAndSaving-ReadAndCreateInProjectServer-ReadProjectFromProjectServer.cs" >}}

### Create Project on Project Server in C#

Creating a project on Project Server is as simple as pie. Simply connect to Project Server in the same way you have done in the previous example, load the project file (.mpp) using [Project][8] class and call [ProjectServerManager.CreateNewProject()][9] method.

The following code sample shows how to create a new project on Project Server in C#.

{{< gist aspose-com-gists 10d4de13018b7279cf03bab28ed78aeb "Examples-CSharp-WorkingWithProjects-CreatingReadingAndSaving-ReadAndCreateInProjectServer-CreateProjectInProjectServer.cs" >}}

## Working with Project Online

Working with Project Online is quite similar to working with Project Server and it only differs in creating the connection. In order to connect to Project Online, you need to know the following details:

*   URL
*   Username
*   Password

### Read Projects from Project Online in C#

The following are the steps to read projects from Project Online:

*   Set the credentials to connect to Project Online using [ProjectServerCredentials][10].
*   Create and initialize the [ProjectServerManager][11] object.
*   Retrieve the list of projects using [ProjectServerManager.GetProjectList()][12] method.

The following code sample shows how to retrieve the list of projects from Project Online.

{{< gist aspose-com-gists 10d4de13018b7279cf03bab28ed78aeb "Examples-CSharp-ExProjectServerManager-ReadingProjectOnline.cs" >}}

### Create a Project on Project Online in C#

The following are the steps to create a new project on Project Online:

*   Set the credentials to connect to Project Online using [ProjectServerCredentials][13].
*   Load the project file (.mpp) using [Project][14] class.
*   Create and initialized [ProjectServerManager][15] object.
*   Create the project using [ProjectServerManager.CreateNewProject()][16] method.

The following code sample shows how to create a new project on Project Online in C#.

{{< gist aspose-com-gists 10d4de13018b7279cf03bab28ed78aeb "Examples-CSharp-WorkingWithProjects-CreatingReadingAndSaving-CreateProjectOnline.cs" >}}

## Learn more about Aspose.Tasks for .NET

You can learn more about project management using Aspose.Tasks for .NET from the [documentation][17].




[1]: https://products.aspose.com/tasks/net
[2]: https://www.nuget.org/packages/Aspose.Tasks/
[3]: http://downloads.aspose.com/tasks/net
[4]: https://docs.microsoft.com/en-us/dotnet/api/system.net.networkcredential?view=netframework-4.8
[5]: https://apireference.aspose.com/net/tasks/aspose.tasks/projectservercredentials
[6]: https://apireference.aspose.com/net/tasks/aspose.tasks/projectservermanager
[7]: https://apireference.aspose.com/net/tasks/aspose.tasks/projectservermanager/methods/getprojectlist
[8]: https://apireference.aspose.com/net/tasks/aspose.tasks/project
[9]: https://apireference.aspose.com/net/tasks/aspose.tasks/projectservermanager/methods/createnewproject
[10]: https://apireference.aspose.com/net/tasks/aspose.tasks/projectservercredentials/constructors/2
[11]: https://apireference.aspose.com/net/tasks/aspose.tasks/projectservermanager
[12]: https://apireference.aspose.com/net/tasks/aspose.tasks/projectservermanager/methods/getprojectlist
[13]: https://apireference.aspose.com/net/tasks/aspose.tasks/projectservercredentials/constructors/2
[14]: https://apireference.aspose.com/net/tasks/aspose.tasks/project
[15]: https://apireference.aspose.com/net/tasks/aspose.tasks/projectservermanager
[16]: https://apireference.aspose.com/net/tasks/aspose.tasks/projectservermanager/methods/createnewproject
[17]: https://docs.aspose.com/display/tasksnet/Getting+Started






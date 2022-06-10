---
title: 'Renumber WBS Codes in Projects using C# with Aspose.Tasks for .NET 18.2'
date: Sun, 18 Feb 2018 06:30:09 +0000
draft: false
url: /2018/02/18/renumber-wbs-codes-with-aspose.tasks-for-.net-18.2/
author: Kashif Iqbal
summary: ''
tags: []
categories: ['Aspose.Tasks Product Family']
---



{{< figure align=center src="images/Aspose.Tasks-for-.NET_.png" alt="aspose-tasks-for-net">}}


We are pleased to announce the release of [Aspose.Tasks for .NET 18.2][1]. This new version of API introduces a new feature of renumbering WBS Codes for tasks like the Renumber function of Microsoft Project. It also provides an enhancement to get page count from a document for defined start and end dates. For a detailed note on what is new and fixed, you can visit the [release notes][2] section of API documentation.

# Renumber WBS Codes in MS Project in C#

Aspose.Tasks for .NET API lets you work with WBS codes associated with tasks in a project. This latest release of API introduces a new feature of [Renumbering WBS codes][3] for tasks like Microsoft Project’s _Renumber_ functionality. It lets you renumber all or selective WBS codes of tasks in a project as shown in the following code sample.



# Get Page Count for Specific Dates in Project

This release also introduces an enhancement for getting the number of pages based on specified Start and End dates. This feature can be used to get specific page count for specified dates even during conversion to various output formats.

```
Project project = new Project(dataDir + "GetNumberOfPages.mpp");

var options = new ImageSaveOptions(SaveFileFormat.PNG)
{
    SaveToSeparateFiles = true,
    PageSize = PageSize.A3,
    Timescale = Timescale.Months,
    StartDate = project.Get(Prj.StartDate) - TimeSpan.FromDays(10),
    EndDate = project.Get(Prj.FinishDate) + TimeSpan.FromDays(30)
};
int pageCount = project.GetPageCount(
    PageSize.A3,
    Timescale.Months,
    project.Get(Prj.StartDate) - TimeSpan.FromDays(10),
    project.Get(Prj.FinishDate) + TimeSpan.FromDays(30));

Console.WriteLine(pageCount); 
```

## API Resources

You may visit the following API resources for getting started and working with the API.

*   [Product Documentation][4] – Detailed API documentation with code examples and details about API functional areas
*   [API Reference Guide][5] – Detailed information about the API namespaces and classes
*   [GitHub Examples][6] – Ready to run code samples in downloadable form
*   [Aspose.Tasks Forum][7] – Our online support forum where we address your queries and inquiries




[1]: https://www.nuget.org/packages/Aspose.Tasks/
[2]: https://docs.aspose.com/display/tasksnet/Aspose.Tasks+for+.NET+18.2+Release+Notes
[3]: https://docs.aspose.com/display/tasksnet/WBS+Associated+with+a+Task#WBSAssociatedwithaTask-RenumberWBSCodes
[4]: https://docs.aspose.com/display/tasksnet/Home
[5]: https://apireference.aspose.com/tasks/net
[6]: https://github.com/asposetasks/Aspose_Tasks_NET
[7]: https://forum.aspose.com/c/tasks





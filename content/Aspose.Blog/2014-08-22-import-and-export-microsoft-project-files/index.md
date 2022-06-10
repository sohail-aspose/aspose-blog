---
title: 'XenTek accomplished data Import and export from Microsoft Project files without Microsoft Interop and MPXJ'
date: Fri, 22 Aug 2014 04:07:35 +0000
draft: false
url: /2014/08/22/import-and-export-microsoft-project-files/
author: Jonathan Tooth
summary: ''
tags: ['Aspose.Tasks', 'Aspose.Tasks for .NET an alternative to MPXJ', 'Easy and reliable MPP processing API', 'Export data from MPP project file', 'Import and Export data from MPP file', 'Import data into MPP Project file', 'MPP Automation without Microsoft InterOp', 'Manipulate MPP file without using Microsoft Interop', 'Process MS Project files wihout MPXJ', 'Success Stories']
categories: ['Aspose.Tasks Product Family']
---

## About XenTek Limited



{{< figure align=center src="images/Screenshot-2020-04-20-at-11.46.06-PM-1024x137.png" alt="XenTek Limited company logo">}}


[XenTek][1] is a small software house developing primarily a product called Plan Runner – a tool to aid Project Managers. There is just one employee, Jonathan Tooth who is an accomplished software developer, analyst & consultant with over 30 years of commercial experience ranging from Z80 machine code to C#, VB.Net.

## Problem

The tool [Planrunner][2] is a complex piece of software that provides a level of control and visibility of 'running' projects previously unreachable by Project Managers. One of its Vital aspects includes its capability to accept the assets the Project Manager has created. To this end, the tool provides two mechanisms to input existing project plans. A sync tool that sits inside Microsoft Project and provides the easiest method to the user and an import/export tool built into the website for Project Managers, who are unwilling or unable to download and install programs from the internet. This import/export tool requires a mechanism to read and write Microsoft project files.

## Solution

Three solutions were trialed over the course of PlanRunner's development. The first two (_Microsoft Interop and MPXJ_) were discounted due to following reasons. The third solution that we trialed was [Aspose.Tasks for .NET][3]. However, the license cost is an issue for a ‘Start-up’ company, and having a commercially developed tool needs to ensure that it is kept up to date and faults are dealt with and fixed in a timely manner.

PlanRunner users do not directly experience the tool and they are presented with an interface as shown below:



{{< figure align=center src="images/XenTek-planrunner-aspose.tasks-case-study.png" alt="Project File upload page preview" caption="Image 1:- Project file upload page">}}


## Upload

This facilitates the user to get their project plan into Plan Runner. By simply selecting their project file using the 'Choose file' button and clicking on the 'Upload' button. The website uploads and reads its project file and stores the selected contents inside a SQL Server database.

The user gets the capabilities to merge the data into the website or overwrite existing content.



{{< figure align=center src="images/XenTek-planrunner-aspose.tasks-case-study-1.png" alt="Project File download page preview" caption="Image 2:- Project file download page">}}


## Download

This facilitates the additional information stored by the website to be inserted into the project file the user originally uploaded. The simplest use is to click the ‘Prepare and download the file’ button which updates the originally uploaded project file and downloads it to the user.

## Experience

### **Finding a solution**

Originally the reading and writing of Microsoft project files were performed by Microsoft’s own Interop assemblies. It was fine for organizations that were hosting the website internally. However, Microsoft licensing prevented this from being used on public-facing websites.

In a subsequent attempt, a decision was made to use MPXJ, which is an open-source library that enabled the reading of Microsoft Project files. Unfortunately, this tool sometimes had issues reading Microsoft Project 2013 files. The incorrect reading of the file affected our first customer extensively and was not an acceptable solution.

Later on, [Aspose.Tasks for .NET][4] was trialed to see if it could read and write all of the project files accurately. A [free trial][5] reduced financial risk enabling a full POC to be performed. The following criteria were measured to determine the suitability of the product:

*   Ease of integration
*   Reliability of product
*   Performance of product
*   Quality of help
*   Availability of [support][6]

## Implementation

### **Effort**

Integration of [Aspose.Tasks for .NET][7] into the Plan Runner import/export mechanism took:

*   Coding and unit testing Upload mechanism – 7 hours
*   System Testing including bug fixing – 7 hours
*   Coding and unit testing Download mechanism – 5 hours
*   System Testing including bug fixing – 7 hours
*   User Acceptance Testing (of both mechanisms) – 6.5 hours

This resulted in a total effort of 32.5 man-hours.

A rough comparison regarding the integration of MPXJ is possible. We recommend using [Aspose.Tasks for .NET][8] as compared to MPXJ, because MPXJ coding was quicker at ~10 hours but testing and debugging took over 40 hours.

### Technical Solution

Implementation was made easier by having had two previous mechanisms. While integrating MPXJ, the decision was made to isolate all project file reading and writing. A shared library that provided the business logic and connectivity to SQL Server was created along with a ‘Neutral Task’ class that hid tool specific code.

The sample implementation to read Task Name.

```
Public ReadOnly Property Name() As String
  Get
    Select Case cGlobals.ActiveImportExportMechanism
      Case cGlobals.ImportExportMechanism.UseMPXJ
        Return _TaskMPXJ.Name
      Case cGlobals.ImportExportMechanism.UseMicrosoft_OfficeInterop
        Return _TaskMSP.Name
      Case cGlobals.ImportExportMechanism.UseAsposeTasks
        Return _TaskAspose.Name
      Case Else
        Return String.Empty
    End Select
  End Get
End Property
```

However, some task elements were presented in a significantly different way. As per user expectations, the Predecessors and Duration fields required the most work to convert them into the visual format.

Setting fields were hidden from the Plan Runner specific code, where we used the three interface methods:

```
Public Function SetFieldValue(ByVal task As Aspose.Tasks.Task, ByVal eFieldName 
As AsposeFieldNames, ByVal Value As String) As Boolean

Public Function SetFieldValue(ByVal task As Aspose.Tasks.Task, ByVal eFieldName 
As AsposeFieldNames, ByVal Value As DateTime) As Boolean

Public Function SetFieldValue(ByVal task As Aspose.Tasks.Task, ByVal eFieldName 
As AsposeFieldNames, ByVal Value As Integer) As Boolean
```

We were also required to allow Plan Runner to set any field in a task without needing to understand how it is done. Note that Plan Runner does not use calendars, resource scheduling or project information, so these were not used or evaluated.

### Challenges

The initial provision of the import and export mechanisms was relatively straight forward. The example code supplied on the [ExamplesDashboard][9] and [online help][10] provided enough help.

A later addition to the creation of a new project file on download created some problems. However, the [forums][11] proved very useful while providing advice and example code which we could not earlier find inside online [documentation][12] i.e. using a [blank project file][13]. Many problems were experienced with Start and Finish times being set incorrectly and [Appendix 1][14] provided some guidance on this.

### Outcome

For the most part, a successful outcome was achieved. [Import and export to MPP files][15] was fully operational and tested successfully with over 20 different project files from various versions of Microsoft Project. Export to CSV has been rewritten to generate directly from the PlanRunner SQL Server database as going via Microsoft Project gave no real benefit. [Export to Excel][16] proved to be problematic as we started to face difficulties when we tried to open files with Excel 2010. It was deemed prudent at this time to disable the facility and revisit when the impact on delaying other development is reduced.

## Next Steps

So far [Aspose.Tasks for .NET][17] have been working fine and in the near future, it is expected to have to tweak the mechanism to allow for edge cases and bugs being found. At some later point, further refactoring of the code is required including the removal of Interop code to cater to further formats supported by [Aspose.Tasks for .NET][18].

## Summary

Overall, the implementation went reasonably smoothly. The product appears robust, performs well and once coded was stable. It coped well with Project files from 2007 to 2013 and extensive testing was performed to ensure that the task fields were being read and written correctly. Once users would be able to put a few of their own project files through this new mechanism, we expect to be able to fully sign off this part of the system.

I certainly would recommend [Aspose.Tasks for .NET][19] to anyone requiring read and write access to Microsoft Project files.

**Appendix 1 – Recommendations on creating a new task**

When creating a new task, you may experience problems with the Start and Finish times (_and to a lesser extent dates_) changing or being reset. The following rules should provide some help in this endeavor.

*   Set Duration first
*   Then set Work, RemainingWork, RegularWork and Work again to the duration
*   Then set DurationFormat
*   Then set the Start, ManualStart, Finish, and ManualFinish

If you assign resources to the task, use following code line

```
Resource = mppFile.AddResource(resourceName)
```

Don’t use the following approach

```
 Resource = New Aspose.Tasks.Resource mppFile.Resources.Add(resource)
```

Please note that Microsoft Project automatically assigns the times and dates to the resource assignment when you link them using Microsoft’s interface. Therefore when using [Aspose.Tasks for .NET][20], this needs to be done manually.

How to assign a resource

```
Dim ra As New ResourceAssignment(Me.neutralTask, resource)
ra.Start = Me.neutralTask.Start
ra.Finish = Me.neutralTask.Finish
ra.Task.Work = ra.Task.Duration
ra.RemainingWork = ra.Task.Work
ra.RegularWork = ra.RemainingWork
ra.Work = ra.RegularWork
ra.Finish = Me.neutralTask.Finish
mppFile.ResourceAssignments.Add(ra)
```

Similarly, we found that using AddTaskLink in preference to [TaskLinkCollection.Add][21] seemed to create a more stable result.

**Jonathan Tooth  
**Managing Director, XenTek Ltd  
[www.xentek.co.uk][22]  
[www.planrunner.co.uk][23]




[1]: http://www.xentek.co.uk/
[2]: https://www.planrunner.co.uk/
[3]: https://products.aspose.com/tasks/net
[4]: https://products.aspose.com/tasks/net
[5]: https://downloads.aspose.com/tasks/net
[6]: https://forum.aspose.com/c/tasks
[7]: https://products.aspose.com/tasks/net
[8]: https://products.aspose.com/tasks/net
[9]: https://github.com/aspose-tasks/Aspose.Tasks-for-.NET
[10]: https://docs.aspose.com/display/tasksnet/Home
[11]: https://forum.aspose.com/c/tasks
[12]: https://docs.aspose.com/display/tasksnet/Home
[13]: https://docs.aspose.com/display/tasksnet/Creating%2C+Reading+and+Saving+Projects#Creating,ReadingandSavingProjects-CreatinganEmptyProjectFile
[14]: https://docs.aspose.com/display/tasksnet/Microsoft+Project+Data+Reading+and+Writing+Summary
[15]: https://docs.aspose.com/display/tasksnet/Importing+and+Exporting+Project+Data+to+Primavera+Format
[16]: https://docs.aspose.com/display/tasksnet/Convert+Project+Data+to+Excel
[17]: https://products.aspose.com/tasks/net
[18]: https://products.aspose.com/tasks/net
[19]: https://products.aspose.com/tasks/net
[20]: https://products.aspose.com/tasks/net
[21]: https://apireference.aspose.com/tasks/net/aspose.tasks/tasklinkcollection
[22]: http://www.xentek.co.uk
[23]: https://www.planrunner.co.uk/





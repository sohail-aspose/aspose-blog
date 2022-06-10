---
title: 'Reading Project Data from MPD Files using C#'
date: Fri, 29 Jan 2016 15:10:58 +0000
draft: false
url: /2016/01/29/reading-project-data-from-mpd-files-using-csharp/
author: Kashif Iqbal
summary: ''
tags: []
categories: ['Aspose.Tasks Product Family']
---



{{< figure align=center src="images/aspose-Tasks-for-net_100.png" alt="">}}


We are pleased to announce the release of [Aspose.Tasks for .NET 9.2.1][1]. This month's release includes a new feature of reading project data from Microsoft Access Database file and enhancements. It also includes a number of bug fixes that overall improves the API functionality. Our documentation section, Public API Changes, lists all the changes that are part of this month's release.

## Reading Project Data from Microsoft Access Database (MPD) File

This month's release introduces a new feature of reading project data from Microsoft Access Database (MPD) file. The DBSettings class can be used to initiate the connection to the MPD File to be read as shown in the following code sample.

```
DbSettings settings = new MpdSettings(GetConnectionString(), 1);
Project project = new Project(settings);

private string GetConnectionString()
{
    return "Provider=Microsoft.Jet.OLEDB.4.0; Data Source=MpdFileToRead.mpd";
}
```

## Reading Work Weeks from Calendar

This month's release also provides the capability to read work weeks information from Project Calendar. This is supported for XML and MPP file formats only. the _WorkWeekCollection_ represents collection of Work weeks in the calendar and can be used as shown in the following code sample.

```
Project project = new Project("TestWorkWeek.mpp");
Calendar calendar = project.Calendars.GetByUid(3);
WorkWeekCollection collection = calendar.WorkWeeks;

foreach(WorkWeek workWeek in collection)
{
    string Name = workWeek.Name;  //name
    DateTime fromDate = workWeek.FromDate;  //start
    DateTime toDate = workWeek.ToDate;      //finish

    //This data is all about "Details.." button you can set special working times for special WeekDay or even make nonworking
    WeekDayCollection weekDays = workWeek.WeekDays;   //Aspose.Tasks.WeekDayCollection
    foreach(WeekDay day in weekDays)   //Aspose.Tasks.WeekDay
    {
       WorkingTimeCollection workingTimes = day.WorkingTimes;  //Aspose.Tasks.WorkingTimeCollection
    }
} 
```

## Customizing TimeScale Tier

Aspose.Tasks API provides the capability to customize Timescale tier labels according to the current CultureInfo of the machine.The DateTimeConverter(DateTime date) delegate provides a converter method to convert date to string in view timescale tiers. In addition, the TimescaleTier.DateTimeConverter enables rendering of date in desired format.

## API Resources

You may visit the following API resources for getting started and working with the API.

*   [Product Documentation][2] – Detailed API documentation with code examples and details about API functional areas
*   [API Reference Guide][3] – Detailed information about the API namespaces and classes
*   [GitHub Examples][4] – Ready to run code samples in downloadable form
*   [Aspose.Tasks Forum][5] – Our online support forum where we address your queries and inquiries




[1]: https://products.aspose.com/tasks/net
[2]: https://docs.aspose.com/tasks/net
[3]: https://apireference.aspose.com/tasks/net
[4]: https://github.com/asposetasks/Aspose_Tasks_NET
[5]: https://forum.aspose.com/c/tasks





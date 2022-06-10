---
title: 'Aspose.Tasks for .NET Supports Mono Framework'
date: Wed, 30 Dec 2015 13:29:29 +0000
draft: false
url: /2015/12/30/aspose.tasks-for-.net-supports-mono-framework/
author: Kashif Iqbal
summary: ''
tags: []
categories: ['Aspose.Tasks Product Family']
---



{{< figure align=center src="images/aspose-Tasks-for-net_100.png" alt="">}}


We are pleased to announce the release of [Aspose.Tasks for .NET 9.1.0][1]. This month’s release of Aspose.Tasks has been enhanced and tested to work with Mono Framework. Moreover, it includes a number of bug fixes that improves overall API functionality.  You can also visit our Product documentation page to have an idea about the Public API changes that are part of this month’s release.

## Support for Mono Framework

[Mono][2] is a software platform designed to allow developers for creating cross platform applications. It is an open source implementation of Microsoft’s .NET Framework based on the ECMA standards for C# and the Common Language Runtime.

We are pleased to share that Aspose.Tasks API is now supported for Mono Framework. Hence, developers can now use the API to write applications for manipulating Microsoft Project as well as Primavera documents over a number of platforms. The API has been tested with Mono on Linux Operating System (Ubuntu) for functionality. It can be used to develop applications for:

*   Working with Projects
*   Working with Tasks
*   Working with Task Links
*   Working with Task Baselines
*   Working with Resources
*   Working with Resource Assignments
*   Working with Calendar and Calendar Exceptions
*   Working with Currencies

### Limitations

The API, however, has certain limitations as follow:

*   Following properties are not supported for working with Mono Framework.
    *   Aspose.Tasks.Saving.SaveFileFormat.TIFF
    *   Aspose.Tasks.Saving.ImageSaveOptions.TiffCompression
    *   Aspose.Tasks.Saving.ImageSaveOptions.PixelFormat
    *   Aspose.Tasks.Saving.ImageSaveOptions.HorizontalResolution
    *   Aspose.Tasks.Saving.ImageSaveOptions.VerticalResolution
    *   Aspose.Tasks.Saving.ImageSaveOptions.SaveToSeparateFiles
*   The use of _TrustServerCertificate_ and _Encrypt_ in connection string (while retrieving project data from Microsoft as well as Primavera database) is not supported by Mono and, hence, it is also not supported by the API

## Reading Task Duration as Text

This month’s release also includes a new property to the _Tsk_ class for retrieving task duration as text. This can be retrieved using the _Tsk.DurationText_ property. If this field returns NULL, the Duration filed can be used to get the task duration as shown in the following code sample.

```
Project project = new Project("Project1.mpp");
ChildTasksCollector collector = new ChildTasksCollector();

// Collect all the tasks from RootTask using TaskUtils
TaskUtils.Apply(project.RootTask, collector, 0);

foreach (Task task in collector.Tasks)
{
    string durationText = task.Get(Tsk.DurationText);
    if (durationText != null)
        Console.WriteLine(durationText);
    else 
        Console.WriteLine(task.Get(Tsk.Duration));
}
```

## Other Improvements

The API also includes a number of bug fixes that further improves the overall functionality. These include different types of exceptions while reading certain project files. For detailed information about these, please visit our [product download page][3].

## API Resources

You may visit the following API resources for getting started and working with the API.

*   Product Documentation – Detailed API documentation with code examples and details about API functional areas
*   API Reference Guide – Detailed information about the API namespaces and classes
*   [GitHub Examples][4] – Ready to run code samples in downloadable form
*   [Aspose.Tasks Forum][5] – Our online support forum where we address your queries and inquiries




[1]: https://products.aspose.com/tasks/net
[2]: http://www.mono-project.com/
[3]: https://downloads.aspose.com/tasks/net
[4]: https://github.com/asposetasks/Aspose_Tasks_NET
[5]: https://forum.aspose.com/c/tasks





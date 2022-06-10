---
title: 'Eliminate Gap Between Tasks List and Footer in Projects using C#'
date: Sun, 18 Mar 2018 04:43:56 +0000
draft: false
url: /2018/03/18/eliminate-gap-between-tasks-list-and-footer-with-aspose.tasks-for-.net-18.3/
author: Kashif Iqbal
summary: ''
tags: []
categories: ['Aspose.Tasks Product Family']
---



{{< figure align=center src="images/Aspose.Tasks-for-.NET_.png" alt="aspose-tasks-for-net">}}


We are pleased to announce the release of [Aspose.Tasks for .NET 18.3][1]. This month’s release introduces a new feature for reducing the gap between the tasks list and page footer information. It also includes improvements in terms of bug fixes that further add to the overall API stability. For a detailed note on what is new and fixed, please visit the [release notes][2] section of API documentation.

## Eliminating Gap between Tasks List and Page Footer

The rendering capabilities of project data to various formats is one of the powerful features of Aspose.Tasks API.  We have further improved this functionality by providing the feature of [reducing gap][3] between project’s tasks list and footer information in output. This improves the visualization of project’s rendered information in the output. The ReduceFooterGap property of SaveOptions class can be used to achieve this as shown in the following code sample.

```
//Read the MPP file.
Project project = new Project(dataDir + "CreateProject2.mpp");

//Use ReduceFooterGap property to reduce the gap between list of tasks and Footer
var imageSaveOptions =
    new ImageSaveOptions(SaveFileFormat.PNG) { ReduceFooterGap = true, /* set to true */ SaveToSeparateFiles = true, PageSize = PageSize.A0, Timescale = Timescale.Days };
project.Save(dataDir + "ReducingGapBetweenTasksListAndFooter_out.png", (SaveOptions)imageSaveOptions);

var pdfSaveOptions = new PdfSaveOptions { ReduceFooterGap = true, /* set to true */ SaveToSeparateFiles = true, PageSize = PageSize.A0, Timescale = Timescale.Days };
project.Save(dataDir + "ReducingGapBetweenTasksListAndFooter_out.pdf", (SaveOptions)pdfSaveOptions); 
```

## API Resources

You may visit the following API resources for getting started and working with the API.

*   [Product Documentation][4] – Detailed API documentation with code examples and details about API functional areas
*   [API Reference Guide][5] – Detailed information about the API namespaces and classes
*   [GitHub Examples][6] – Ready to run code samples in downloadable form
*   [Aspose.Tasks Forum][7] – Our online support forum where we address your queries and inquiries




[1]: https://www.nuget.org/packages/Aspose.Tasks/
[2]: https://docs.aspose.com/tasks/net/aspose-tasks-for-net-18-3-release-notes/
[3]: https://docs.aspose.com/tasks/net/reduce-gap-between-tasks-list-and-footer/
[4]: https://docs.aspose.com/tasks/net/
[5]: http://www.aspose.com/api/net/tasks
[6]: https://github.com/asposetasks/Aspose_Tasks_NET
[7]: https://forum.aspose.com/c/tasks





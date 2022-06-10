---
title: 'Set Image Quality of MS Project Data using C#'
date: Mon, 06 Nov 2017 14:29:55 +0000
draft: false
url: /2017/11/06/setting-image-quality-of-project-data-with-aspose.tasks-for-.net-17.11/
author: Kashif Iqbal
summary: ''
tags: []
categories: ['Aspose.Tasks Product Family']
---



{{< figure align=center src="images/Aspose.Tasks-for-.NET_.png" alt="aspose-tasks-for-net">}}


We are pleased to announce the release of [Aspose.Tasks for .NET 17.11][1]. This month’s release includes a new feature of setting output image quality while exporting project data to JPEG. Other than the new feature and enhancement, it also includes several improvements in terms of bug fixes that further add to the stability of the API. For a detailed note on what is new and fixed, please visit the release notes section of API documentation.

## Improvements in Aspose.Tasks for .NET 17.11

Setting output Image Quality for Exported Project Data: This month’s release includes a new feature setting output JPEG image quality while exporting project data. This is achieved using the JpegQuality property of ImageSaveOptions class as shown in the code sample below.

```
Project project = new Project(dataDir + "CreateProject2.mpp");

// in order to manipulate JPEG quality one can use ImageSaveOptions.JpegQuality property.
// The allowed value range is 0..100.
var options = new ImageSaveOptions(SaveFileFormat.JPEG) { JpegQuality = 50 };

project.Save(dataDir + "image_out.jpeg", options);
```

## Other Improvements

This version of the API comes with several bug fixes relating to different functional areas of the API. These fixes include:

*   Issues with recalculation method of the API for manually scheduled tasks
*   Problems with actual duration and finish dates of MPP and XML project data files
*   Missing time span from split parts collection
*   Rendering of sub-tasks while converting MPX to PDF1b
*   Calculation issue with percent complete in MPP as compared to XML output
*   Exceptions while loading certain project files
*   Errors raised by Microsoft Project 2010 with MPP files generated using Aspose.Tasks API

## API Resources

You may visit the following API resources for getting started and working with the API.

*   [Product Documentation][2] – Detailed API documentation with code examples and details about API functional areas
*   [API Reference Guide][3] – Detailed information about the API namespaces and classes
*   [GitHub Examples][4] – Ready to run code samples in downloadable form
*   [Aspose.Tasks Forum][5] – Our online support forum where we address your queries and inquiries




[1]: https://www.nuget.org/packages/Aspose.Tasks/17.11.0
[2]: https://docs.aspose.com/tasks/net/
[3]: https://apireference.aspose.com/tasks/net
[4]: https://github.com/asposetasks/Aspose_Tasks_NET
[5]: https://forum.aspose.com/c/tasks





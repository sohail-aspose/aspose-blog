---
title: 'Default Font for Rendering MS Project Documents using C#'
date: Sun, 20 May 2018 15:30:23 +0000
draft: false
url: /2018/05/20/metered-licensing-support-with-aspose.tasks-for-.net-18.5/
author: Kashif Iqbal
summary: ''
tags: []
categories: ['Aspose.Tasks Product Family']
---



{{< figure align=center src="images/Aspose.Tasks-for-.NET_.png" alt="aspose-tasks-for-net">}}


We are pleased to announce the release of [Aspose.Tasks for .NET 18.5][1]. This month’s release introduces support for Metered Licensing in the API. In addition, it also brings improvements to the API in terms of enhancements and bug fixes. For a detailed note on what is new and fixed, please visit the [release notes][2] section of API documentation.

## Default Font for Rendering MS Project Documents

Since version 17.12, the API supports setting default font while converting project documents to PDF. This new release of API provides the same functionality while exporting project data to image formats such JPG, BMP, PNG and HTML as well.

## Support for Metered Licensing

Usage of Metered Licensing scheme is simple and can be used along with existing licensing method. The new licensing mechanism will be used along with existing licensing method. Those customers who want to be billed based on the usage of the API features can use the metered licensing. 

```
Aspose.Tasks.Metered metered = new Aspose.Tasks.Metered();
// Access the SetMeteredKey property and pass public and private keys as parameters
metered.SetMeteredKey("*****", "*****");

// The path to the documents directory. 
string dataDir = RunExamples.GetDataDir_Email();

// Load the project from file system
Project project = new Project(dataDir + "HomeConstruction.mpp"); 
```

## API Resources

You may visit the following API resources for getting started and working with the API.

*   [Product Documentation][3] – Detailed API documentation with code examples and details about API functional areas
*   [API Reference Guide][4] – Detailed information about the API namespaces and classes
*   [GitHub Examples][5] – Ready to run code samples in downloadable form
*   [Aspose.Tasks Forum][6] – Our online support forum where we address your queries and inquiries




[1]: https://www.nuget.org/packages/Aspose.Tasks/
[2]: https://docs.aspose.com/tasks/net/aspose-tasks-for-net-18-5-release-notes/
[3]: https://docs.aspose.com/display/tasksnet/Home
[4]: http://www.aspose.com/api/net/tasks
[5]: https://github.com/asposetasks/Aspose_Tasks_NET
[6]: https://forum.aspose.com/c/tasks





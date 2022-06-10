---
title: 'Improved Performance of Tasks Creation using Aspose.Tasks for .NET 9.5.0'
date: Wed, 03 Aug 2016 18:09:56 +0000
draft: false
url: /2016/08/03/improved-performance-of-tasks-creation-using-aspose.tasks-for-.net-9.5.0/
author: Kashif Iqbal
summary: ''
tags: []
categories: ['Aspose.Tasks Product Family']
---



{{< figure align=center src="images/Aspose.Tasks-for-.NET_.png" alt="">}}


We are pleased to announce the release of [Aspose.Tasks for .NET 9.5.0][1]. This month’s release includes minor enhancements related to API functionality of exporting project data. It also includes performance improvement while creating large number of tasks. In addition, a number of reported bugs have been fixed in this month’s release that further improves the overall stability and functionality of the API. For a detailed note on what is new and fixed, please visit our [Product download page][2].

## Control Document Header Name during Export to HTML

Exporting project data to HTML included document header in output Title as well as page header. This month’s release provides control to avoid exporting this information to output HTML file if not required. The IncludeProjectNameInTitle and IncludeProjectNameInPageHeader properties can be used to achieve this.  These properties are set to true by default.

## Performance Improvement while Creating Tasks

This month’s release brings performance improvement while creating large number of tasks using the API. The automatic calculation mode of the API calculates each and every field of a task upon adding new tasks. This can be taken care of by using the Manual Calculation mode of the API. We have further improved the manual calculation mode so that it takes less time while creating large number of tasks such as up to 10,000.

## Other Improvements

This month’s release also fixes a number of bugs reported by our valued customers. These include issues related to loading Primavera project files, change in predecessor’s information while loading and saving MPP file, and setting task notes to Chinese language.

## API Resources

You may visit the following API resources for getting started and working with the API.

*   [Product Documentation][3] – Detailed API documentation with code examples and details about API functional areas
*   [API Reference Guide][4] – Detailed information about the API namespaces and classes
*   [GitHub Examples][5] – Ready to run code samples in downloadable form
*   [Aspose.Tasks Forum][6] – Our online support forum where we address your queries and inquiries




[1]: https://products.aspose.com/tasks/net
[2]: https://downloads.aspose.com/tasks/net
[3]: https://docs.aspose.com/tasks/net
[4]: http://www.aspose.com/api/net/tasks
[5]: https://github.com/asposetasks/Aspose_Tasks_NET
[6]: https://forum.aspose.com/c/tasks





---
title: 'Importing Project Data from Primavera Database using C#'
date: Mon, 10 Aug 2015 14:52:00 +0000
draft: false
url: /2015/08/10/importing-project-data-from-primavera-database-using-csharp/
author: Kashif Iqbal
summary: ''
tags: []
categories: ['Aspose.Tasks Product Family']
---



{{< figure align=center src="images/aspose-Tasks-for-net_100.png" alt="">}}


We are pleased to announce the release of [Aspose.Tasks for .NET][1] 8.6.0. This month’s release includes enhancement related to reading project data from Primavera Database. It also includes a number of bug fixes related to different API functional areas. You may visit Aspose.Tasks [product page][2] to have complete details about the issues fixed in this month’s release. Our documentation article, Public API Changes in Aspose.Tasks for .NET 8.6.0, lists all the changes included in this latest version.

## Retrieving Project Data from Primavera Database in C#

Aspose.Tasks API already supports importing Project data from various Primavera file formats such as XML and MPX. This month’s release further extends the capability of the API to retrieve Project data from Primavera database. The PrimaveraDBSettings class provides the interface for setting a connection to the Primavera Database. This is achieved by specifying the connection stirng parameters in the SqlConnectionStringBuilder class. The Project class now offers an overloaded method that accepts the PrimaveraDBSettings class object. The complete snippet for connecting and importing data from Primavera database is as follow:

```
 SqlConnectionStringBuilder sb = new SqlConnectionStringBuilder();
sb.DataSource = "192.168.56.3,1433";
sb.Encrypt = true;
sb.TrustServerCertificate = true;
sb.InitialCatalog = "PrimaveraEDB";
sb.NetworkLibrary = "DBMSSOCN";
sb.UserID = "privuser";
sb.Password = "***";

// Initialize a new instance of the PrimaveraDbSettings class 
//with connection string and project id
PrimaveraDbSettings settings = new PrimaveraDbSettings(sb.ConnectionString, 4502);

// Initialize a new instance of the Project class
Project project = new Project(settings); 
```

## Bug Fixes

This month’s release also includes a number of API improvements as a result of various bug fixes. These include:

*   Calculation errors while setting task duration with 24 hour calendar
*   Difference in dates calculation with different types of task links
*   Incorrect rendering of task links
*   Exception while loading MPP file with resource assignment work having large values

## API Resources

Our documentation and Examples contain a number of API resources that can help getting started with the API in no time. You can:

*   Navigate through the API Documentation for having an idea about the overall API sections and code samples.
*   Visit the [GitHub examples][3] page of the API for downloadable code samples.
*   Go through the API reference guide for details about the Project classes, methods and properties.

If you have any queries related to the API usage or anything, please feel free to write to us over [Aspose.Tasks forum][4].




[1]: https://products.aspose.com/tasks/net
[2]: https://products.aspose.com/tasks/net
[3]: https://github.com/asposetasks/Aspose_Tasks_NET
[4]: https://forum.aspose.com/c/tasks





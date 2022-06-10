---
title: 'Mega Systems reduced MS Project files processing time from hours to minutes using Aspose APIs'
date: Tue, 13 Mar 2018 17:05:59 +0000
draft: false
url: /2018/03/13/reading-and-writing-mpp-files-using-aspose-tasks/
author: Henrique Ramos
summary: ''
tags: ['Aspose.Tasks', 'Easily create and manipulate MS Project files', 'Efficient and reliable MS Project file processing APIs', 'Extensive documentation and helpful code samples', 'Process MS Project files using Aspose.Tasks for .NET', 'Success Stories']
categories: ['Aspose.Tasks Product Family']
---

## About Mega Systems



{{< figure align=center src="images/logo-mega-sistemas.png" alt="Mega Sistemas company logo">}}


[Mega Systems][1] is a Brazilian company that produces a business management system (ERP) focused on companies in the civil construction and manufacturing sector. Mega Sistemas has 400 employees and over 2000 clients.

## Problem

In the construction industry, it is very normal for our clients to send data from the ERP to MSProject and also to consume MPP files to update the data in the ERP. Previously we used the MSProject APIs to read and write data to MPP files, but the process was very slow. We controlled the construction of large buildings where the MPP file usually had more than 7000 tasks and 5000 resources, and through the MSProject APIs, this generation process used to take around 2 hours.

## Solution

Using the [Aspose Tasks for .NET][2], we achieved the same result but within a few minutes.

In order to use [Aspose.Tasks for .NET][3], a server application was created, which executed in the application server of the company (_which used our system_). The client application made a call to the server sending the data in JSON format and received the MPP file with all the content. Or, it uploaded the MPP file and as a result, it received the data in JSON format.

The communication process between the client application and the server used Google GRPC.



{{< figure align=center src="images/Case_Study_MegaSistemas-aspose.tasks_-1024x550.png" alt="Aspose.Tasks.Project class in code" caption="Image 1:- Using [Aspose.Tasks.Project class](https://apireference.aspose.com/tasks/net/aspose.tasks/project) to read and write MPP files">}}




{{< figure align=center src="images/Case_Study_MegaSistemas-aspose.tasks-1-1024x550.png" alt="Class distribution preview of Aspose.Tasks for .NET" caption="Image 2:- Class Distribution">}}


## Experience

### Finding a solution

[Aspose.Tasks for .NET][4], as well as other components, were found through Google. So we set up a study project with the [trial version][5] to test all the components we found over the internet. In the end, we decided on [Aspose.Tasks for .NET][6] due to the ease of use, performance in generating the MPP files and the [technical support][7] obtained from [Aspose][8].

### Implementation

The development of the final solution with [Aspose.Tasks for .NET][9] took about 1 month and the [Code Samples][10], [Documentation][11] and [API References][12] were found exceptional while obtaining the expected result. We accomplished our goals simply and fairly quickly.

The final application was a specific model developed by the Mega System to model the ERP data in the format that was used to communicate. The client application did not know the [Aspose][13] model but only the ERP model. In the server application, the ERP model was converted to the [Aspose.Tasks for .NET][14] model and the MPP file was generated. At the end of the process, the server application sent the MPP file in binary format to the client application.

### Outcome

As a result of the project, we will have a much simpler deploy and without the need for MSProject validations with each new version, making our work more profitable.

## Next Steps

If we need to integrate with any other MSOffice product, of course, we will initially test with [Aspose products][15].

## Summary

It was very good to use the [Aspose Tasks for .NET][16], as we were able to develop our server application for generating MPP files fairly quickly and cheaply.

In the end, we got a simpler system to maintain, deploy and also a cheaper solution for our customers.

**Henrique Ramos**, Systems Analyst  
[Mega Sistemas Corporativos S/A][17]




[1]: https://www.mega.com.br/home/
[2]: https://products.aspose.com/tasks/net
[3]: https://products.aspose.com/tasks/net
[4]: https://products.aspose.com/tasks/net
[5]: https://downloads.aspose.com/tasks/net
[6]: https://products.aspose.com/tasks/net
[7]: https://forum.aspose.com/c/tasks
[8]: https://www.aspose.com/
[9]: https://products.aspose.com/tasks/net
[10]: https://github.com/aspose-tasks/Aspose.Tasks-for-.NET
[11]: https://docs.aspose.com/display/tasksnet/Home
[12]: https://apireference.aspose.com/tasks/net
[13]: https://www.aspose.com/
[14]: https://products.aspose.com/tasks/net
[15]: https://products.aspose.com/
[16]: https://products.aspose.com/tasks/net
[17]: https://www.mega.com.br/





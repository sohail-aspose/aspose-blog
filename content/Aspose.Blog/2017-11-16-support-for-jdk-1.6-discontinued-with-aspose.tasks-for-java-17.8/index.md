---
title: 'Support for JDK 1.6 Discontinued with Aspose.Tasks for Java 17.8'
date: Thu, 16 Nov 2017 16:05:59 +0000
draft: false
url: /2017/11/16/support-for-jdk-1.6-discontinued-with-aspose.tasks-for-java-17.8/
author: Kashif Iqbal
summary: ''
tags: []
categories: ['Aspose.Tasks Product Family']
---



{{< figure align=center src="images/Aspose.Tasks-for-Java.png" alt="Aspose.Tasks for Java">}}


We are pleased to announce the release of [Aspose.Tasks for Java 17.8][1]. This release includes a new feature of providing support for rate scale information in MPP files. It also includes several improvements in terms of bug fixes that further add to the overall stability of the API. From this month’s release, support for JDK 1.6 has been discontinued. For a complete list of what is new and fixed, please visit the [release notes][2] section of API documentation.

## Discontinued Support for JDK 1.6

From this release onwards, Aspose.Tasks for Java won’t support JDK 1.6. All our customers, who are using older version of JDK and want to use this latest version of API, need to upgrade their Java version to meet the minimum requirement of API i.e. JDK 1.7 or higher.

## Improvements in Aspose.Tasks for Java 17.8

**Support for Rate Scale Information Reading Writing:** Aspose.Tasks for Java already supported reading/writing rate scale information of resource assignment for MPP 2013 and below versions. With this release, the API now supports [reading and writing rate scale data][3] for MSP 2013 and above file formats. This is as illustrated in the following code sample:

```
String dataDir = Utils.getDataDir(AssignmentCost.class);
		
Project project = new Project(dataDir + "New project 2013.mpp");

Task task = project.getRootTask().getChildren().add("t1");

Resource materialResource = project.getResources().add("materialResource");
materialResource.set(Rsc.TYPE, ResourceType.Material);

Resource nonMaterialResource = project.getResources().add("nonMaterialResource");
nonMaterialResource.set(Rsc.TYPE, ResourceType.Work);

ResourceAssignment materialResourceAssignment = project.getResourceAssignments().add(task, materialResource);
materialResourceAssignment.set(Asn.RATE_SCALE, RateScaleType.Week);

ResourceAssignment nonMaterialResourceAssignment = project.getResourceAssignments().add(task, nonMaterialResource);
nonMaterialResourceAssignment.set(Asn.RATE_SCALE, RateScaleType.Week);

project.save("output.mpp", SaveFileFormat.MPP); 
```

**Loading Project Data from MSP Database:**  Working with loading project data from Microsoft Project Data was supported in one of the earlier versions of API. This, however, had issues with the update of [Microsoft Project Database versions][4] update and the functionality was broken. We are glad to share that this issue has been fixed now. You can now load Project data from Project database using this latest version of the API.

## API Resources

*   [Product Documentation][5]– Provides complete information about system requirements, installation, Programmer’s Guide, Technical articles and API Changes
*   [API Reference Guide][6]– Provides information about the product namespaces, classes and methods
*   [GitHub Examples][7]– Ready to download and execute examples of the API
*   [Forum Support][8]– Post your queries/inquiries on Aspose.Tasks forum to get support from our technical support team.




[1]: http://downloads.aspose.com/tasks/java
[2]: https://docs.aspose.com/tasks/java/aspose-tasks-for-java-17-8-release-notes/
[3]: https://docs.aspose.com/tasks/java/
[4]: https://docs.aspose.com/tasks/java/creating-reading-and-saving-projects/#reading-project-data-from-microsoft-project-database
[5]: https://docs.aspose.com/tasks/java/
[6]: https://apireference.aspose.com/tasks/java/
[7]: https://github.com/asposetasks/Aspose_TASKS_Java
[8]: https://forum.aspose.com/c/tasks





---
title: 'Read OpenProj XML Files and Export Project Data using Java'
date: Tue, 01 Jul 2014 13:46:13 +0000
draft: false
url: /2014/07/01/read-openproj-xml-files-and-export-project-data-using-java/
author: Kashif Iqbal
summary: ''
tags: []
categories: ['Aspose.Tasks Product Family']
---



{{< figure align=center src="images/aspose-Tasks-for-Java_100.png" alt="">}}


We are pleased to announce the release of Aspose.Tasks for Java 6.8.0. Ported from the equivalent .NET version, this month’s release offers the same new features, enhancements and bug fixes. To get an idea about what is new and fixed, visit the Aspose.Tasks [product download page][1]. You can also download this latest version from the same download page.

## Export Project Data to Individual Image Files

This month’s release further empowers Aspose.Tasks users to [render project data][2] to multiple individual image files, which was not possible with earlier versions of the API. The setSaveToSeparateFiles method of the ImageSaveOptions class allows developers to save project data to separate files. In addition, the getPages() method of ImageSaveOptions returns a list of page numbers to save when saving Project layouts to separate files.

## Read OpenProj XML Files using Java

OpenProj, also known as ProjectLibre, is an open source project management tool that can export project data to XML format. Previously, the Aspose.Tasks API lacked support for reading the output XML files. However, we are pleased to share that this month’s release supports reading XML files created by OpenProj.

## Setting TimeScale Count using Java

Rendering time scale information to output formats is already supported by Aspose.Tasks API. However, the feature didn’t include the time scale count information. This month’s release further enhances this rendering capability by providing the facility to set [time scale count][3] for a Project. The TimeScaleTier class’s setCount() method can be used to achieve this.

## Displaying Custom Field Columns in Gantt Chart View

This month’s release also introduces a new feature: configuring the Gantt chart view to display custom fields by default in Microsoft Project. Each time the file is opened in MSP, the saved columns settings are displayed to the user. This can be achieved by customizing a project's table data.




[1]: https://downloads.aspose.com/tasks
[2]: https://docs.aspose.com/tasks/java/render-project-to-multipage-tiff/
[3]: https://docs.aspose.com/tasks/java/working-with-project-views/





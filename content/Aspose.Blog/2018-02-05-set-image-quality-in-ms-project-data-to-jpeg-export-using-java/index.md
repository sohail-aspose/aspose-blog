---
title: 'Set Image Quality When Exporting Project to JPEG using Java'
date: Mon, 05 Feb 2018 15:35:31 +0000
draft: false
url: /2018/02/05/set-image-quality-in-ms-project-data-to-jpeg-export-using-java/
author: Kashif Iqbal
summary: ''
tags: []
categories: ['Aspose.Tasks Product Family']
---



{{< figure align=center src="images/Aspose.Tasks-for-Java.png" alt="Aspose.Tasks for Java">}}


[Aspose.Tasks for Java 17.11][1] has been published. This release includes a new feature that allows users to set image quality while exporting project data to JPEG format. It also includes several other improvements as result of bug fixes that further enhances the API functionality. For a detailed note on what is new and fixed, please visit the [release notes][2] section in API documentation.

## Export Project Data to JPEG - Set Image Quality

This release of Aspose.Tasks for Java API includes a new feature that lets you set the [image quality][3] while exporting project data to JPEG. The setJPEGQuality method of ImageSaveOptions lets you achieve this by providing image quality at a scale from 0 to 100, as shown in the following code sample.

{{< gist aspose-com-gists 472405ac9bab4502a485ee007b92074c "Examples-src-main-java-com-aspose-tasks-examples-Projects-SaveProjectAsJPEG-SaveProjectAsJPEG.java" >}}

## Other Improvements

This version also includes other improvements in terms of bug fixes that add to the overall improvement of the API in terms of expected behavior. These include:

*   Exceptions while loading certain MPP files
*   Errors while converting Project data to PDF
*   Calculation issues with Calendar times set to 24 hours
*   Task reading exceptions while loading MPP files
*   Wrong calculation of Finish date and Percent Complete in MPP files
*   Problem with setting working days
*   Missing time span with SplitParts collection
*   Improvements in the manual calculation of tasks data

## API Resources

*   [Product Documentation][4] – Provides complete information about system requirements, installation, Programmer’s Guide, Technical articles and API Changes.
*   API Reference Guide – Provides information about the product namespaces, classes, and methods.
*   [GitHub Examples][5] – Ready to download and execute examples of the API.
*   [Forum Support][6] – Post your queries/inquiries on Aspose.Tasks forum to get support from our technical support team.




[1]: http://maven.aspose.com/repository/simple/ext-release-local/com/aspose/aspose-tasks/17.11/
[2]: https://docs.aspose.com/display/tasksjava/Aspose.Tasks+for+Java+17.11+Release+Notes
[3]: https://docs.aspose.com/display/tasksjava/Saving+Project+Data+to+JPEG#SavingProjectDatatoJPEG-ExportingProjectDatatoJPEG
[4]: https://docs.aspose.com/display/tasksjava/Home
[5]: https://github.com/asposetasks/Aspose_TASKS_Java
[6]: https://forum.aspose.com/c/tasks





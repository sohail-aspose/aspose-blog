---
title: 'Improved Project Data Rendering with Aspose.Tasks for .NET 7.1.0'
date: Fri, 03 Oct 2014 20:33:25 +0000
draft: false
url: /2014/10/03/improved-project-data-rendering-with-aspose.tasks-for-.net-7.1.0/
author: Kashif Iqbal
summary: ''
tags: []
categories: ['Aspose.Tasks Product Family']
---

[![][1]](https://products.aspose.com/tasks/net)We are pleased to announce the release of Aspose.Tasks for .NET 7.1.0 which comes with a number of enhancements related to data rendering. It also fixes a number of bugs reported with last month’s release. For detailed information about the issues fixed in this month’s release, please visit the [product download page][2]. You may also consider sharing your feedback with us over the [Aspose.Tasks forum][3].

## Rendering Footer Section Elements

Microsoft Project renders Microsoft Project information and other legend entries while writing project data to formats such as PDF, PNG, BMP, etc. Aspose.Tasks lacked this functionality in that it missed certain information. However, this month’s release implements the difference between rendering the Gantt chart information by MSP and Aspose.Tasks. This includes addition of:

*   Tasks deadline rendering in Gantt chart.
*   Tasks progress rendering in Gantt chart.
*   Project information such as name and current date.
*   Start, finish and duration to page legend.
*   Inactive milestones, summary and manual summary roll up to Gantt chart and page legend.

## Support for Rendering Source MPP Columns in TaskUsage and ResourceUsage

In last month’s release, the API incorporated the capability to render all the columns as in the source MPP files. This was supported for the GanttChart, TaskSheet and ResourceSheet views. This month’s release further adds this functionality for the TaskUsage and ResourceUsage views.

## Other Enhancements

This month’s release also includes additional enhancements as detailed below:

**Saving project data to multiple PDF files:** In one of our earlier versions, we introduced the feature of rendering project data to multiple output image files. This month’s version further modifies the same functionality for rendering data to separate PDF files as follow:

```
Project project = new Project("RenderMe.mpp");
PdfSaveOptions saveOptions = new PdfSaveOptions();
saveOptions.SaveToSeparateFiles = true;
saveOptions.Pages = new List<int>();
saveOptions.Pages.Add(1);
saveOptions.Pages.Add(4);
project.Save("result.pdf", saveOptions); 
```

**Specifying date/time format for rendering:** This month’s release introduces the feature of setting project date rendering format. The project’s DateFormat property has been introduced for this purpose that can be set to a number of date formats using the DateFormat enumeration as shown in the following code sample.

```
Project project = new Project();
project.StartDate = new DateTime(2014, 9, 22);
// By default project.DateFormat == DateFormat.Date_ddd_mm_dd_yy (Mon 09/22/14)
// customize DateFormat (September 22, 2014)
project.DateFormat = DateFormat.Date_mmmm_dd_yyyy;
project.Save("saved.pdf", SaveFileFormat.PDF); 
```

**Custom styling for overallocated resources**: With this month’s release, the API provides the facility to customize the text style for overallocated resources. By default, the TextStyle for overallocated resources is similar to Microsoft Project (MSP), that is, red color and bold. The implementation of the TextItemType.OverallocatedResources enables for customizing the color and style for the overallocated resoures as follow:

```
Project project = new Project("Advanced Assignments A_Start.mpp");
SaveOptions options = new PdfSaveOptions();
options.PresentationFormat = PresentationFormat.ResourceSheet;
TextStyle style = new TextStyle();
style.Color = Color.OrangeRed;
style.FontStyle = FontStyle.Bold;
style.FontStyle |= FontStyle.Italic;
style.ItemType = TextItemType.OverallocatedResources;
options.TextStyles = new List<TextStyle>();
options.TextStyles.Add(style);
project.Save("temp.pdf", options); 
```

**Retaining source MPP time scale information during rendering:** This month’s release also provides the capability to retain the source MPP’s time scale information while rendering the project data to various formats.

## Bug Fixes and Other Improvements

This month’s release also fixes a number of bugs that further ads to the overall API functionality improvement. These include:

*   Task reading exceptions while loading some MPP files.
*   Reading tasks from a MPP.
*   Missing output data while rendering MPP to PDF.
*   Issues related to Gantt chart.




[1]: https://blog.aspose.com/wp-content/uploads/sites/2/2014/10/aspose-Tasks-for-net_100.png "aspose-Tasks-for-net_100"
[2]: http://www.aspose.com/community/files/51/.net-components/aspose.tasks-for-.net/entry577288.aspx
[3]: http://www.aspose.com/community/forums/aspose.tasks-product-family/96/showforum.aspx





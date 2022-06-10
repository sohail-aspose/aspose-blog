---
title: 'Enhanced MPP to HTML Conversion with Aspose.Tasks for .NET 18.7'
date: Sun, 05 Aug 2018 18:51:20 +0000
draft: false
url: /2018/08/05/enhanced-mpp-to-html-conversion-with-aspose.tasks-for-.net-18.7/
author: Kashif Iqbal
summary: ''
tags: ['Convert MS Project MPP files to HTML', 'NET API for MS Project', 'mpp to html']
categories: ['Aspose.Tasks Product Family']
---



{{< figure align=center src="images/Aspose.Tasks-for-.NET_.png" alt="aspose-tasks-for-net">}}


We are pleased to announce the release of [Aspose.Tasks for .NET 18.7][1]. This release further enhances the Project data conversion to HTML by providing the capability to save HTML elements to separate files. It also fixes several issues reported with the API that further enhances the adds to the overall stability of the API. For a detailed note on what is new and fixed, please visit the [release notes][2] section of API documentation.

# MPP to HTML - Saving Fonts, Images and CSS Styles Separately

This release of Aspose.Tasks for .NET API lets you export the fonts, images and CSS styles to separate files while exporting project data to HTML. It also provides the options to assign callback functions to the export process for assignment of necessary parameters. These modifications have been added to the HtmlSaveOptions class of the API and can be utilized as shown in the following code sample.

```
var options = new HtmlSaveOptions { FontFaceTypes = FontFaceType.Ttf, PageSize = PageSize.A0, ExportImages = ResourceExportType.AsFile };

var savingCallbacks = new UserSavingCallbacks
{
    RootFolder = this.ResultFolder.Value + "SavingCallbacks",
    KeepCssStreamOpened = true,
    CssFolder = "css",
    ImagesFolder = "images",
    FontsFolder = "fonts"
};
options.CssSavingCallback = savingCallbacks;
options.FontSavingCallback = savingCallbacks;
options.ImageSavingCallback = savingCallbacks;
if (!Directory.Exists(savingCallbacks.RootFolder))
{
    if (!Directory.Exists(savingCallbacks.RootFolder))
    {
        Directory.CreateDirectory(savingCallbacks.RootFolder);
    }
}

var project = new Project(Common.TestdataPath + "HtmlTest\\TestExportCssFontsImages.mpp");
project.Save(Path.Combine(savingCallbacks.RootFolder, "document.html"), options);

using (var writer = new StreamWriter(savingCallbacks.CssStream))
{
    writer.WriteLine();
    writer.WriteLine("/* This line is appended to stream manually by user */");
}
```

# Removal of Obsolete Extended Attributes Members

From this release onward, the obsolete members of ExtendedAttributeDefinition and OutlineValue have been removed. This is important to note as you’ll have to replace any such occurrences of Obsolete members with the new methods and techniques that have been available as a replacement for a long time now. All the examples related to these have been updated in the [API documentation][3] and can be referred for utilization.

## API Resources

You may visit the following API resources for getting started and working with the API.

*   [Product Documentation][4] – Detailed API documentation with code examples and details about API functional areas
*   [API Reference Guide][5] – Detailed information about the API namespaces and classes
*   [GitHub Examples][6] – Ready to run code samples in downloadable form
*   [Aspose.Tasks Forum][7] – Our online support forum where we address your queries and inquiries




[1]: https://www.nuget.org/packages/Aspose.Tasks/
[2]: https://docs.aspose.com/display/tasksnet/Aspose.Tasks+for+.NET+18.7+Release+Notes
[3]: https://docs.aspose.com/display/tasksnet/Working+with+Extended+Attributes+of+a+Project
[4]: https://docs.aspose.com/display/tasksnet/Home
[5]: http://www.aspose.com/api/net/tasks
[6]: https://github.com/asposetasks/Aspose_Tasks_NET
[7]: https://forum.aspose.com/c/tasks





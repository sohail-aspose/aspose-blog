---
title: 'ASP.NET Excel Viewer - View Excel Files in ASP.NET MVC using C#'
seoTitle: ""
description: ""
date: Fri, 31 Jan 2020 13:26:59 +0000
draft: false
url: /2020/01/31/view-excel-files-in-asp-net-mvc-csharp-excel-viewer/
author: Usman Aziz
summary: ''
tags: ['ASP.NET MVC Excel Viewer', 'Display Excel Files in ASP.NET', 'Display Excel Sheets in ASP.NET Web Page', 'Excel Viewer', 'Excel Viewer in ASP.NET MVC', 'Excel file viewer']
categories: ['Aspose.Cells Product Family']
---



{{< figure align=center src="images/ASP.NET-Excel-Viewer.png" alt="C# ASP.NET Excel Viewer">}}


Do you want to display Microsoft Excel worksheets within your web application? Are you looking for an **ASP.NET MVC Excel Viewer**? If yes, you have landed in an absolutely correct place. In this blog, you will learn how to create an **Excel Viewer** and **display Excel worksheets in ASP.NET MVC** applications using **C#**. After spending a few minutes and following some simple steps you will have your own Excel (**XLS** or **XLSX**) Viewer up and running. So let's begin.

## Features of ASP.NET MVC Excel Viewer

Our ASP.NET Excel Viewer will have the following features and you can enhance them as per your requirements.

1.  Browse and view Excel files.
2.  Load default Excel file on page load.
3.  Tabs to navigate between Excel worksheets.

## Steps to Create Excel Viewer in ASP.NET MVC

The following are some easy steps to view Excel files in ASP.NET MVC.

**1.** Create a new _ASP.NET MVC_ web application in Visual Studio.



{{< figure align=center src="images/C-ASP.NET-MVC-Project.png" alt="ASP.NET MVC Web Application">}}


**2.** Open _NuGet Package Manager_ and install [Aspose.Cells for .NET][1] package.



{{< figure align=center src="images/NPM-Aspose.Cells-for-.NET_.png" alt="View Excel files in ASP.NET in browser">}}


**3.** Create a new folder "_Documents_" to keep the Excel files and a subfolder "_Rendered_" to save rendered images.

**4.** Create a new folder with the name "_Helpers_" in the root folder.

**5.** Create a new class with the name "_Sheet_" in the "_Helpers_" folder to store the Excel worksheets' information.

{{< gist aspose-com-gists cb30d0f5d0b3fb1ffe74a2ee6681eee9 "Sheet.cs" >}}

**6.** Open the "_HomeController_" class and replace it's code with the following. Make sure to replace the default Excel file's name in _Index_ action.

{{< gist aspose-com-gists cb30d0f5d0b3fb1ffe74a2ee6681eee9 "HomeController.cs" >}}

**7.** Open _Views/Home/index.cshtml_ and replace its content with the following script.

{{< gist aspose-com-gists cb30d0f5d0b3fb1ffe74a2ee6681eee9 "index.cshtml" >}}

**8.** Build the application and run it in your favorite browser.

## View Excel Files in ASP.NET MVC Viewer - Demo

The default Excel file will be displayed when you'll start the application for the first time.



{{< figure align=center src="images/Excel-Viewer-1024x571.png" alt="Excel Viewer in ASP.NET C#">}}


### Open an Excel File

In order to open an Excel file, click the _browse_ button and select the file from the list.



{{< figure align=center src="images/Browse-Excel-File-Button.png" alt="Browse Excel Files">}}




{{< figure align=center src="images/Browse-Excel-File.png" alt="Open Excel file in ASP.NET C#">}}


### Navigate Between Excel Worksheets using Tabs

All the worksheets in the Excel workbook will be displayed in the form of tabs. You can click the tabs to navigate between worksheets.



{{< figure align=center src="images/Excel-Worksheet-Tabs.png" alt="Display Excel Files in ASP.NET">}}


### Download Source Code

This application is open source and its source code is available on [GitHub][2].

## Get a Temporary License for Aspose.Cells for .NET

You can get the [temporary license][3] of _Aspose.Cells for .NET_ API to avoid evaluation/trial limitations.




[1]: https://products.aspose.com/cells/net
[2]: https://github.com/Usman Azizgroupdocs/ASP.NET-MVC-Excel-Viewer
[3]: https://purchase.aspose.com/temporary-license






---
title: 'Create, Read, and Edit Excel Spreadsheets in ASP.NET MVC'
seoTitle: "Create, Read, Edit Excel Files in ASP.NET MVC C# | Source Code"
description: "Create your own spreadsheet application in ASP.NET MVC to display, create or edit Excel and other spreadsheet files. Download source code of application."
date: Wed, 25 Aug 2021 11:41:00 +0000
draft: false
url: /2021/08/25/create-read-edit-excel-spreadsheet-in-asp-net-mvc/
author: Usman Aziz
summary: 'In this article, you will learn **how to create, read, and edit Excel spreadsheets in **an ASP.NET MVC application****. For this, we will create a spreadsheet application consisting of a feature-rich grid control to display and edit Excel files, as shown below.'
tags: ['asp-net spreadsheet application', 'create excel files in asp-net', 'edit excel files in asp-net', 'excel application in asp-net']
categories: ['Aspose.Cells Product Family']
---

In this article, you will learn **how to create, read, and edit Excel spreadsheets in **an ASP.NET MVC application****. For this, we will create a spreadsheet application consisting of a feature-rich grid control to display and edit Excel files, as shown below.



{{< figure align=center src="images/ASP.NET-UI.jpg" alt="">}}


*   [.NET API to Create ASP.NET Spreadsheet Application][1]
*   [Steps to Create ASP.NET Spreadsheet Application][2]
*   [Demo][3]
*   [Download Source Code][4]

## .NET API to Create ASP.NET MVC Spreadsheet Application {#NET-API-to-Create-ASP-NET-Spreadsheet-Application}

In order to create the spreadsheet application in ASP.NET MVC, we will use **Aspose.Cells.GridJs**. The API allows you to create web-based applications to display or edit spreadsheet documents quickly and easily. Furthermore, you can import the popular spreadsheet (XLS, XLSX, XLSM, XLSB, CSV, SpreadsheetML, ODS) file formats ([read more][5]. In addition, It provides a strong and rich Formula Calculation Engine to calculate not only the built-in functions but also custom formulas. You can install **Aspose.Cells.GridJs** from [NuGet][6].

```
PM> Install-Package Aspose.Cells.GridJs
```

## Steps to Create ASP.NET MVC Spreadsheet Application {#Steps-to-Create-ASP-NET-Spreadsheet-Application}

The following are the steps to create a web-based spreadsheet application in ASP.NET MVC.

1.  Create a new **ASP.NET Core Web App (Model-View-Controller)** in Visual Studio.



{{< figure align=center src="images/Create-Project.jpg" alt="">}}


2\. Install **Aspose.Cells.GridJs** from NuGet.



{{< figure align=center src="images/Install-AsposeCells_GridJs.jpg" alt="">}}


3\. Insert the following code into **HomeController.cs**.

{{< gist aspose-com-gists 16c772f40a913fd05a8095ae63bff248 "HomeController.cs" >}}

4\. Create a new class named **TestConfig.cs** in **Models** folder and add the following code (change the folder paths according to your environment).

{{< gist aspose-com-gists 16c772f40a913fd05a8095ae63bff248 "TestConfig.cs" >}}

5\. Create a new class named **LocalFileCache.cs** in **Models** folder and add the following code.

{{< gist aspose-com-gists 16c772f40a913fd05a8095ae63bff248 "LocalFileCache.cs" >}}

6\. Create a new controller named **GridJs2Controller.cs** and add the following code.

{{< gist aspose-com-gists 16c772f40a913fd05a8095ae63bff248 "GridJs2Controller.cs" >}}

7\. Insert the following code in the **Configure** function of **Startup.cs** and set the license file's path ([get a license for free][7].

{{< gist aspose-com-gists 16c772f40a913fd05a8095ae63bff248 "Startup.cs" >}}

8\. Insert the following code in **Views/Home/index.cshtml**.

{{< gist aspose-com-gists 16c772f40a913fd05a8095ae63bff248 "index.cshtml" >}}

9\. Create a new view named **list.cshtml** under **Views/Home/** folder and insert the following code.

{{< gist aspose-com-gists 16c772f40a913fd05a8095ae63bff248 "list.cshtml" >}}

10\. Download the [xspread][8] folder from GitHub and place it under **wwwroot** folder, as shown below.



{{< figure align=center src="images/Import-GridJs-Folder.jpg" alt="">}}


11\. Make sure that the port number specified in **wwwroot/xspread/index.html** is the same as the project's port number.

12\. Build the application and run it in your favorite browser.

## Demo - Create or Edit Excel Files in ASP.NET MVC {#Demo}

The following is the demonstration of the ASP.NET MVC spreadsheet application we have just created.



{{< figure align=center src="images/GridJsDemo.gif" alt="">}}


## Download Source Code {#Download-Source-Code}

You can download the complete source code of the spreadsheet application from [GitHub][9].

## Get a Free License {#Get-a-Free-License}

You can use Aspose.Cells.GridJs without evaluation limitations using a [temporary license][10].

## Conclusion

In this article, you have learned how to create an ASP.NET MVC spreadsheet application with a range of features to create and edit Excel and other spreadsheet files. You can customize this application or integrate it into your own web application. In case you would have any queries, feel free to post to our [forum][11].

## See Also

*   [Create MS Excel Files Programmatically in C# without MS Office][12]




[1]: #NET-API-to-Create-ASP-NET-Spreadsheet-Application
[2]: #Steps-to-Create-ASP-NET-Spreadsheet-Application
[3]: #Demo
[4]: #Download-Source-Code
[5]: https://docs.aspose.com/cells/net/aspose-cells-gridjs/)
[6]: https://www.nuget.org/packages/Aspose.Cells.GridJs
[7]: https://purchase.aspose.com/temporary-license)
[8]: https://github.com/aspose-cells/Aspose.Cells-for-.NET/tree/master/Examples_GridJs/wwwroot/xspread
[9]: https://github.com/aspose-cells/Aspose.Cells-for-.NET/tree/master/Examples_GridJs/
[10]: https://purchase.aspose.com/temporary-license
[11]: https://forum.aspose.com/
[12]: https://blog.aspose.com/2020/01/21/create-excel-xls-xlsx-programmatically-in-csharp-net/






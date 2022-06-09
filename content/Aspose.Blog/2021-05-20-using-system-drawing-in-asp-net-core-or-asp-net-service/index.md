---
title: 'Using System.Drawing with ASP.NET Core or ASP.NET Service'
seoTitle: "Using System.Drawing with ASP.NET Core or ASP.NET Service"
description: "You can use System.Drawing in ASP.NET or ASP.NET Core. C# .NET Graphics API for working with graphics. Alternate Aspose.Drawing API for 2D Graphics."
date: Thu, 20 May 2021 21:53:00 +0000
draft: false
url: /2021/05/20/using-system-drawing-in-asp-net-core-or-asp-net-service/
author: Farhan Raza
summary: 'There are a lot of questions dedicated to the usage of System.Drawing library in ASP.NET services. The most common answer is that Microsoft does not recommend the usage of System.Drawing in ASP.NET services. In this article, you will learn details about using the interface of System.Drawing library in ASP.NET services with [Aspose.Drawing for .NET][1]. The following sections structure all the relevant information:'
tags: ['Aspose.Drawing in ASP.NET', 'Csharp Graphics Library', 'System.Drawing in ASP .NET Core', 'System.Drawing in ASP.NET']
categories: ['Aspose.Drawing Product Family']
---



{{< figure align=center src="images/System.Drawing-in-ASP-1024x536.png" alt="System.Drawing in ASP .NET ASP.NET Core">}}


There are a lot of questions dedicated to the usage of System.Drawing library in ASP.NET services. The most common answer is that Microsoft does not recommend the usage of System.Drawing in ASP.NET services.

In this article, you will learn details about using the interface of System.Drawing library in ASP.NET services with [Aspose.Drawing for .NET][2]. The following sections structure all the relevant information:

*   [Why Apose.Drawing?][3]
*   [Installing Aspose.Drawing for .NET API][4]
*   [Aspose.Drawing for .NET API - Introduction][5]
*   [Using Aspose.Drawing in ASP.NET Services][6]
    *   [Demonstration for using Aspose.Drawing in ASP.NET Services][7]
*   [Download Source Code][8]
*   [Conclusion][9]

## Why Aspose.Drawing? {#section1}

Microsoft does not recommend the usage of its System.Drawing library in ASP.NET services. The home page of System.Drawing [documentation][10] reads:

> _Classes within the System.Drawing namespace are not supported for use within a Windows or ASP.NET service. Attempting to use these classes from within one of these application types may result in run-time exceptions and diminished service performance._

There are two basic problems that compel Microsoft to write above caution. The first problem is the usage of GDI+ native library and, as result, usage of GDI handles. While the second concern is concurrency issues. For instance, a process-wide lock occurs during any DrawImage() operation. Therefore, you can not create fast and scalable ASP.NET services using the System.Drawing library from Microsoft.

## Installing Aspose.Drawing for .NET API {#section2}

You can easily download the DLL file from the [Downloads][11] section, or configure it via [NuGet][12] package Manager with the following command:

```
PM> Install-Package Aspose.Drawing
```

## Aspose.Drawing for .NET API - Introduction {#section3}

We understand that System.Drawing is very popular among developers because of its image manipulation features. That is why we have created a similar and compatible API without any compatibility issues. For your convenience and adaptability, the API contains the same names of classes, functions, enums, and interfaces. You can simply change the project reference from System.Drawing to Aspose.Drawing and recompile the program.

Moreover, Aspose.Drawing is a managed library available for NET Framework 2.0 and NET Core 2.0. Unlike System.Drawing, it has no dependencies on any platform like Linux, Azure, etc.

## Using Aspose.Drawing in ASP.NET Services {#section4}

Aspose.Drawing implementation does not depend on GDI or GDI+. It doesn't use GDI handles and rarely uses process-wide locks.

### Demonstration for using Aspose.Drawing in ASP.NET Services {#section5}

Let us create a simple application that explains the benefits of using Aspose.Drawing library:

Imagine that you decide to create an entirely new web service or application. The application will generate a set of thumbnails with filters attached to them from the user's image.

You can start by introducing few new entities:

{{< gist aspose-com-gists e5a714ced9148321c908cf1be53d034f "FilterType.cs" >}}

{{< gist aspose-com-gists e5a714ced9148321c908cf1be53d034f "FilterThumbnailResult.cs" >}}

Now you can define the interface for the generation of thumbnails with attached filters:

{{< gist aspose-com-gists e5a714ced9148321c908cf1be53d034f "IThumbnailGenerator.cs" >}}

Moving on to the implementation, assume implementing the IThumbnailGenerator interface using System.Drawing library. It will look like the next code snippet:

{{< gist aspose-com-gists e5a714ced9148321c908cf1be53d034f "ThumbnailGenerator.cs" >}}

The code will work fine but it has one disadvantage - it generates all thumbnails sequentially. System.Drawing library is based on quite old GDI+ library which was designed as single thread library so it can waste resources when there are multiple CPU cores.

Using Aspose.Drawing can help to significantly improve the performance because it does not has any limitations related to single thread. Please try changing only one function:

{{< gist aspose-com-gists e5a714ced9148321c908cf1be53d034f "GenerateAllThumbnails.cs" >}}

This code can now use multiple CPU cores without any significant changes in the original source code. Replacing System.Drawing with Aspose.Drawing expedites the performance of your applications and services.

## Download Source Code {#section6}

You may download the [Source Code][13] related to this example for your reference.

## Free API Evaluation License

You can request a [Free Temporary License][14] to test the API in its full capacity.

## Conclusion {#section7}

In conclusion, you have learned with example that how simple it is to use Aspose.Drawing library in your ASP.NET and ASP.NET Core services. Moreover, Aspose.Drawing has no problems or external dependencies that exist in System.Drawing. Furthermore, you can explore the API in detail by going through the [Documentation][15]. Please feel free to contact us anytime via [Free Support Forum][16] for any of your queries!

## See Also

[Using System.Drawing in Linux without libgdiplus][17]




[1]: https://docs.aspose.com/drawing/net/
[2]: https://docs.aspose.com/drawing/net/
[3]: #section1
[4]: #section2
[5]: #section3
[6]: #section4
[7]: #section5
[8]: #section6
[9]: #section7
[10]: https://docs.microsoft.com/en-us/dotnet/api/system.drawing?view=net-5.0
[11]: https://downloads.aspose.com/drawing/net
[12]: https://www.nuget.org/packages/Aspose.Drawing
[13]: https://drive.google.com/file/d/1JsLQzk8sqK-zHDmH8m-b_XnuscsjkLEV/view?usp=sharing
[14]: https://purchase.aspose.com/temporary-license
[15]: https://docs.aspose.com/drawing/net/
[16]: https://forum.aspose.com/c/drawing
[17]: https://blog.aspose.com/2020/12/13/using-system-drawing-in-linux/






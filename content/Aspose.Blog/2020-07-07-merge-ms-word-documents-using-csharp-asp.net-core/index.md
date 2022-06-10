---
title: 'Merge MS Word Documents using C# ASP.NET'
seoTitle: "Merge MS Word Documents in C# ASP.NET | Merge Multiple DOCX Files"
description: "Merge MS Word DOC/DOCX documents into a single document in C# ASP.NET Core. Merge Word documents into a single DOCX or PDF document in ASP.NET."
date: Tue, 07 Jul 2020 02:45:00 +0000
draft: false
url: /2020/07/07/merge-ms-word-documents-using-csharp-asp.net-core/
author: Usman Aziz
summary: ''
tags: ['append words documents in asp.net', 'asp.net word document merger app', 'merge MS Word documents in asp.net']
categories: ['Aspose.Words Product Family']
---



{{< figure align=center src="images/Merge-Word-Documents-ASP.NET_.jpg" alt="Merge Word Documents ASP.NET">}}


Merging multiple MS Word documents could be useful in various scenarios. For example, it can be used in keeping a similar type of documents into a single file, combining multiple documents before sharing, and so on. Various [online tools][1] are available that allow you to merge MS Word documents quite easily, however, what if you want to add this feature within your own application? To make you achieve this, I'll show you how to merge MS Word (DOC/DOCX) documents using C# within your ASP.NET web applications. This Word Document Merger application will have the following features:

*   Merge MS Word Documents into a Single Document
*   Download Merged Word Documents as DOCX Format
*   Download Merged Word Documents as PDF Format

## .NET API to Merge MS Word Documents in ASP.NET

[Aspose.Words for .NET][2] is a feature-rich word processing API that lets you process MS Word documents with ease. It also allows you to merge multiple Word documents into a single document within ASP.NET or any .NET/.NET Core application. Aspose.Words for .NET can be installed using [NuGet][3] as well as downloaded as a [DLL][4] file.

```
PM> install-package Aspose.Words
```

## Merge MS Word Documents in ASP.NET

The following are the steps to create an ASP.NET application that will let you merge two or more Word (DOC/DOCX) documents without using MS Office/Word.

*   Create an **ASP.NET Core Web Application** in Visual Studio.



{{< figure align=center src="images/ASP.NET-Core-MVC-Web-Application.jpg" alt="Create ASP.NET Core Web Application">}}


*   Choose the **Web Application (Model-View-Controller)** from the template list.



{{< figure align=center src="images/MVC-Project-Template.jpg" alt="Select MVC Application">}}


*   Install the **Aspose.Words for .NET** from NuGet Package Manager or Package Manager Console.



{{< figure align=center src="images/Aspose.Words-NuGet.jpg" alt=".NET API for Word Comparison">}}


*   Insert the following script in your **index.cshtml** file.

{{< gist aspose-com-gists a27eeff32f91830229096fff65c479d0 "index.cshtml" >}}

*   Insert the following code in your **HomeController.cs** class.

{{< gist aspose-com-gists a27eeff32f91830229096fff65c479d0 "HomeController.cs" >}}

*   Include the following JS and CSS files of drag and drop plugin within the head tag of **\_layout.cshtml** file.

{{< gist aspose-com-gists a27eeff32f91830229096fff65c479d0 "_layout.cshtml" >}}

*   Build the application and run it in your browser.



{{< figure align=center src="images/Merge-Word-DOCX-in-ASP.NET_.jpg" alt="ASP.NET Word Document Merger">}}


## ASP.NET Word Document Merger App - Demo

The following is the demonstration of merging MS Word documents using our ASP.NET Word Document Merger app.



{{< figure align=center src="images/giphy.gif" alt="Merge multiple DOCX files in ASP.NET">}}


## Download

Download the source code of ASP.NET Word Document Merger application from [here][5].

## Try Aspose.Words for .NET for Free

Get your [temporary license][6] (a complete license for 30 days) to try Aspose.Words for .NET for free.

## Related Article

*   [Compare Two Word Documents using C# in ASP.NET][7]




[1]: https://products.aspose.app/words/merger
[2]: https://products.aspose.com/words/net
[3]: http://nuget.org/packages/Aspose.Words
[4]: https://downloads.aspose.com/words/net
[5]: https://github.com/usman-aziz/ASP.NET-Word-Document-Merger
[6]: https://purchase.aspose.com/temporary-license
[7]: https://blog.aspose.com/2020/07/06/compare-two-word-documents-using-csharp-in-asp.net-core/






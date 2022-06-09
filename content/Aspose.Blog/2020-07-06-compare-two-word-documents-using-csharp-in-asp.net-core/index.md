---
title: 'Compare Two Word Documents using C# in ASP.NET'
seoTitle: ""
description: ""
date: Mon, 06 Jul 2020 01:46:00 +0000
draft: false
url: /2020/07/06/compare-two-word-documents-using-csharp-in-asp.net-core/
author: Usman Aziz
summary: ''
tags: ['Compare two word documents in asp.net', 'asp.net diff checker for word documents', 'compare two docx in asp.net']
categories: ['Aspose.Words Product Family']
---



{{< figure align=center src="images/Compare-Word-Document-in-ASP.NET_.jpg" alt="Compare Word Documents in ASP.NET">}}


We often need to compare two MS Word DOC/DOCX documents to check the similarities or differences. The comparison gives us an idea of what has been changed in the two versions of a single Word document. Various [online document comparison][1] applications are available that let you compare two Word documents. However, there could be the case when you need to integrate document comparison features within your web application. On the other hand, you may want to build your own online document comparison app. To deal with such cases, I'll show you how to compare two Word documents using C# within ASP.NET web application. This application will have the following features.

*   Compare two Word (DOC/DOCX) documents
*   Download the comparison result in DOCX format
*   Download the comparison result in PDF format

## .NET API to Compare Word Documents

To perform the comparison of the Word documents without MS Office, we'll use [Aspose.Words for .NET][2] which is a powerful word processing API for ASP.NET or other .NET/.NET Core applications. You can [download][3] API or install it within your ASP.NET application using [NuGet][4].

```
PM> Install-Package Aspose.Words
```

## Compare Two Word Documents in C# ASP.NET

*   Create a new **ASP.NET Core Web Application** in Visual Studio 2017 or later.



{{< figure align=center src="images/ASP.NET-Core-MVC-Web-Application.jpg" alt="Create ASP.NET Core Web Application">}}


*   Choose the **Web Application (Model-View-Controller)** template.



{{< figure align=center src="images/MVC-Project-Template.jpg" alt="Select MVC Application">}}


*   Install the **Aspose.Words for .NET** package using NuGet Package Manager.



{{< figure align=center src="images/Aspose.Words-NuGet.jpg" alt=".NET API for Word Comparison">}}


*   Copy and paste the following script in **index.cshtml** view.

{{< gist aspose-com-gists 7b72ec2db5e0192e560b45a8c650660b "index.cshtml" >}}

*   Copy and paste the following method in **HomeController.cs** controller.

{{< gist aspose-com-gists 7b72ec2db5e0192e560b45a8c650660b "HomeController.cs" >}}

*   Insert the following CSS and JS files of drag and drop plugin in the **head** tag of **\_layout.cshtml** view.

{{< gist aspose-com-gists 7b72ec2db5e0192e560b45a8c650660b "_layout.cshtml" >}}

*   Build the application and run in the browser.

## ASP.NET Word Document Comparison App - Demo

The following is the demonstration of how to compare two Word documents using our ASP.NET document comparison application.



{{< figure align=center src="images/giphy.gif" alt="Compare Word DOCX in ASP.NET">}}


## Download

You may download the complete source code of ASP.NET Word document comparison application from [here][5].

## About Aspose.Words for .NET

*   [Documentation][6]
*   [Source Code][7]

## Try Aspose.Words for .NET for Free

Aspose offers a [temporary license][8] to try Aspose APIs for free. Get yours to evaluate Aspose.Words for .NET.

## Related Article

*   [Create MS Word Editor in ASP.NET MVC][9]




[1]: https://products.aspose.app/words/comparison
[2]: https://products.aspose.com/words/net
[3]: https://downloads.aspose.com/words/net
[4]: http://nuget.org/packages/Aspose.Words
[5]: https://github.com/usman-aziz/ASP.NET-Word-Document-Comparison
[6]: https://docs.aspose.com/display/wordsnet
[7]: https://github.com/aspose-words/Aspose.Words-for-.NET
[8]: https://purchase.aspose.com/temporary-license
[9]: https://blog.aspose.com/2020/04/17/asp.net-mvc-word-editor-create-edit-word-documents/






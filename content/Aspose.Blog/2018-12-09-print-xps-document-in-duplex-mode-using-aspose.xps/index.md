---
title: 'Print XPS Document in Duplex Mode in C# or Java using Aspose.XPS'
date: Sun, 09 Dec 2018 23:58:15 +0000
draft: false
url: /2018/12/09/print-xps-document-in-duplex-mode-using-aspose.xps/
author: Asad Ali
summary: ''
tags: ['Asad Ali', 'Print XPS documents in duplex mode']
---



{{< figure align=center src="images/aspose_xps-for-net-128.png" alt="">}}


It is our honor to announce the new release of Aspose.XPS for both .NET and Java Platforms. As per the regular monthly revision process, new features and enhancements have been introduced in the API in order to enhance its usability. Some performance improvements have als3wrtyo been made in the latest release to make API perform efficiently. In case you are planning to upgrade to the latest version of the API, you can download it from the links given below as per your working environment e.g. .NET and Java:

*   [Aspose.XPS for .NET 18.11][1]
*   [Aspose.XPS for Java 18.11][2]

Release Notes for both .NET and Java APIs can be checked using the following links:

*   Release Notes of Aspose.XPS for .NET 18.11
*   Release Notes of Aspose.XPS for Java 18.11

The following section includes a worth-mentioning feature in the latest release of the API:

## Print XPS Document in Duplex Mode

With the latest version of Aspose.XPS, you can make your printer print an XPS document in duplex mode. Following .NET code snippet shows how you can specify **JobPrintTicket** property of **Document** object in order to achieve the functionality depending upon the page flip mode:

**\[.NET\]**

```
doc.JobPrintTicket = new JobPrintTicket(JobFeature.JobDuplexAllDocumentsContiguously.TwoSidedLongEdge);
```

OR

```
doc.JobPrintTicket = new JobPrintTicket(JobFeature.JobDuplexAllDocumentsContiguously.TwoSidedShortEdge);
```

## Aspose.XPS for .NET and Java Resources

The following resources will help you work with Aspose.XPS for .NET and Java APIs:

*   [Home page for Aspose.XPS API][3].
*   [Aspose.XPS API wiki docs][4]– Help documentation and API reference documents.
*   [Aspose.XPS product family forum][5]– Post your technical questions, queries and any other problem you faced while running Aspose.XPS APIs.
*   [Enable email subscription][6]– Do not limit yourself, stay up-to-date with the latest news about the Aspose.XPS APIs and new features, fixes, plus other API related topics by subscribing to Aspose.XPS Blog.
*   [Aspose.XPS for .NET Examples][7]– We have published our code examples on the social coding website GitHub.com. Anyone can explore the code examples for learning purposes.
*   [Aspose.XPS for Java Examples][8] – We have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.
*   Release Notes (.NET and Java) – For details on API fixes, please check Release Notes having a complete list of the new features.




[1]: https://www.nuget.org/packages/Aspose.XPS/18.11.0
[2]: https://repository.aspose.com/webapp/#/artifacts/browse/tree/General/repo/com/aspose/aspose-page
[3]: https://products.aspose.com/page
[4]: https://docs.aspose.com/
[5]: https://forum.aspose.com/c/xps
[6]: https://blog.aspose.com/category/aspose-products/aspose-xps-product-family/
[7]: https://github.com/aspose-page/Aspose.Page-for-.NET
[8]: https://github.com/aspose-page/Aspose.Page-for-Java




---
title: 'Preserving Print Tickets and Fixed Document Sequence Support in Aspose.XPS for .NET 18.8'
date: Sat, 22 Sep 2018 21:52:13 +0000
draft: false
url: /2018/09/22/preserving-print-tickets-and-fixed-document-sequence-support-in-aspose.xps-for-.net-18.8/
author: Asad Ali
summary: ''
tags: []
categories: ['Aspose.Total Product Family']
---



{{< figure align=center src="images/aspose_xps-for-net-128.png" alt="Aspose.XPS for .NET">}}


We are pleased to announce the August release of [Aspose.XPS for .NET 18.8][1] which is available on NuGet Gallery for download. As per the regular monthly update process, new features and enhancements have been incorporated in this release of the API. In case you are planning to use the latest version of the API, we recommend you to please go through the release notes page in API documentation to have an idea what has been introduced and changed in the API after its first public release. The release notes section has detailed information about public API Changes and Improvements in 18.8 version of the Aspose.XPS for .NET.

## Preserving Print Tickets

A print ticket is an XPS document component that contains the preferred printer settings for a page in a document, or for an entire document, or for a print job that contains one or more documents. In the latest version of the API, support to preserve print tickets while processing an XPS document has been implemented. As the Print Tickets feature is based upon long XPS specification, we are continuously working over implementing its full set in the API. We intend to provide creating new and modifying existing print tickets feature in future releases of Aspose.XPS for .NET.

## Fixed Document Sequence (FDS) Support

According to the XPS specification and the MS API, an XPS file contains a single FDS (Fixed Document Sequence). An FDS contains one or more FD (Fixed Document) where each FD contains one or more FP (Fixed Pages). In the latest release of the API, support of loading and removing a Fixed Document has been introduced. Following code snippet demonstrates the usage of the new feature with Aspose.XPS for .NET 18.8:

```
// Load a XPS with multiple FDs   
Aspose.Xps.XpsDocument doc = new Aspose.Xps.XpsDocument(dataDir + "combined.01.xps");   
// Load desired fixed document/page in XpsDocument initialized instance   
doc.SelectActiveDocument(2);   
// Remove desired FD   
doc.RemoveDocumentAt(3);  

```

## Aspose.XPS for .NET Resources

As it is always recommended to use latest releases of our API’s, so we suggest you please download the latest release [Aspose.XPS for .NET 18.8][2] and check following resources which will help you working with API:

*   [Home page for Aspose.XPS for .NET][3]
*   [Download Aspose.XPS for .NET 18.8][4]
*   [Aspose.XPS product family forum][5]– Post your technical questions and queries, or any other problem you faced while running Aspose.XPS APIs.
*   Aspose.XPS for .NET online documentation– help documentation and API reference documents.
*   [Enable Blog Subscription][6]– Do not limit yourself, you can keep yourself updated with the latest news on Aspose.XPS APIs, new features, fixes, and other API related topics by subscribing to Aspose.XPS blog.
*   [Aspose.XPS for .NET Examples][7] – We have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: http://nuget.org/packages/Aspose.XPS/18.8.0
[2]: https://www.nuget.org/packages/Aspose.XPS/18.8.0
[3]: https://products.aspose.com/page/net
[4]: https://www.nuget.org/packages/Aspose.XPS/18.8.0
[5]: https://forums.aspose.com/c/xps
[6]: https://blog.aspose.com/category/aspose-products/aspose-xps-product-family/
[7]: https://github.com/aspose-page/Aspose.Page-for-.NET





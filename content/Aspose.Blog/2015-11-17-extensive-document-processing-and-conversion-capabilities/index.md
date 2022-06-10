---
title: 'Tivity Accomplished Extensive document Processing and Conversion Capabilities without any third-party dependencies'
date: Tue, 17 Nov 2015 13:16:31 +0000
draft: false
url: /2015/11/17/extensive-document-processing-and-conversion-capabilities/
author: Vladimir Juric
summary: ''
tags: ['Aspose.Total', 'Create and Manipulate Office Apps without using MS Office Interop', 'MS Office files processing without using MS Office Automation', 'Manipulate Office files without installing MS Office Package', 'OpenOffice SDK alternative for MS Office files processing', 'OpenOffice files processing without using OpenOffice SDK', 'Success Stories']
categories: ['Aspose.Total Product Family']
---

## About TIVITY GmbH



{{< figure align=center src="images/TIVITY-Logo-Name-Slogan-300x156-1.png" alt="Tivity logo">}}


[Tivity][1] is a German SaaS Startup founded in 2015. Backed by a self-developed mobile enterprise application platform (MEAP) Tivity aims to improve enterprise mobility and productivity by a lean and customizable business suite. This set of business software functions enables and supports core business processes inside and beyond organizational boundaries with a focus on collaboration functionalities regardless of application.

## Product

The Document Application Server provides basic document operations (_Add, Delete, Check-In, Check-Out, Indexing, etc._) and saves metadata of a document. Indexing documents for full-text search, generation of thumbnails (_for image documents), conversion to PDF,_ and generation of Single-Page PDF Preview and physical storage of the document as per configuration.

Documents Application Server saves document meta information e.g. document information, version, check-in/check out/delete/restore/download access, and history to its own database base. The physical storage of documents is configurable as per storage provider (connectors) e.g. Microsoft SharePoint, Microsoft SQL Server, Cloud Storage Provider like Dropbox, OneDrive, Box, etc.

Indexing, Conversion, and Thumbnail services can be configured to run as stand-alone Windows Services or can be run as a part of DMS Server. Running these services independent reduces the waiting time during Check-in, Finalize, Create-New-Version, Delete, and Restore operations. All database requests(queries) to fetch the metadata are parameterized to avoid SQL Injection.



{{< figure align=center src="images/About-TIVITY-aspose-total-case-study-1024x700.png" alt="Tivity solution preview" caption="Image 1:- Tivity solution preview">}}


## Problem

Server-side document conversion based on Microsoft Office was not performant and very unstable. Unfortunately, Microsoft does not recommend and does not support the automation of Microsoft Office applications from any unattended, non-interactive client application or component (including ASP, ASP.NET, DCOM, and NT Services), because Office may exhibit unstable behavior and/or deadlock when Office is run in this environment.

Although certain coding practices can help reduce the likelihood of this issue, these practices cannot prevent the issue entirely. This fact alone makes running Office Applications from a server-side environment risky and unsupported.

Even though different solution providers offer document processing services based on 3rd party libraries such as Microsoft Office package, Microsoft Office Interop, OpenOffice SDK, etc. Tivity was searching for a provider with extensive processing and conversion capabilities without additional third-party dependencies and was highly impressed by the multitude of supported file formats by [Aspose.Total for .NET][2].

## Solution

The integration and deployment of [Aspose.Total for .NET][3] was very fast due to the fact that it is just a group of class libraries without any dependencies (_except on the .NET Framework itself_). Regardless of integration efforts, we’ve covered a significant performance improvement. The average PDF-A Conversion went from ~ 13-18 documents/minute (_while using MS Office Provider as conversion provider_) to ~ 40-50 documents/minute (_by using [Aspose][4] as conversion provider_).



{{< figure align=center src="images/About-TIVITY-aspose-total-case-study-1-1024x557.png" alt="Document client structure" caption="Image 2:- Document client structure">}}


## Summary and Next Steps

Tivity picked [Aspose.Total for .NET][5] after an intensive benchmarking of document processing providers. Stable and high-performance conversion services are right now on-demand, but the scope of [Aspose.Total for .NET][6] functionality is so great that our product development team was highly inspired by its incredibly versatile file processing capabilities of handling the most popular MS Office file formats. We were so inspired that upcoming products will focus on the creation and modification of these files.




[1]: https://www.tivity.one/en/
[2]: https://products.aspose.com/total/net
[3]: https://products.aspose.com/total/net
[4]: https://www.aspose.com/
[5]: https://products.aspose.com/total/net
[6]: https://products.aspose.com/total/net





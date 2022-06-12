---
title: 'Render IFC Files using C# .NET Core and Java'
seoTitle: "Render IFC Files using C# .NET Core and Java"
description: ""
date: Sun, 26 May 2019 17:17:34 +0000
draft: false
url: /2019/05/26/.net-core-and-ifc-rendering-support-available-in-aspose.cad-19.5/
author: Mudassir
summary: ''
tags: []
categories: ['Aspose.CAD Product Family']
---



{{< figure align=center src="images/aspose_cad-for-net-100x100.png" alt="">}}


Hi guys! I am back with an all-new blog to give you a walk through of the latest Aspose.CAD for .NET/Java 19.5. As a standard practice, the Aspose team publishes both .NET and Java-based API having the same features sets simultaneously. I will be giving you an overview of what new features have been included in API along with example code to use them.

One important feature included in Aspose.CAD for .NET 19.5 is support for .NET Core. With this support available, now API can work with the latest Visual Studio 2017 on onward environments that support .NET Core.

## Work with IFC Files in C# and Java

Files with IFC extension are referred to as Industry Foundation Classes (IFC) and establishes international standards to import and export building objects and their properties. This file format provides interoperability between different software applications. IFC can hold data for geometry, calculation, quantities, facility management, pricing, etc. for many different professions (architect, electrical, HVAC, structural, terrain, etc.).

Aspose.CAD allows developers to export an IFC file to PNG or other formats. In the following example, an IFC file is being processed and exported to PNG using IfcRasterizationOptions and PngOptions classes.

{{< gist aspose-com-gists 88cdd0899132edaf0afff77d33d11ae5 "Examples-CSharp-IFC-Drawings-ExportingIFCtoPNG-ExportingIFCtoPNG.cs" >}}

The equivalent Java implementation for this is as under.

{{< gist aspose-cad 9c5a3f5ddf329a1362916037ccd8c6e0 "Examples-src-main-java-com-aspose-cad-examples-IFCDrawings-ExportIFCToPNG-ExportIFCToPNG.java" >}}

## Export DWG to SVG in C# and Java {#mce_6}

DWG has been one of the widely used file formats by a range of applications and has a robust file structure. DWG is a binary file format, it is not human-readable like the plain ASCII DXF file format. DWG files usually include information about the image coordinates (both in 2D and 3D) and any associated metadata. It contains the vector image and metadata for the representation of the contents of CAD files.

Aspose.CAD allows loading AutoCAD drawings in DWG format and converting them to SVG. The following C# based example loads the DWG and export to SVG.

{{< gist aspose-com-gists 88cdd0899132edaf0afff77d33d11ae5 "Examples-CSharp-DWG-Drawings-ExportToSVG-ExportToSVG.cs" >}}

The equivalent Java implementation for this is as under:

{{< gist aspose-com-gists 49c1b75d9a84e149ecf374ece2c2597d "Examples-src-main-java-com-aspose-cad-examples-DWGDrawings-ExportToSVG-ExportToSVG.java" >}}

## Enabling Tracking for CAD Rendering Process {#ConvertingCADDrawingstoPDFandRasterImageFormats-EnablingTrackingforCADRenderingProcess}

Aspose.CAD has introduced a series of classes and supporting enumeration fields to assist with the tracking of CAD rendering process. With these changes in place, the CAD to PDF conversion can now be achieved as following while enabling the tracking.

{{< gist aspose-com-gists 88cdd0899132edaf0afff77d33d11ae5 "Examples-CSharp-DXF-Drawings-EnableTracking-EnableTracking.cs" >}}

The equivalent Java implementation for this is as under:

{{< gist aspose-com-gists 49c1b75d9a84e149ecf374ece2c2597d "Examples-src-main-java-com-aspose-cad-examples-DXFDrawings-EnableTracking-EnableTracking.java" >}}

You can check the official product release notes for many other issues and enhancements carried out in the product as well. [Here you can get the detail!][1]

When time allows you can check out API [examples at Github][2], talk about this release and other API related issues in our [forum][3].




[1]: https://docs.aspose.com/display/cadnet/Aspose.CAD+for+.NET+19.5+-+Release+Notes
[2]: https://github.com/aspose-cad
[3]: https://forum.aspose.com/c/cad





---
title: 'Customize Date Formatting of Visio Timeline using C# or VB.NET'
date: Fri, 23 Oct 2015 23:36:02 +0000
draft: false
url: /2015/10/23/custom-date-formatting-of-visio-timeline-and-unsigned-libraries-in-aspose.diagram-for-.net-5.6.0/
author: Imran Rafique
summary: ''
tags: ['Imran.Rafique']
categories: ['Aspose.Diagram Product Family']
---



{{< figure align=center src="images/aspose-Diagram-for-net_100.png" alt="Aspose.Diagram for .NET logo">}}


We're pleased to announce the new release version of [Aspose.Diagram for .NET][1] 5.7.0. While making a timeline in the Visio drawing, users were not able to customize date formatting. Now onward, they would be able to do so. In addition to that, we have included unsigned Aspose.Diagram libraries for each supported .NET Framework. Our primary goal is to provide quality, performance, and easy to implement the approach. To achieve that goal, we always welcome the feedback of our users and all the evidence they provide to test a failure use case. We focused on the cause of the fault and the generic way to get rid of the defect. This leading release version addresses formatting, misplaced elements and export quality fixes.

## Customize the Date on a Visio Timeline using C#

From this release version, we have managed to add support for customizing the date on a Visio Timeline. The TimelineHelper class allows doing so.

{{< gist aspose-diagram cce69e51f567ea17ef24bc35fef0f689 "Examples-CSharp-Working-Shapes-ConfigureTimeLineShapes-ConfigureTimeLine-ConfigureTimeLine.cs" >}}

Please refer to the following help topic: [Set Time Period and Date Format of Timeline Shape][2]

## Unsigned Aspose.Diagram Assemblies

From the release version 5.7.0 of Aspose.Diagram for .NET APIs, we now also provide assemblies without Authenticode signed. It is based on the users demand because the unsigned version of Aspose assembly increases its performance slightly, but we recommend using the signed version, it ensures the integrity of the assembly.

In the recent release version, we have improved its formatting quality, Visio drawing export quality and shape properties retrieval system. Please check a list of fixed defects:

*   Fixed: TimeLineHelper.TimeScale property is not working.
*   Fixed: the shape text goes outside the rectangle box.
*   Fixed: VDX to PNG conversion, incorrect fonts in the output PNG file.
*   Fixed: VSD to PDF conversion, the text items of various shapes are misplaced.
*   Fixed: Error in element Masters occurred while saving VSDX into VDX format.
*   Fixed: Can't detect connector ID of two connected shapes
*   Fixed: Invisible value property is not correct when retrieved from a VSS stencil file.
*   Fixed: Index out of range error occurred while loading diagram stream.
*   Fixed: ArgumentException error occurred while loading a VSDX diagram.
*   Fixed: VSD to PDF conversion, the text items are changed.
*   Fixed: VSD to PDF conversion, the output PDF is missing a process type shape.
*   Fixed: VSD to PDF conversion, the text items of Anmerkung shape are misplaced.
*   Fixed: VSDX to PDF/HTML conversion, missing shape's text item.

## Public API Changes

The following API changes in the new version are also worth noting:

*   The new DateFormatStringForBE and DateFormatStringForIntm properties have been added to the TimelineHelper class.

## Aspose.Diagram for .NET Resources

The following resources will help you work with Aspose.Diagram for .NET:

*   [Home page for Aspose.Diagram for .NET API][3].
*   [Download Aspose.Diagram for .NET][4]
*   [Aspose.Diagram for .NET wiki docs][5] - Help documentation and API reference documents.
*   [Aspose.Diagram product family forum][6] - Post your technical questions and queries, or any other problem you faced while running Aspose.Diagram APIs.
*   [Enable email subscription][7] - Don't limit yourself, stay up-to-date with the latest news about the Aspose.Diagram APIs and new features, fixes, plus other API related topics by subscribing to Aspose.Diagram blog.
*   [Aspose.Diagram for .NET Examples][8] – We have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.

We hope you’ll enjoy this new release that saves time and effort. The API is quite simple and developers can use it in application easily.




[1]: https://products.aspose.com/diagram/net
[2]: http://docs.aspose.com/display/diagramnet/Configure+Visio+TimeLine+Shapes#ConfigureVisioTimeLineShapes-SetTimePeriodandDateFormatofTimelineShape
[3]: https://products.aspose.com/diagram
[4]: https://downloads.aspose.com/diagram/net
[5]: http://docs.aspose.com/display/diagramnet/Home
[6]: http://forum.aspose.com
[7]: https://blog.aspose.com/
[8]: https://github.com/asposediagram/Aspose_diagram_NET





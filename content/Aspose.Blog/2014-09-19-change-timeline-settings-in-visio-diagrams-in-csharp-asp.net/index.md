---
title: 'Change Timeline and Milestone Shape Settings with Aspose.Diagram for .NET 4.4.0'
date: Fri, 19 Sep 2014 06:16:07 +0000
draft: false
url: /2014/09/19/change-timeline-settings-in-visio-diagrams-in-csharp-asp.net/
author: Imran Rafique
summary: ''
tags: ['Imran.Rafique']
categories: ['Aspose.Diagram Product Family']
---



{{< figure align=center src="images/aspose-Diagram-for-net_100.png" alt="Aspose.Diagram for .NET logo">}}


We are happy to announce that Aspose.Diagram for .NET 4.4.0 has been released and is available on NuGet. This new release adds features that let you change the settings of timeline and milestone shapes. The Configure Timeline and Configure Milestone dialogs can now be managed by these new features. Developers can also get the property of a specific shape by passing the property name parameter. Detailed release notes are listed below.

## Setting the Timeline Dialog Box

Timelines help you plan and communicate project schedules by showing project phases and deadlines in a format that’s easy to read and understand. In previous versions, developers could place timeline shapes on the Microsoft Visio drawing page. However, they could not manage the configuration timeline dialog values. You can find the details of this feature in the following help topic: [Set Time Period and Date Format of TimeLine Shape][1]

## Setting the Milestone Dialog Box

Using Microsoft Office Visio, users can quickly create clean, organized timelines that make it easy to order events and share information. Previously, the Aspose.Diagram API allowed developers to populate the timeline with milestones and intervals. There was no way to set the date, date format, type, and auto-update flag, however. These features are now supported. Features added across the API allow the milestones to update date, date format, type, and auto-update flag to create professional diagrams. Specifically, we made it easier: [Set Milestone Shape Properties][2]

## Read Shape's Property by Name

Developers can now retrieve a shape's properties using its name. The Shape.PropCollection.GetProp method searches all properties of the shape. Previously, it was difficult to find the exact property ID, and then get the property. With this latest release, we just need to pass the exact property name. Developers can use either the property ID or name: the PropCollection.GetProp method gives developers these options. You can find the details of this feature in the following help topic: Reading Visio Shape Data

## Public API Changes

The following API changes in the new version are also worth noting:

*   The PropCollection.GetProp(string name) method has been added. This method takes a property name as parameter to get shape property.
*   The new TimeLineHelper class has been added. It allows developers to modify the timeline shape dialog.
*   The new MilestoneHelper class has been added. It allows developers to modify milestone shape dialog.

## Other Bug Fixes

This new version brings fixes to reported bugs, error messages and include various other enhancements. Please see the complete list of bugs fixed in the new version.

*   Fixed: .NET Application gets stuck while adding a container shape on the diagram page.
*   Fixed: NullReferenceException message when saving VSDX/VSD to PDF/HTML formats.
*   Fixed: Error in the elements when loading VSD drawing.
*   Fixed: Shape's hyperlink is not visible in the output VDX format using Microsoft Visio 2013 Viewer.
*   Fixed: Shape's data is not visible using Microsoft Visio 2013 Viewer.
*   Fixed: VSD to PDF conversion, the portion of the source PDF file gets cut off.
*   Fixed: VSD to PDF conversion, all smiley faces and a few shape colors are changed.
*   Fixed: VSD to PDF conversion, shape's text items have blurred.
*   Fixed: VSD to PDF conversion, image shape has become dark from gray.
*   Fixed: VSD to PDF conversion, Microsoft Outlook icon is replaced by Microsoft Word icon.
*   Fixed: VSD to PDF conversion, map shapes and hyperlinks are missing.

To view a complete list of API features and try the API at your end, please visit the following page and [download the latest version of Aspose.Diagram for .NET][3]. If you need any help, please feel free to ask in the [Aspose.Diagram forum][4]. For more details, please visit the [Aspose.Diagram for .NET documentation][5].




[1]: https://docs.aspose.com/display/diagramnet/Configure+Visio+TimeLine+Shapes#ConfigureVisioTimeLineShapes-SetTimePeriodandDateFormatofTimelineShape
[2]: https://docs.aspose.com/display/diagramnet/Configure+Visio+TimeLine+Shapes#ConfigureVisioTimeLineShapes-SetMilestoneShapeProperties
[3]: https://downloads.aspose.com/diagram/net
[4]: https://forum.aspose.com/
[5]: https://docs.aspose.com/display/diagramnet/Home





---
title: 'Set Timeline and Milestone Dialog in Visio Drawings in Java'
date: Fri, 26 Sep 2014 14:08:25 +0000
draft: false
url: /2014/09/26/visio-drawing-export-and-settings-of-timeline-and-milestone-shapes-in-aspose.diagram-for-java-2.3.0/
author: Imran Rafique
summary: ''
tags: ['Imran.Rafique']
categories: ['Aspose.Diagram Product Family']
---



{{< figure align=center src="images/aspose_diagram-for-java-e1401178596961.png" alt="Aspose.Diagram for Java logo">}}


We have released version 2.3.0 of the [Aspose.Diagram for Java][1] API. As part of this release, the Microsoft Visio drawing load and export features have been improved by resolving reported bugs and adding feature requests. We have also ported the new features of the latest Aspose.Diagram for .NET version. These new features let developers change the settings of timeline and milestone shapes. The Configure Timeline and Milestone dialogs can be managed.

## Set Timeline and Milestone Dialog in Visio Drawings in Java

Aspose.Diagram for Java is fully ported from the Aspose.Diagram for .NET API. The porting process has added a few more features that are already available in the latest version of Aspose.Diagram for .NET. Below is a list of new features.

*   **Setting the Timeline dialog** - Timelines help you plan and communicate project schedules by showing project phases and deadlines in a format that’s easy to read and understand. In previous versions, developers could place timeline shapes on a Microsoft Visio drawing page. However, they could not manage the configuration timeline dialog values. You can find the details of this feature in the following help topic: [Set Time Period and Date Format of TimeLine Shape][2].
*   **Setting the Milestone dialog box** - Using Microsoft Visio, users can quickly create clean, organized timelines that make it easy to order events and share information. Previously, the Aspose.Diagram API allowed developers to populate the timeline with milestones and intervals. There was no way to set the date, date format, type and auto update flag, however. These features are now supported. Features added across the API allow the milestones to update date, date format, type and auto update flag to create professional diagrams. Specifically, we made it easier: [Set Milestone Shape Properties][3].
*   **Read shape properties by name** - Developers can now retrieve shape properties using their name. The Shape.PropCollection.GetProp method searches all properties of the shape. Previously, it was difficult to find the exact property ID, and then get the property. With this latest release, we just need to pass the exact property name. Developers can use either the property ID or name: the PropCollection.GetProp method gives developers these options. You can find the details of this feature in the following help topic: [Reading Visio Shape Data][4].

## Load and Export Visio Drawings

We have enhanced the load and export features of Visio drawings in the latest Aspose.Diagram API version 2.3.0. It's easy to deal with complex Visio drawings in beautiful layouts. We're improving based on current experience and upcoming complex scenarios. This release includes a number of key fixes that help us improve Visio loading and export features:

*   Fixed: An added hyperlink to a Visio shape was not visible in the Microsoft Visio Viewer 2013.
*   Fixed: An added shape's property was not visible in the Microsoft Visio Viewer 2013.
*   Fixed: The text and image items were jumbled up with each other when exporting a VSD drawing to PDF format.
*   Fixed: The shape's color was changed when exporting a Visio drawing to PDF format.
*   Fixed: The shape's text items were blurred or missing when exporting a Visio drawing to PDF format.
*   Fixed: The image shape was dark instead of gray when exporting a Visio drawing to PDF format.
*   Fixed: The central vertical line was missing when exporting a Visio drawing to PDF format.

## Public API Changes

The following API changes in the new version are also worth noting:

*   The PropCollection.getProp(string name) method has been added. This method takes a property name as parameter to get shape property.
*   The new TimeLineHelper class has been added. It allows developers to modify the timeline shape dialog.
*   The new MilestoneHelper class has been added. It allows developers to modify milestone shape dialog.

## Aspose.Diagram for Java Resources

The following resources will help you work with Aspose.Diagram for Java:

*   [Homepage for Aspose.Diagram for Java API][5]
*   [Download Aspose.Diagram for Java][6]
*   Aspose.Diagram for Java wiki docs - help documentation and API reference documents.
*   [Aspose.Diagram product family forum][7] - post your technical questions and queries, or any other problem you faced while running Aspose.Diagram APIs.
*   [Enable email subscription][8] - Don't limit yourself, you can keep yourself updated with the latest news about the Aspose.Diagram APIs and new features, fixes, plus other API related topics by subscribing to Aspose.Diagram blog.
*   [Aspose.Diagram for Java Examples][9] – We have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.

We hope you’ll enjoy this new release that save time and efforts. The API is quite simple and developers can use it in application easily.




[1]: https://products.aspose.com/diagram/java
[2]: https://docs.aspose.com/display/diagramjava/Configure+Visio+TimeLine+Shapes
[3]: https://docs.aspose.com/display/diagramjava/Working+with+Visio+Shape+Data
[4]: https://docs.aspose.com/display/diagramjava/Working+with+Visio+Shape+Data#WorkingwithVisioShapeData-ReadingVisioShapeData
[5]: https://products.aspose.com/diagram/java
[6]: https://downloads.aspose.com/diagram/java
[7]: http://forum.aspose.com
[8]: https://blog.aspose.com/
[9]: https://github.com/asposediagram/Aspose_Diagram_Java





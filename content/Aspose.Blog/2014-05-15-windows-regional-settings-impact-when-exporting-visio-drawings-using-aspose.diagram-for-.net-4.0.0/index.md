---
title: 'Windows Regional Settings Impact when Exporting Visio Drawings using Aspose.Diagram for .NET 4.0.0'
date: Thu, 15 May 2014 15:31:48 +0000
draft: false
url: /2014/05/15/windows-regional-settings-impact-when-exporting-visio-drawings-using-aspose.diagram-for-.net-4.0.0/
author: Imran Rafique
summary: ''
tags: ['Imran.Rafique']
categories: ['Aspose.Diagram Product Family']
---

[![Aspose.Diagram for .NET logo][1]](https://blog.aspose.com/wp-content/uploads/sites/2/2013/06/aspose-Diagram-for-net_100.png)We are pleased to announce the availability of Aspose.Diagram for .NET 4.0.0. Users can now upgrade to the latest release. This new release has covered three areas as accurate fetching of properties, the impact of changing Windows Regional Settings when exporting the Visio drawings and layout perfections.

## Fetching Shape and User-defined Cell Properties

In previous version, a few shapes and user-defined cell properties were not retrieved correctly. Based on a scenario, in a Visio drawing, there were three shapes having numerical values, along with three properties each. When we loaded this diagram and try to get the shape properties, it has 11 items on each shapes(x).props object, whereas there should be only 3. Similarly, when exported a few VSD files to VDX format, the Shapesheet shows improper Guid value of the User.UniqueID. We’ve fixed these issues in this latest release.

## Windows Regional Settings Effect

Microsoft Office uses the default input language in the Windows operating system to determine the default language for Office programs. Since a customer was doing so. He changed 'Regional Settings' in the Control Panel to "Dutch - Netherlands" and when exported his VSDX drawings to VDX format, he got an empty diagram. Now, there is no issue using this latest release.

## Other Fixes and Layout Perfections

This release also increases the layout perfections when rendering the diagram to various other formats. These layout perfections improve the shape’s shadow. Previously, all shapes having a light blue shadow in the source VSD drawing become a darker blue. It is when saved in VDX format. Another issue was about losing some transparency when saving Visio drawing in PDF format. One more about additional white space at the top of the drawing while convert Visio drawings to PNG and PDF formats.

To view a complete list of new features, fixes and enhancements [download the new release of Aspose.Diagram for .NET][2]




[1]: https://blog.aspose.com/wp-content/uploads/sites/2/2013/06/aspose-Diagram-for-net_100.png "Aspose.Diagram for .NET logo"
[2]: http://www.aspose.com/community/files/51/.net-components/aspose.diagram-for-.net/default.aspx





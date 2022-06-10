---
title: 'Glue Shapes Together with Connection Points .NET Visio API'
date: Tue, 27 May 2014 15:23:54 +0000
draft: false
url: /2014/05/27/glue-shapes-together-with-connection-points-using-aspose.diagram-for-.net-4.1.0/
author: Imran Rafique
summary: ''
tags: ['Imran.Rafique']
categories: ['Aspose.Diagram Product Family']
---



{{< figure align=center src="images/aspose-Diagram-for-net_100.png" alt="Aspose.Diagram for .NET logo">}}


We are pleased to offer the new version of [Aspose.Diagram for .NET][1] 4.1.0. This version allows developers to glue shapes together with connection points. A connection point is a special point on a shape that can be used to “glue” other shapes to it. When developers glue a shape to a connection point, the shapes stay connected, even if one of the shapes is moved. All users are encouraged to update to this latest version. You’ll see this feature in the following help topic: Glue Visio Shapes Together with Connection Point

## Additional White Space, Lost Hyperlinks and Empty Sub-shape Names

Prior to this release, we noticed a few queries relating to the additional white space problems around the actual drawing,  not able to preserve hyperlinks on shapes and retrieving empty strings instead of sub-shapes names. This release improves these areas. Please have a look at the improvements, as listed below:

*   Improved the rendering of PDF & HTML with hyperlinks.
*   Improved the rendering of PDF & PNG with no more additional white space around the actual Visio drawing.
*   Improved the rendering of sub-shape name property.

## Public API Changes

The following API changes in the new version are also worth noting:

*   The Page.GlueShapes method has been added.

It takes three parameters:

1.  long shapeFromId or Shape shapeFrom
2.  ConnectionPointPlace placeTo
3.  long shapeToId or Shape shapeTo

## Other Bug Fixes

This release also reduces the occurrence of exception messages. In this regard, we’ve fixed a few error messages as listed below:

*   Added more descriptive error messages for easier troubleshooting.
*   Fixed NullReferenceException message while calling Shape.SetWidth, Shape.SetAngle and Shape.AddShape methods.
*   Fixed DiagramException message while loading VDX drawing.

To view a complete list of API features and try the API at your end, please visit the following page and [download the latest version of Aspose.Diagram for .NET][2]. If you need any help, please feel free to ask in the [Aspose.Diagram forum][3]. For more details, please visit the Aspose.Diagram for .NET documentation.




[1]: https://products.aspose.com/diagram/net
[2]: https://downloads.aspose.com/diagram/net
[3]: http://forum.aspose.com





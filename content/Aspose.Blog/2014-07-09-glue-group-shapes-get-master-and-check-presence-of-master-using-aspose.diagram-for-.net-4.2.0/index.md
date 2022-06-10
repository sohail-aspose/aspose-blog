---
title: 'Glue Group Shapes, Get Master and Check Presence of Master using Aspose.Diagram for .NET 4.2.0'
date: Wed, 09 Jul 2014 09:14:39 +0000
draft: false
url: /2014/07/09/glue-group-shapes-get-master-and-check-presence-of-master-using-aspose.diagram-for-.net-4.2.0/
author: Imran Rafique
summary: ''
tags: ['Imran.Rafique']
categories: ['Aspose.Diagram Product Family']
---

[![Aspose.Diagram for .NET logo][1]](https://blog.aspose.com/wp-content/uploads/sites/2/2013/06/aspose-Diagram-for-net_100.png)We are pleased to offer the new version of Aspose.Diagram for .NET 4.2.0. This API has a great track record of excellent performance and has gained a solid community. Based on this new build, developers can now glue group shapes inside a container. Also, this release allows them to get and check for the presence of a master by name. This release includes all changes and fixes we’ve made.

## Get Master from the Visio Drawing by Name

Developers can now retrieve a master object using its name. The MasterCollection.GetMasterByName method searches all masters in the masters collection's containing master. Previously, it was difficult to find the exact master ID, and then get the master. The new release of the Aspose.Diagram API has now made it very easy: just pass the exact master name.  Developers can use either the master ID or name: the MasterCollection.GetMaster and MasterCollection.GetMasterByName methods give developers that option. You can find the details of this feature in the following help topic: Get Master from a Visio Drawing by Name.

## Glue Group Shapes Inside a Container

In the previous version, we announced support for gluing shapes together by connection points. It works perfectly with ungroup shapes. However, there are many points in group shapes where it was not supported quite so well. We have now added group shape support. Developers can dynamically glue group shapes inside the container group shape. You can find details of this feature in the following help topic: Glue Group Shape Inside a Container

## Check Presence of Master in the Visio Drawing by Its Name

Every Microsoft Visio document contains a masters collection, which refers to the various "master shapes" that are used by it. Developers can now check the presence of a master object by its name using the MasterCollection.IsExist method. It checks that the title master exists and, if it does, returns true, otherwise false. Developers can use either the master ID or name: the MasterCollection.IsExist method supports both options. You can find details of this feature in the following help topic: Check Presence of a Master in a Visio Drawing

## Public API Changes

The following API changes in the new version are also worth noting:

*   The MasterCollection.GetMasterByName method has been added. It takes a master name as parameter and returns a master object.
    
*   The MasterCollection.IsExist method has been added. It takes a master ID or name as parameter and returns true in case the master is present.
    
*   The Page.GlueShapesInContainer method has been added. It's used to glue shapes in the container.
    

## Other Bug Fixes

This new version brings fixes to reported bugs, error messages and include various other enhancements. Please see the complete list of bugs fixed in the new version.

*   Fixed: Shapes were missing when exporting a VSDX drawing to PNG or PDF format.
    
*   Fixed: A shape's text was rotated when exporting a VSDX drawing to PNG format.
    
*   Fixed: Shape properties were not readable from a VSDX drawing.
    
*   Fixed: A shape's fill color was black instead of white when exporting a VSDX drawing to PDF or image formats.
    
*   Fixed: The arrow thickness was ignored when converting a VSD drawing to PDF format.
    
*   Fixed: Additional white space around the drawing when exporting sample VSD/VSDX drawings to PNG format.
    
*   Fixed: DiagramException message while loading VSDX drawing.
    

To view a complete list of API features and try the API at your end, please visit the following page and [download the latest version of Aspose.Diagram for .NET][2]. If you need any help, please feel free to ask in the [Aspose.Diagram forum][3]. For more details, please visit the Aspose.Diagram for .NET documentation.




[1]: https://blog.aspose.com/wp-content/uploads/sites/2/2013/06/aspose-Diagram-for-net_100.png "Aspose.Diagram for .NET logo"
[2]: http://www.aspose.com/community/files/51/.net-components/aspose.diagram-for-.net/default.aspx
[3]: http://www.aspose.com/community/forums/aspose.diagram-product-family/489/showforum.aspx





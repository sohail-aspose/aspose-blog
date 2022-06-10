---
title: 'Import Bitmap Image as a Visio Shape using C# with Aspose.Diagram for .NET 4.3.0'
date: Wed, 13 Aug 2014 20:22:50 +0000
draft: false
url: /2014/08/13/import-bitmap-image-as-a-visio-shape-and-other-enhancement-using-aspose.diagram-for-.net-4.3.0/
author: Imran Rafique
summary: ''
tags: ['Imran.Rafique']
categories: ['Aspose.Diagram Product Family']
---



{{< figure align=center src="images/aspose-Diagram-for-net_100.png" alt="Aspose.Diagram for .NET logo">}}


Today, we took another step forward and released the next version of Aspose.Diagram for .NET 4.3.0. Under the hood, the Aspose.Diagram API now supports importing a bitmap image as a Microsoft Visio shape. This is something our users have asked for in our forums. We have also improved various other manipulation features along with performance. Overview of help topic: [Import Bitmap Image as a Visio Shape][1]

## Glue Shapes in Container using Connection Names

There are many ways to glue shapes in the container, we've covered the basics of handling glue. Developers can now glue shapes in the container by passing connection name parameters. Previously, it was only possible by connection IDs. The new release of the Aspose.Diagram API has now made it very easy: just pass the exact connection name.  Developers can use either the connection IDs or name by using either the Page.GlueShapesInContainer or Page.GlueShapesInContainerByID methods.

You can find the details of this feature in the following help topic: [Glue Shapes Inside the Container][2]

## Add Master to Diagram from Source Diagram

This feature is useful primarily if we have added the new shapes and saved them to a source Microsoft Visio diagram. It helps developers to add a master to diagram from source diagram.  We have added a new overloaded Diagram.AddShape method. It takes a master name and a Diagram class object (the object that represents a Visio drawing). Please find details of this feature in the following help topic: [Add Master from the Stencil of Shapes][3]

## Public API Changes

The following API changes in the new version are also worth noting:

*   The Page.GlueShapesInContainer and Page.GlueShapesInContainerByID methods have been added. These methods take connection IDs or Name/NameU as parameters to glue shapes in the container.
*   The overloaded Diagram.AddMaster method has been added. It takes a master name and the source diagram object as parameters.
*   The Page.AddShape method has been added. It's used to import a bitmap image as a Visio shape.

## Other Bug Fixes

This new version brings fixes to reported bugs, error messages and include various other enhancements. Please see the complete list of bugs fixed in the new version.

*   Fixed: The bullet characters were not available in the text of shapes when converted VSD drawing to other supported formats.
*   Fixed: Connection arrows were enlarged in size. We have restored to their original size while exporting to any other supported formats.
*   Fixed: The rounded rectangle shape was folded in the output PDF document.
*   Fixed: The text items were outside the shape's boundary. It was the case with VSD to PDF conversion.
*   Fixed: The solid style border of shapes was changed to the dash style.
*   Fixed: There were improper spaces between the text lines.
*   Fixed: We noticed that a few Microsoft Visio samples with missing shapes, for example during VSD to PDF conversion.
*   Fixed: The text items and images were jumbled up with each other, for example during VSD to PDF conversion.
*   Fixed: Incorrect shape's fill color and changed case text of the shape problems are now fixed.

To view a complete list of API features and try the API at your end, please visit the following page and [download the latest version of Aspose.Diagram for .NET][4]. If you need any help, please feel free to ask in the [Aspose.Diagram forum][5]. For more details, please visit the [Aspose.Diagram for .NET documentation][6].




[1]: https://docs.aspose.com/display/diagramnet/Working+with+Images#WorkingwithImages-ImportBitmapImageasaVisioShape
[2]: https://docs.aspose.com/display/diagramnet/Working+with+Shapes+Gluing#WorkingwithShapesGluing-GlueShapesInsidetheContainer
[3]: https://docs.aspose.com/display/diagramnet/Working+with+Masters#WorkingwithMasters-AddMasterfromtheStencilofShapes
[4]: https://downloads.aspose.com/diagram/net
[5]: http://forum.aspose.com
[6]: http://docs.aspose.com/display/diagramnet/Home





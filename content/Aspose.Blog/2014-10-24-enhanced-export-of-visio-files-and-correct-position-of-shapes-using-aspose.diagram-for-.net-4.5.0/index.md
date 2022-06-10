---
title: 'Enhanced Export of Visio Files and Correct Position of Shapes using Aspose.Diagram for .NET 4.5.0'
date: Fri, 24 Oct 2014 22:14:14 +0000
draft: false
url: /2014/10/24/enhanced-export-of-visio-files-and-correct-position-of-shapes-using-aspose.diagram-for-.net-4.5.0/
author: Imran Rafique
summary: ''
tags: ['Imran.Rafique']
categories: ['Aspose.Diagram Product Family']
---

[![Aspose.Diagram for .NET logo][1]](https://blog.aspose.com/wp-content/uploads/sites/2/2013/06/aspose-Diagram-for-net_100.png)We have released the new version of Aspose.Diagram for .NET 4.5.0. Our releases are typically based on customer feedback about the operational features of the API. This release brings a number of fixes and enhancements that also improve performance of the API. A connection point on a shape can be used to connect with other shapes. After the manipulation of a Visio shapes, we were not able to move sub shapes along with connection points. It is now fixed. Similarly, there is a list of other defects, those we have fixed in this release.

## Plotting Visio Drawings within the Actual Scale

The problem was that a few customers reported Visio file samples which they exported to PDF or thumbnail formats. The API was bringing whitespace under or besides the actual figure. In this release, we have fixed most of these type of issues.

## Removal of Additional Shapes

During the export of Visio files to PDF or HTML formats, the Aspose.Diagram API was placing a few additional shapes like moustache, half circle and half circle with black color fill. It was the case with few sample Visio drawings. There was no presence of these shapes in the source Visio drawings.

## Error Message Fixes

This new version brings fixes to reported error messages and include various other enhancements. Please see the complete list of fixed error messages in the new version.

*   Fixed: Error in elements when loading VSD drawing
    
*   Fixed: ArgumenetException when saving to the JPG format after SetWidth method call
    
*   Fixed: Input string format error when converting VDX drawing in PDF format
    
*   Fixed: Error in element VisioDocument when loading a VSD diagram
    

This release also increases the layout perfections when rendering the Visio diagram to various other supported formats. These perfections were fruitful in calculating the accurate height / width of the page or shape of the Visio drawings. There have been a few numbers of defects  already reported. Please see other resolved problems below:

*   Fixed: Action cell is not properly preview able in the MS Office Visio 2013
    
*   Fixed: The shape's properties are not being added properly
    
*   Fixed: VSD to PDF conversion, incorrect page number sequence
    
*   Fixed: The shape is cut off when saving to the VDX format
    

To view a complete list of API features and try the API at your end, please visit the following page and [download the latest version of Aspose.Diagram for .NET][2]. If you need any help, please feel free to ask in the [Aspose.Diagram forum][3]. For more details, please visit the Aspose.Diagram for .NET documentation.



[1]: https://blog.aspose.com/wp-content/uploads/sites/2/2013/06/aspose-Diagram-for-net_100.png "Aspose.Diagram for .NET logo"
[2]: http://www.aspose.com/community/files/51/.net-components/aspose.diagram-for-.net/default.aspx
[3]: http://www.aspose.com/community/forums/aspose.diagram-product-family/489/showforum.aspx





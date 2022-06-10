---
title: 'Improved Licensing for OMR Template Editor with Aspose.OCR for .NET 2.5.0'
date: Fri, 08 May 2015 13:34:01 +0000
draft: false
url: /2015/05/08/improved-licensing-for-omr-template-editor-with-aspose.ocr-for-.net-2.5.0/
author: Babar Raza
summary: ''
tags: ['Babar Raza']
categories: ['Aspose.OCR Product Family']
---



{{< figure align=center src="images/aspose-OCR-for-net_100.png" alt="Aspose.OCR for .NET logo">}}


We're pleased to announce the release of Aspose.OCR for .NET 2.5.0. The biggest attraction of this month's release is the improved licensing mechanism for OMR Template Editor tool, shipped with Aspose.OCR for .NET API to create, manipulate & scan OMR templates against OMR sheets. Please review the release notes of [Aspose.OCR for .NET 2.5.0][1] for a complete list of enhancements & fixes included in this release. If you are planning to upgrade the API from any previous revision, we strongly suggest you to check the Public API Changes section first.

## What Is OMR Template Editor?

Those of you who are not familiar with OMR Template Editor or haven't used it so far, here is a little overview.

The OMR Template Editor is a simple graphical tool, available with Aspose.OCR for .NET API in an executable format (.exe). There could be several usage scenarios however, the main purpose of the tool is to create & save OMR templates that in turn can be used to [dynamically identify optical markers][2] from a batch of scanned sheets. Whereas, the template itself is a simple XML file (.amr) in which the elements are defined in the form of XML nodes along with their dimensions, size, name and other properties. The OMR Template Editor allows creating the aforesaid XML through its UI without even having the knowledge of the XML structure.

In order to create the OMR templates, one must be familiar with [different OMR elements][3] and their usage. The OMR Template Editor currently supports a variety of elements to suit most of the optical marker recognition requirements and provides the drag-n-drop functionality to place the elements on required location. Moreover, the OMR Template Editor allows manipulating the element properties such as follow.

*   Name – the element's name.
*   Values Count – the number of values associated with the element.
*   Values Orientation – the direction of the element's value lines.
*   Items Number – the number of value lines in the element (grid only).
*   Multiple Selection – indicates whether multiple values can be marked within the element (choice box only).
*   Horizontal Offset – the element's offset from the left edge of the page, in millimeters.
*   Vertical Offset – the element's offset from the top edge of the page, in millimeters.
*   Width – the element's width, in millimeters.
*   Height – the element's height, in millimeters.
*   Values Spacing – the spacing between individual areas of marks inside the element, in millimeters.

The OMR Template Editor can also be used to [extract the data][4] from the scanned images against a particular template. In this mode, the users can test the template elements for correct data extraction and may tweak the element location, size, orientation, and other aspects to get 100% accurate results. To do so, the OMR Template Editor requires to load the image of the scanned OMR sheet also refereed to as Template Image in Aspose.OCR for .NET documentation.

## OMR Template Editor Licensing

By default, the OMR Template Editor works in evaluation mode and restricts the recognition to not more than 3 elements per page and not more than 10 pages in total. If the limit is exceeded, the recognized value gets replaced with an error message similar to "Trial mode. Recognition is not performed for more than 3 elements.". In order to work in licensed mode, the OMR Template Editor allows to [set a valid license through its Settings interface][5]. The settings dialog can be triggered by clicking the **Edit** menu and then **Settings**.



{{< figure align=center src="images/Setting-GeneralTab.jpg" alt="Create OMR Template">}}


The above snapshot shows the General tab of the Settings dialog, where the license can be set using the **Change License** button. Once clicked, it will prompt to specify the location to the license file, and after validation, the status will be changed to **Licensed**. Moreover, the OMR Template Editor can also accept valid Aspose.OCR for Java & Aspose.Total for Java licenses. In order to set the Java licenses, one has to first change the mode to Java by clicking the **Switch to Aspose.OCR for Java** button, whereas the rest of the process to apply the license is the same as of setting a .NET license with one change, that is: the OMR Template Editor also requires the location of Aspose.OCR.jar file to validate the license as shown in the following illustration.



{{< figure align=center src="images/OmrTemplateEditor-Java-Licensing.jpg" alt="OMR in Images">}}


As always we appreciate your feedback so if you ever have anything to tell us about this release or anything else, please head to the [Aspose.OCR forum][6] for a chat.




[1]: https://downloads.aspose.com/ocr/net
[2]: https://docs.aspose.com/display/omrnet/Perform+OMR+on+Images
[3]: https://docs.aspose.com/omr/net/developer-guide/
[4]: https://docs.aspose.com/display/ocrnet/Performing+OCR+on+an+Image#PerformingOCRonanImage-ExtractTextfromImage
[5]: https://docs.aspose.com/display/ocrnet/Licensing
[6]: http://www.aspose.com/community/forums/aspose.ocr-product-family/493/showforum.aspx





---
title: 'Add New Layouts, Improved SmartArt and Scaled Image for Picture Frame Available in Aspose.Slides for .NET 14.4.0'
date: Mon, 02 Jun 2014 12:48:38 +0000
draft: false
url: /2014/06/02/support-to-add-new-layouts-improved-smartart-and-scaled-image-for-picture-frame-available-in-aspose.slides-for-.net-14.4.0/
author: Mudassir
summary: ''
tags: []
categories: ['Aspose.Total Product Family', 'Aspose.Slides Product Family']
---

[![][1]](https://blog.aspose.com/wp-content/uploads/sites/2/2013/08/aspose-Slides-for-net_100.png)We like to share the release announcement of Aspose.Slides for .NET 14.4.0. This is a major product releases where we have included some new features and have also stabilized many existing ones.

## New Features

We have introduced support for adding, inserting and removing layout slides inside a presentation. In earlier releases, when cloning slides from a source to a target presentation, an exception was thrown if the layout of the source presentation slide that is cloned was not available in the layout slides collection of the target presentation master. Now, if the target presentation master does not have the intended source slide layout in its collection, the missing layout is added to its collection automatically.

We have also resumed support for setting relative image height and width for picture frames in this release. Please visit the documentation article Setting relative image width and height of image for further information.

We have made some noticeable improvement in SmartArt shapes support as well. Now, it is possible to access to SmartArt node bullet images. Also, significant improvement has been made towards SmartArt rendering while exporting to PDF and slide thumbnails.

## Resolved Issues

The presentation rendering support has been enhanced to a great extent. The issue of small caps getting converted to lower case in generated slide thumbnails has been addressed in this release alongside other text rendering issues. In this release, we have resolved issues pertaining to accessing and saving presentations that resulted in different exceptions in earlier product versions. We have also rectified issues related to corrupted PDF files getting generated using Aspose.Slides.

Setting SmartArt nodes and child nodes position had some issues in earlier releases and we have also addressed this area. Also the exception issue while accessing the SmartArt node text frame has been rectified.

Issues pertaining to slide cloning have also been addressed which previously resulted in loss of animation effects when slides got cloned from one presentation to another. Also, the issue related to an exception thrown when the target slide master does not have a layout slide of the source slide that is being cloned has also been resolved in this release.

The chart rendering has also been improved and we have resolved the chart rendering issues including wrong number format getting rendered for the value axis and improper chart outline inside chart for exported PDF.

We have made some enhancements to the new API. Please visit the documentation article Public API and Backwards Incompatible Changes in Aspose.Slides for .NET 14.4.0 for further reference.

To see a complete list of fixes and to download Aspose.Slides for .NET 14.4.0, [please visit the download page][2].




[1]: https://blog.aspose.com/wp-content/uploads/sites/2/2013/08/aspose-Slides-for-net_100.png "Aspose.Slides or .NET logo"
[2]: http://www.aspose.com/community/files/51/.net-components/aspose.slides-for-.net/default.aspx





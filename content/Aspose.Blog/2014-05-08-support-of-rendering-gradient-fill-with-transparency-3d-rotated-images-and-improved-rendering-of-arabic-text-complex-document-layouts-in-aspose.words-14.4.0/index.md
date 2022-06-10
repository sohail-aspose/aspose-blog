---
title: 'Support of Rendering Gradient Fill with Transparency, 3D Rotated Images and Improved Rendering of Arabic Text, Complex Document Layouts in Aspose.Words 14.4.0'
date: Thu, 08 May 2014 08:19:50 +0000
draft: false
url: /2014/05/08/support-of-rendering-gradient-fill-with-transparency-3d-rotated-images-and-improved-rendering-of-arabic-text-complex-document-layouts-in-aspose.words-14.4.0/
author: Awais Hafeez
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---

[![Aspose.Words generic logo][1]](https://blog.aspose.com/wp-content/uploads/sites/2/2014/01/aspose.words_logo.png)Aspose.Words 14.4.0 has been released with this month’s release containing over 83 useful new features, enhancements and bug fixes to the Aspose.Words products.

You can download the latest releases of Aspose.Words from the following links:

*   [Aspose.Words for .NET 14.4.0][2]
*   [Aspose.Words for Java 14.4.0][3]

Here is a look at just a few of the biggest features and API changes in this month’s release. For a full list of bug fixes and improvements please refer to the download pages in the links above.

*   Improvements to rendering of Arabic texts
*   Improvements to rendering of complex document layouts
*   Improved handling of themes, list styles and building blocks when joining documents
*   Added support of text frames in ODT import/export
*   Improvements in TXT import capabilities
*   Gradient fill with transparency rendering in PDF implemented
*   3D rotated DrawingML shapes (and images) rendering implemented
*   Better support of tab stops and underlines in HTML import/export

## Simple Mail Merge now Ignores MailMergeCleanupOptions.RemoveUnusedRegions Option

Previously, when there was no mail merge region defined in template document and simple mail merge was performed using an empty data source after specifying MailMergeCleanupOptions.RemoveUnusedRegions, Aspose.Words used to produce an empty output document. This was because simple mail merge is technically a particular case of mail merge with regions where the whole document acts as a single region. Now starting with this release, **simple mail merge is no more affected by the MailMergeCleanupOptions.RemoveUnusedRegions option** since it is meaningless to produce empty documents.

## PixelFormat Kept with Non Default Image Settings

Previously, when ImageSaveOptions.ImageColorMode or ImageSaveOptions.ImageBrightness were set to non default values, the output image had always 32BppArgb pixel format. Now, ImageSaveOptions.PixelFormat is taken into account and the output image tries to keep that format. However, pixel format of the output image may be changed by GDI+ while saving. For example, the 8bpp is indexed pixel format, and GDI+ has some limitations when working with such format. In this case, when you want to save to 8bpp GrayScale image, unfortunately because of GDI+ limitations it is not possible.




[1]: https://blog.aspose.com/wp-content/uploads/sites/2/2014/01/aspose.words_logo.png "Aspose.Words generic logo"
[2]: http://www.aspose.com/community/files/51/.net-components/aspose.words-for-.net/category1188.aspx
[3]: http://www.aspose.com/community/files/72/java-components/aspose.words-for-java/category1378.aspx





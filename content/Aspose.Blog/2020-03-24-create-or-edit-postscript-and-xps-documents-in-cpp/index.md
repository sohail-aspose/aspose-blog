---
title: 'Create or Edit XPS Documents Programmatically in C++'
seoTitle: "Create or Edit XPS Documents in C++ | C++ XPS API | XPS Library"
description: "C++ XPS API. Create and edit XPS documents in C++. Convert XPS, PS, and EPS documents programmatically. Native C++ Library for XPS and PostScript documents."
date: Tue, 24 Mar 2020 16:28:40 +0000
draft: false
url: /2020/03/24/create-or-edit-postscript-and-xps-documents-in-cpp/
author: Usman Aziz
summary: ''
tags: ['Create XPS Document in CPP', 'Edit XPS Document in CPP', 'XPS Document API']
categories: ['Aspose.Page Product Family']
---



{{< figure align=center src="images/aspose_page-for-cpp.png" alt="Create PS EPS XPS Documents in C++">}}


[Aspose.Page for C++][1] is a valuable addition to [Aspose.Page Product Family][2] which is developed for manipulation of PostScript (PS/EPS) and XPS documents using C++. _Aspose.Page for C++_ is a native C++ library for creating new XPS files as well as modifying and converting the existing PostScript and XPS documents programmatically. The API also lets you work with the pages and elements such as canvases and glyphs in the XPS documents. Furthermore, it supports converting the documents to PDF and raster images. This article demonstrates how to perform the following operations related to XPS documents using _Aspose.Page for C++_.

*   Create a new XPS document in C++
*   Edit an existing XPS document in C++
*   Add a page or document to an XPS document in C++

## Installation of XPS API for C++

_Aspose.Page for C++_ is hosted on the [NuGet][3] as well as available as downloadable [binaries][4]. The downloadable package also contains a C++ console application containing the source code of basic examples.

## Create an XPS Document in C++

The following are the simple steps to create an XPS document containing text and image using _Aspose.Page for C++_.

*   Create an object of the [XpsDocument][5] class.
*   Add text and image using [XpsGlyphs][6] and [XpsPath][7] objects respectively.
*   Save the document using the [Save][8] method.

The following code sample shows how to create an XPS document in C++.

{{< gist aspose-com-gists 623196ea203d6b1080fe5db9a172996d "create-xps-document.cpp" >}}

### Output



{{< figure align=center src="images/Create-XPS-in-CPP.png" alt="Edit PS EPS XPS Document C++">}}


## Edit an XPS Document in C++

The following are the steps to edit an existing XPS document:

*   Create an object of the [XpsDocument][9] class and initialize it with the XPS document's path.
*   Access the document's elements using the _XpsDocument_ object.
*   Save the updated document using the [Save][10] method.

The following code sample shows how to edit an existing XPS document in C++.

{{< gist aspose-com-gists 623196ea203d6b1080fe5db9a172996d "edit-xps-document.cpp" >}}

## Add Page and Document to XPS in C++

_Aspose.Page for C++_ also lets you add pages as well as multiple documents in an XPS document. The following are the steps to create a new XPS document and add an additional page and document.

*   Create an object of the [XpsDocument][11] class.
*   Use [AddPage][12] and [AddDocument][13] methods to add page and document respectively.
*   Use the [SelectActiveDocument][14] method to select the active document for processing.
*   Add text or image to the document.
*   Save the document.

The following code sample shows how to add additional pages and documents to XPS using C++.

{{< gist aspose-com-gists 623196ea203d6b1080fe5db9a172996d "add-page-document-to-xps.cpp" >}}

## Learn more about Aspose.Page for C++

You can learn more about _Aspose.Page for C++_ using the [documentation][15] and the [source code examples][16] available on GitHub.




[1]: https://products.aspose.com/page/cpp
[2]: https://products.aspose.com/page
[3]: https://www.nuget.org/packages/Aspose.Page.Cpp/
[4]: https://downloads.aspose.com/page/cpp
[5]: https://apireference.aspose.com/cpp/page/class/aspose.page.x_p_s.xps_document/
[6]: https://apireference.aspose.com/cpp/page/class/aspose.page.x_p_s.xps_model.xps_glyphs/
[7]: https://apireference.aspose.com/cpp/page/class/aspose.page.x_p_s.xps_model.xps_path/
[8]: https://apireference.aspose.com/cpp/page/class/aspose.page.x_p_s.xps_document/#a253a0130918537f5e0b97e1ba1d20d0c
[9]: https://apireference.aspose.com/cpp/page/class/aspose.page.x_p_s.xps_document/
[10]: https://apireference.aspose.com/cpp/page/class/aspose.page.x_p_s.xps_document/#a253a0130918537f5e0b97e1ba1d20d0c
[11]: https://apireference.aspose.com/cpp/page/class/aspose.page.x_p_s.xps_document/
[12]: https://apireference.aspose.com/cpp/page/class/aspose.page.x_p_s.xps_document/#a68c739360eee70c0b260f7d1cc0c18c1
[13]: https://apireference.aspose.com/cpp/page/class/aspose.page.x_p_s.xps_document/#a11b50261beea487744a2d716ac99dcab
[14]: https://apireference.aspose.com/cpp/page/class/aspose.page.x_p_s.xps_document/#a7188c8df85e8c12195d56adf3281aebe
[15]: https://docs.aspose.com/display/pagecpp/Getting+Started
[16]: https://github.com/aspose-page/Aspose.Page-for-C






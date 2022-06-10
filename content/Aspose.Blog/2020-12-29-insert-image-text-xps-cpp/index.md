---
title: 'Insert Text or Image in XPS File Programmatically using C++'
seoTitle: "Insert Text or Image in XPS File Programmatically using C++"
description: "You can insert image or text in XPS files programmatiaclly using C++. Add or update a picture, graphic in tiled form or text as unicode string."
date: Tue, 29 Dec 2020 12:42:00 +0000
draft: false
url: /2020/12/29/insert-image-text-xps-cpp/
author: Farhan Raza
summary: 'You can create, edit, or manipulate [XPS][1] files easily. Moreover, you can control the contents and their position as per your requirements. You can **insert an image or text in XPS** files programmatically using C++ language.'
tags: ['add image or text in xps with cpp', 'insert image in xps', 'insert text in xps', 'watermark in xps']
categories: ['Aspose.Page Product Family']
---



{{< figure align=center src="images/Add-Image-Text-XPS.png" alt="Insert Text Image XPS C++">}}


You can create, edit, or manipulate [XPS][2] files easily. Moreover, you can control the contents and their position as per your requirements. You can insert an image or text in XPS files programmatically using C++ language. Let us explore this feature in detail under the following topics:

*   [Work with Text or Image Contents in XPS Files - API Installation][3]
*   [Add Text in XPS File using C++][4]
*   [Add Text in XPS File using Unicode String in C++][5]
*   [Insert Image in XPS Document using C++][6]
*   [Insert Tiled Image in XPS File using C++][7]

## Work with Text or Image Contents in XPS Files - API Installation {#section0}

You can add text or image contents into XPS files in C++ applications. You do not need to consider minor details about the file format of the document as few API calls can do the job as per your requirements. [**Aspose.Page for C++**][8] API can be configured easily either by downloading it from [New Releases][9] or with the below [NuGet][10] installation command:

```
PM> Install-Package Aspose.Page.Cpp
```

## Add Text in XPS File using C++ {#section1}

Text can be used in XPS file to label some drawing, image or other contents. Likewise, you can also use the text as watermark for the file. You need to follow the steps below to add or insert text in XPS files:

1.  Create a new [XPS Document][11]
2.  Create a brush to add text
3.  Add glyph to the document
4.  Save output XPS document

The code below shows how to add text in XPS file using C++:

{{< gist aspose-com-gists 5bdabe13c8a4cd202b41d266a9508831 "AddText.cpp" >}}

## Add Text in XPS File using Unicode String in C++ {#section2}

We have learned adding simple text string to an XPS file. Let us proceed and consider a scenario where you need to add Unicode string in the XPS files. You need to follow the below steps for adding text in XPS file, based on Unicode string:

1.  Create new XPS Document
2.  Add Unicode Text
3.  Save output XPS document

The following code is based on these steps, which shows how to add text in XPS file using Unicode string in C++ language:

{{< gist aspose-com-gists 5bdabe13c8a4cd202b41d266a9508831 "AddText_unicode.cpp" >}}

## Insert Image in XPS Document using C++ {#section3}

Images can contain a lot of visual information so the API supports inserting an image in XPS file in your C++ applications. Aspose.Page for C++ API lets you insert pictures or images in XPS files with below steps:

1.  Create a new XPS Document
2.  Load input Image
3.  Create a Matrix and [ImageBrush][12]
4.  Save output XPS file

The code example below shows how to insert image in XPS document with C++:

{{< gist aspose-com-gists 5bdabe13c8a4cd202b41d266a9508831 "AddImage.cpp" >}}

## Insert Tiled Image in XPS File using C++ {#section4}

We have learned the first step of adding or inserting image in an XPS file, let us proceed with related example of inserting tiled image in XPS document. Below are the steps for adding tiled image in XPS file:

1.  Create new XPS Document
2.  Add [ImageBrush][13] filled rectangle
3.  Add tiled image
4.  Save resultant XPS document

The following code snippet demonstrates how to add tiled image in XPS file using C++:

{{< gist aspose-com-gists 5bdabe13c8a4cd202b41d266a9508831 "AddTiledImage.cpp" >}}

## Conclusion

In this article, you have learned how to insert or add some text, or image in XPS files using C++ language. This feature can be helpful in scenarios like when you need to add a watermark in XPS documents, or adding some stamp as per your requirements. Likewise, a lot of other exciting features are supported for the XPS file format. You can learn more by visiting the [API Documentation][14], or you can also discuss with us at [Free Support Forum][15]. We look forward to getting in touch with you!

## See Also

[Convert XPS, OXPS to JPG or PNG Image using C# VB.NET][16]




[1]: https://docs.fileformat.com/page-description-language/xps/
[2]: https://docs.fileformat.com/page-description-language/xps/
[3]: #section0
[4]: #section1
[5]: #section2
[6]: #section3
[7]: #section4
[8]: https://products.aspose.com/page/cpp
[9]: https://downloads.aspose.com/page/cpp
[10]: https://www.nuget.org/packages/Aspose.Page.Cpp/
[11]: https://apireference.aspose.com/page/cpp/class/aspose.page.x_p_s.xps_document/
[12]: https://apireference.aspose.com/page/cpp/class/aspose.page.x_p_s.xps_model.xps_image_brush
[13]: https://apireference.aspose.com/page/cpp/class/aspose.page.x_p_s.xps_model.xps_image_brush
[14]: https://docs.aspose.com/display/pagecpp/Getting+Started
[15]: https://forum.aspose.com/c/page
[16]: https://blog.aspose.com/2020/11/02/convert-xps-to-jpg-png-image-csharp-vb-net/






---
title: 'Create, Edit, Read and Convert SVG Files using C# - Aspose.SVG for .NET'
seoTitle: ""
description: ""
date: Thu, 13 Feb 2020 16:32:20 +0000
draft: false
url: /2020/02/13/create-edit-read-and-convert-svg-files-using-c-aspose.svg-for-.net/
author: Usman Aziz
summary: ''
tags: ['.NET SVG API', 'C# SVG library', 'Create SVG files in .NET', 'Create SVG files in csharp', 'SVG API for .NET Core']
categories: ['Aspose.SVG Product Family']
---



{{< figure align=center src="images/Aspose_SVG-for-net-1.png" alt="C# SVG API, Create edit convert SVG files">}}


Its time to announce the addition of the C# SVG library to our product line - [Aspose.SVG for .NET][1]. It is a .NET class library that lets you **create, edit, read and convert SVG files programmatically** using **C#** in **.NET** or **.NET Core** based applications. Let's have a quick walk through the installation methods and salient features of the API.

## C# .NET SVG API - Installation

_Aspose.SVG for .NET_ DLL can be downloaded from our [Downloads][2] section. On the other hand, you can install it via _NuGet Package Manager_ or the _Package Manager Console_ in Visual Studio.

### NuGet Package Manager



{{< figure align=center src="images/Aspose.SVG-NPM.png" alt="C# .NET SVG library">}}


### Package Manager Console```
PM> Install-Package Aspose.SVG
```

Let's now have a glance at some salient features of the API to deal with SVG files.

## Create an SVG File using C#

_Aspose.SVG for .NET_ lets you create an empty file having an SVG structure. Furthermore, you can also create an SVG file from a user-defined string. The API provides [SVGDocument][3] class to create SVG files and you can further use this object to fill the document with SVG elements. Once done, you can save the file using [SVGDocument.Save()][4] method. The following code samples show how to create an SVG file from scratch.

#### Create Empty SVG File in C#

{{< gist aspose-com-gists 0420a5530f73658aebea7f98ea4d705f "Examples-CSharp-LoadSaveConvert-CreateEmptySVGDocument-CreateEmptySVGDocument.cs" >}}

#### Create SVG with User Defined String in C#

{{< gist aspose-com-gists 0420a5530f73658aebea7f98ea4d705f "Examples-CSharp-LoadSaveConvert-CreateSVGDocumentFromContent-CreateSVGDocumentFromContent.cs" >}}

## Edit SVG Files in C#

_Aspose.SVG for .NET_ also allows you to edit the SVG files to update their content. The API's Data Object Model efficiently maps the official specifications of SVG to access and edit SVG nodes and their elements. The following code sample shows how to edit an SVG file in C#.

{{< gist aspose-com-gists 0420a5530f73658aebea7f98ea4d705f "Examples-CSharp-WorkingWithSVGDocument-EditSVGFile-EditSVGFile.cs" >}}

## Read SVG Files in C#

In case you would want to read an existing SVG file, you can load it using the [SVGDocument][5] class. Simply create a new object and initialize it with SVG file's path as shown in the following code sample.

{{< gist aspose-com-gists 0420a5530f73658aebea7f98ea4d705f "Examples-CSharp-LoadSaveConvert-LoadSVGDocumentFromFile-LoadDocumentFromFile.cs" >}}

## Convert SVG Files to PSD, XPS or Raster Images

You can also convert the SVG files to various other file formats. The supported conversions include:

*   SVG to PDF
*   SVG to XPS
*   SVG to Image (JPEG, PNG, BMP, GIF, TIFF)

The following code sample shows how to convert an SVG file to PDF in C#.

{{< gist aspose-com-gists 0420a5530f73658aebea7f98ea4d705f "Examples-CSharp-LoadSaveConvert-ConvertSVGToPDF-ConvertSVGToPDF.cs" >}}

For code samples of SVG to XPS and SVG to image, please visit [Converting SVG Files in C#][6].

## Learn more about .NET SVG API

You can evaluate the API's features by downloading the [examples project][7]. For more details, consult the [documentation][8] of the API. In case you would have any questions or queries, feel free to let us know via our [forum][9].

## See Also

*   [Convert DICOM to JPEG, GIF, PNG, and BMP Images in C#][10]




[1]: https://products.aspose.com/svg/net
[2]: https://downloads.aspose.com/svg
[3]: https://apireference.aspose.com/net/svg/aspose.svg/svgdocument
[4]: https://apireference.aspose.com/net/svg/aspose.svg.svgdocument/save/methods/3
[5]: https://apireference.aspose.com/net/svg/aspose.svg/svgdocument
[6]: https://docs.aspose.com/svg/net/how-to-work-with-aspose-svg-api/converting/
[7]: https://github.com/aspose-svg/Aspose.SVG-for-.NET
[8]: https://docs.aspose.com/svg/net/getting-started/
[9]: https://forum.aspose.com/
[10]: https://blog.aspose.com/2020/04/01/convert-dicom-to-jpeg-gif-png-bmp-images-in-csharp-net/






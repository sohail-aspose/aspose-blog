---
title: 'Load, Save or Merge SVG Images Programmatically in C#'
seoTitle: "Load, Save or Merge SVG Images to PDF XPS Programmatically in C#"
description: "You can load save or merge SVG files to PDF XPS JPG GIFF TIFF and other file formats. You can export programmatically using C# language in .NET."
date: Wed, 10 Feb 2021 21:32:29 +0000
draft: false
url: /2021/02/10/load-save-merge-svg-pdf-xps-csharp/
author: Farhan Raza
summary: 'SVG (Scalable Vector Graphics) is a vector image format for two-dimensional graphics. These images are based on XML format that enables you to traverse different nodes to edit or search the file contents easily. You can load, save or merge SVG image files programmatically in C#. Likewise, several other features related to SVG images allow your .NET based applications to process several supported file formats.'
tags: ['Merge SVG files', 'Merge SVG files C#', 'Merge SVG to PDF', 'Merge SVG to PNG', 'Merge SVG to XPS', 'load SVG file', 'save SVG file']
categories: ['Aspose.SVG Product Family']
---



{{< figure align=center src="images/load-save-merge-svg.png" alt="Load Save Merge SVG C#">}}


[SVG][1] (Scalable Vector Graphics) is a vector image format for two-dimensional graphics. These images are based on XML format that enables you to traverse different nodes to edit or search the file contents easily. You can load, save or merge SVG image files programmatically in C#. Likewise, several other features related to SVG images allow your .NET based applications to process several supported file formats. Let us explore the following sections for further information:

*   [Install C# .NET SVG API][2]
*   [Load SVG file Programmatically using C#][3]
*   [Save SVG file Programmatically in C#][4]
*   [Merge SVG images Programmatically with C#][5]

## Install C# .NET SVG API {#section1}

[Aspose.SVG for .NET][6] API supports creating, editing, or converting SVG files. You can download the DLL file as ZIP from [Official Downloads][7], and add it to the resources of your project. Moreover, you can also configure it via NuGet Package Manager in Microsoft Visual Studio. It will install the API from [NuGet gallery][8] along with other dependencies, if any. Below is the NuGet installation command:

```
PM> Install-Package Aspose.SVG
```

## Load SVG file Programmatically using C# {#section2}

While initiating work with existing SVG images, the first step we need to do is to load the input file. You can load an SVG file programmatically from a file as well as from the web. Below steps show how to load an SVG file:

1.  Specify the file path to input SVG
2.  OR specify the URL to load the SVG image
3.  Load an SVG document from a file or URL

The following code snippet shows how to load SVG file programmatically using C#:

{{< gist aspose-com-gists d58bf88bb1bca6af7affe9383e3a015b "load-SVG.cs" >}}

However, it is important to note here that the API can throw DOMException if the resource is not found at specified URL.

## Save SVG file Programmatically in C# {#section3}

We have already learned how to load SVG file. Likewise, you can save an SVG file to a file or URL. The following steps explain how to save SVG files in your .NET based applications:

1.  Set a full (complete) path for SVG document saving
2.  Save SVG to a file
3.  Or Save SVG to Url

The [Save(Url)][9] overloaded method Saves the document to a local file specified by Url. The following code snippet shows how to save SVG file using C#:

{{< gist aspose-com-gists d58bf88bb1bca6af7affe9383e3a015b "save-SVG.cs" >}}

## Merge SVG images Programmatically with C# {#section4}

You can merge different SVG files to PDF, XPS, JPG, TIFF, and other file formats. You need to follow the following steps to merge different SVG images:

1.  Load multiple SVG input files
2.  Initialize an instance of [SvgRenderer][10]
3.  Merge all SVG files to the required output format

The code below is an example of how to merge SVG files programmatically using C#:

{{< gist aspose-com-gists d58bf88bb1bca6af7affe9383e3a015b "merge-SVG-PDF.cs" >}}

## Conclusion

In this article, we have explored how to load and save SVG files to a file or URL as per your requirements. Moreover, we have explored how to merge different SVG files to PDF, XPS, PNG, JPG, etc. However, the example and code snippet we have considered here is related to merging the SVG files to a PDF document. You can explore the API further by checking out the [Example Project][11] as well as the [Product Documentation][12]. In case of any query, you can always reach out to us at [Free Support Forums][13]. We look forward to getting in touch with you!

## See Also

[Create, Edit, Read and Convert SVG Files using C#][14]




[1]: https://docs.fileformat.com/page-description-language/svg/
[2]: #section1
[3]: #section2
[4]: #section3
[5]: #section4
[6]: https://products.aspose.com/svg/net
[7]: https://releases.aspose.com/
[8]: https://www.nuget.org/packages/Aspose.SVG/
[9]: https://apireference.aspose.com/svg/net/aspose.svg.svgdocument/save/methods/3
[10]: https://apireference.aspose.com/svg/net/aspose.svg.rendering/svgrenderer
[11]: https://github.com/aspose-svg/Aspose.SVG-for-.NET
[12]: https://docs.aspose.com/svg/net/
[13]: https://forum.aspose.com/c/svg
[14]: https://blog.aspose.com/2020/02/13/create-edit-read-and-convert-svg-files-using-c-aspose.svg-for-.net/






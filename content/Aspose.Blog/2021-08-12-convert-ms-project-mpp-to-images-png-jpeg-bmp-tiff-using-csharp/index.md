---
title: 'Convert MS Project MPP to Images (PNG, JPEG, BMP, TIFF) using C#'
seoTitle: "Convert MS Project MPP to Images (PNG, JPEG, BMP, TIFF) using C#"
description: "Convert Microsoft Project MPP files to JPEG, PNG, BMP, and TIFF image formats using the robust and simple to use Aspose.Tasks for .NET API."
date: Thu, 12 Aug 2021 10:58:42 +0000
draft: false
url: /2021/08/12/convert-ms-project-mpp-to-images-png-jpeg-bmp-tiff-using-csharp/
author: Muhammad Ahmad
summary: 'Microsoft Project ([MPP][1] files are used to track, organize and manage projects. These files contain tasks, assignments, and other project-related resources and information. If you want to share project information with someone and they do not have MS Project installed, you can convert the MPP file to images like [PNG][2], [JPEG][3], [BMP][4], and [TIFF][5] and share those. To that end, this article will teach you **how to convert Microsoft Project MPP files to images programmatically using C#**.'
tags: ['Convert MPP to BMP using C#', 'Convert MPP to Images using C#', 'Convert MPP to JPEG using C#', 'Convert MPP to PNG using C#', 'Convert MPP to TIFF using C#']
categories: ['Aspose.Tasks Product Family']
---



{{< figure align=center src="images/MPP-to-Image.jpg" alt="Convert MS Project MPP to Images (PNG, JPEG, BMP, TIFF) using C#">}}


Microsoft Project ([MPP][6] files are used to track, organize and manage projects. These files contain tasks, assignments, and other project-related resources and information. If you want to share project information with someone and they do not have MS Project installed, you can convert the MPP file to images like [PNG][7], [JPEG][8], [BMP][9], and [TIFF][10] and share those. To that end, this article will teach you **how to convert Microsoft Project MPP files to images programmatically using C#**.

*   [C# API for Converting MPP Files to Images][11]
*   [Convert MPP Files to JPEG Format using C#][12]
*   [Converting MPP Files to PNG Images using C#][13]
*   [Convert MPP Files to BMP Images using C#][14]
*   [Convert MPP Files to Multipage TIFF using C#][15]

## C# API for Converting MPP Files to Images {#CSharp-API-for-Converting-MPP-Files-to-Images}

[Aspose.Tasks for .NET][16] is a .NET library that allows you to read and write MPP/XML files without requiring Microsoft Project to be installed. Furthermore, the API supports converting MPP files to images. You can either install the API through [NuGet][17] or download it directly from the [Downloads][18] section.

```
PM> Install-Package Aspose.Tasks
```

## Convert MPP Files to JPEG Format using C# {#Convert-MPP-Files-to-JPEG-Format-using-CSharp}

The following are the steps to convert MPP files to JPEG format using C#.

*   Load the MPP file using the [Project][19] class.
*   Create an instance of the [ImageSaveOptions][20] class using the [SaveFileFormat.JPEG][21] enumeration.
*   Specify the quality of the JPEG image using the [JpegQuality][22] property of the [ImageSaveOptions][23] class.
*   Save the JPEG image using the [Project.Save(string filename, SaveOptions options)][24] method.

The following sample code shows how to convert an MPP file to JPEG images using C#.

{{< gist aspose-com-gists 05bd9878e2618d39e0633beccc2eb507 "Convert_MPP_To_JPEG.cs" >}}

## Converting MPP Files to PNG Images using C# {#Converting-MPP-Files-to-PNG-Images-using-CSharp}

In order to convert an MPP file to PNG images, follow the steps given below.

*   Load the MPP file using the [Project][25] class.
*   Create an instance of the [ImageSaveOptions][26] class using the [SaveFileFormat.PNG][27] enumeration.
*   Save the PNG image using the [Project.Save(string filename, SaveOptions options)][28] method.

The following sample code shows how to convert an MPP file to PNG images using C#.

{{< gist aspose-com-gists 05bd9878e2618d39e0633beccc2eb507 "Convert_MPP_To_PNG.cs" >}}

## Convert MPP Files to BMP Images using C# {#Convert-MPP-Files-to-BMP-Images-using-CSharp}

The following are the steps to convert an MPP file to BMP images using C#.

*   Load the MPP file using the [Project][29] class.
*   Create an instance of the [ImageSaveOptions][30] class using the [SaveFileFormat.BMP][31] enumeration.
*   Save the BMP image using the [Project.Save(string filename, SaveOptions options)][32] method.

The following sample code shows how to convert an MPP file to BMP images using C#.

{{< gist aspose-com-gists 05bd9878e2618d39e0633beccc2eb507 "Convert_MPP_To_BMP.cs" >}}

## Convert MPP Files to Multipage TIFF using C# {#Convert-MPP-Files-to-Multipage-TIFF-using-CSharp}

The following are the steps to convert an MPP file to a multipage TIFF using C#.

*   Load the MPP file using the [Project][33] class.
*   Create an instance of the [ImageSaveOptions][34] class using the [SaveFileFormat.TIFF][35] enumeration.
*   Save the TIFF image using the [Project.Save(string filename, SaveOptions options)][36] method.

The following sample code shows how to convert an MPP file to a multipage TIFF image using C#

{{< gist aspose-com-gists 05bd9878e2618d39e0633beccc2eb507 "Convert_MPP_To_Multipage_TIFF.cs" >}}

## Get a Free License

In order to try the API without evaluation limitations, you can request [a free temporary license][37].

## Conclusion

In this article, you have learned how to convert Microsoft Project MPP files to image format using C#. Specifically, you have learned how to convert MPP files to JPEG, PNG, BMP, and TIFF image formats using Aspose.Tasks for .NET API. The API provides a bunch of additional features for working with MPP files that you can explore in detail by visiting the [official documentation][38]. In case of any questions, please feel free to reach us at our [free support forum][39].

## See Also

*   [Convert MPP to Excel XLSX or CSV Programmatically in C#][40]
*   [Convert MPP File to PDF Programmatically using C# .NET][41]




[1]: https://docs.fileformat.com/project-management/mpp/)
[2]: https://docs.fileformat.com/image/png/
[3]: https://docs.fileformat.com/image/jpeg/
[4]: https://docs.fileformat.com/image/bmp/
[5]: https://docs.fileformat.com/image/tiff/
[6]: https://docs.fileformat.com/project-management/mpp/)
[7]: https://docs.fileformat.com/image/png/
[8]: https://docs.fileformat.com/image/jpeg/
[9]: https://docs.fileformat.com/image/bmp/
[10]: https://docs.fileformat.com/image/tiff/
[11]: #CSharp-API-for-Converting-MPP-Files-to-Images
[12]: #Convert-MPP-Files-to-JPEG-Format-using-CSharp
[13]: #Converting-MPP-Files-to-PNG-Images-using-CSharp
[14]: #Convert-MPP-Files-to-BMP-Images-using-CSharp
[15]: #Convert-MPP-Files-to-Multipage-TIFF-using-CSharp
[16]: https://products.aspose.com/tasks/net/
[17]: https://www.nuget.org/packages/Aspose.Tasks
[18]: https://downloads.aspose.com/tasks/net
[19]: https://apireference.aspose.com/tasks/net/aspose.tasks/project
[20]: https://apireference.aspose.com/tasks/net/aspose.tasks.saving/imagesaveoptions
[21]: https://apireference.aspose.com/tasks/net/aspose.tasks.saving/savefileformat
[22]: https://apireference.aspose.com/tasks/net/aspose.tasks.saving/imagesaveoptions/properties/jpegquality
[23]: https://apireference.aspose.com/tasks/net/aspose.tasks.saving/imagesaveoptions
[24]: https://apireference.aspose.com/tasks/net/aspose.tasks.project/save/methods/6
[25]: https://apireference.aspose.com/tasks/net/aspose.tasks/project
[26]: https://apireference.aspose.com/tasks/net/aspose.tasks.saving/imagesaveoptions
[27]: https://apireference.aspose.com/tasks/net/aspose.tasks.saving/savefileformat
[28]: https://apireference.aspose.com/tasks/net/aspose.tasks.project/save/methods/6
[29]: https://apireference.aspose.com/tasks/net/aspose.tasks/project
[30]: https://apireference.aspose.com/tasks/net/aspose.tasks.saving/imagesaveoptions
[31]: https://apireference.aspose.com/tasks/net/aspose.tasks.saving/savefileformat
[32]: https://apireference.aspose.com/tasks/net/aspose.tasks.project/save/methods/6
[33]: https://apireference.aspose.com/tasks/net/aspose.tasks/project
[34]: https://apireference.aspose.com/tasks/net/aspose.tasks.saving/imagesaveoptions
[35]: https://apireference.aspose.com/tasks/net/aspose.tasks.saving/savefileformat
[36]: https://apireference.aspose.com/tasks/net/aspose.tasks.project/save/methods/6
[37]: https://purchase.aspose.com/temporary-license
[38]: https://docs.aspose.com/tasks/net/
[39]: https://forum.aspose.com/c/tasks/15
[40]: https://blog.aspose.com/2021/07/23/convert-mpp-to-excel-xlsx-csv-csharp/
[41]: https://blog.aspose.com/2021/05/24/convert-mpp-file-to-pdf-programmatically-using-csharp-net/






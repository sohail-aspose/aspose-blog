---
title: 'Convert MS Visio Diagrams to PDF using C#'
seoTitle: "Convert Visio VSD(X) to PDF using C# | C# Visio to PDF Converter"
description: "Use .NET Visio diagram manipulation API to convert Visio VSD and VSDX to PDF using C#. Convert diagrams to PDF with high fidelity within .NET applications."
date: Fri, 22 Jan 2021 07:00:38 +0000
draft: false
url: /2021/01/22/convert-visio-diagrams-to-pdf-csharp/
author: Usman Aziz
summary: '[MS Visio][1] is a widely used application for creating a multitude of diagrams such as flowcharts, business flow diagrams, etc. However, in various cases, you may need to convert the diagram files to other file formats. For example, when sharing the diagrams you can convert them to a PDF file. On the other hand, you can convert a diagram to an image for embedding it into your web or desktop application. In this article, we will target Visio diagram to PDF conversion programmatically. Particularly, you will learn **how to convert VSDX or VSD files to PDF using C#**.'
tags: ['csharp-visio-to-pdf', 'csharp-vsd-to-pdf', 'csharp-vsdx-to-pdf']
categories: ['Aspose.Diagram Product Family']
---



{{< figure align=center src="images/Visio-to-PDF-1024x361.jpg" alt="">}}


[MS Visio][2] is a widely used application for creating a multitude of diagrams such as flowcharts, business flow diagrams, etc. However, in various cases, you may need to convert the diagram files to other file formats. For example, when sharing the diagrams you can convert them to a PDF file. On the other hand, you can convert a diagram to an image for embedding it into your web or desktop application. In this article, we will target Visio diagram to PDF conversion programmatically. Particularly, you will learn **how to convert VSDX or VSD files to PDF using C#**.

*   [C# Visio to PDF Converter API][3]
*   [Steps to Convert Visio to PDF][4]
*   [C# Visio to PDF - Complete Code][5]
*   [Get Free License][6]

## C# Visio to PDF Converter API {#CSharp-Visio-to-PDF-Converter-API}

[Aspose.Diagram for .NET][7] is a C# class library that is designed to create and manipulate MS Visio diagrams from within the .NET applications. Furthermore, it provides a high fidelity converter API that allows you to convert Visio diagrams to PDF and other formats. You can either [download][8] the API's DLL or install it using [NuGet][9].

```
Install-Package Aspose.Diagram
```

## Steps to Convert Visio to PDF in C# {#Steps-to-Convert-Visio-to-PDF-in-CSharp}

The following are the steps to convert a Visio diagram to PDF using Aspose.Diagram for .NET.

*   Load Visio VSD or VDSX file using [Diagram][10] class.

{{< gist aspose-com-gists f7837f256dbaeec060de473b43d80bd1 "load-visio-file.cs" >}}

*   Create a [MemoryStream][11] object.
*   Convert Visio file to PDF and save it into [MemoryStream][12] object using [Diagram.Save(MemoryStream, SaveFileFormat.PDF)][13] method.

{{< gist aspose-com-gists f7837f256dbaeec060de473b43d80bd1 "create-memory-stream.cs" >}}

*   Create a new [FileStream][14] object for the converted PDF file.
*   Save the converted PDF using [MemoryStream.WriteTo(FileStream)][15] method.

{{< gist aspose-com-gists f7837f256dbaeec060de473b43d80bd1 "save-pdf.cs" >}}

*   Close the [MemoryStream][16] and [FileStream][17].

{{< gist aspose-com-gists f7837f256dbaeec060de473b43d80bd1 "close-streams.cs" >}}

## C# Visio to PDF - Complete Code {#CSharp-Visio-to-PDF-Complete-Code}

The following is the complete source code of how to convert a Visio file to PDF using C#.

{{< gist aspose-com-gists f7837f256dbaeec060de473b43d80bd1 "convert-visio-to-pdf.cs" >}}

## Results

The following are the screenshots of the results you would obtain using the above-mentioned code.

### Visio Diagram



{{< figure align=center src="images/Visio-Diagram-JPEG.jpg" alt="Visio to PDF C#">}}


### Converted PDF



{{< figure align=center src="images/Visio-to-PDF.jpg" alt="Visio to PDF">}}


## Get a Free License {#Get-Free-License}

You can [get a free temporary license][18] in order to try the API without evaluation limitations.

## Conclusion

Aspose.Diagram for .NET provides a wide range of features for the manipulation of Visio diagrams. In addition, it provides high-quality conversion of diagrams to PDF format. In this article, you have learned how to convert the VDS or VSDX diagrams to PDF format using C#. You can explore more about the API using the [documentation][19].

## See Also

*   [Create MS Visio Diagrams using C#][20]




[1]: https://en.wikipedia.org/wiki/Microsoft_Visio
[2]: https://en.wikipedia.org/wiki/Microsoft_Visio
[3]: #CSharp-Visio-to-PDF-Converter-API
[4]: #Steps-to-Convert-Visio-to-PDF-in-CSharp
[5]: #CSharp-Visio-to-PDF-Complete-Code
[6]: #Get-Free-License
[7]: https://products.aspose.com/diagram/net
[8]: https://downloads.aspose.com/diagram/net
[9]: https://www.nuget.org/packages/Aspose.Diagram
[10]: https://apireference.aspose.com/diagram/net/aspose.diagram/diagram
[11]: https://docs.microsoft.com/en-us/dotnet/api/system.io.memorystream
[12]: https://docs.microsoft.com/en-us/dotnet/api/system.io.memorystream
[13]: https://apireference.aspose.com/diagram/net/aspose.diagram/diagram/methods/save
[14]: https://docs.microsoft.com/en-us/dotnet/api/system.io.filestream?view=net-5.0
[15]: https://docs.microsoft.com/en-us/dotnet/api/system.io.memorystream.writeto?view=net-5.0#System_IO_MemoryStream_WriteTo_System_IO_Stream_
[16]: https://docs.microsoft.com/en-us/dotnet/api/system.io.memorystream
[17]: https://docs.microsoft.com/en-us/dotnet/api/system.io.filestream?view=net-5.0
[18]: https://purchase.aspose.com/temporary-license
[19]: https://docs.aspose.com/diagram/net/developer-guide/
[20]: https://blog.aspose.com/2020/12/01/create-ms-visio-vsdx-diagrams-using-csharp/






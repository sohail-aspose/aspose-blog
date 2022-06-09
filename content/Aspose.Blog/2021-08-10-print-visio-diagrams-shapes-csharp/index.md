---
title: 'Print Visio Diagram Documents VSDX, DWGX, VSTX Programmatically in C#'
seoTitle: "Print Visio Diagram Documents VSDX, DWGX, VSTX in C#"
description: "You can print Microsoft Visio Diagram files programmatically using C#. Export Visio shapes or documents to a default or specific printer using XpsPrinter."
date: Tue, 10 Aug 2021 20:15:00 +0000
draft: false
url: /2021/08/10/print-visio-diagrams-shapes-csharp/
author: Farhan Raza
summary: 'You can print Diagram documents like VSDX, DWG, VDW, VSTX programmatically using C#. Aspose.Diagram for .NET API can be integrated into your .NET-based applications to work with Microsoft Visio files. Please refer to the following use cases for printing diagram documents,'
tags: ['print visio', 'print visio diagram', 'print visio documents', 'print visio in csharp']
categories: ['Aspose.Diagram Product Family']
---



{{< figure align=center src="images/print-visio-diagram.jpg" alt="">}}


You can print Diagram documents like [VSDX][1], [DWG][2], [VDW][3], [VSTX][4] programmatically using C#. [Aspose.Diagram for .NET][5] API can be integrated into your .NET-based applications to work with Microsoft Visio files. Please refer to the following use cases for printing diagram documents:

*   [Visio Document VSD, VSDX, DWG, etc., Printer – C# API Installation][6]
*   [Print a Visio Document with XpsPrint Programmatically using C#][7]
*   [Printing a Visio Diagram to the Default Printer Programmatically in C#][8]
*   [Print a Visio Diagram to a Specific Printer Programmatically with C#][9]

## Visio Document VSD, VSDX, DWG, etc., Printer – C# API Installation {#section1}

You can print Visio shapes and diagrams in VSD, VSDX, DWG, and many other supported file formats using [Aspose.Diagram for .NET][10]. Simply configure the API by downloading the DLL file from the [New Releases][11], or quickly install it from [NuGet][12] Package Manager with the following installation command:

```
PM> Install-Package Aspose.Diagram
```

## Print a Visio Document with XpsPrint Programmatically using C# {#section2}

XpsPrint class is really helpful for printing Diagram files on a server-side application because using .NET Framework printing classes is not supported by a service. The following steps explain how to print a Visio Document with XpsPrint programmatically with C#:

1.  Use Aspose.Diagram to convert the document to XPS and store it in a memory stream.
2.  Send a Diagram document to a printer using the XpsPrint API.

The following code shows how to print a Visio document by sending it to a printer with XpsPrint API:

{{< gist aspose-com-gists 5ae21aefe19e33728280366226573cb8 "Print-Diagram-XpsPrint.cs" >}}

## Print a Visio Diagram to the Default Printer Programmatically in C# {#section3}

You can print a Visio Diagram file such as VSDX, DWG, VST, etc. programmatically using C#. Please follow the steps below:

1.  Create an instance of the [Diagram][13] class to load a diagram for printing.
2.  Call the [Print][14] method without any parameters or arguments.

The code below explains how to print Microsoft Diagram files to default printer programmatically with C#:

{{< gist aspose-com-gists 5ae21aefe19e33728280366226573cb8 "Print-Default.cs" >}}

## Print a Visio Diagram to a Specific Printer Programmatically with C# {#section4}

You can print a Visio diagram containing different shapes to a specific printer with the below steps:

1.  Load the input diagram file with the [Diagram][15] class.
2.  Specify the printer name and Job name and call the [Print()][16] method.

The following code elaborates how to print a Diagram file to a specific printer in C#:

{{< gist aspose-com-gists 5ae21aefe19e33728280366226573cb8 "Print-Visio-Job-Printer.cs" >}}

## Get Free API License

You can request a [Free Temporary License][17] to evaluate the API without any limitations.

## Conclusion

In this article, you have learned how to print Microsoft Visio Diagrams and shapes in VSDX, VSD, DWG, and other file formats programmatically using C#. You can set different options like default or specific printer or job name, etc. as per your requirements. Furthermore, you can go through the [Documentation][18] to explore other features. In case of any concerns, please feel free to contact us at the [Free Support Forum][19].

## See Also

[Convert Visio VSD/VSDX File to Image Programmatically in C#][20]




[1]: https://docs.fileformat.com/image/vsdx/
[2]: https://docs.fileformat.com/cad/dwg/
[3]: https://docs.fileformat.com/web/vdw/
[4]: https://docs.fileformat.com/image/vstx/
[5]: https://products.aspose.com/diagram/net/
[6]: #section1
[7]: #section2
[8]: #section3
[9]: #section4
[10]: https://products.aspose.com/diagram/net/
[11]: https://downloads.aspose.com/diagram/net
[12]: https://www.nuget.org/packages/Aspose.Diagram/
[13]: https://apireference.aspose.com/diagram/net/aspose.diagram/diagram
[14]: https://apireference.aspose.com/diagram/net/aspose.diagram/diagram/methods/print/index
[15]: https://apireference.aspose.com/diagram/net/aspose.diagram/diagram
[16]: https://apireference.aspose.com/diagram/net/aspose.diagram/diagram/methods/print/index
[17]: https://purchase.aspose.com/temporary-license
[18]: https://purchase.aspose.com/temporary-license
[19]: https://forum.aspose.com/c/diagram
[20]: https://blog.aspose.com/2021/07/02/convert-visio-vsdx-to-image-csharp/






---
title: 'Insert or Remove Header and Footer in VSD VSDX Files in C#'
date: Sun, 10 Apr 2022 21:26:00 +0000
draft: false
url: /2022/04/10/insert-remove-header-footer-vsd-vsdx-csharp/
author: 'Farhan Raza'
summary: 'Headers and footers are used to display information over the top and bottom margin of each page of a file. They can include the topic, chapter, author, page number, and other relevant information. Visio diagrams in VSD or VSDX format can also contain a header and footer to show important information. This article covers how to **insert or remove the header and footer in Visio files programmatically in C#.**'
tags: ['Add Header in Visio File', 'Delete Header in Visio File', 'Header Footer in VSD', 'Header Footer in VSDX', 'Insert Header in Visio File', 'Insert or Delete Header Footer in Visio csharp', 'Remove Header in Visio File', 'csharp Insert or Delete Header Footer']
categories: ['Aspose.Diagram Product Family']
---



{{< figure align=center src="images/Header-Footer-Visio-1024x536.jpeg" alt="Header Footer Visio csharp">}}


Headers and footers are used to display information over the top and bottom margin of each page of a file. They can include the topic, chapter, author, page number, and other relevant information. Visio diagrams in [VSD](https://docs.fileformat.com/visio/vsd/) or [VSDX](https://docs.fileformat.com/visio/vsdx/) format can also contain a header and footer to show important information. This article covers how to insert or remove the header and footer in Visio files programmatically in C#.

*   [Manipulate Header and Footer in VSD/VSDX Diagram File  – C# API Installation](#section1)
*   [Insert Header and Footer in Visio Diagram File Programmatically in C#](#section2)
*   [Remove Header and Footer in Visio File in C#](#section3)

## Manipulate Header and Footer in VSD/VSDX Diagram File – C# API Installation {#section1}

You can create, edit, or manipulate Visio files in VSD, VSDX, and several other file formats. For working with the header and footer section in Visio diagrams, you need to download the DLL file of [Aspose.Diagram for .NET](https://products.aspose.com/diagram/net/)  from the [Downloads](https://downloads.aspose.com/) section, or run the following NuGet installation commands:

```
PM> Install-Package Aspose.Diagram
```

## Insert Header and Footer in Visio Diagram File Programmatically in C# {#section2}

You can insert or add the header and footer in a Visio diagram file by following the steps below:

1.  Initialize an instance of the [Diagram](https://apireference.aspose.com/diagram/net/aspose.diagram/diagram) class to load the input VSD or VSDX Visio file.
2.  Set different properties of the [HeaderFooter](https://apireference.aspose.com/diagram/net/aspose.diagram/headerfooter) class.
3.  Save the output Visio diagram.

The following code snippet demonstrates how to insert or add a header and footer in a VSD or VSDX diagram programmatically in C#:

\[gist id="ef14ca1efafcd835cc694f763926ddd6" file="Insert Header Footer.cs"\]

The screenshot below shows a sample Visio file after inserting the header and footer in a VSD/VSDX diagram file:



{{< figure align=center src="images/Header-Footer-Preview.jpeg" alt="Header Footer Visio">}}


## Remove Header and Footer in Visio File in C# {#section3}

You can remove or delete the header and footer from a Visio diagram with the following steps:

1.  Create an object of the [Diagram](https://apireference.aspose.com/diagram/net/aspose.diagram/diagram) class to load the input Visio file.
2.  Access different properties of the [HeaderFooter](https://apireference.aspose.com/diagram/net/aspose.diagram/headerfooter) classes and clear the properties.
3.  Save the output Visio file after removing the header and footer.

The code snippet below shows how to remove or delete the header and footer from a Visio file in C#:

\[gist id="ef14ca1efafcd835cc694f763926ddd6" file="Remove Header Footer.cs"\]

## Get a Free API License

You can evaluate the API in its full capacity by getting a [free temporary license](https://purchase.aspose.com/temporary-license).

## Conclusion

In this article, you have learned how to insert or remove the header and footer from a Visio diagram in VSD or VSDX file format programmatically in C#. Furthermore, you may visit the [documentation](https://docs.aspose.com/diagram/net/developer-guide/) section to learn various other features offered by the API. Please contact us at the [forum](https://forum.aspose.com/c/diagram) in case of any concerns or queries.

## See Also

[Convert Visio VSD or VSDX to XAML in C#](https://blog.aspose.com/2022/03/29/convert-vsd-vsdx-to-xaml-csharp/)




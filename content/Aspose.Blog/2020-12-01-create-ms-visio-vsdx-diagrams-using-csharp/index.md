---
title: 'Create MS Visio VSDX Diagrams using C#'
seoTitle: "Create Visio VSDX Diagrams using C# | Create Shapes or Flowcharts"
description: "Create MS Visio VSDX diagrams using C#. Create flowcharts, insert Visio master, pages, shapes, and text within new or existing MS Visio VSDX diagrams."
date: Tue, 01 Dec 2020 22:51:01 +0000
draft: false
url: /2020/12/01/create-ms-visio-vsdx-diagrams-using-csharp/
author: Usman Aziz
summary: '[MS Visio][1] is a popular application that lets you create a wide range of diagrams such as flowcharts, data flow diagrams, business process models and etc. [VSDX][2] is the file format that MS Visio uses to store the diagrams. In order to automate VSDX manipulation, this article provides you a basic tutorial of **how to create VSDX diagrams from scratch in C#**. Furthermore, it covers how to insert pages, shapes, and text in the VSDX diagrams from within .NET applications.'
tags: ['create ms visio vsdx diagrams in csharp', 'create vsdx files in csharp', 'insert pages in vsdx', 'insert shapes in vsdx']
categories: ['Aspose.Diagram Product Family']
---

[MS Visio][3] is a popular application that lets you create a wide range of diagrams such as flowcharts, data flow diagrams, business process models and etc. [VSDX][4] is the file format that MS Visio uses to store the diagrams. In order to automate VSDX manipulation, this article provides you a basic tutorial of **how to create Visio diagrams from scratch in C#**. Furthermore, it covers how to insert pages, shapes, and text in the VSDX diagrams from within .NET applications.

*   [C# Visio API - Free Download][5]
*   [Create MS Visio Diagram using C#][6]
*   [Add Master to VSDX Diagram in C#][7]
*   [Insert Pages in a Visio Diagram in C#][8]
*   [Create a Shape in a Visio Diagram in C#][9]
*   [Add a Text Shape in the Visio Page in C#][10]

## C# Visio API - Free Download {#CSharp-Visio-API-Free-Download}

[Aspose.Diagram for .NET][11] is a feature-rich API that lets you create, edit, convert, and process MS Visio diagrams from within your .NET applications. The API makes it easier for you to manipulate the VSDX diagrams with easy to use properties and methods. You can either [download][12] API's DLL or get it installed within your .NET applications using [NuGet][13].

```
Install-Package Aspose.Diagram
```

## Create Visio VSDX Diagram using C# {#Create-MS-Visio-Diagram-using-CSharp}

First of all, let's create an empty VSDX diagram from scratch. The following are the steps to do so:

*   Create an instance of [Diagram][14] class.
*   Use the [Diagram.Save(Sring fileName, SaveFileFormat.VSDX)][15] method to save the file as VSDX.

The following code sample shows how to create Visio VSDX diagram in C#.

{{< gist aspose-diagram cce69e51f567ea17ef24bc35fef0f689 "Examples-CSharp-Working-Diagrams-CreateDiagram-CreateDiagram.cs" >}}

## Add Master to Visio Diagram in C# {#Add-Master-to-VSDX-Diagram-in-CSharp}

Master is used to add the stencil which contains a collection of shapes to be used in diagrams. If you want to add the master, you need a VSS stencil file and master ID. The following are the steps to add a master to the Visio diagram using Aspose.Diagram.

*   Create a new diagram or load an existing one using the [Diagram][16] class.
*   Add master using [Diagram.AddMaster(String fileName, Int masterID)][17] method.
*   Add a shape from the master to the diagram using the [Diagram.AddShape(Double, Double, String, Int)][18] method.
*   Save diagram using [Diagram.Save(Sring fileName, SaveFileFormat.VSDX)][19] method.

The following code sample shows how to add a master to the Visio diagram using C#.

{{< gist aspose-diagram cce69e51f567ea17ef24bc35fef0f689 "Examples-CSharp-Working-with-Masters-AddMasterFromStencil-AddMasterFromStencil.cs" >}}

For more details, please visit [working with master][20].

## Insert Pages in a Visio Diagram in C# {#Insert-Pages-in-a-Visio-Diagram-in-CSharp}

MS Visio diagrams consist of one or more pages and each page contains the diagrams. Therefore, before adding a shape, you need to add a page using the following steps.

*   Create a new diagram or load an existing one using the [Diagram][21] class.
*   Check if the diagram already contains a page using [Diagram.Pages.Count][22] property.
*   If it does, get the ID of the last page using _Diagram.Pages\[index\].ID_ property.
*   Create a new page using [Page][23] class and set its name and ID.
*   Add page to the diagram using the [Diagram.Pages.Add(Page)][24] method.
*   Save VSDX diagram using [Diagram.Save(Sring fileName, SaveFileFormat.VSDX)][25] method.

The following code sample shows how to add a page in Visio VSDX diagram using C#.

{{< gist aspose-diagram cce69e51f567ea17ef24bc35fef0f689 "Examples-CSharp-Working-with-Pages-InsertBlankPageInVisio-InsertBlankPageInVisio.cs" >}}

For more details, please visit [working with pages][26].

## Create a Shape in Visio Diagram using C# {#Create-a-Shape-in-a-Visio-Diagram-in-CSharp}

Shapes are the building blocks of the Visio diagrams. MS Visio supports a wide range of shapes to create diagrams in various domains. The following steps show how to insert a shape in Visio Diagram.

*   Create a new diagram or load an existing one using the [Diagram][27] class.
*   Create a Page or get the desired page in a Page object.
*   Add master to the diagram using [Diagram.AddMaster(String fileName, Int masterID)][28] method.
*   Add a new rectangular shape using [Diagram.AddShape(pinX, pinY, width, height, masterName, PageIndex)][29] method.
*   Store the shape ID returned by _Diagram.AddShape()_ method.
*   Retrieve the newly added shape in the Shape object using _Page.Shapes.GetShape(long ID)_ method.
*   Set shape's properties such as text, color, etc.
*   Save VSDX diagram using [Diagram.Save(Sring fileName, SaveFileFormat.VSDX)][30] method.

The following code sample shows how to add a shape in the Visio diagram using C#.

{{< gist aspose-diagram cce69e51f567ea17ef24bc35fef0f689 "Examples-CSharp-Working-Shapes-AddingNewShape-AddingNewShape.cs" >}}

For more details, please visit [working with shapes][31].

## Add a Text Shape in the Visio Page in C# {#Add-a-Text-Shape-in-the-Visio-Page-in-CSharp}

In various cases, you also need to add text to the Visio diagrams. For this, you can follow the below steps.

*   Create a new diagram or load an existing one using the [Diagram][32] class.
*   Add text to a particular page using [Diagram.Pages\[0\].AddText(PinX, PinY, Width, Height, "Test text")][33] method.
*   Save the VSDX diagram using [Diagram.Save(Sring fileName, SaveFileFormat.VSDX)][34] method.

The following code sample shows how to add text in a VSDX diagram using C#.

{{< gist aspose-diagram cce69e51f567ea17ef24bc35fef0f689 "Examples-CSharp-Working-with-Text-InsertTextShape-InsertTextShape.cs" >}}

For more details, please visit [working with text][35].

## Conclusion

In this post, you have learned some basic features of Aspose.Diagram for .NET to create Visio VSDX diagrams from scratch. The code samples have shown how to add masters, pages, shapes, and text in VSDX diagrams using C#. You can explore more about the API using the [documentation][36].

## See Also

*   [Convert MS Visio Diagrams to PDF, PNG, JPEG, SVG, HTML and XAML in Node.js][37]




[1]: https://en.wikipedia.org/wiki/Microsoft_Visio
[2]: https://docs.fileformat.com/image/vsdx/
[3]: https://en.wikipedia.org/wiki/Microsoft_Visio
[4]: https://docs.fileformat.com/image/vsdx/
[5]: #CSharp-Visio-API-Free-Download
[6]: #Create-MS-Visio-Diagram-using-CSharp
[7]: #Add-Master-to-VSDX-Diagram-in-CSharp
[8]: #Insert-Pages-in-a-Visio-Diagram-in-CSharp
[9]: #Create-a-Shape-in-a-Visio-Diagram-in-CSharp
[10]: #Add-a-Text-Shape-in-the-Visio-Page-in-CSharp
[11]: https://products.aspose.com/diagram/net
[12]: https://downloads.aspose.com/diagram/net
[13]: http://nuget.org/packages/Aspose.Diagram
[14]: https://apireference.aspose.com/diagram/net/aspose.diagram/diagram
[15]: https://apireference.aspose.com/diagram/net/aspose.diagram.diagram/save/methods/2
[16]: https://apireference.aspose.com/diagram/net/aspose.diagram/diagram
[17]: https://apireference.aspose.com/diagram/net/aspose.diagram.diagram/addmaster/methods/3
[18]: https://apireference.aspose.com/diagram/net/aspose.diagram.diagram/addshape/methods/2
[19]: https://apireference.aspose.com/diagram/net/aspose.diagram.diagram/save/methods/2
[20]: https://docs.aspose.com/diagram/net/working-with-masters/
[21]: https://apireference.aspose.com/diagram/net/aspose.diagram/diagram
[22]: https://apireference.aspose.com/diagram/net/aspose.diagram/collection/properties/count
[23]: https://apireference.aspose.com/diagram/net/aspose.diagram/page
[24]: https://apireference.aspose.com/diagram/net/aspose.diagram/pagecollection/methods/add
[25]: https://apireference.aspose.com/diagram/net/aspose.diagram.diagram/save/methods/2
[26]: https://docs.aspose.com/diagram/net/working-with-pages/
[27]: https://apireference.aspose.com/diagram/net/aspose.diagram/diagram
[28]: https://apireference.aspose.com/diagram/net/aspose.diagram.diagram/addmaster/methods/3
[29]: https://apireference.aspose.com/diagram/net/aspose.diagram.diagram/addshape/methods/1
[30]: https://apireference.aspose.com/diagram/net/aspose.diagram.diagram/save/methods/2
[31]: https://docs.aspose.com/diagram/net/working-with-shapes/
[32]: https://apireference.aspose.com/diagram/net/aspose.diagram/diagram
[33]: https://apireference.aspose.com/diagram/net/aspose.diagram/page/methods/addtext
[34]: https://apireference.aspose.com/diagram/net/aspose.diagram.diagram/save/methods/2
[35]: https://docs.aspose.com/diagram/net/working-with-text/
[36]: https://docs.aspose.com/diagram/net/developer-guide/
[37]: https://blog.aspose.com/2020/05/13/convert-ms-visio-vsd-vsdx-to-pdf-png-jpeg-svg-html-xaml-in-node-js/






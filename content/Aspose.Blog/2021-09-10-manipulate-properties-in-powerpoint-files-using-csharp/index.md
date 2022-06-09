---
title: 'Access or Modify Properties of PowerPoint Files using C#'
seoTitle: "C# Add, Access, Modify Properties in PowerPoint Files | .NET API"
description: "Use .NET PowerPoint API to add, access, and modify document properties in PowerPoint presentations using C#. Access built-in or custom properties."
date: Fri, 10 Sep 2021 14:54:23 +0000
draft: false
url: /2021/09/10/manipulate-properties-in-powerpoint-files-using-csharp/
author: Usman Aziz
summary: 'The document properties or metadata in PowerPoint files are used for identification of the presentations. Moreover, they provide additional information about the presentation such as author, title, keywords, subject, etc. In this article, you will learn **how to access or modify the properties in PowerPoint files programmatically using C#**.'
tags: ['access or modify builtin properties in powerpoint csharp', 'access or modify custom properties in powerpoint csharp', 'document properties in powerpoint files csharp']
categories: ['Aspose.Slides Product Family']
---



{{< figure align=center src="images/Document-Properties-in-PowerPoint.jpg" alt="Document Properties in PowerPoint C#">}}


The document properties or metadata in PowerPoint files are used for identification of the presentations. Moreover, they provide additional information about the presentation such as author, title, keywords, subject, etc. In this article, you will learn **how to access or modify the properties in PowerPoint files programmatically using C#**.

*   [.NET API to Access/Modify Properties in PowerPoint Files][1]
*   [Types of Properties in PowerPoint Presentations][2]
*   [Access Built-in Properties in PowerPoint Presentations][3]
*   [Modify Built-in Properties in PowerPoint Presentations][4]
*   [Add Custom Properties in PowerPoint Presentations][5]
*   [Access Custom Properties in PowerPoint Presentations][6]
*   [Modify Custom Properties in PowerPoint Presentations][7]

## .NET API to Access/Modify Properties in PowerPoint Files {#API-to-Access-Modify-Properties-in-PowerPoint-Files}

To access or modify the built-in or custom document properties, we will use [Aspose.Slides for .NET][8]. It is a powerful API for creating and manipulating PowerPoint and OpenOffice documents. The API is available as a [downloadable DLL][9] as well as on [NuGet][10].

```
PM> Install-Package Aspose.Slides.NET 
```

## Types of Properties in PowerPoint Presentations {#Types-of-Properties-in-PowerPoint-Presentations}

The PowerPoint presentations support two types of document properties: built-in and custom. The built-in properties provide general information about the presentations such as title, author, subject, etc. Whereas, the custom properties are defined by the users in the form of key/value pairs. The following sections demonstrate how to add, access, and modify properties belonging to each of the above-mentioned types.

## Access Built-in Properties in PowerPoint Presentations using C# {#Access-Built-in-Properties-in-PowerPoint-Presentations}

The following are the steps to access the built-in properties in PowerPoint presentations using C#.

*   Load the PowerPoint presentation using [Presentation][11] class.
*   Access the built-in properties in an [IDocumentProperties][12] object from [Presentation.DocumentProperties][13] property.
*   Read each built-in property in the presentation using _IDocumentProperties_ object, such as, [IDocumentProperties.Author][14].

The following code sample shows how to access built-in properties in PowerPoint presentations.

{{< gist aspose-com-gists c5d443992489bba0bbd7256a8fb2d2e0 "access-builtin-properties.cs" >}}

## Modify Built-in Properties in PowerPoint Presentations using C# {#Modify-Built-in-Properties-in-PowerPoint-Presentations}

The following are the steps to modify the values of the built-in properties in PowerPoint presentations using C#.

*   First, load the PowerPoint presentation using [Presentation][15] class.
*   Then, get reference of the built-in properties in an [IDocumentProperties][16] object from [Presentation.DocumentProperties][17] property.
*   Modify the desired built-in property in the presentation using _IDocumentProperties_ object, such as, [IDocumentProperties.Author][18].
*   Finally, save the presentation using [Presentation.Save(String, SaveFormat)][19] method.

The following code sample shows how to modify the built-in properties in PowerPoint Presentations.

{{< gist aspose-com-gists c5d443992489bba0bbd7256a8fb2d2e0 "modify-builtin-properties.cs" >}}

## Add Custom Properties in PowerPoint Presentations using C# {#Add-Custom-Properties-in-PowerPoint-Presentations}

The following are the steps to add custom properties in a PowerPoint presentation using C#.

*   First, load the PowerPoint presentation using [Presentation][20] class.
*   Then, get reference of the document properties in an [IDocumentProperties][21] object from [Presentation.DocumentProperties][22] property.
*   Add a custom property by defining its key and value, e.g. _IDocumentProperties\["Key"\] = "Value"_.
*   Finally, save the presentation using [Presentation.Save(String, SaveFormat)][23] method.

The following code sample shows how to add custom properties in a PowerPoint presentation.

{{< gist aspose-com-gists c5d443992489bba0bbd7256a8fb2d2e0 "add-custom-properties.cs" >}}

## Access Custom Properties in PowerPoint Presentations using C# {#Access-Custom-Properties-in-PowerPoint-Presentations}

The following steps demonstrate how to access the custom properties in a PowerPoint Presentation using C#.

*   First, load the PowerPoint presentation using [Presentation][24] class.
*   Get reference of the document properties in an [IDocumentProperties][25] object from [Presentation.DocumentProperties][26] property.
*   Access each custom property using [IDocumentProperties.GetCustomPropertyName(int32 index)][27] method in a loop.

The following code sample shows how to access custom properties in a PowerPoint Presentation.

{{< gist aspose-com-gists c5d443992489bba0bbd7256a8fb2d2e0 "access-custom-properties.cs" >}}

## Modify Custom Properties in PowerPoint Presentations using C# {#Modify-Custom-Properties-in-PowerPoint-Presentations}

The following are the steps to modify the custom properties in a PowerPoint presentation.

*   First, load the PowerPoint presentation using [Presentation][28] class.
*   Then, get reference of the document properties in an [IDocumentProperties][29] object from [Presentation.DocumentProperties][30] property.
*   Access each custom property using [IDocumentProperties.GetCustomPropertyName(int32 index)][31] method in a loop.
*   Modify the value of a property by specifying its key in _IDocumentProperties\[IDocumentProperties.GetCustomPropertyName(int index)\]_ array.
*   Finally, save the presentation using [Presentation.Save(String, SaveFormat)][32] method.

The following code sample shows how to modify a custom property in a PowerPoint presentation.

{{< gist aspose-com-gists c5d443992489bba0bbd7256a8fb2d2e0 "modify-custom-properties.cs" >}}

## Get a Free API License {#Get-a-Free-API-License}

You can use Aspose.Slides for .NET without evaluation limitations by requesting a [temporary license][33].

## Online Demo

You can also try the [online tool][34] to view and edit document properties in presentations, which is based on Aspose.Slides.

You may also want to try out Aspose [free online PowerPoint editor.][35]

## Conclusion

In this article, you have learned how to add, access, and modify document properties in PowerPoint presentations using C#. The article has covered the manipulation of built-in and custom document properties explicitly. In addition, you can visit the [documentation][36] to explore more about Aspose.Slides for .NET. Also, you can post your queries to our [forum][37].

## See Also

*   [Create MS PowerPoint Presentations in C#][38]
*   [Convert PowerPoint PPTX/PPT to PNG Images in C#][39]
*   [Set Slide Background in PowerPoint Presentations using C#][40]
*   [Generate Thumbnails for PowerPoint PPTX or PPT using C#][41]
*   [Apply Animation to Text in PowerPoint using C#][42]
*   [Split PowerPoint Presentations using C#][43]




[1]: #API-to-Access-Modify-Properties-in-PowerPoint-Files
[2]: #Types-of-Properties-in-PowerPoint-Presentations
[3]: #Access-Built-in-Properties-in-PowerPoint-Presentations
[4]: #Modify-Built-in-Properties-in-PowerPoint-Presentations
[5]: #Add-Custom-Properties-in-PowerPoint-Presentations
[6]: #Access-Custom-Properties-in-PowerPoint-Presentations
[7]: #Modify-Custom-Properties-in-PowerPoint-Presentations
[8]: https://products.aspose.com/slides/net
[9]: https://downloads.aspose.com/slides/net
[10]: https://www.nuget.org/packages/Aspose.Slides.NET
[11]: https://apireference.aspose.com/net/slides/aspose.slides/presentation
[12]: https://apireference.aspose.com/slides/net/aspose.slides/idocumentproperties
[13]: https://apireference.aspose.com/slides/net/aspose.slides/presentation/properties/documentproperties
[14]: https://apireference.aspose.com/slides/net/aspose.slides/idocumentproperties/properties/author
[15]: https://apireference.aspose.com/net/slides/aspose.slides/presentation
[16]: https://apireference.aspose.com/slides/net/aspose.slides/idocumentproperties
[17]: https://apireference.aspose.com/slides/net/aspose.slides/presentation/properties/documentproperties
[18]: https://apireference.aspose.com/slides/net/aspose.slides/idocumentproperties/properties/author
[19]: https://apireference.aspose.com/slides/net/aspose.slides.presentation/save/methods/5
[20]: https://apireference.aspose.com/net/slides/aspose.slides/presentation
[21]: https://apireference.aspose.com/slides/net/aspose.slides/idocumentproperties
[22]: https://apireference.aspose.com/slides/net/aspose.slides/presentation/properties/documentproperties
[23]: https://apireference.aspose.com/slides/net/aspose.slides.presentation/save/methods/5
[24]: https://apireference.aspose.com/net/slides/aspose.slides/presentation
[25]: https://apireference.aspose.com/slides/net/aspose.slides/idocumentproperties
[26]: https://apireference.aspose.com/slides/net/aspose.slides/presentation/properties/documentproperties
[27]: https://apireference.aspose.com/slides/net/aspose.slides/idocumentproperties/methods/getcustompropertyname
[28]: https://apireference.aspose.com/net/slides/aspose.slides/presentation
[29]: https://apireference.aspose.com/slides/net/aspose.slides/idocumentproperties
[30]: https://apireference.aspose.com/slides/net/aspose.slides/presentation/properties/documentproperties
[31]: https://apireference.aspose.com/slides/net/aspose.slides/idocumentproperties/methods/getcustompropertyname
[32]: https://apireference.aspose.com/slides/net/aspose.slides.presentation/save/methods/5
[33]: https://purchase.aspose.com/temporary-license
[34]: https://products.aspose.app/slides/metadata
[35]: https://products.aspose.app/slides/editor
[36]: https://docs.aspose.com/slides/net/developer-guide/
[37]: https://forum.aspose.com/
[38]: https://blog.aspose.com/2020/12/04/create-powerpoint-presentations-in-csharp/
[39]: https://blog.aspose.com/2021/09/01/convert-powerpoint-to-png-in-csharp/
[40]: https://blog.aspose.com/2021/08/31/set-background-in-powerpoint-using-csharp/
[41]: https://blog.aspose.com/2021/08/30/generate-pptx-thumbnails-using-csharp/
[42]: https://blog.aspose.com/2021/08/20/apply-animation-to-text-in-powerpoint-using-csharp/
[43]: https://blog.aspose.com/2021/09/03/split-powerpoint-presentations-using-csharp/





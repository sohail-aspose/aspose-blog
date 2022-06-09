---
title: 'Add, Extract, and Remove VBA Macros in PowerPoint using C#'
seoTitle: "C# Add, Extract, Remove VBA Macros in PowerPoint | .NET API"
description: "Use .NET PowerPoint API to work with VBA macros in PowerPoint using C#. Add, extract, and remove PowerPoint VBA macros using C# in .NET applications."
date: Wed, 31 Mar 2021 11:12:00 +0000
draft: false
url: /2021/03/31/add-extract-remove-vba-macros-in-powerpoint-chsarp/
author: Usman Aziz
summary: 'The VBA macros are used to automate different functionalities in PowerPoint presentations. For example, you can use VBA to perform repetitive tasks, generate charts and forms, etc. In this article, you will learn how to work with PowerPoint VBA macros programmatically. Particularly, the article will cover **how to add, extract or remove VBA macros in PowerPoint presentations using C#**.'
tags: ['Add VBA Macros in PowerPoint in Csharp', 'Extract VBA Macros in PowerPoint in Csharp', 'Remove VBA Macros in PowerPoint in Csharp']
categories: ['Aspose.Slides Product Family']
---



{{< figure align=center src="images/Add-Remove-VBA-Module.jpg" alt="add remove powerpoint vba C#">}}


The VBA macros are used to automate different functionalities in PowerPoint presentations. For example, you can use VBA to perform repetitive tasks, generate charts and forms, etc. In this article, you will learn how to work with PowerPoint VBA macros programmatically. Particularly, the article will cover **how to add, extract or remove VBA macros in PowerPoint presentations using C#**.

*   [C# API for PowerPoint VBA Macros][1]
*   [Add VBA Macros in PowerPoint Presentations using C#][2]
*   [Extract VBA Macros from PowerPoint Presentations][3]
*   [Remove VBA Macros from PowerPoint Presentations][4]
*   [Get a Free API License][5]

**TIP**

You may want to check out Aspose [FREE macro removal web app][6].

## C# API for PowerPoint VBA Macros {#C-API-for-VBA-Macros-in-PowerPoint}

[Aspose.Slides for .NET][7] is a feature-rich API that lets you create, edit and convert PowerPoint presentations using C#. Furthermore, the API allows you to work with VBA macros seamlessly. In order to use the API, you can either [download][8] its DLL or install it using [NuGet][9].

```
PM> Install-Package Aspose.Slides.NET
```

## Add VBA Macro in PowerPoint Presentations using C# {#Add-VBA-Macros-in-PowerPoint-Presentations-in-C}

The following are the steps to add a VBA macro in a PowerPoint presentation using C#.

*   First, create an instance of the [Presentation][10] class to load the PowerPoint presentation.
*   Assign a new [VbaProject][11] to [Presentation.VbaProject][12] property.
*   Add an empty VBA module using [Presentation.VbaProject.Modules.AddEmptyModule(string)][13] method.
*   Get the reference of the added module into an [IVbaModule][14] object.
*   Add source code to the VBA module using [IVbaModule.SourceCode][15] property.
*   Create references to Microsoft Office and add them to [Presentation.VbaProject.References][16] collection.
*   Finally, save the presentation file using [Presentation.Save(string, SaveFormat.Pptm)][17] method.

The following code sample shows how to add VBA macro in a PowerPoint presentation using C#.

{{< gist aspose-com-gists 857bcf1b08c99566ed492b445ba33214 "add-vba-macro-in-powerpoint.cs" >}}

## Extract VBA Macros from PowerPoint using C# {#Extract-VBA-Macros-in-PowerPoint-Presentations}

Aspose.Slides for .NET also allows you to extract VBA modules from VBA projects in PowerPoint presentations. The following are the steps to perform this operation.

*   First, load the macro-enabled PowerPoint presentation using the [Presentation][18] class.
*   Check if [Presentation.VbaProject][19] property is not null.
*   Loop through each [IVbaModule][20] in [Presentation.VbaProject.Modules][21] collection.
*   Finally, extract source code using [IVbaModule.SourceCode][22] property.

The following code sample shows how to extract PowerPoint VBA macros using C#.

{{< gist aspose-com-gists 857bcf1b08c99566ed492b445ba33214 "extract-vba-macro-in-powerpoint.cs" >}}

## Remove PowerPoint VBA Macros {#Remove-VBA-Macros-in-PowerPoint-Presentations}

You can also remove a particular VBA macro from a PowerPoint presentation. For this, you will access and remove the VBA module by its index from the VBA project. The following are the steps to perform this operation.

*   First, load the macro-enabled PowerPoint presentation using the [Presentation][23] class.
*   Remove VBA module by index using [Presentation.VbaProject.Modules.Remove(Presentation.VbaProject.Modules\[0\])][24] method.
*   Finally, save the updated presentation using [Presentation.Save(string, SaveFormat.Pptm)][25] method.

The following code sample shows how to remove a PowerPoint VBA macro.

{{< gist aspose-com-gists 857bcf1b08c99566ed492b445ba33214 "remove-vba-macro-in-powerpoint.cs" >}}

## Get a Free API License {#Get-a-Free-API-License}

You can try Aspose.Slides for .NET without evaluation limitations by requesting a [temporary license][26].

## Conclusion

In this article, you have learned how to work with PowerPoint VBA macros using C#. Particularly, you have seen how to add, extract and remove VBA macros in PowerPoint presentations. In order to explore other features of the API, you can consult the [documentation][27]. Moreover, you can feel free to let us know about your queries via our [forum][28].

## See Also

*   [Create MS PowerPoint Presentations in C#][29]




[1]: #C-API-for-VBA-Macros-in-PowerPoint
[2]: #Add-VBA-Macros-in-PowerPoint-Presentations-in-C
[3]: #Extract-VBA-Macros-in-PowerPoint-Presentations
[4]: #Remove-VBA-Macros-in-PowerPoint-Presentations
[5]: #Get-a-Free-API-License
[6]: https://products.aspose.app/slides/remove-macros
[7]: https://products.aspose.com/slides/net
[8]: https://downloads.aspose.com/slides/net
[9]: https://www.nuget.org/packages/Aspose.Slides.Net
[10]: http://www.aspose.com/api/net/slides/aspose.slides/presentation
[11]: https://apireference.aspose.com/slides/net/aspose.slides.vba/vbaproject
[12]: https://apireference.aspose.com/slides/net/aspose.slides/presentation/properties/vbaproject
[13]: https://apireference.aspose.com/slides/net/aspose.slides.vba/ivbamodulecollection/methods/addemptymodule
[14]: https://apireference.aspose.com/slides/net/aspose.slides.vba/ivbamodule
[15]: https://apireference.aspose.com/slides/net/aspose.slides.vba/ivbamodule/properties/sourcecode
[16]: https://apireference.aspose.com/slides/net/aspose.slides.vba/ivbaproject/properties/references
[17]: https://apireference.aspose.com/slides/net/aspose.slides.presentation/save/methods/4
[18]: http://www.aspose.com/api/net/slides/aspose.slides/presentation
[19]: https://apireference.aspose.com/slides/net/aspose.slides/presentation/properties/vbaproject
[20]: https://apireference.aspose.com/slides/net/aspose.slides.vba/ivbamodule
[21]: https://apireference.aspose.com/slides/net/aspose.slides.vba/ivbaproject/properties/modules
[22]: https://apireference.aspose.com/slides/net/aspose.slides.vba/ivbamodule/properties/sourcecode
[23]: http://www.aspose.com/api/net/slides/aspose.slides/presentation
[24]: https://apireference.aspose.com/slides/net/aspose.slides.vba/ivbamodulecollection/methods/remove
[25]: https://apireference.aspose.com/slides/net/aspose.slides.presentation/save/methods/4
[26]: https://purchase.aspose.com/temporary-license
[27]: https://docs.aspose.com/slides/net/developer-guide/
[28]: https://forum.aspose.com/
[29]: https://blog.aspose.com/2020/12/04/create-powerpoint-presentations-in-csharp/






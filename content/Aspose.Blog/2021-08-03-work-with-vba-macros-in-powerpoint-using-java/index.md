---
title: 'Add, Extract, and Remove VBA Macros in PowerPoint using Java'
seoTitle: "Java: Add, Extract, Remove VBA Macros in PowerPoint | Aspose.Slides"
description: "Use Java PowerPoint API to work with VBA macros in PowerPoint using Java. Add, extract, and remove PowerPoint VBA macros using Java."
date: Tue, 03 Aug 2021 17:19:00 +0000
draft: false
url: /2021/08/03/work-with-vba-macros-in-powerpoint-using-java/
author: Usman Aziz
summary: 'VBA macros are used to perform repetitive tasks, generate charts and forms, etc. in PowerPoint presentations. While working with the presentations programmatically, you may need to manipulate VBA macros. In accordance with that, in this article, you will learn **how to add, extract or remove VBA macros in PowerPoint presentations using Java**.'
tags: ['Add VBA Macros in PowerPoint Presentations', 'Extract VBA Macros from PowerPoint Presentations', 'Java API for PowerPoint VBA Macros', 'Remove VBA Macros from PowerPoint Presentations']
categories: ['Aspose.Slides Product Family']
---



{{< figure align=center src="images/Add-Remove-VBA-Module.jpg" alt="add remove powerpoint vba Java">}}


VBA macros are used to perform repetitive tasks, generate charts and forms, etc. in PowerPoint presentations. While working with the presentations programmatically, you may need to manipulate VBA macros. In accordance with that, in this article, you will learn **how to add, extract or remove VBA macros in PowerPoint presentations using Java**.

*   [Java API for PowerPoint VBA Macros][1]
*   [Add VBA Macros in PowerPoint Presentations][2]
*   [Extract VBA Macros from PowerPoint Presentations][3]
*   [Remove VBA Macros from PowerPoint Presentations][4]

**TIP**

You may want to try Aspose [online VBA macro removal tool][5].

## Java API for PowerPoint VBA Macros {#API-for-VBA-Macros-in-PowerPoint}

In order to work with VBA macros in presentations, we will use [Aspose.Slides for Java][6]. It is a feature-rich API that lets you create or manipulate PowerPoint presentations from within your Java applications. You can either [download][7] the API or install it using the following Maven configurations.

```
<repository>
    <id>AsposeJavaAPI</id>
    <name>Aspose Java API</name>
    <url>http://repository.aspose.com/repo/</url>
</repository>
```
```
<dependency>
    <groupId>com.aspose</groupId>
    <artifactId>aspose-slides</artifactId>
    <version>21.7</version>
    <classifier>jdk16</classifier>
</dependency>
```

## Add VBA Macro in PowerPoint Presentations using Java {#Add-VBA-Macros-in-PowerPoint-Presentations-in-Java}

The following are the steps to add a VBA macro in a PowerPoint presentation using Java.

*   First, create an instance of the [Presentation][8] class to load the PowerPoint presentation.
*   Assign a new [VbaProject][9] using [Presentation.setVbaProject()][10] method.
*   Add an empty VBA module using [Presentation.getVbaProject().getModules().addEmptyModule(String)][11] method.
*   Get the reference of the added module into an [IVbaModule][12] object.
*   Add source code to the VBA module using [IVbaModule.setSourceCode()][13] method.
*   Create references to Microsoft Office and add them to [Presentation.getVbaProject().getReferences()][14] collection.
*   Finally, save the presentation file using [Presentation.save(String, SaveFormat.Pptm)][15] method.

The following code sample shows how to add VBA macro in a PowerPoint presentation using Java.

{{< gist aspose-com-gists 0b663631cf9b657ec067f5b07720e8a0 "add-vba-macro-in-powerpoint.java" >}}

## Extract VBA Macros from PowerPoint using Java {#Extract-VBA-Macros-in-PowerPoint-Presentations}

The following are the steps to extract VBA macros from a PowerPoint presentation using Java.

*   First, load the macro-enabled PowerPoint presentation using the [Presentation][16] class.
*   Then, check if [Presentation.getVbaProject()][17] returns null.
*   Loop through each [IVbaModule][18] in collection using [Presentation.getVbaProject().getModules()][19].
*   Finally, extract source code using [IVbaModule.getSourceCode()][20] method.

The following code sample shows how to extract PowerPoint VBA macros.

{{< gist aspose-com-gists 0b663631cf9b657ec067f5b07720e8a0 "extract-vba-macro-in-powerpoint.java" >}}

## Remove PowerPoint VBA Macros {#Remove-VBA-Macros-in-PowerPoint-Presentations}

You can also remove a particular VBA macro from a PowerPoint using its index in the VBA project. The following are the steps to perform this operation.

*   First, load the macro-enabled PowerPoint presentation using the [Presentation][21] class.
*   Then, remove VBA module by index using [Presentation.getVbaProject().getModules().remove(IVbaModule)][22] method.
*   Finally, save the updated presentation using [Presentation.save(String, SaveFormat.Pptm)][23] method.

The following code sample shows how to remove a PowerPoint VBA macro.

{{< gist aspose-com-gists 0b663631cf9b657ec067f5b07720e8a0 "remove-vba-macro-in-powerpoint.java" >}}

## Get a Free API License {#Get-a-Free-API-License}

You can use Aspose.Slides for Java without evaluation limitations by requesting a [temporary license][24].

**TIP**

You may want to try Aspose [online VBA macro removal tool][25].

## Conclusion

In this article, you have learned how to work with PowerPoint VBA macros using Java. Particularly, you have seen how to add, extract and remove VBA macros in PowerPoint presentations. In order to explore other features of the API, you can consult the [documentation][26]. Moreover, you can feel free to let us know about your queries via our [forum][27].

## See Also

*   [Create MS PowerPoint Presentations in Java][28]




[1]: #API-for-VBA-Macros-in-PowerPoint
[2]: #Add-VBA-Macros-in-PowerPoint-Presentations-in-Java
[3]: #Extract-VBA-Macros-in-PowerPoint-Presentations
[4]: #Remove-VBA-Macros-in-PowerPoint-Presentations
[5]: https://products.aspose.app/slides/remove-macros
[6]: https://products.aspose.com/slides/java
[7]: https://downloads.aspose.com/slides/java
[8]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation
[9]: https://apireference.aspose.com/slides/java/com.aspose.slides/VbaProject
[10]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation#setVbaProject-com.aspose.slides.IVbaProject-
[11]: https://apireference.aspose.com/slides/java/com.aspose.slides/IVbaModuleCollection#addEmptyModule-java.lang.String-
[12]: https://apireference.aspose.com/slides/java/com.aspose.slides/IVbaModule
[13]: https://apireference.aspose.com/slides/java/com.aspose.slides/IVbaModule#setSourceCode-java.lang.String-
[14]: https://apireference.aspose.com/slides/java/com.aspose.slides/IVbaProject#getReferences--
[15]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation#save-java.lang.String-int-
[16]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation
[17]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation#getVbaProject--
[18]: https://apireference.aspose.com/slides/java/com.aspose.slides/IVbaModule
[19]: https://apireference.aspose.com/slides/java/com.aspose.slides/IVbaProject#getModules--
[20]: https://apireference.aspose.com/slides/java/com.aspose.slides/IVbaModule#getSourceCode--
[21]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation
[22]: https://apireference.aspose.com/slides/java/com.aspose.slides/IVbaModuleCollection#remove-com.aspose.slides.IVbaModule-
[23]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation#save-java.lang.String-int-
[24]: https://purchase.aspose.com/temporary-license
[25]: https://products.aspose.app/slides/remove-macros
[26]: https://docs.aspose.com/slides/java
[27]: https://forum.aspose.com/
[28]: https://blog.aspose.com/2021/01/18/create-powerpoint-presentations-using-java/






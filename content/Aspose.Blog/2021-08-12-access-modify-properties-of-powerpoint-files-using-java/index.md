---
title: 'Access or Modify Properties of PowerPoint Files using Java'
seoTitle: "Java Add or Modify Document Properties in PowerPoint Files | Java"
description: "Use Java PowerPoint API to add, access, and modify document properties in PowerPoint presentations using Java. Manipulate built-in or custom properties."
date: Thu, 12 Aug 2021 16:03:00 +0000
draft: false
url: /2021/08/12/access-modify-properties-of-powerpoint-files-using-java/
author: Usman Aziz
summary: 'PowerPoint files contain some additional information known as document properties. These properties are used for the identification of the presentations, which include author, title, keywords, subject, etc. In this article, you will learn **how to add, access or modify the document properties in PowerPoint files using Java**.'
tags: ['Access Built-in Properties in PowerPoint Presentations Java', 'Access Custom Properties in PowerPoint Presentations Java', 'Add Custom Properties in PowerPoint Presentations Java', 'Modify Built-in Properties in PowerPoint Presentations Java', 'Modify Custom Properties in PowerPoint Presentations Java']
categories: ['Aspose.Slides Product Family']
---



{{< figure align=center src="images/Document-Properties-in-PowerPoint.jpg" alt="Document Properties in PowerPoint Java">}}


PowerPoint files contain some additional information known as document properties. These properties are used for the identification of the presentations, which include author, title, keywords, subject, etc. In this article, you will learn **how to add, access or modify the document properties in PowerPoint files using Java**.

*   [Java API to Access/Modify Properties in PowerPoint Files][1]
*   [Types of Properties in PowerPoint Presentations][2]
*   [Access Built-in Properties in PowerPoint Presentations][3]
*   [Modify Built-in Properties in PowerPoint Presentations][4]
*   [Add Custom Properties in PowerPoint Presentations][5]
*   [Access Custom Properties in PowerPoint Presentations][6]
*   [Modify Custom Properties in PowerPoint Presentations][7]

## Java API for Document Properties in PowerPoint Files {#API-to-Access-Modify-Properties-in-PowerPoint-Files}

To access or modify the document properties in PowerPoint presentations, we will use [Aspose.Slides for Java][8]. The API allows you to create and manipulate PowerPoint and OpenOffice documents. It is available as a [downloadable JAR][9] as well as on Maven. You can install it using the following Maven configurations.

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
    <version>21.8</version>
    <classifier>jdk16</classifier>
</dependency>
```

## Types of Document Properties in PowerPoint Presentations {#Types-of-Properties-in-PowerPoint-Presentations}

There are two types of document properties in PowerPoint files: built-in and custom. The former provides general information about the presentations such as title, author, subject, etc. Whereas, the latter is used to add user-defined properties. In the below sections, you will see how to add, access, and modify built-in and custom document properties in PowerPoint presentations.

## Access Built-in Properties in PowerPoint Presentations using Java {#Access-Built-in-Properties-in-PowerPoint-Presentations}

The following are the steps to access the built-in properties in PowerPoint presentations using Java.

*   First, load the PowerPoint presentation using [Presentation][10] class.
*   Then, access the built-in properties in an [IDocumentProperties][11] object using [Presentation.getDocumentProperties()][12] method.
*   Read each built-in property in the presentation using _IDocumentProperties_ object, such as, [IDocumentProperties.getAuthor()][13].

The following code sample shows how to access built-in properties in PowerPoint presentations.

{{< gist aspose-com-gists 399dd464fe55eed7d9c9a2f088292039 "access-builtin-properties.java" >}}

## Modify Built-in Properties in PowerPoint Presentations using Java {#Modify-Built-in-Properties-in-PowerPoint-Presentations}

The following are the steps to modify the values of the built-in properties in PowerPoint presentations using Java.

*   First, load the PowerPoint presentation using [Presentation][14] class.
*   Then, get reference of the built-in properties in an [IDocumentProperties][15] object using [Presentation.getDocumentProperties()][16] method.
*   Modify the desired built-in property in the presentation using _IDocumentProperties_ object, such as, [IDocumentProperties.setAuthor()][17].
*   Finally, save the presentation using [Presentation.save(String, SaveFormat)][18] method.

The following code sample shows how to modify the built-in properties in PowerPoint Presentations.

{{< gist aspose-com-gists 399dd464fe55eed7d9c9a2f088292039 "modify-builtin-properties.java" >}}

## Add Custom Properties in PowerPoint Presentations using Java {#Add-Custom-Properties-in-PowerPoint-Presentations}

The following are the steps to add custom properties in a PowerPoint presentation using Java.

*   First, load the PowerPoint presentation using [Presentation][19] class.
*   Then, get reference of the document properties in an [IDocumentProperties][20] object using [Presentation.getDocumentProperties()][21] method.
*   Add a custom property by defining its key and value, e.g. _IDocumentPropertiesd.set\_Item("New Custom", 12)_.
*   Finally, save the presentation using [Presentation.save(String, SaveFormat)][22] method.

The following code sample shows how to add custom properties in a PowerPoint presentation.

{{< gist aspose-com-gists 399dd464fe55eed7d9c9a2f088292039 "add-custom-properties.java" >}}

## Access Custom Properties in PowerPoint Presentations using Java {#Access-Custom-Properties-in-PowerPoint-Presentations}

The following steps demonstrate how to access the custom properties in a PowerPoint Presentation using Java.

*   First, load the PowerPoint presentation using [Presentation][23] class.
*   Then, get reference of the document properties in an [IDocumentProperties][24] object using [Presentation.getDocumentProperties()][25] method.
*   Access each custom property using [IDocumentProperties.getCustomPropertyName(int index)][26] method in a loop.

The following code sample shows how to access custom properties in a PowerPoint Presentation.

{{< gist aspose-com-gists 399dd464fe55eed7d9c9a2f088292039 "access-custom-properties.java" >}}

## Modify Custom Properties in PowerPoint Presentations using Java {#Modify-Custom-Properties-in-PowerPoint-Presentations}

The following are the steps to modify the custom properties in a PowerPoint presentation.

*   First, load the PowerPoint presentation using [Presentation][27] class.
*   Then, get reference of the document properties in an [IDocumentProperties][28] object using [Presentation.getDocumentProperties()][29] method.
*   Access each custom property using [IDocumentProperties.getCustomPropertyName(int index)][30] method in a loop.
*   Set the value of a property by specifying its key.
*   Finally, save the presentation using [Presentation.save(String, SaveFormat)][31] method.

The following code sample shows how to modify a custom property in a PowerPoint presentation.

{{< gist aspose-com-gists 399dd464fe55eed7d9c9a2f088292039 "modify-custom-properties.java" >}}

## Get a Free API License {#Get-a-Free-API-License}

You can use Aspose.Slides for Java without evaluation limitations by requesting a [temporary license][32].

## Online Demo

Try Aspose.Slides based [online tool][33] to view and edit document properties in the presentations.

## Conclusion

In this article, you have learned how to access and modify document properties in PowerPoint presentations using Java. We have explicitly covered the manipulation of built-in as well as custom document properties in the presentations. In addition, you can visit the [documentation][34] to explore other features of Aspose.Slides for Java. Also, you can post your queries to our [forum][35].

## See Also

*   [Add Watermark to PowerPoint Slides using Java][36]
*   [Extract Text from PowerPoint Files using Java][37]
*   [Add, Connect, Remove, or Clone PowerPoint Shapes in Java][38]
*   [Convert PowerPoint PPTX/PPT to PNG Images in Java][39]
*   [Generate Thumbnails for PowerPoint PPTX or PPT using Java][40]




[1]: #API-to-Access-Modify-Properties-in-PowerPoint-Files
[2]: #Types-of-Properties-in-PowerPoint-Presentations
[3]: #Access-Built-in-Properties-in-PowerPoint-Presentations
[4]: #Modify-Built-in-Properties-in-PowerPoint-Presentations
[5]: #Add-Custom-Properties-in-PowerPoint-Presentations
[6]: #Access-Custom-Properties-in-PowerPoint-Presentations
[7]: #Modify-Custom-Properties-in-PowerPoint-Presentations
[8]: https://products.aspose.com/slides/java
[9]: https://downloads.aspose.com/slides/java
[10]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation
[11]: https://apireference.aspose.com/slides/java/com.aspose.slides/IDocumentProperties
[12]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation#getDocumentProperties--
[13]: https://apireference.aspose.com/slides/java/com.aspose.slides/IDocumentProperties#getAuthor--
[14]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation
[15]: https://apireference.aspose.com/slides/java/com.aspose.slides/IDocumentProperties
[16]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation#getDocumentProperties--
[17]: https://apireference.aspose.com/slides/java/com.aspose.slides/IDocumentProperties#setAuthor-java.lang.String-
[18]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation#save-java.lang.String-int-
[19]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation
[20]: https://apireference.aspose.com/slides/java/com.aspose.slides/IDocumentProperties
[21]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation#getDocumentProperties--
[22]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation#save-java.lang.String-int-
[23]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation
[24]: https://apireference.aspose.com/slides/java/com.aspose.slides/IDocumentProperties
[25]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation#getDocumentProperties--
[26]: https://apireference.aspose.com/slides/java/com.aspose.slides/IDocumentProperties#getCustomPropertyName-int-
[27]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation
[28]: https://apireference.aspose.com/slides/java/com.aspose.slides/IDocumentProperties
[29]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation#getDocumentProperties--
[30]: https://apireference.aspose.com/slides/java/com.aspose.slides/IDocumentProperties#getCustomPropertyName-int-
[31]: https://apireference.aspose.com/slides/java/com.aspose.slides/Presentation#save-java.lang.String-int-
[32]: https://purchase.aspose.com/temporary-license
[33]: https://products.aspose.app/slides/metadata
[34]: https://docs.aspose.com/slides/java
[35]: https://forum.aspose.com/
[36]: https://blog.aspose.com/2021/06/13/add-watermark-to-powerpoint-using-java/
[37]: https://blog.aspose.com/2021/07/28/extract-text-from-powerpoint-files-using-java/
[38]: https://blog.aspose.com/2021/04/09/add-connect-remove-or-clone-powerpoint-shapes-in-java/
[39]: https://blog.aspose.com/2021/08/01/convert-powerpoint-to-png-in-java/
[40]: https://blog.aspose.com/2021/08/03/generate-thumbnails-for-powerpoint-using-java/






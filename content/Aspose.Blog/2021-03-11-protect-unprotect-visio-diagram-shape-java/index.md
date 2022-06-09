---
title: 'Protect or Unprotect Visio Diagram or Shapes from Changes in Java'
seoTitle: "Java Protect Unprotect Visio Diagram File or Shapes | Avoid Changes"
description: "You can easily protect or unprotect visio diagram file or shapes programmatically using Java language. Avoid changes or modifications in Visio."
date: Thu, 11 Mar 2021 16:13:00 +0000
draft: false
url: /2021/03/11/protect-unprotect-visio-diagram-shape-java/
author: Farhan Raza
summary: 'Microsoft Visio files can contain different pages, masters, shapes, layers, and other objects for creating diagrams. You can easily create, edit, or manipulate Microsoft Visio Diagram Files in your Java applications. Likewise, you can protect or unprotect a Visio file or its shapes to avoid any changes to the data.'
tags: ['protect diagram shape', 'protect visio', 'protect visio from changes java', 'unprotect dagram shape', 'unprotect visio']
categories: ['Aspose.Diagram Product Family']
---



{{< figure align=center src="images/Protect-Unprotect-Visio-Diagram.png" alt="Protect Unprotect Visio Diagram">}}


Microsoft Visio files can contain different pages, shapes, layers, and other objects of diagrams. You can easily create, edit, or manipulate Microsoft Visio Diagram Files with Java. Likewise, you can protect or unprotect a Visio file or its shapes to avoid any changes to the data. Let us go through the following topics for further details:

*   [Protect or Unprotect Visio Diagram files and Shapes – Java API Installation][1]
*   [Protect Visio Diagram File from Changes Programmatically using Java][2]
*   [Unprotect Visio Diagram File using Java][3]
*   [Protect Visio Shapes from Changes with Java][4]
*   [Unprotect Visio Shapes in Java][5]

## Protect or Unprotect Visio Diagram files and Shapes – Java API Installation {#section1}

[Aspose.Diagram for Java][6] API lets you work with Microsoft Visio-related formats like VSDX, VSDM, VSD, and several other [file formats][7]. You do not need to install any third-party application to work with these files. Furthermore, installing the API is simple as you can quickly download its JAR file from the [Downloads][8] section, or with the following details to install it from [Aspose Repository][9]:

### Repository```
 <repositories>

    <repository>

        <id>AsposeJavaAPI</id>

        <name>Aspose Java API</name>

        <url>http://repository.aspose.com/repo/</url>

    </repository>

</repositories>
```

### Dependency```
 <dependencies>

    <dependency>

        <groupId>com.aspose</groupId>

        <artifactId>aspose-diagram</artifactId>

        <version>21.2</version>

        <classifier>jdk16</classifier>

    </dependency>

</dependencies>
```

## Protect Visio Diagram File from Changes using Java {#section2}

Microsoft Visio files like VSD, VSDX, VSTX, or, VDW can contain a lot of information about diagrams, processes, flow charts, and much more. A Visio diagram file may contain Background, Master, Shapes, Styles, etc. and you can protect these contents to avoid any changes. Please follow the following steps to protect a Visio Diagram file:

1.  Load input Visio file with [Diagram][10] class
2.  Protect Background, Shapes, Master shapes, and, Styles of Visio file.
3.  Save protected output diagram file.

The code below shows how to protect a Visio Diagram file using Java:

{{< gist aspose-com-gists fcf8a76ee5c0374c7be5305ff579e8ff "protect-visio-diagram.java" >}}

## Unprotect Visio Diagram File with Java {#section3}

Sometimes you might need to update a protected diagram file. First of all, you need to unprotect such files and then process them further. The below steps elaborate how to unprotect a Visio diagram:

1.  Load the protected input Visio diagram file.
2.  Unprotect Background, Shapes, Master shapes, and, Styles with [DocumentSettings][11] class.
3.  Finally, save unprotected output diagram file.

The following code elaborates how to unprotect a Visio Diagram File with Java:

{{< gist aspose-com-gists fcf8a76ee5c0374c7be5305ff579e8ff "unprotect-visio-diagram.java" >}}

## Protect Visio Shapes from Changes using Java {#section4}

Visio Diagrams consist of different shapes. that are combined to form a diagram or drawing. You can move, rotate, delete, or modify different shapes to achieve results. Furthermore, you can also avoid any changes to Visio shapes by restricting different properties of Shapes. Let us proceed and learn how to protect Visio shapes from any changes, with the steps below:

1.  Load input diagram.
2.  Get page by name.
3.  Get shape by ID.
4.  Set different shape protections.
5.  Save protected output Visio diagram.

The code snippet below explains how to protect Visio shapes from changes with Java:

{{< gist aspose-com-gists fcf8a76ee5c0374c7be5305ff579e8ff "protect-visio-shape.java" >}}

## Unprotect Visio Shapes with Java {#section5}

You may need to unprotect Visio Diagram shapes for changing or updating its contents. The following steps show how to unprotect Visio shapes:

1.  Load input Visio diagram.
2.  Access page by name.
3.  Get shape by ID.
4.  Unprotect Visio shapes with [Bool][12] values.
5.  Finally, save output Visio diagram.

The code below shows how to unprotect Visio Diagram shapes with Java:

{{< gist aspose-com-gists fcf8a76ee5c0374c7be5305ff579e8ff "unprotect-visio-shape.java" >}}

## Conclusion

In this article, you have learned how to protect or unprotect Visio Diagram files. Likewise, you have read how to protect and unprotect shapes from changes using Java language. Moreover, you can find many other features of Aspose.Diagram for Java API by visiting the [Documentation][13]. In case of any concerns, please feel free to contact us via the [Free Support Forum][14].

## See Also

[Convert MS Visio Diagrams to PDF using C#][15]




[1]: #section1
[2]: #section2
[3]: #section3
[4]: #section4
[5]: #section5
[6]: https://products.aspose.com/diagram/java
[7]: https://docs.aspose.com/diagram/java/supported-file-formats/
[8]: https://downloads.aspose.com/diagram/java
[9]: https://repository.aspose.com/webapp/#/artifacts/browse/tree/General/repo/com/aspose/aspose-diagram
[10]: https://apireference.aspose.com/diagram/java/com.aspose.diagram/Diagram
[11]: https://apireference.aspose.com/diagram/java/com.aspose.diagram/DocumentSettings
[12]: https://apireference.aspose.com/diagram/java/com.aspose.diagram/bool
[13]: https://docs.aspose.com/diagram/java/
[14]: https://forum.aspose.com/c/diagram
[15]: https://blog.aspose.com/2021/01/22/Convert-Visio-Diagrams-to-PDF-Csharp/






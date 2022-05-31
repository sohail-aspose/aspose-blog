---
title: 'Insert or Delete Header and Footer in Visio Files in Java'
date: Thu, 10 Mar 2022 19:59:00 +0000
draft: false
url: /2022/03/10/insert-delete-header-footer-visio-java/
author: 'Farhan Raza'
summary: 'Header and footer sections are commonly used to show important information about a document. In some cases, you may need to insert or delete a header or footer in Visio files. This article covers how to **insert or remove header and footer in VSD or VSDX files programmatically in Java**.'
tags: ['Delete Header Footer in Visio Java', 'Insert Header Footer in VSD VSDX Java', 'Remove Header Footer from VSD VSDX']
categories: ['Aspose.Diagram Product Family']
---



{{< figure align=center src="images/Header-Footer-Visio-1-1024x536.jpeg" alt="Header Footer Visio Java">}}


Header and footer sections are commonly used to show important information about a document. In some cases, you may need to insert or delete a header or footer in Visio files. This article covers how to insert or remove header and footer in [VSD](https://docs.fileformat.com/visio/vsd/) or [VSDX](https://docs.fileformat.com/visio/vsdx/) files programmatically in Java.

*   [Insert or Delete Header and Footer in Visio Diagrams - Java API Installation](#section1)
*   [Insert Header and Footer in VSD or VSDX File Programmatically in Java](#section2)
*   [Delete Header and Footer from VSD VSDX Diagram File in Java](#section3)

## Insert or Delete Header and Footer in Visio Diagrams – Java API Installation {#section1}

[Aspose.Diagram for Java](https://products.aspose.com/diagram/java/) API can be used to work with different features of Visio diagram files. You can easily configure it by downloading its JAR files from the [New Releases](https://downloads.aspose.com/diagram/java) section, or access it from [Aspose Repository](https://repository.aspose.com/webapp/#/artifacts/browse/tree/General/repo/com/aspose/aspose-diagram) using the following details in the pom.xml file of your project:

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
        <version>22.4</version>
        <classifier>jdk16</classifier>
    </dependency>
</dependencies>
```

## Insert Header and Footer in VSD or VSDX File Programmatically in Java {#section2}

You can insert or add a header and footer in a VSD or VSDX Visio file by following the steps below:

1.  Create an instance of the [Diagram](https://apireference.aspose.com/diagram/java/com.aspose.diagram/Diagram) class to load the source file.
2.  Set different properties exposed by the [HeaderFooter](https://apireference.aspose.com/diagram/java/com.aspose.diagram/HeaderFooter) class.
3.  Save the output Visio file.

The following code sample shows how to insert the header and footer into a Visio Diagram file in VSD or VSDX format programmatically in Java:



The screenshot below is showing a sample file after inserting the header and footer with the above code snippet:



{{< figure align=center src="images/Header-Footer-Preview-1.jpeg" alt="Header Footer VSD VSDX Java">}}


## Delete Header and Footer from VSD VSDX Diagram File in Java {#section3}

You can delete or remove the header and footer in a VSD or VSDX Diagram file with the following steps:

1.  Initialize an object of the [Diagram](https://apireference.aspose.com/diagram/java/com.aspose.diagram/Diagram) class to load the input Visio file.
2.  Remove the header and footer then save the output VSD/VSDX Diagram.

The following code snippet shows how to delete the header and footer from a VSD VSDX drawing programmatically in Java:



## Get a Free License

You can evaluate the API without any limitations by getting a [free temporary license](https://purchase.aspose.com/temporary-license).

## Conclusion

In this article, you have learned how to insert or delete header and footer from Visio diagram files in VSD or VSDX format programmatically in Java. However, you can learn many other features of the API by visiting the [documentation](https://docs.aspose.com/diagram/java/). Please contact us at the [forum](https://forum.aspose.com/c/diagram) in case of any concerns or ambiguity.

## See Also

[Convert Visio VSD or VSDX File to XAML in Java](https://blog.aspose.com/2022/02/28/convert-visio-to-xaml-java/)





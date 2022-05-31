---
title: 'Insert Text or Image in XPS Programmatically in Java'
date: Tue, 15 Mar 2022 08:46:00 +0000
draft: false
url: /2022/03/15/insert-text-image-xps-java/
author: 'Farhan Raza'
summary: 'XPS files are based on XML paper specifications which are used to save information about the appearance, layout, and printing. You can easily **insert any text or image into an XPS file programmatically in Java.**'
tags: ['Add Text in XPS Java', 'Add Unicode Text in XPS Java', 'Insert Image in XPS Java', 'Insert Text in XPS Java']
categories: ['Aspose.Page Product Family']
---



{{< figure align=center src="images/Image-Text-XPS-1-1024x536.jpg" alt="Text Image XPS Java">}}


[XPS](https://docs.fileformat.com/page-description-language/xps/) files are based on XML paper specifications which are used to save information about the appearance, layout, and printing. You can easily insert any text or image into an XPS file programmatically in Java.

*   [Add Text or Image in an XPS Document – Java API Installation](#section0)
*   [Insert Text in XPS File using Java](#section1)
*   [Insert Text in XPS File using Unicode String in Java](#section2)
*   [Add Image in XPS Document using Java](#section3)
*   [Add Tiled Image in XPS File using Java](#section4)

## Insert Text or Image in an XPS Document – Java API Installation {#section0}

You can insert text or image in an XPS file by configuring [Aspose.Page for Java](https://products.aspose.com/page/java) API by downloading its JAR file from the [New Releases](https://downloads.aspose.com/page/java) page or with the following configurations in the pom.xml file of your project:

### Repository```
 <repositories>
     <repository>
         <id>snapshots</id>
         <name>repo</name>
         <url>http://repository.aspose.com/repo/</url>
     </repository>
</repositories>
```

### Dependency```
 <dependencies>
    <dependency>
        <groupId>com.aspose</groupId>
        <artifactId>aspose-page</artifactId>
        <version>22.2</version>
    </dependency>
</dependencies>
```

## Insert Text in XPS File using Java {#section1}

You need to follow the steps below in order to insert text in an XPS file:

1.  Create an instance of the [XPSDocument](https://apireference.aspose.com/page/java/com.aspose.xps/XpsDocument) class.
2.  Create a brush of any color and add the glyph.
3.  Save the output XPS document.

The code sample below elaborates on how to insert text in an XPS file programmatically in Java:



## Insert Text in XPS File using Unicode String in Java {#section2}

You can also insert a Unicode string in the XPS document by following the steps below:

1.  Initialize an object of the [XPSDocument](https://apireference.aspose.com/page/java/com.aspose.xps/XpsDocument) class.
2.  Add the Unicode string while specifying the font and size.
3.  Write the output XPS file.

The code sample below shows how to insert text with Unicode string into an XPS file using Java:



## Add Image in XPS Document using Java {#section3}

You can add an image in the XPS document with the following steps:

1.  Initialize a new XPS Document.
2.  Load the source Image.
3.  Create an [ImageBrush](https://apireference.aspose.com/page/java/com.aspose.xps/XpsImageBrush) class object.
4.  Save the output XPS file.

The following code sample demonstrates how to add an image in an XPS document with Java:



## Add Tiled Image in XPS File using Java {#section4}

You can add a tiled image in an XPS file using Java by following the steps below:

1.  Create a new XPS Document.
2.  Add a filled rectangle with [ImageBrush](https://apireference.aspose.com/page/java/com.aspose.xps/XpsImageBrush) and add the tiled image.
3.  Save the output XPS document.

The code sample below explains how to add a tiled image in an XPS file using Java:



## Conclusion

In this article, you have explored how to add text or an image in an XPS file programmatically in Java. It explains inserting a simple string or a Unicode-based string. It also covers adding an image in a tiled manner based on your application requirements. You may like to visit the [documentation](https://docs.aspose.com/page/java/) space to check out several other features offered by the API. In case you need any assistance, please feel free to write to us at the [forum](https://forum.aspose.com/c/page).

## See Also

[Convert XPS or OXPS to Word Document using Java](https://blog.aspose.com/2022/01/07/convert-xps-oxps-word-java/)





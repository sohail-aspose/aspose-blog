---
title: 'Insert or Extract Image from a OneNote File in Java'
seoTitle: "Insert or Extract Image from a OneNote file Programmatically in Java"
description: "You can insert or extract image in OneNote files programmatically in Java. Logos, signatures, drawings can be added as image in .one file."
date: Sun, 07 Nov 2021 02:36:00 +0000
draft: false
url: /2021/11/07/insert-extract-image-onenote-java/
author: Farhan Raza
summary: 'OneNote files can include visual information like images or drawings, in addition to text contents. In certain scenarios, you may need to insert or extract images in a OneNote document. This article explains how you can insert or extract images in a .one file using Java.'
tags: ['Extract Image from OneNote in Java', 'Extract image from OneNote', 'Insert Extract Image in OneNote', 'Insert Image in OneNote', 'Insert Image in OneNote with Java']
categories: ['Aspose.Note Product Family']
---



{{< figure align=center src="images/Insert-Extract-Image-OneNote.jpg" alt="Insert Extract image onenote">}}


OneNote files can include visual information like images or drawings in addition to text contents. In certain scenarios, you may need to insert or extract images in a OneNote document. This article explains how you can insert or extract images in a [.one][1] file in Java.

*   [Insert or Extract Image from OneNote .one File – Java API Installation][2]
*   [Insert Image in OneNote .one File in Java][3]
*   [Extract Images from OneNote .one File in Java][4]

## Insert or Extract Image in OneNote .one File – Java API Installation {#section1}

You can insert or extract images in a OneNote file using [Aspose.Note for Java][5] API. You can download its JAR file from the [New Releases][6] section. Likewise, you can configure it with the following Maven specifications in the pom.xml file:

### Repository```
 <repositories>
    <repository>
        <id>AsposeJavaAPI</id>
        <name>Aspose Java API</name>
        <url>https://repository.aspose.com/repo/</url>
    </repository>
</repositories>
```

### Dependency```
 <dependencies>
    <dependency>
        <groupId>com.aspose</groupId>
        <artifactId>aspose-note</artifactId>
        <version>21.9</version>
        <classifier>jdk17</classifier>        
    </dependency>
</dependencies>
```

## Insert Image in OneNote .one File in Java {#section2}

You can insert an image in a OneNote .one file by following these steps:

1.  Firstly, initialize [LoadOptions][7] class object.
2.  Load the input OneNote file with the [Document][8] class.
3.  Get the first page of the document and load input image.
4.  Set image location and alignment.
5.  Add the image to the page with [appendChildLast][9] method.
6.  Finally, save the output OneNote file.

The following code snippet shows how to insert an image in OneNote .one file in Java:

{{< gist aspose-com-gists a203abbe23ea73343ae424e0c6ebe423 "InsertImageOneNote.java" >}}

## Extract Images from OneNote .one File in Java {#section3}

You can extract images from a OneNote file with the below steps:

1.  Load the input OneNote file with the [Document][10] class.
2.  Get all images using [getChildNodes][11] method.
3.  Finally, traverse the list and save output images.

The code snippet below demonstrates how to extract images from a OneNote file in Java:

{{< gist aspose-com-gists a203abbe23ea73343ae424e0c6ebe423 "ExtractImageOneNote.java" >}}

## Get Free API License

You can test all the features of the API without any limitations by requesting a [free evaluation license][12].

## Conclusion

In this article, you have explored how to insert or extract images from a OneNote .one file in Java. Please visit the [documentation][13] to check several other features of the API. Moreover, please feel free to reach us out at the [free support forum][14] in case of any queries.

## See Also

[Create OneNote Files in Java][15]




[1]: https://docs.fileformat.com/note-taking/one/
[2]: #section1
[3]: #section2
[4]: #section3
[5]: https://products.aspose.com/note/java/
[6]: https://downloads.aspose.com/note/java
[7]: https://apireference.aspose.com/note/java/com.aspose.note/LoadOptions
[8]: https://apireference.aspose.com/note/java/com.aspose.note/Document
[9]: https://apireference.aspose.com/note/java/com.aspose.note/CompositeNode#appendChildLast-T1-
[10]: https://apireference.aspose.com/note/java/com.aspose.note/Document
[11]: https://apireference.aspose.com/note/java/com.aspose.note/CompositeNode#getChildNodes-java.lang.Class-
[12]: https://purchase.aspose.com/temporary-license
[13]: https://docs.aspose.com/note/java/
[14]: https://forum.aspose.com/
[15]: https://blog.aspose.com/2021/08/03/create-onenote-files-programmatically-using-java/





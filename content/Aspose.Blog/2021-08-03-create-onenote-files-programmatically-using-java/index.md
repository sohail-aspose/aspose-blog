---
title: 'Create OneNote Files Programmatically using Java'
seoTitle: "Create OneNote .One Files Programmatically using Java"
description: "You can create OneNote .one files programmatically using Java. Add simple or formatted rich text and insert pages or tags in OneNote files."
date: Tue, 03 Aug 2021 15:41:39 +0000
draft: false
url: /2021/08/03/create-onenote-files-programmatically-using-java/
author: Farhan Raza
summary: 'OneNote files are used to keep the information organized as digital notes. You can create OneNote files from scratch using Java. In this article, you will explore different features like adding text, pages, or tags in .One files.'
tags: ['Create OneNote documents using Java']
categories: ['Aspose.Note Product Family']
---



{{< figure align=center src="images/Create-OneNote.jpg" alt="Create OneNote file">}}


OneNote files are used to keep the information organized as digital notes. You can create OneNote files from scratch using Java. In this article, you will explore different features like adding text, pages, or tags in .One files:

*   [OneNote Document Creator – Java API Installation][1]
*   [Create OneNote Document with Simple Rich Text Programmatically using Java][2]
*   [Create OneNote Document with Formatted Rich Text Programmatically using Java][3]
*   [Insert Pages in OneNote File Programmatically with Java][4]
*   [Add Tags in OneNote Files in Java][5]

## OneNote Document Creator – Java API Installation {#section1}

[Aspose.Note for Java][6] API supports creating, editing, or manipulating OneNote files. You can easily make some API calls and the output file is generated as per your requirements. Please download the JAR file from the [Downloads][7] section, or use the following configuration in your Maven-based projects:

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
        <version>21.7</version>
        <classifier>jdk17</classifier>        
    </dependency>
</dependencies>
```

## Create OneNote Document with Simple Rich Text Programmatically using Java {#section2}

You can create a OneNote document with simple rich text with the following steps:

1.  Create an object of the [Document][8] class.
2.  Initialize [Page][9] and [Outline][10] class objects.
3.  Add [RichText][11] node.
4.  Save output OneNote document.

The following code shows how to create a OneNote document with simple rich text using Java:

{{< gist aspose-com-gists 9105f6e7434342a8499dd10ec4345f72 "Create-OneNote-Simple-RichText.java" >}}

## Create OneNote Document with Formatted Rich Text Programmatically using Java {#section3}

Moving another step further, you can learn how to create a OneNote file with formatted rich text using Java:

1.  Create an object of the [Document][12] class.
2.  Initialize [Page][13] and [TextStyle][14] class objects.
3.  Format and add [RichText][15] node.
4.   Save output OneNote file.

The code below explains how to create a OneNote document with formatted rich text using Java:

{{< gist aspose-com-gists 9105f6e7434342a8499dd10ec4345f72 "Create-OneNote-Formatted-RichText.java" >}}

## Insert Pages in OneNote File Programmatically with Java {#section4}

You can insert roots as well as sub-level pages in the OneNote document with the below steps:

1.  Initialize an instance of the [Document][16] class.
2.  Insert 3 pages while specifying their levels.
3.  Add nodes to the pages and insert pages in the OneNote document.
4.  Finally, save output OneNote document.

The code below elaborates how to insert pages in the OneNote file with Java:

{{< gist aspose-com-gists 9105f6e7434342a8499dd10ec4345f72 "Insert-Pages-OneNote.java" >}}

## Add Tags in OneNote Files in Java {#section5}

You can tag the contents in OneNote files. The following steps explain how to add a text node with a tag:

1.  Create an object of the [Document][17] class.
2.  Add [RichText][18] and Initialize [NoteTag][19] class object.
3.  Save output OneNote file.

The following code shows how to add tags in the OneNote file using Java:

{{< gist aspose-com-gists 9105f6e7434342a8499dd10ec4345f72 "Add-Tags-OneNote.java" >}}

## Get Free API License

You can request a [Free Temporary License][20] for evaluating the API in its full capacity.

## Conclusion

In this article, you have learned how to create OneNote files from scratch programmatically using Java. It covers all the details for inserting pages, adding rich text with a simple or formatted appearance in .One file. Moreover, you can check several other features by visiting the [Documentation][21]. Furthermore, please feel free to contact us at the [Free Support Forum][22] for any inquiries.

## See Also

[Convert OneNote File to Image Programmatically using Java][23]




[1]: #section1
[2]: #section2
[3]: #section3
[4]: #section4
[5]: #section5
[6]: https://products.aspose.com/note/java/
[7]: https://releases.aspose.com/
[8]: https://apireference.aspose.com/note/java/com.aspose.note/Document
[9]: https://apireference.aspose.com/note/java/com.aspose.note/Page
[10]: https://apireference.aspose.com/note/java/com.aspose.note/Outline
[11]: https://apireference.aspose.com/note/java/com.aspose.note/RichText
[12]: https://apireference.aspose.com/note/java/com.aspose.note/Document
[13]: https://apireference.aspose.com/note/java/com.aspose.note/Page
[14]: https://apireference.aspose.com/note/java/com.aspose.note/TextStyle
[15]: https://apireference.aspose.com/note/java/com.aspose.note/RichText
[16]: https://apireference.aspose.com/note/java/com.aspose.note/Document
[17]: https://apireference.aspose.com/note/java/com.aspose.note/Document
[18]: https://apireference.aspose.com/note/java/com.aspose.note/RichText
[19]: https://apireference.aspose.com/note/java/com.aspose.note/NoteTag
[20]: https://purchase.aspose.com/temporary-license
[21]: https://docs.aspose.com/note/java/
[22]: https://forum.aspose.com/c/note
[23]: https://blog.aspose.com/2021/06/14/convert-onenote-file-to-image-programmatically-using-java/






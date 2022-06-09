---
title: 'Find and Replace Text in OneNote (.ONE) File in Java'
seoTitle: "Find and Replace Text in OneNote (.ONE) File in Java"
description: "OneNote files can be used to organize different tasks. For example, planning your trips, some checklist, or brainstorming. Moreover, you may need to find or replace text in a OneNote Document sometimes."
date: Wed, 03 Feb 2021 10:38:00 +0000
draft: false
url: /2021/02/03/find-and-replace-text-in-onenote-one-file-in-java/
author: Farhan Raza
summary: 'OneNote files can be used to organize different tasks. For example, planning your trips, some checklist, or brainstorming. Moreover, you may need to find or replace text in a OneNote Document sometimes.'
tags: ['Find and replace text in one note file', 'search and replace in onenote']
categories: ['Aspose.Note Product Family']
---



{{< figure align=center src="images/Find-Replace-Text-OneNote.png" alt="Find Replace Text OneNote">}}


OneNote files can be used to organize different tasks. For example, planning your trips, some checklist, or brainstorming. Moreover, you may need to find or replace text in a OneNote Document sometimes. Let us explore the following topics:

*   [Search and Replace Text in OneNote File – Java API Installation][1]
*   [Find and Replace Text on Specific Page of OneNote File in Java][2]
*   [Find and Replace Text on All Pages of OneNote in Java][3]

## Search and Replace Text in OneNote File – Java API Installation {#section1}

[Aspose.Note for Java][4] API lets you create, convert, or manipulate .one files. You can quickly configure the API by downloading the JAR file from the official [Downloads][5] section, or with the following configurations in the pom.xml file of your project. It will easily download the files from [Aspose Repository][6].

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
        <version>21.1</version>
        <classifier>jdk17</classifier>        
    </dependency>
</dependencies>
```

## Find and Replace Text on Specific Page of OneNote File in Java {#section2}

You may use a OneNote file to keep notes, reminders, pictures etc. For textual contents, you can find and replace text in OneNote file with few simple steps as listed below:

1.  Load input OneNote file
2.  Get the list of page nodes
3.  Traverse all nodes to find text
4.  Replace text
5.  Save output .one file

The following code shows how to find and replace text on a specific page of .one file programmatically in Java:

{{< gist aspose-com-gists ff3caac59f4abf615a02c6efc71771a1 "Replace-Text-Note-Specific.java" >}}

## Find and Replace Text on All Pages of OneNote File in Java {#section3}

Sometimes there are several occurrences of text across multiple pages of a OneNote file. In order to find and replace text on all pages, you need to follow the steps below:

1.  Load input .one file
2.  Get all [RichText][7] nodes
3.  Traverse all nodes and compare text
4.  Replace the text
5.  Save output file

The code snippet explains how to find and replace text on all pages of OneNote file programmatically using Java:

{{< gist aspose-com-gists ff3caac59f4abf615a02c6efc71771a1 "Replace-Text-Note-AllPages.java" >}}

## Conclusion

In this article, we have explored how to work with OneNote files. You have learned how to find and replace text in OneNote files programmatically using Java language. Likewise, several other features are supported by the API. You can learn further features by taking a look at [API Documentation][8]. We would love to hear your feedback at [Free Support Forum][9]. Cheers!

## See Also

[Create OneNote (.ONE) Documents Programmatically in C#][10]




[1]: #section1
[2]: #section2
[3]: #section3
[4]: https://products.aspose.com/note/java
[5]: https://releases.aspose.com/
[6]: https://repository.aspose.com/repo/com/aspose/aspose-note/
[7]: https://apireference.aspose.com/note/java/com.aspose.note/class-use/RichText
[8]: https://docs.aspose.com/note/java/
[9]: https://forum.aspose.com/c/note
[10]: https://blog.aspose.com/2020/05/08/create-onenote-files-add-images-tables-tags-to-onenote-file-using-csharp/






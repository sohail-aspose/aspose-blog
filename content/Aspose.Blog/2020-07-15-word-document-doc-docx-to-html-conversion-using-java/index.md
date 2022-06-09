---
title: 'Word Document (DOC/DOCX) to HTML Conversion using Java'
seoTitle: ""
description: ""
date: Wed, 15 Jul 2020 21:32:44 +0000
draft: false
url: /2020/07/15/word-document-doc-docx-to-html-conversion-using-java/
author: Farhan Raza
summary: ''
tags: ['docx to html', 'docx to html5', 'docx to mhtml', 'word to html', 'word to html5', 'word to mhtml']
categories: ['Aspose.Words Product Family']
---

Microsoft Word file formats DOC/DOCX are famous because the word processor supports a variety of features to organize and explain information. Likewise, HTML file format is helpful to show information in web applications. In this article, you will be learning Word files (DOC/DOCX) to HTML or HTML5 conversion using Java. Following are the use cases that you will be exploring here:

*   [Convert Word (DOC/DOCX) to HTML using Java][1]
*   [Convert DOCX to HTML5 using Java][2]
*   [Convert Password-Protected Word file to HTML using Java][3]
*   [Convert Word to MHTML using Java][4]

## Java DOCX to HTML or HTML5 Converter - Installation

First things first, you can easily configure Aspose.Words for Java API in your applications. You can download the JAR file from new [Releases section][5] where all APIs are updated almost every month. Moreover, all of the Java APIs, offered by Aspose, are hosted over the Maven repository. Likewise, Aspose.Words for Java dependency can be defined in your Maven project with the following configurations:

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
        <artifactId>aspose-words</artifactId>
        <version>20.6</version>
        <classifier>jdk17</classifier>
    </dependency>
    <dependency>
        <groupId>com.aspose</groupId>
        <artifactId>aspose-words</artifactId>
        <version>20.6</version>
        <classifier>javadoc</classifier>
    </dependency>
</dependencies>
```

Now we are all set for DOCX to HTML conversion in a Java application.

## Convert Word (DOC/DOCX) to HTML using Java {#section1}

You can convert Word to HTML by following the steps below:

1.  Load source Word file with DOC or DOCX extension
2.  Save the file as output HTML

The code sample below shows how to convert DOCX to HTML using Java:

{{< gist aspose-cloud 7b6fd21096e2fbbda3548cdd8c565b96 "WordToHTML.java" >}}

**Input DOCX file Preview**



{{< figure align=center src="images/Word-to-HTML-Java.png" alt="Word to HTML in Java">}}


**Output HTML file Preview**



{{< figure align=center src="images/DOCX-to-HTML-Java.png" alt="DOCX to HTML in Java">}}


So you can notice the high fidelity of document rendering with these screenshots. The API is capable of converting text, images, tables, and much more.

## Convert DOCX to HTML5 using Java {#section2}

HTML5 is the latest version of HTML. We have noted repeated requests for supporting [HTML5][6] in Aspose.Words API. Therefore, DOCX to HTML5 conversion is supported and you can convert files by following steps:

1.  Firstly, load input DOCX file
2.  Set HtmlSaveOptions while setting SaveFormat
3.  Set enumeration value of HtmlVersion.HTML\_5
4.  Save output file

The code snippet below shows how to convert DOCX to HTML5 in Java:

{{< gist aspose-cloud 7b6fd21096e2fbbda3548cdd8c565b96 "DOCXtoHTML5.java" >}}

## Convert Password-Protected Word file to HTML using Java {#section3}

DOC or DOCX files are sometimes password protected or encrypted using a password. You can also convert such files to HTML. However, you will need the password while loading the word file. You can follow the steps below for DOCX to HTML conversion:

1.  Firstly, initialize an object of LoadOptions class
2.  Set the password
3.  Load the encrypted DOCX file
4.  Convert DOCX to HTML

Likewise, the following code sample shows how to convert password protected DOCX file to HTML using Java:

{{< gist aspose-cloud 7b6fd21096e2fbbda3548cdd8c565b96 "Password-WordToHTML.java" >}}

## Convert Word to MHTML using Java {#section4}

MHTML files are single files that contain embedded contents and media. You can convert word files (DOC/DOCX) to MHTML with following steps:

1.  Load input DOCX file
2.  Save output MHTML file using SaveFormat.MHTML

The code snippet below is based on this steps. Therefore, it shows how to convert DOCX to MHML with Java:

{{< gist aspose-cloud 7b6fd21096e2fbbda3548cdd8c565b96 "WordtoMHTML.java" >}}

## Conclusion

Concludingly, we have learned conversion of word documents without needing Microsoft Word. For example, DOCX to HTML, MHTML, or HTML5 as per your requirements. Likewise, we have observed with screenshots that the conversion is performed with high fidelity and compatibility between the file formats. So you can try the API in your own Java environment. However, if you face any problem while setting up or testing the API then you can get in touch with us via [Free Support Forums][7]!

## See Also

[Mail Merge in Word Documents][8]




[1]: #section1
[2]: #section2
[3]: #section3
[4]: #section4
[5]: https://releases.aspose.com/
[6]: https://en.wikipedia.org/wiki/HTML5
[7]: https://forum.aspose.com/c/words
[8]: https://blog.aspose.com/2020/07/14/mail-merge-in-word-documents-using-csharp-or-vb.net/






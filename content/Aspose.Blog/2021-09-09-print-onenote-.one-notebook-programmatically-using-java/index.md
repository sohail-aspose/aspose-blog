---
title: 'Print OneNote .one Notebook Programmatically using Java'
seoTitle: "Print OneNote Notebook .one File or a Page Programmatically in Java"
description: "You can print the Microsoft OneNote Notebook file in .one format easily or with advanced options. Print the notes to Virtual Printer in Java."
date: Thu, 09 Sep 2021 08:43:00 +0000
draft: false
url: /2021/09/09/print-onenote-.one-notebook-programmatically-using-java/
author: Farhan Raza
summary: 'OneNote notebooks are commonly used to keep important notes. You may need to print your notes on paper for some reason. In this article, you will learn how to print the OneNote Notebook files in your Java applications.'
tags: ['Print .one file', 'Print OneNote file', 'Print notebook in Java']
categories: ['Aspose.Note Product Family']
---



{{< figure align=center src="images/OneNote.png" alt="Print OneNote .one Notebook">}}


OneNote notebooks are commonly used to keep important notes. You may need to print your notes on paper for some reason. In this article, you will learn how to print the OneNote Notebook files in your Java applications.

*   [OneNote Notebook Printer – Java API Installation][1]
*   [Print OneNote Notebook .one File Programmatically using Java][2]
*   [Print OneNote Notebook .one File with Advanced Options in Java][3]
*   [Printing OneNote Notebook to a Virtual Printer with Java][4]

## OneNote Notebook Printer – Java API Installation {#section1}

[Aspose.Note for Java][5] API supports creating and manipulating .one files programmatically. You only need to make simple method calls and the API takes care of minor details. So please configure the API by downloading the JAR file from the [Downloads][6] section, or use the below details in the pom.exe file of your Maven-based project:

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

## Print OneNote Notebook .one File Programmatically using Java {#section2}

Considering the basic case of printing .one files, you can print a OneNote file with a couple of lines of code. You need to follow the steps below for printing a .one format file:

1.  Load input OneNote file with the [Document][7] constructor.
2.  Print the OneNote document with the [print][8] method.

The following code shows how to print the OneNote .one Notebook programmatically in Java:

{{< gist aspose-com-gists bb076338de32dba29b0a50e9a6b64b17 "Print-OneNote.java" >}}

## Print OneNote Notebook .one File with Advanced Options in Java {#section3}

Moving another step further, you can set advanced options to customize the printing of the OneNote Notebook .one file, as per your requirements. Please follow the steps below for printing .one format file with advanced options:

1.  Firstly, load the input OneNote file with the [Document][9] class.
2.  Specify page range and printer name.
3.  Finally, call the [print()][10] method to print the file.

The code below explains how to print OneNote file programmatically with Java:

{{< gist aspose-com-gists bb076338de32dba29b0a50e9a6b64b17 "Print-OneNote-Options.java" >}}

## Print OneNote .one File to a Virtual Printer with Java {#section4}

A virtual printer is an application that replicates a software interface like a physical printer. You can configure printing with a virtual printer with the below steps:

1.  Load input OneNote file.
2.  Specify the virtual printer and properties.
3.  Set printer settings with [DocumentPrintAttributeSet][11].
4.  Finally, print the OneNote file to virtual printer.

The following code demonstrates how to print OneNote .one file programmatically to a Virtual Printer using Java:

{{< gist aspose-com-gists bb076338de32dba29b0a50e9a6b64b17 "Print-OneNote-Virtual.java" >}}

## Get Free Evaluation License

You can request a [Free Temporary License][12] for evaluating the API without any limitations.

## Conclusion

In conclusion, you have learned how to print a OneNote Notebook .one file programmatically in your Java applications. You have explored different use cases that vary based on different requirements. Furthermore, you can visit the API [Documentation][13] to explore several other features of the API. In case you want to discuss any of your concerns or requirements, please feel free to reach out at the [Free Support Forum][14].

## See Also

[Convert OneNote File to Image Programmatically using Java][15]




[1]: #section1
[2]: #section2
[3]: #section3
[4]: #section4
[5]: https://products.aspose.com/note/java/
[6]: https://downloads.aspose.com/note/java
[7]: https://apireference.aspose.com/note/java/com.aspose.note/Document
[8]: https://apireference.aspose.com/note/java/com.aspose.note/Document#print--
[9]: https://apireference.aspose.com/note/java/com.aspose.note/Document
[10]: https://apireference.aspose.com/note/java/com.aspose.note/Document#print--
[11]: https://apireference.aspose.com/note/java/com.aspose.note/DocumentPrintAttributeSet
[12]: https://purchase.aspose.com/temporary-license
[13]: https://docs.aspose.com/note/java/
[14]: https://forum.aspose.com/c/note
[15]: https://blog.aspose.com/2021/06/14/convert-onenote-file-to-image-programmatically-using-java/





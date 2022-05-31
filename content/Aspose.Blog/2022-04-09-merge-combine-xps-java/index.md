---
title: 'Merge XPS Files Programmatically in Java'
date: Sat, 09 Apr 2022 08:12:00 +0000
draft: false
url: /2022/04/09/merge-combine-xps-java/
author: 'Farhan Raza'
summary: 'XPS format consists of XML markup which explains visual representation or rendering rules for a document. In certain cases, you may need to merge or combine many XPS documents. For such use cases, this article covers how to **merge XPS files programmatically in Java.**'
tags: ['Combine XPS in Java', 'Merge XPS Files in Java', 'Merge XPS in Java']
categories: ['Aspose.Page Product Family']
---



{{< figure align=center src="images/Merge-XPS-1-1024x536.jpg" alt="Merge XPS Java">}}


[XPS](https://docs.fileformat.com/page-description-language/xps/) format consists of XML markup which explains visual representation or rendering rules for a document. In certain cases, you may need to merge or combine many XPS documents. For such use cases, this article covers how to merge XPS files programmatically in Java.

*   [Combine or Merge XPS Files – Java API Installation](#section1)
*   [Merge XPS files Programmatically in Java](#section2)
*   [Merge XPS files with Advanced Options in Java](#section3)

## Combine or Merge XPS files – Java API Installation {#section1}

[Aspose.Page for Java](https://products.aspose.com/page/java) API can be used to work with EPS, XPS, and other popular [file formats](https://docs.aspose.com/page/java/supported-file-formats/). You can configure the API by downloading its JAR files from the [Downloads](https://downloads.aspose.com/page/java) page or paste the following configurations into the pom.xml file of your project:

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
        <version>22.4</version>
    </dependency>
</dependencies>
```

## Merge XPS files Programmatically in Java {#section2}

You can merge different XPS documents into one file with the following steps:

1.  Load an input XPS file to combine other XPS documents.
2.  Initialize a rendering device to write the output file.
3.  Declare and initialize an array to hold the input XPS documents.
4.  Merge the XPS documents and write the output file in PDF format.

The code snippet below elaborates on how to merge different XPS files into one and export the output file as a PDF document programmatically in Java:

\[gist id="26d821b928f8ca3cac014e4a5c80d714" file="Merge XPS.java"\]

## Merge XPS files with Advanced Options in Java {#section3}

You can enhance the XPS merging process by configuring several properties. For example, PDF passwords, permissions, privileges, or compression can be controlled based on your requirements. Please follow the steps below in order to merge XPS files with advanced options:

1.  Load the input XPS file for combining files.
2.  Create an object of the [PdfSaveOptions](https://apireference.aspose.com/page/java/com.aspose.xps.rendering/PdfSaveOptions) class.
3.  Make a rendering device and initialize a string array to store file paths.
4.  Merge multiple input XPS files and save the output as PDF.

The code sample below explains how to merge XPS files with advanced options in Java:

\[gist id="26d821b928f8ca3cac014e4a5c80d714" file="Merge XPS Advanced.java"\]

## Get Free Temporary License

You can get a [free temporary license](https://purchase.aspose.com/temporary-license) in order to test the API at its full capacity.

## Online Demo

Please try the [XPS Merging](https://products.aspose.app/page/merger/xps) web app to check the XPS file combining capabilities.

## Conclusion

In this article, you have learned how to merge many XPS files together programmatically in Java. However, if you want to discuss your requirements or concerns, please feel free to reach out to us at the [forum](https://forum.aspose.com/c/svg/42).

## See Also

[Convert a Postscript PS or EPS file to PDF using Java](https://blog.aspose.com/2021/06/08/convert-postscript-ps-eps-to-pdf-java/)




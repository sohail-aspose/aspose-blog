---
title: 'Convert XML to MPP or Vice Versa Programmatically in Java'
seoTitle: "Java Convert XML to MPP or Import Microsoft Project Data File as XML"
description: "You can convert or import XML to MPP as well as Microsoft Project Files to XML programmatically using Java. Export or change XML MPP file."
date: Tue, 09 Mar 2021 09:12:00 +0000
draft: false
url: /2021/03/09/convert-import-xml-mpp-java/
author: Farhan Raza
summary: '[**XML**][1] is abbreviated for Extensible Markup Language. It’s like some information stored between different tags for storing and transmitting purposes. On the other hand, we use the [**MPP**][2] file format for Project Management. You can convert XML to MPP as well as MPP to XML format files using Java language. It is helpful when you want to import or export between XML and MPP files as per your requirements.'
tags: ['Export mpp to xml', 'convert xml to mpp', 'import xml to mpp', 'mpp to xml', 'xml to mpp']
categories: ['Aspose.Tasks Product Family']
---



{{< figure align=center src="images/Convert-XML-MPP.png" alt="convert xml mpp java">}}


[XML][3] is abbreviated for Extensible Markup Language. It is like some information stored between different tags for storing and transmitting purposes. On the other hand, we use the [MPP][4] file format for Project Management. You can convert XML to MPP as well as MPP to XML format files using Java language. It is helpful when you want to import or export between XML and MPP files as per your requirements. Let us proceed to the following sections for further details:

*   [XML to MPP or Microsoft Project Data File to XML Conversion – Java API Installation][5]
*   [Convert or Import XML to MPP File Programmatically using Java][6]
*   [Convert MPP to XML File Programmatically in Java][7]

## XML to MPP or Microsoft Project File to XML Conversion – Java API Installation {#section1}

[Aspose.Tasks for Java][8] API support MPP, XML, MPT, HTML, and several [other file formats][9]. You can convert or import XML file to Microsoft Project file, as well as from MPP format to XML file in your Java applications. Configuring the API is quite simple as you can quickly download the JAR file from the [Downloads][10] section. Otherwise, you can specify the below [Repository][11] details in the pom.xml file of your Maven-based Java applications:

### Repository```
<repository>
    <id>AsposeJavaAPI</id>
    <name>Aspose Java API</name>
    <url>http://repository.aspose.com/repo/</url>
</repository>
```

### Dependency```
<dependency>
    <groupId>com.aspose</groupId>
    <artifactId>aspose-tasks</artifactId>
    <version>21.2</version>
    <classifier>jdk18</classifier>
</dependency>
```

## Convert or Import XML to MPP File Programmatically using Java {#section2}

Please follow the steps below for converting XML to MPP file:

1.  Load input XML file.
2.  Then load the template MPP file.
3.  Call [copyTo()][12] method of Project class.
4.  Finally, save output MPP (Microsoft Project File).

The following code snippet shows how to convert or import the XML file to MPP programmatically using Java:

{{< gist aspose-com-gists a58d91fc3940675de3c3895f0f1c1537 "convert-xml-to-mpp.java" >}}

## Convert MPP to XML File Programmatically in Java {#section3}

Microsoft Project file, MPP, stores information about project management. MPP to XML conversion is helpful when some information is to be utilized by different systems for some specific purpose. Please follow the steps below for converting MPP to XML format:

1.  Load input MPP file using Project class.
2.  Save output XML file with [SaveFileFormat][13] enumeration.

The code snippet below explains how to convert MPP to XMP programmatically with Java:

{{< gist aspose-com-gists a58d91fc3940675de3c3895f0f1c1537 "convert-mpp-to-xml.java" >}}

## Conclusion

In conclusion, you have learned the conversion of XML to MPP and MPP to XML file format. Moreover, we have explored this topic with sample code and step by step guide with all the details. Furthermore, you may visit API [Documentation][14] to explore other features. Feel free to contact us via the [Free Support Forum][15], in case of any query. We look forward to helping you out with your concerns!

## See Also

[Create MS Project Files Programmatically using Java][16]




[1]: https://docs.fileformat.com/web/xml/
[2]: https://docs.fileformat.com/project-management/mpp/
[3]: https://docs.fileformat.com/web/xml/
[4]: https://docs.fileformat.com/project-management/mpp/
[5]: #section1
[6]: #section2
[7]: #section3
[8]: https://products.aspose.com/tasks/java
[9]: https://docs.aspose.com/tasks/java/supported-file-formats/
[10]: https://downloads.aspose.com/tasks/java
[11]: https://repository.aspose.com/webapp/#/artifacts/browse/tree/General/repo/com/aspose/aspose-tasks
[12]: https://apireference.aspose.com/tasks/java/com.aspose.tasks/Project#copyTo-com.aspose.tasks.Project-
[13]: https://apireference.aspose.com/tasks/java/com.aspose.tasks/savefileformat
[14]: https://docs.aspose.com/tasks/java/
[15]: https://forum.aspose.com/c/tasks/15
[16]: https://blog.aspose.com/2021/01/06/create-ms-project-files-programmatically-using-java/






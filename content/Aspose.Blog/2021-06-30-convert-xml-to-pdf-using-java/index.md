---
title: 'Convert XML to PDF using Java'
seoTitle: "Convert XML to PDF using Java | Generate PDF from XML in Java"
description: "Use Java PDF API to convert XML data to PDF using Java. Generate PDF files from XML from within your Java Spring applications."
date: Wed, 30 Jun 2021 10:51:00 +0000
draft: false
url: /2021/06/30/convert-xml-to-pdf-using-java/
author: Usman Aziz
summary: 'In this article, you will learn **how to convert XML to PDF programmatically using Java**. This feature can be useful for generating PDF files dynamically from the XML. Furthermore, the article also provides the complete XML schema that is used to create a PDF document.'
tags: ['Convert XML to PDF in Java', 'Generate PDF from XML in Java', 'Java API for XML to PDF Conversion']
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/XML-to-PDF-1.jpg" alt="XML to PDF">}}


In this article, you will learn **how to convert XML to PDF programmatically using Java**. This feature can be useful for generating PDF files dynamically from the XML. Furthermore, the article also provides the complete XML schema that is used to create a PDF document.

*   [Java API for XML to PDF Conversion][1]
*   [Supported XML Schema for PDF Generation][2]
*   [Convert XML to PDF in Java][3]

## Java XML to PDF Conversion API {#Java-API-for-XML-to-PDF-Conversion}

In order to generate PDF files from XML, we will use [Aspose.PDF for Java][4]. The API is designed to create, process, and convert PDF files dynamically from within the Java applications. You can either [download][5] the API's JAR or install it using the following Maven configurations.

```
<repository>
    <id>AsposeJavaAPI</id>
    <name>Aspose Java API</name>
    <url>https://repository.aspose.com/repo/</url>
</repository>
```
```
<dependency>
    <groupId>com.aspose</groupId>
    <artifactId>aspose-pdf</artifactId>
    <version>21.6</version>
</dependency>
```

## Support Schema for XML to PDF {#Supported-XML-Schema-for-PDF-Generation}

Aspose.PDF for Java provides its XML schema to define the structure of the PDF document. You can find the complete XML schema [here][6].

## Convert XML to PDF in Java {#Convert-XML-to-PDF-in-Java}

Let's check out how to convert a given XML to PDF using Aspsoe.PDF for Java. Most often, you will have the XML document containing the application data. In this case, you will first transform it to the Aspose.PDF compatible XML using [XSLT][7]. So let's begin.

The following is the sample XML data that we need to convert to the PDF document.

{{< gist aspose-com-gists a7599829acc2abcd7b08e66f8d41b948 "data.xml" >}}

In order to make this data compatible with the Aspose.PDF XML, we will perform XSLT transformation. For this we will define a template in an XSLT stylesheet file, as shown below.

{{< gist aspose-com-gists a7599829acc2abcd7b08e66f8d41b948 "stylesheet.xslt" >}}

Once you have created the template file, you can proceed to convert XML to PDF following the below steps.

*   Create an object of [Document][8] class.
*   Bind XML using [Document.bindXml(String, String)][9] method by providing XML and XSLT file.
*   Convert XML to PDF using [Document.save(String)][10] method.

The following code sample shows how to convert an XML file to PDF using Java.

{{< gist aspose-com-gists a7599829acc2abcd7b08e66f8d41b948 "xml-to-pdf.java" >}}

### Generated PDF



{{< figure align=center src="images/xml-to-pdf.jpg" alt="XML to PDF in Java">}}


## Get a Free API License {#Get-a-Free-API-License}

You can [get a temporary license][11] in order to use the API without evaluation limitations.

## Conclusion

In this article, you have learned how to convert XML to PDF using Java. You can integrate this feature in your Java applications to generate PDF files from XML. You can learn more about the Java PDF API using the [documentation][12] as well as the source code samples available on [GitHub][13]. In case you would have any questions, feel free to let us know via our [forum][14].

## See Also

*   [Create PDF Files using Java][15]




[1]: #Java-API-for-XML-to-PDF-Conversion
[2]: #Supported-XML-Schema-for-PDF-Generation
[3]: #Convert-XML-to-PDF-in-Java
[4]: https://products.aspose.com/pdf/java
[5]: https://downloads.aspose.com/pdf/java
[6]: https://docs.aspose.com/pdf/net/supported-xml-schema/
[7]: https://en.wikipedia.org/wiki/XSLT#:~:text=XSLT%20(Extensible%20Stylesheet%20Language%20Transformations,as%20PDF%2C%20PostScript%20and%20PNG.
[8]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/Document
[9]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/Document#bindXml-java.lang.String-java.lang.String-
[10]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/Document#save-java.lang.String-
[11]: https://purchase.aspose.com/temporary-license
[12]: https://docs.aspose.com/pdf/java
[13]: https://github.com/aspose-pdf/Aspose.PDF-for-Java
[14]: https://forum.aspose.com/
[15]: https://blog.aspose.com/2020/12/31/create-pdf-files-in-java/






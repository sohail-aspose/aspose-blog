---
title: 'HTML to PDF Java Conversion using Java PDF API'
seoTitle: "HTML to PDF in Java | Convert HTML from Webpage or URL to PDF"
description: "Convert HTML or HTML5 content to PDF using Java. Free download Java library to convert HTML with CSS & SVG to PDF with high fidelity."
date: Thu, 30 Jan 2020 17:40:03 +0000
draft: false
url: /2020/01/30/convert-html-to-pdf-in-java/
author: Usman Aziz
summary: 'The **online HTML to PDF converters** allow you to convert single or multiple HTML pages to PDF documents. However, in case you want to perform this conversion programmatically or you need to do a **batch conversion of HTML files to PDF**, you'll definitely look for some library or API. So let's have a look at how to cope with such scenarios.'
tags: ['Aspose.Pdf for Java', 'convert html to pdf in java', 'html to pdf converter', 'java html to pdf converter', 'java library for html to pdf']
categories: ['Aspose.PDF Product Family']
---

This article shows [HTML][1] to [PDF][2] conversion from a file or web page using Java.



{{< figure align=center src="images/HTML-to-PDF-Java.png" alt="HTML to PDF Java">}}


The **online HTML to PDF converters** allow you to convert single or multiple HTML pages to PDF documents. However, in case you want to perform this conversion programmatically or you need to do a **batch conversion of HTML files to PDF**, you'll definitely look for some library or API. So let's have a look at how to cope with such scenarios.

*   [HTML to PDF converter API][3]
*   [HTML to PDF in Java conversion][4]
*   [Convert HTML to password-protected PDF in Java][5]
*   [HTML to PDF conversion using URL][6]
*   [Convert HTML content to single-page PDF][7]

**Info**: Aspose also provides a [Java PowerPoint API][8] that allows you to create [PDFs from presentations][9] and a free online [PowerPoint to PDF Converter][10] that demonstrates the process.

## HTML to PDF Java Converter API - Free Download {#HTML-to-PDF-Java-Converter-API}

[Aspose.PDF for Java][11] is a powerful Java class library to work with PDF documents. In addition to the other PDF manipulation features, the API also provides high-quality HTML to PDF conversion features. You can [download][12] the API's JAR file or install using Maven configurations.

### Repository```
<repository>
    <id>AsposeJavaAPI</id>
    <name>Aspose Java API</name>
    <url>https://repository.aspose.com/repo/</url>
</repository>
```

### Dependency```
<dependency>
    <groupId>com.aspose</groupId>
    <artifactId>aspose-pdf</artifactId>
    <version>19.12</version>
    <classifier>jdk17</classifier>
</dependency>
```

## How to Convert HTML to PDF

The following are the steps to convert HTML content to PDF using Aspose.PDF API.

*   Download the Aspose.PDF for Java
*   Integrate the API within your application
*   Load the HTML content from file or URL
*   Create PDF from provided HTML content

## HTML to PDF Java Conversion {#Convert-HTML-to-PDF-in-Java}

This is how you can convert an HTML file to PDF using Java.

*   Create an instance of the [HtmlLoadOptions][13] class.
*   Create an instance of [Document][14] class and initialize it with the HTML file's path and _HtmlLoadOptions_ object.
*   Call [Document.save(String)][15] method with the output PDF file's name.

The following code sample shows how to convert an HTML document to a PDF.

{{< gist aspose-com-gists c6fe5ccefe38a5ec03d983307eb0e850 "convert-html-to-pdf.java" >}}

### Input HTML File



{{< figure align=center src="images/HTML-Document.png" alt="Java HTML to PDF ">}}


### Converted PDF Document



{{< figure align=center src="images/HTML-to-PDF.png" alt="Java HTML to PDF Library ">}}


## Convert HTML to Password-Protected PDF in Java {#Convert-HTML-to-Password-Protected-PDF-in-Java}

_Aspose.PDF_ also lets you convert HTML files to encrypted PDF documents. You can protect the resultant PDF document by specifying the user's password, owner's password, access permissions, and cryptographic algorithm in the [Document.encrypt()][16] method.

The following code sample shows how to convert HTML to an encrypted PDF.

{{< gist aspose-com-gists c6fe5ccefe38a5ec03d983307eb0e850 "convert-html-to-password-protected-pdf.java" >}}

### Output



{{< figure align=center src="images/HTML-to-Password-Protected-PDF.png" alt="Convert HTML to PDF">}}


## Convert HTML to PDF using URL in Java {#Convert-HTML-to-PDF-using-URL-in-Java}

You can also convert the web page from the live URL to the PDF document. Below are the steps to achieve this:

*   Create and initialize the _URL_ object.
*   Get the web page into the _InputStream_ object.
*   Create the _Document_ object and initialize it with _InputStream_ and _HtmlLoadOptions_ objects.
*   Save HTML stream as PDF using _Document.save()_ method.

The following code sample shows how to convert HTML content from URL to PDF.

{{< gist aspose-com-gists c6fe5ccefe38a5ec03d983307eb0e850 "convert-html-to-pdf-using-URL.java" >}}

## HTML to a Single Page PDF {#Convert-HTML-to-a-Single-Page-PDF-in-Java}

In case you want to convert the whole HTML content into a single page PDF document, you can set [HtmlLoadOptions.setRenderToSinglePage(true)][17] as shown in the following Java code sample.

{{< gist aspose-com-gists c6fe5ccefe38a5ec03d983307eb0e850 "convert-html-to-single-page-pdf.java" >}}

## Get API's License for Free

Get your [temporary license][18] to use and evaluate Aspose.PDF for Java **for free** for one month.

## Conclusion

In this article, you have seen how to convert HTML content from a file or URL to PDF using Java. In addition, the code samples demonstrated how to convert HTML to a single-paged or password-protected PDF. You can explore more about Aspose.PDF for Java using [documentation][19].

## Related Articles

*   [Create PDF Files in Java][20]
*   [Convert PowerPoint PPT/PPTX to PDF in Java][21]




[1]: https://docs.fileformat.com/web/html/
[2]: https://docs.fileformat.com/pdf/
[3]: #HTML-to-PDF-Java-Converter-API
[4]: #Convert-HTML-to-PDF-in-Java
[5]: #Convert-HTML-to-Password-Protected-PDF-in-Java
[6]: #Convert-HTML-to-PDF-using-URL-in-Java
[7]: #Convert-HTML-to-a-Single-Page-PDF-in-Java
[8]: https://products.aspose.com/slides/java/
[9]: https://products.aspose.com/slides/java/conversion/ppt-to-pdf/
[10]: https://products.aspose.app/slides/conversion
[11]: https://products.aspose.com/pdf/java
[12]: https://downloads.aspose.com/pdf/java
[13]: https://apireference.aspose.com/java/pdf/com.aspose.pdf/HtmlLoadOptions
[14]: https://apireference.aspose.com/java/pdf/com.aspose.pdf/Document
[15]: https://apireference.aspose.com/java/pdf/com.aspose.pdf/Document#save-java.lang.String-
[16]: https://apireference.aspose.com/java/pdf/com.aspose.pdf/Document#encrypt-java.lang.String-java.lang.String-int-int-
[17]: https://apireference.aspose.com/java/pdf/com.aspose.pdf/HtmlLoadOptions#setRenderToSinglePage-boolean-
[18]: https://purchase.aspose.com/temporary-license
[19]: https://docs.aspose.com/pdf/java/
[20]: https://blog.aspose.com/2020/12/31/create-pdf-files-in-java/
[21]: https://blog.aspose.com/2019/12/31/convert-powerpoint-ppt-pptx-to-pdf-in-java-using-aspose-slides/






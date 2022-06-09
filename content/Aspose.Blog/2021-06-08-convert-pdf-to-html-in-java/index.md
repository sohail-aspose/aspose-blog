---
title: 'Convert PDF Files to HTML in Java'
seoTitle: "Convert PDF to HTML in Java | Customize PDF to HTML Conversion"
description: "Use Java PDF API to convert PDF files to HTML pages using Java. Use additional options to customize the PDF to HTML conversion programmatically."
date: Tue, 08 Jun 2021 06:51:00 +0000
draft: false
url: /2021/06/08/convert-pdf-to-html-in-java/
author: Usman Aziz
summary: 'You may often need to convert a PDF file into HTML to embed it within a web page. In order to perform this conversion programmatically, this article covers **how to convert a PDF file to HTML using Java**. Furthermore, you will learn how to use additional options to customize the PDF to HTML conversion.'
tags: ['Convert PDF Files to HTML in Java', 'Java API for PDF to HTML Conversion', 'Java PDF to HTML Converter', 'PDF to HTML with Additional Options']
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/PDF-to-HTML.jpg" alt="PDF to HTML Java">}}


You may often need to convert a PDF file into HTML to embed it within a web page. In order to perform this conversion programmatically, this article covers **how to convert a PDF file to HTML using Java**. Furthermore, you will learn how to use additional options to customize the PDF to HTML conversion.

*   [Java API for PDF to HTML Conversion][1]
*   [Convert PDF Files to HTML][2]
*   [PDF to HTML with Additional Options][3]

## Java API for PDF to HTML Conversion {#Java-API-for-PDF-to-HTML-Conversion}

In order to convert PDF files to HTML, we'll use [Aspose.PDF for Java][4]. It is a feature-rich PDF manipulation API that lets you generate, modify, and convert PDF files. Furthermore, it provides easy-to-use methods to convert PDF to HTML pages. You can either [download][5] the API or install it using the following Maven configurations.

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
    <version>21.5</version>
</dependency>
```

## Convert PDF to HTML in Java {#Convert-PDF-Files-to-HTML}

The following are the steps to convert a PDF file to HTML using Java.

*   Load the PDF document using [Document][6] class.
*   Convert PDF to HTML using [Document.save("pdf-to-html.html", SaveFormat.Html)][7] method.

The following code sample shows how to convert PDF files to HTML.

{{< gist aspose-com-gists 8fe7879cbd2b52f75da4035617105d2e "pdf-to-html.java" >}}

## PDF to HTML with Additional Options {#PDF-to-HTML-with-Additional-Options}

Aspose.PDF for Java also provides additional options to customize the PDF to HTML conversion. Such as, you can compress the images, split the output into multiple HTML pages, specify folder for images, etc. The following are the steps to specify additional options for PDF to HTML conversion.

*   Load the PDF document using [Document][8] class.
*   Create an instance of [HtmlSaveOptions][9] class.
*   Set desired options such as [HtmlOptions.setSplitIntoPages(true)][10] to split HTML content into multiple pages.
*   Convert PDF to HTML using [Document.save("pdf-to-html.html", HtmlSaveOptions)][11] method.

The following code sample shows how to customize PDF to HTML conversion.

{{< gist aspose-com-gists 8fe7879cbd2b52f75da4035617105d2e "pdf-to-html-custom.java" >}}

You can explore other options using the following documentation links.

*   [Avoid Saving Images in SVG Format][12]
*   [Compressing SVG Images During Conversion][13]
*   [Specify Images Folder][14]
*   [Create Subsequent Files with Body Contents Only][15]
*   [Transparent Text rendering][16]
*   [PDF document layers rendering][17]
*   [Exclude Font Resources][18]

## Get a Free License {#Get-a-Free-License}

You can use Aspose.PDF for Java without evaluation limitations using the temporary license. [Get yours now][19].

## Conclusion

In this article, you have learned how to convert PDF files to HTML using Java. Furthermore, you have seen how to use different options to customize PDF to HTML conversion. You can explore more about the API using the [documentation][20]. In addition, you can post your queries to our [forum][21].

## See Also

*   [Generate PDF Files using Java – Java PDF API][22]




[1]: #Java-API-for-PDF-to-HTML-Conversion
[2]: #Convert-PDF-Files-to-HTML
[3]: #PDF-to-HTML-with-Additional-Options
[4]: https://products.aspose.com/pdf/java
[5]: https://downloads.aspose.com/pdf/java
[6]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/Document
[7]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/Document#save-java.lang.String-int-
[8]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/Document
[9]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/HtmlSaveOptions
[10]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/HtmlSaveOptions#setSplitIntoPages-boolean-
[11]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/Document#save-java.lang.String-com.aspose.pdf.SaveOptions-
[12]: https://docs.aspose.com/pdf/java/convert-pdf-to-html/#convert-pdf-to-html---avoid-saving-images-in-svg-format
[13]: https://docs.aspose.com/pdf/java/convert-pdf-to-html/#compressing-svg-images-during-conversion
[14]: https://docs.aspose.com/pdf/java/convert-pdf-to-html/#convert-pdf-to-html---specify-images-folder
[15]: https://docs.aspose.com/pdf/java/convert-pdf-to-html/#create-subsequent-files-with-body-contents-only
[16]: https://docs.aspose.com/pdf/java/convert-pdf-to-html/#transparent-text-rendering
[17]: https://docs.aspose.com/pdf/java/convert-pdf-to-html/#pdf-document-layers-rendering
[18]: https://docs.aspose.com/pdf/java/convert-pdf-to-html/#pdf-to-html---exclude-font-resources
[19]: https://purchase.aspose.com/temporary-license
[20]: https://docs.aspose.com/pdf/java/overview/
[21]: https://forum.aspose.com/
[22]: https://blog.aspose.com/2020/12/31/create-pdf-files-in-java/






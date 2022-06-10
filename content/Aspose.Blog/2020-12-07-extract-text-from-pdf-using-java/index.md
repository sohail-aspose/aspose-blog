---
title: 'Extract Text from PDF using Java'
seoTitle: "Extract Text from PDF in Java | Java Text Extractor API for PDF"
description: "Use Java text extractor API to extract text from PDF files in Java. Extract text from whole PDF, a specific page, section or using regular expression."
date: Mon, 07 Dec 2020 23:09:31 +0000
draft: false
url: /2020/12/07/extract-text-from-pdf-using-java/
author: Usman Aziz
summary: "In this post, you will learn **how to extract text from [PDF][1] documents seamlessly using Java**. Text extraction could be useful in various scenarios such as text analysis, information retrieval, document parsing, and so on. Since PDF is one of the most widely used digital documents, the use cases of text extraction from PDF documents are more in number. So let's begin and check how to perform PDF text extraction from within Java applications."
tags: ['Extract Text from PDF', 'extract text from page in pdf in java', 'extract text from pdf in java']
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/Extract-Text-From-PDF.jpg" alt="extract text from pdf java">}}


In this post, you will learn **how to extract text from [PDF][2] files seamlessly using Java**. Text extraction could be useful in various scenarios such as text analysis, information retrieval, document parsing, and so on. Since PDF is one of the most widely used digital documents, the use cases of text extraction from PDF documents are more in number. So let's begin and check how to perform PDF text extraction from within Java applications.

*   [Java Text Extraction API - Free Download][3]
*   [Extract Text from PDF using Java][4]
*   [Extract Text from Specific Page in PDF][5]
*   [Text Extraction from a Page Region in PDF][6]

**Info**: Aspose recently developed a free online [Text to GIF][7] service that allows you to animate texts or generate GIFs from simple texts.

## Java API to Extract Text from PDF - Free Download {#Java-Text-Extraction-API-Free-Download}

[Aspose.PDF for Java][8] is a well-known PDF file manipulation API that provides a wide range of features to create and process PDF files. The API contains a powerful text extractor that provides various ways of extracting text from PDF documents within a few lines of code. You can either [download][9] the API's JAR or install it within your Maven-based applications using the following configurations.

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
    <version>20.11</version>
</dependency>
```

## Extract Text from PDF using Java {#Extract-Text-from-PDF-using-Java}

The following are the steps to extract text from a PDF document using Aspose.PDF for Java.

*   Use [Document][10] class to load the PDF file.
*   Create an object of [TextAbsorber][11] class.
*   Accept the _TextAbsorber_ for all pages of the PDF using [Document.getPages().accept(TextAbsorber)][12] method.
*   Use [TextAbsorber.getText()][13] method to fetch all the text from the PDF.
*   Save the text into a TXT file (optional).

The following code sample shows how to extract text from PDF using Java.

{{< gist aspose-pdf 474c352a71ac9477aa0d604fd32e1c6a "Examples-src-main-java-com-aspose-pdf-examples-NewDocumentObject-text-ExtractTextFromAllThePagesOfPDFDocument-.java" >}}

## Extract Text from Specific Page in PDF {#Extract-Text-from-Specific-Page-in-PDF}

You can also extract text from a specific page of the PDF document using the following steps.

*   Use [Document][14] class to load the PDF file.
*   Create an instance of [TextDevice][15] class.
*   Define additional options using [TextExtractionOptions][16] class.
*   Set options using [TextDevice.setExtractionOptions(TextExtractionOptions)][17] method.
*   Use [TextDevice.Process(Page, String)][18] to extract the text from the specified page.

The following code sample shows how to extract text from a specific page in PDF using Java.

{{< gist aspose-pdf 474c352a71ac9477aa0d604fd32e1c6a "Examples-src-main-java-com-aspose-pdf-examples-NewDocumentObject-text-ExtractTextFromPDFUsingTextDevice-ExtractTextFromParticularPage.java" >}}

## Extract Text from a Page Region in PDF {#Extract-Text-from-a-Page-Region-in-PDF}

You can also extract text from a particular region of the page in PDF. For this, you can define a rectangle to cover the region from where you need to extract the text. The following are the steps to extract text from a page region.

*   Use [Document][19] class to load the PDF file.
*   Create an object of [TextAbsorber][20] class.
*   Set limit to page bound and create a rectangle using [TextAbsorber.getTextSearchOptions().setLimitToPageBounds(true)][21] and [TextAbsorber.getTextSearchOptions().setRectangle(new Rectangle(100, 200, 250, 350))][22] methods respectively.
*   Accept the absorber for the particular page.
*   Use [TextAbsorber.getText()][23] method to extract text.

The following code sample shows how to extract text from a particular page region in Java.

{{< gist aspose-pdf 474c352a71ac9477aa0d604fd32e1c6a "Examples-src-main-java-com-aspose-pdf-examples-NewDocumentObject-text-ExtractTextFromAnParticularPageRegion-.java" >}}

## Conclusion

In this article, you have learned how to extract text from PDF using Java. You have seen various ways of text extraction such as extracting text from a whole PDF, a specific page, or a specific page region. You can learn more about the Java PDF API using [documentation][24].

## See Also

*   [Convert PDF to DOCX in Java][25]




[1]: https://docs.fileformat.com/pdf/
[2]: https://docs.fileformat.com/pdf/
[3]: #Java-Text-Extraction-API-Free-Download
[4]: #Extract-Text-from-PDF-using-Java
[5]: #Extract-Text-from-Specific-Page-in-PDF
[6]: #Extract-Text-from-a-Page-Region-in-PDF
[7]: https://products.aspose.app/slides/text-to-gif
[8]: https://products.aspose.com/pdf/java
[9]: https://downloads.aspose.com/pdf/java
[10]: https://apireference.aspose.com/pdf//java/com.aspose.pdf/document
[11]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/TextAbsorber
[12]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/PageCollection#accept-com.aspose.pdf.TextAbsorber-
[13]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/TextAbsorber#getText--
[14]: https://apireference.aspose.com/pdf//java/com.aspose.pdf/document
[15]: https://apireference.aspose.com/pdf/java/com.aspose.pdf.devices/TextDevice
[16]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/TextExtractionOptions
[17]: https://apireference.aspose.com/pdf/java/com.aspose.pdf.devices/TextDevice#setExtractionOptions-com.aspose.pdf.TextExtractionOptions-
[18]: https://apireference.aspose.com/pdf/java/com.aspose.pdf.devices/PageDevice#process-com.aspose.pdf.Page-com.aspose.ms.System.Drawing.Graphics-
[19]: https://apireference.aspose.com/pdf//java/com.aspose.pdf/document
[20]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/TextAbsorber
[21]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/TextSearchOptions#setLimitToPageBounds-boolean-
[22]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/TextSearchOptions#setRectangle-com.aspose.pdf.Rectangle-
[23]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/TextAbsorber#getText--
[24]: https://docs.aspose.com/pdf/java/
[25]: https://blog.aspose.com/2020/01/17/convert-pdf-to-word-doc-docx-in-java/






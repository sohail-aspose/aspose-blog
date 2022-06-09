---
title: 'Convert LaTeX to Word using Java'
seoTitle: "Convert LaTeX to Word using Java | TEX to DOCX in Java"
description: "Use Java PDF API to convert LaTeX files to Word format using Java. Convert TEX files to DOCX format programmatically in Java."
date: Mon, 28 Jun 2021 04:19:00 +0000
draft: false
url: /2021/06/28/convert-latex-to-word-using-java/
author: Usman Aziz
summary: '[TEX][1] is a widely used format for typesetting articles, books, and other publications. A TEX file is comprised of different tags to insert text, graphics, mathematical equations, symbols, etc. Most of the TEX editors generate the output of a TEX file as a PDF document. However, in certain cases, you may need to generate a Word document from the TEX file. For such cases, this article covers **how to convert LaTeX file (.tex) to Word format using Java**.'
tags: ['Java LaTeX to Word Converter API', 'Latex to Word in Java', 'TEX to DOCX in Java']
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/TeX-to-DOCX.jpg" alt="Latex to Word Java">}}


[TEX][2] is a widely used format for typesetting articles, books, and other publications. A TEX file is comprised of different tags to insert text, graphics, mathematical equations, symbols, etc. Most of the TEX editors generate the output of a TEX file as a PDF document. However, in certain cases, you may need to generate a Word document from the TEX file. For such cases, this article covers **how to convert LaTeX file (.tex) to Word format using Java**.

*   [LaTeX to Word Converter API][3]
*   [Convert a LaTeX TEX File to DOCX in Java][4]

## Java LaTeX to Word Converter API {#LaTeX-to-Word-Converter-API}

In order to convert the LaTeX files to Word DOCX format, we will use [Aspose.PDF for Java][5]. It is a powerful PDF manipulation API to generate, modify or convert PDF documents. You can either [download][6] the API or install it using the following Maven configurations.

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

## Convert a LaTeX TEX File to DOCX in Java {#Convert-a-LaTeX-TEX-File-to-DOCX}

The following are the steps to convert a LaTeX TEX file to Word DOCX format using Java.

*   Create an instance of [TeXLoadOptions][7] class.
*   Use [Document][8] class to load TEX file by passing its path and [TeXLoadOptions][9] object.
*   Convert TEX to DOCX using [Document.save(String, SaveFormat)][10] method and pass the output file path and SaveFormat.DocX as parameters.

The following code sample shows how to convert LaTeX files to Word DOCX format.

{{< gist aspose-com-gists 81dd3ad1eb6d6998aa1684887f77f896 "latex-to-word.java" >}}

## Get a Free API License {#Get-a-Free-API-License}

You can [get a temporary license][11] in order to use the API without evaluation limitations.

## Conclusion

In this article, you have learned how to convert LaTeX files to Word format using Java. You can easily embed the code in your Java applications to automate TEX to DOCX conversion. In order to explore more about Aspose.PDF for Java, visit the [documentation][12]. In case you would have any queries, contact us via our [forum][13].

## See Also

*   [Generate PDF Files using Java][14]




[1]: https://docs.fileformat.com/page-description-language/tex/
[2]: https://docs.fileformat.com/page-description-language/tex/
[3]: #LaTeX-to-Word-Converter-API
[4]: #Convert-a-LaTeX-TEX-File-to-DOCX
[5]: https://products.aspose.com/pdf/java
[6]: https://downloads.aspose.com/pdf/java
[7]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/TeXLoadOptions
[8]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/Document
[9]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/TeXLoadOptions
[10]: https://apireference.aspose.com/pdf/java/com.aspose.pdf/Document#save-java.lang.String-int-
[11]: https://purchase.aspose.com/temporary-license
[12]: https://docs.aspose.com/pdf/java
[13]: https://forum.aspose.com/
[14]: https://blog.aspose.com/2020/12/31/create-pdf-files-in-java/






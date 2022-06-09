---
title: 'Create Custom TeX (LaTeX) Format and Typeset to PDF, XPS in Java'
seoTitle: "Create Custom TeX (LaTeX) Format | Convert Typeset to PDF, XPS Java"
description: "You can create custom TeX LaTeX and then typeset it to pdf or xps file programmatically in Java. Convert TeX to PDF or XPS file for custom format."
date: Wed, 21 Apr 2021 09:33:00 +0000
draft: false
url: /2021/04/21/create-custom-tex-latex-format-convert-typeset-to-pdf-xps-java/
author: Farhan Raza
summary: 'Many books and journals related to Computer Science, Mathematics, and Engineering are published using TeX. You can create a custom TeX (LaTeX) format and typeset it to different formats like XPS, PDF, or image. Custom TeX is helpful when you need to design many documents in a uniform way.'
tags: ['Convert LateX to XPS in Java', 'Convert Latex to PDF in Java', 'Convert custom TeX', 'TeX to PDF in Java', 'TeX to XPS', 'Typeset custom TeX']
categories: ['Aspose.TeX Product Family']
---



{{< figure align=center src="images/TeX-to-PDF-XPS-1.png" alt="custom tex typeset pdf xps">}}


Many books and journals related to Computer Science, Mathematics, and Engineering are published using TeX. You can create a custom [TeX][1] (LaTeX) format and typeset it to different formats like XPS, PDF, or image. Custom TeX is helpful when you need to design many documents in a uniform way. The following sections include further details about creating and typesetting custom TeX format:

*   [Creating and Typesetting Custom TeX (LaTeX) Format – Java API Installation][2]
*   [Create a Custom TeX Format Programmatically using Java][3]
*   [Typeset or Convert Custom TeX (LaTeX) to PDF Programmatically with Java][4]
*   [Typeset or Convert Custom TeX (LaTeX) to XPS File in Java][5]
*   [Get Free API License][6]

## Creating and Typesetting Custom TeX (LaTeX) Format – Java API Installation {#section1}

[Aspose.TeX for Java][7] has been designed to programmatically work with TeX files. It does not depend on any 3rd party application so you do not need to install or configure any additional software. Simply download the JAR file from the [New Releases][8] section, or install it with the following Maven configurations:

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
        <artifactId>aspose-tex</artifactId>
        <version>21.4</version>
    </dependency>
</dependencies>
```

## Create a Custom TeX Format Programmatically using Java {#section2}

Please follow the steps below for creating a custom TeX format:

1.  Create typesetting options for no format on [ObjectTeX][9] engine extension.
2.  Specify the file system working directory for input and output.
3.  Run format creation with [createFormat()][10] method.

The following code shows how to create custom TeX (LaTeX) format using Java:

{{< gist aspose-com-gists 0612bbb4c8859ca06406cec4513759ea "create-custom-TeX.java" >}}

Please notice that the code is using [objectIniTeX()][11] method which gets the configuration of the Object TeX engine extension with no preloaded format. This lets you create a custom format from scratch.

## Typeset or Convert Custom TeX (LaTeX) to PDF Programmatically with Java {#section3}

You can typeset or convert custom TeX to PDF with the following steps:

1.  Create a file system input and output working directory.
2.  Create a format provider.
3.  Set typesetting options for a custom format on [ObjectTeX][12] engine extension.
4.  Initialize [PdfSaveOptions][13] class object.
5.  Finally, run typesetting to PDF file with [TexJob][14] instance.

The following code explains how to typeset or convert custom TeX (LaTeX) to PDF using Java:

{{< gist aspose-com-gists 0612bbb4c8859ca06406cec4513759ea "typeset-convert-custom-tex-pdf.java" >}}

## Typeset or Convert Custom TeX (LaTeX) to XPS File with Java {#section4}

You can convert or typeset custom TeX to XPS with below steps:

1.  Create a file system input working directory.
2.  Create a format provider with [FormatProvider][15] class.
3.  Set typesetting options for a custom format on [ObjectTeX][16] engine extension.
4.  Finally, run typesetting by passing [XpsDevice][17] as an argument to [TexJob][18] instance.

The code below demonstrates how to convert custom TeX to XPS using Java:

{{< gist aspose-com-gists 0612bbb4c8859ca06406cec4513759ea "typeset-convert-custom-tex-xps.java" >}}

## Get Free API License {#section5}

You can test all the features of the API without any limitations by requesting a [Free Temporary License][19].

## Conclusion

In this article, you have explored how to create a custom TeX (LaTeX) format programmatically using Java. Moreover, you have also learned how to typeset or convert TeX files to PDF or XPS file format using Java. You can further explore the API [Documentation][20] for more details of the API. Please feel free to contact us at the [Free Support Forum][21] in case of any queries!

## See Also

[Convert PUB to PDF Programmatically in Java][22]

[Convert LaTeX to PNG or JPG Image in Java][23]




[1]: https://docs.fileformat.com/page-description-language/tex/
[2]: #section1
[3]: #section2
[4]: #section3
[5]: #section4
[6]: #section5
[7]: https://products.aspose.com/tex/java
[8]: https://downloads.aspose.com/tex/java
[9]: https://apireference.aspose.com/tex/java/com.aspose.tex/TeXExtension#ObjectTeX
[10]: https://apireference.aspose.com/tex/java/com.aspose.tex/TeXJob#createFormat-java.lang.String-com.aspose.tex.TeXOptions-
[11]: https://apireference.aspose.com/tex/java/com.aspose.tex/TeXConfig#objectIniTeX--
[12]: https://apireference.aspose.com/tex/java/com.aspose.tex/TeXExtension#ObjectTeX
[13]: https://apireference.aspose.com/tex/java/com.aspose.tex.rendering/PdfSaveOptions
[14]: https://apireference.aspose.com/tex/java/com.aspose.tex/TeXJob
[15]: https://apireference.aspose.com/tex/java/com.aspose.tex/FormatProvider
[16]: https://apireference.aspose.com/tex/java/com.aspose.tex/TeXExtension#ObjectTeX
[17]: https://apireference.aspose.com/tex/java/com.aspose.tex.rendering/XpsDevice
[18]: https://apireference.aspose.com/tex/java/com.aspose.tex/TeXJob
[19]: https://purchase.aspose.com/temporary-license
[20]: https://docs.aspose.com/tex/java/
[21]: https://forum.aspose.com/c/tex
[22]: https://blog.aspose.com/2020/12/01/convert-pub-pdf-java/
[23]: https://blog.aspose.com/2021/11/28/convert-latex-to-png-or-jpg-image-in-java/






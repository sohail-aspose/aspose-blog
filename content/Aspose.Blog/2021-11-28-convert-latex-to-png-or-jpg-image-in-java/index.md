---
title: 'Convert LaTeX to PNG or JPG Image in Java'
seoTitle: "Convert LaTeX TeX LTX to PNG JPG Image in Java"
description: "Convert LaTeX format file with LTX or TEX file format to a PNG or JPG file in Java. Export Latex to Image programmatically in Java."
date: Sun, 28 Nov 2021 18:57:00 +0000
draft: false
url: /2021/11/28/convert-latex-to-png-or-jpg-image-in-java/
author: Farhan Raza
summary: 'LaTeX is used to prepare documents with high-quality typesetting. The TeX format is used for communicating or publishing technical and scientific documents. In certain cases, you may need to convert TeX files to images like PNG or JPG. In this article, you will learn how to **convert TeX files to PNG or JPG images programmatically in Java**. Please go through the following sections for more information.'
tags: ['LaTeX to JPG', 'LaTeX to PNG', 'Latex to Image in Java', 'TeX to JPG in Java', 'TeX to PNG in Java']
categories: ['Aspose.TeX Product Family']
---



{{< figure align=center src="images/TeX-to-PNG-JPG-Image.jpg" alt="Convert TeX to PNG JPG Image in Java">}}


LaTeX is used to prepare documents with high-quality typesetting. The [TeX][1] format is used for communicating or publishing technical and scientific documents. In certain cases, you may need to convert TeX files to images like [PNG][2] or [JPG][3]. In this article, you will learn how to convert TeX files to PNG or JPG images programmatically in Java. Please go through the following sections for more information.

*   [LTX/TeX to PNG or JPG Converter – Java API Installation][4]
*   [Convert TeX (LaTeX) to PNG Image in Java][5]
*   [Convert LaTeX (TeX) to JPG Image Programmatically using Java][6]

## LTX/TeX to PNG or JPG Converter – Java API Installation {#section1}

[Aspose.TeX for Java][7] API supports working with LTX, TeX, PNG, JPG, and other [supported formats][8]. You can easily configure the API by downloading its JAR file from the [Downloads][9] section, or using the following Maven configurations:

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
        <version>21.11</version>
    </dependency>
</dependencies>
```

## Convert TeX (LaTeX) to PNG Image in Java {#section2}

You can convert an LTX or TeX file to a PNG image with the following steps:

1.  Load the input LTX or TEX file.
2.  Create conversion options for LaTeX format with [TeXOptions][10] class.
3.  Initialize [PngSaveOptions][11] for saving image in PNG format.
4.  Run LaTeX to PNG conversion with [TexJob][12] class.

The code snippet below explains how to convert TeX to PNG image programmatically in Java:

{{< gist aspose-com-gists d1a62c5a81cdcc0e924de59b6a73f073 "TEX-LTX-to-PNG-image.java" >}}

## Convert LTX or TeX to JPG Image using Java {#section3}

You can convert a LaTeX file with LTX or TEX file extension, to a JPG image with the steps below:

1.  Load the source LaTeX file.
2.  Create options using the [TeXOptions][13] class object.
3.  Specify [JpegSaveOptions][14] class object.
4.  Run LaTeX to JPG using the [TexJob][15] class.

The following code elaborates how to convert TeX to JPG image programmatically using Java:

{{< gist aspose-com-gists d1a62c5a81cdcc0e924de59b6a73f073 "TEX-LTX-to-JPG-image.java" >}}

## Get Free Evaluation License

You can evaluate the API without any limitations by requesting a [free temporary license][16].

## Conclusion

In this article, you have learned how to render LaTeX files in TeX or LTX file format to a PNG or JPG image programmatically in Java. Moreover, you can visit the [documentation][17] to check several other features of the API. Please feel free to write to us at the [forum][18] for any of your inquiries.

## See Also

[Create Custom TeX (LaTeX) Format and Typeset to PDF, XPS in Java][19]




[1]: https://docs.fileformat.com/page-description-language/tex/
[2]: https://docs.fileformat.com/image/png/
[3]: https://docs.fileformat.com/image/jpeg/
[4]: #section1
[5]: #section2
[6]: #section4
[7]: https://products.aspose.com/tex/java
[8]: https://docs.aspose.com/tex/java/supported-file-formats/
[9]: https://downloads.aspose.com/tex/java
[10]: https://apireference.aspose.com/tex/java/com.aspose.tex/class-use/TeXOptions
[11]: https://apireference.aspose.com/tex/java/com.aspose.tex.rendering/PngSaveOptions
[12]: https://apireference.aspose.com/tex/java/com.aspose.tex/TeXJob#TeXJob-com.aspose.tex.rendering.Device-com.aspose.tex.TeXOptions-
[13]: https://apireference.aspose.com/tex/java/com.aspose.tex/class-use/TeXOptions
[14]: https://apireference.aspose.com/tex/java/com.aspose.tex.rendering/JpegSaveOptions
[15]: https://apireference.aspose.com/tex/java/com.aspose.tex/TeXJob#TeXJob-com.aspose.tex.rendering.Device-com.aspose.tex.TeXOptions-
[16]: https://purchase.aspose.com/temporary-license
[17]: https://docs.aspose.com/tex/java/
[18]: https://forum.aspose.com/c/tex
[19]: https://blog.aspose.com/2021/04/21/create-custom-tex-latex-format-convert-typeset-to-pdf-xps-java/





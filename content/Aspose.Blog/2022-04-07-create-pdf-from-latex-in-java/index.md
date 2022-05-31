---
title: 'Create PDF from LaTeX in Java'
date: Thu, 07 Apr 2022 14:12:44 +0000
draft: false
url: /2022/04/07/create-pdf-from-latex-in-java/
author: 'Muzammil Khan'
summary: 'As a Java developer, you can easily create a PDF document from the LaTeX source file programmatically. In this article, you will learn **how to create PDF from LaTeX in Java**.'
tags: ['Convert Latex to PDF in Java', 'LTX to PDF in Java', 'TeX to PDF', 'TeX to PDF in Java', 'TeX to XPS']
categories: ['Aspose.TeX Product Family']
---



{{< figure align=center src="images/create-pdf-from-latex-in-java.jpg" alt="Create PDF from LaTeX in Java">}}


LaTeX is widely used for creating technical and scientific documentation. LaTeX files ([TEX][1] or [LTX][2] are source documents filled with commands to specify the format of the document, including text, symbols, mathematical expressions, and graphics. We can easily generate a [PDF][3] document from the LaTeX source programmatically. PDF allows sharing documents in a read-only format without compromising their style or layout. In this article, we will learn **how to create a PDF document from the LaTeX source file in Java**.

The following topics shall be covered in this article:

*   [Java API to Create PDF from LaTeX][4]
*   [Create PDF from TeX (LaTeX) File in Java][5]
*   [Create PDF from LTX (LaTeX) File in Java][6]
*   [Convert TeX to XPS using Java][7]
*   [Convert TeX ZIP Directory into PDF ZIP Directory using Java][8]

## Java API to Create PDF from LaTeX {#Java-API-to-Create-PDF-from-LaTeX}

For creating PDF documents from LaTeX source files, we will be using the [Aspose.TeX for Java][9] API. It allows typesetting TeX files to different file formats like PDF, [XPS][10], or images. Please either [download][11] the JAR of the API or add the following _pom.xml_ configuration in a Maven-based Java application.

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
    <artifactId>aspose-tex</artifactId>
    <version>21.11</version>
    <type>jar</type>
</dependency>
```

## Create PDF from LaTeX TeX File in Java {#Create-PDF-from-LaTeX-TeX-File-in-Java}

We can create a PDF document from a LaTeX (TeX) file by following the steps given below:

1.  Firstly, create an instance of the [_**TeXOptions**_][12] class using the **_[consoleAppOptions()][13]_** method.
2.  Set TeX configuration as **_[TeXConfig.objectLaTeX()][14]_**.
3.  Next, set input and output working directories.
4.  Then, specify console or memory stream as an output terminal.
5.  After that, set options for rendering into PDF format.
6.  Finally, call the **_[run()][15]_** method for the newly created **_[TexJob][16]_** class instance with the output PDF and the **_[PdfDevice][17]_** class object as arguments.

The following code example demonstrates **how to create a PDF from a TeX file using Java.**

{{< gist aspose-com-gists 2c8cb628fe75575c76185dbf45760ea3 "CreatePDFfromLaTeX_Java_TeXtoPDF.java" >}}



{{< figure align=center src="images/Create-PDF-from-LaTeX-TeX-File-in-Java-1024x512.jpg" alt="Create PDF from LaTeX TeX File in Java" caption="Create PDF from LaTeX TeX File in Java.">}}


## Create PDF from LTX File in Java {#Create-PDF-from-LTX-File-in-Java}

LaTeX uses an LTX file extension typesetting markup tags and properties that define the document structure and content. We can create a PDF from LaTeX (LTX) file as well by following the steps mentioned earlier. However, we just need to input the source file with the .ltx extension in the last step.

The following code example demonstrates **how to create a PDF from an LTX file using Java.**

{{< gist aspose-com-gists 2c8cb628fe75575c76185dbf45760ea3 "CreatePDFfromLaTeX_Java_LTXtoPDF.java" >}}

## Convert TeX to XPS using Java {#Convert-TeX-to-XPS-using-Java}

We can also convert LaTeX (TeX) file to XPS by following the steps mentioned earlier. However, we just need to set the **_[XpsSaveOptions][18]_** instead of **_[PdfSaveOptions][19]_** at step # 5.

The following code example demonstrates **how to convert TeX to XPS using Java.**

{{< gist aspose-com-gists 2c8cb628fe75575c76185dbf45760ea3 "CreatePDFfromLaTeX_Java_TeXtoXPS.java" >}}

## Convert TeX ZIP Directory into PDF ZIP Directory using Java {#Convert-TeX-ZIP-Directory-into-PDF-ZIP-Directory-using-Java}

We can convert multiple TeX files compressed in a ZIP archive to PDF at once by following the steps given below:

1.  Firstly, open streams on ZIP archives as the input and output working directory.
2.  Next, create an instance of the [_**TeXOptions**_][20] class using the **_[consoleAppOptions()][21]_** method.
3.  Then, set TeX configuration as **_[TeXConfig.objectLaTeX()][22]_**.
4.  Next, set input and output ZIP directories.
5.  Then, specify console or memory stream as an output terminal.
6.  After that, set options for rendering into PDF format.
7.  Finally, call the **_[run()][23]_** method for the newly created **_[TexJob][24]_** class instance with the output PDF and the **_[PdfDevice][25]_** class object as arguments.

The following code example demonstrates **how to convert a TeX ZIP archive to a PDF ZIP archive using Java.**

{{< gist aspose-com-gists 2c8cb628fe75575c76185dbf45760ea3 "CreatePDFfromLaTeX_Java_TeXZiptoPDFZip.java" >}}



{{< figure align=center src="images/Convert-TeX-ZIP-Directory-into-PDF-ZIP-Directory-using-Java-1024x424.jpg" alt="Convert a TeX ZIP archive to a PDF ZIP archive" caption="**Convert a TeX ZIP archive to a PDF ZIP archive**.">}}


## Get a Free License {#Get-a-Free-API-License}

You can [get a free temporary license][26] to try the library without evaluation limitations.

## Conclusion

In this article, we have learned how to:

*   generate a PDF output from the LaTeX source file in Java;
*   create an XPS output document from the TeX file programmatically;
*   convert a TeX ZIP archive into a PDF ZIP archive using Java.

Besides, you can learn more about Aspose.TeX for Java API using the [documentation][27]. In case of any ambiguity, please feel free to contact us on the [forum][28].

## See Also

*   [Create Custom TeX (LaTeX) Format and Typeset to PDF, XPS in Java][29]




[1]: https://docs.fileformat.com/page-description-language/tex/
[2]: https://docs.fileformat.com/word-processing/ltx/)
[3]: https://docs.fileformat.com/pdf/
[4]: #Java-API-to-Create-PDF-from-LaTeX
[5]: #Create-PDF-from-LaTeX-TeX-File-in-Java
[6]: #Create-PDF-from-LTX-File-in-Java
[7]: #Convert-TeX-to-XPS-using-Java
[8]: #Convert-TeX-ZIP-Directory-into-PDF-ZIP-Directory-using-Java
[9]: https://products.aspose.com/tex/java
[10]: https://docs.fileformat.com/page-description-language/xps/
[11]: https://downloads.aspose.com/tex/java
[12]: https://apireference.aspose.com/tex/java/com.aspose.tex/TeXOptions
[13]: https://apireference.aspose.com/tex/java/com.aspose.tex/TeXOptions#consoleAppOptions-com.aspose.tex.TeXConfig-
[14]: https://apireference.aspose.com/tex/java/com.aspose.tex/TeXConfig#objectLaTeX--
[15]: https://apireference.aspose.com/tex/java/com.aspose.tex/TeXJob#run--
[16]: https://apireference.aspose.com/tex/java/com.aspose.tex/TeXJob
[17]: https://apireference.aspose.com/tex/java/com.aspose.tex.rendering/PdfDevice
[18]: https://apireference.aspose.com/tex/java/com.aspose.tex.rendering/XpsSaveOptions
[19]: https://apireference.aspose.com/tex/java/com.aspose.tex.rendering/PdfSaveOptions
[20]: https://apireference.aspose.com/tex/java/com.aspose.tex/TeXOptions
[21]: https://apireference.aspose.com/tex/java/com.aspose.tex/TeXOptions#consoleAppOptions-com.aspose.tex.TeXConfig-
[22]: https://apireference.aspose.com/tex/java/com.aspose.tex/TeXConfig#objectLaTeX--
[23]: https://apireference.aspose.com/tex/java/com.aspose.tex/TeXJob#run--
[24]: https://apireference.aspose.com/tex/java/com.aspose.tex/TeXJob
[25]: https://apireference.aspose.com/tex/java/com.aspose.tex.rendering/PdfDevice
[26]: https://purchase.aspose.com/temporary-license
[27]: https://docs.aspose.com/tex/java/
[28]: https://forum.aspose.com/c/tex/47
[29]: https://blog.aspose.com/2021/04/21/create-custom-tex-latex-format-convert-typeset-to-pdf-xps-java/





---
title: 'Convert Word DOC or DOCX to PDF in C++'
seoTitle: "Convert Word DOC/DOCX to PDF in C++ | DOCX to PDF or DOC to PDF"
description: "Convert Word DOCX to PDF or DOC to PDF in C++. Convert DOCX to PDF/A or other PDF Standards in C++. Apply text/image compression in DOCX to PDF in C++."
date: Fri, 10 Apr 2020 14:29:18 +0000
draft: false
url: /2020/04/10/convert-word-doc-or-docx-to-pdf-in-cpp/
author: Usman Aziz
summary: ''
tags: ['Convert DOCX to PDF in CPP', 'Convert Word to PDF CPP', 'DOCX to PDF CPP']
categories: ['Aspose.Words Product Family']
---



{{< figure align=center src="images/Word-to-PDF-Conversion-C.png" alt="Convert Word DOCX to PDF">}}


Welcome again to the Home of File Format APIs! In the recent past, I have written a couple of blog posts to cover various scenarios of converting Word (DOC/DOCX) to PDF programmatically in [.NET][1] (using C#) and [Java][2] applications. Since this is a popular and widely used feature, I thought to cover it for C++ as well. Therefore, in this post, I will show you how to **convert Word DOC/DOCX to PDF** in **C++** applications. This article addresses the following Word to PDF conversions:

*   Simple Word DOC/DOCX to PDF in C++.
*   DOCX to PDF with particular standard i.e. PDF 1.5, PDF/A-1a, etc.
*   Converting selected pages of a DOCX to PDF.
*   Apply image/text compression in DOCX to PDF conversion.

## C++ Word to PDF Converter Library

[Aspose.Words for C++][3] is an advanced library to create and manipulate Word document formats within C++ applications without requiring MS Word. You can either install it via [NuGet][4] or [download][5] the complete package containing the library files as well as ready to run source code examples.

## Convert Word DOC/DOCX to PDF in C++

Converting a Word document to PDF is as simple as pie using Aspose.Words for C++. The following are the steps to convert a DOC/DOCX file to PDF.

*   Create an object of [Document][6] class and initialize it with the Word document's path.
*   Call [Document->Save()][7] method to save the document as PDF.

The following code sample shows how to convert DOCX to PDF in C++.

{{< gist aspose-com-gists 646412e3cb84d611ef4cb124f9c683c6 "DOCX-to-PDF.cpp" >}}

### Input Word Document



{{< figure align=center src="images/DOCX-to-PDF-C.png" alt="DOCX to PDF C++">}}


### Converted PDF Document



{{< figure align=center src="images/DOC-to-PDF-C.png" alt="DOC to PDF in C++">}}


## Convert DOCX to PDF/A or Other PDF Standards in C++

The PDF format supports various PDF standards including PDF/A, PDF/E and etc. There might be the case when you need to convert Word file to a particular standard such as PDF/A-1a. In such a case, Aspose.Words for C++ allows you to set the desired PDF standard for the converted PDF. The following are the steps to set PDF standard in Word to PDF conversion:

*   Create an object of [Document][8] class and initialize it with DOCX file's path.
*   Create an object of [PdfSaveOptions][9] class and set PDF compliance using [PdfSaveOptions->set\_Compliance()][10] method.
*   Call [Document->Save()][11] method to save the document as PDF.

The following code sample shows how to convert Word DOCX to PDF with PDF/A-1a standard.

{{< gist aspose-com-gists 646412e3cb84d611ef4cb124f9c683c6 "DOCX-to-PDFA.cpp" >}}

## Convert Selected Pages of a Word to PDF in C++

You may also convert only the selected pages instead of converting the whole Word to PDF. The following are the steps to convert only the desired pages of Word to PDF:

*   Load the Word document using [Document][12] class.
*   Set the starting page's index using _PdfSaveOptions->set\_PageIndex()_ method.
*   Set the number of pages you want to convert using _PdfSaveOptions->set\_PageCount()_ method.
*   Save the document as PDF using [Document->Save()][13] method.

The following code sample shows how to convert selected pages of DOCX to PDF in C++.

{{< gist aspose-com-gists 646412e3cb84d611ef4cb124f9c683c6 "DOCX-to-PDFA-custom-pages.cpp" >}}

## Apply Image/Text Compression in DOCX to PDF Conversion

You may also compress the resultant PDF document in order to reduce its size. Aspose.Words for C++ lets you apply the text and image compression using [PdfSaveOptions->set\_TextCompression()][14] and [PdfSaveOptions->set\_ImageCompression()][15] methods respectively. The following code sample shows how to apply compression when converting DOCX to PDF in C++.

{{< gist aspose-com-gists 646412e3cb84d611ef4cb124f9c683c6 "DOCX-to-PDF-text-image-compression.cpp" >}}

## Learn more about Aspose.Words for C++

You may explore more about Aspose.Words for C++ using the [documentation][16]. In case you may find anything confusing, feel free to let us know via our [forum][17].

## See Also

*   [Convert Word DOC/DOCX to PDF in C# .NET][18]
*   [Convert Word DOC/DOCX to PDF in Java][19]

.




[1]: https://blog.aspose.com/2020/01/02/convert-word-doc-docx-to-pdf-in-csharp-net-core/
[2]: https://blog.aspose.com/2020/02/20/convert-word-doc-docx-to-pdf-in-java-programmatically/
[3]: https://products.aspose.com/words/cpp
[4]: https://www.nuget.org/packages/Aspose.Words.Cpp/
[5]: https://downloads.aspose.com/words/cpp
[6]: https://apireference.aspose.com/words/cpp/class/aspose.words.document/
[7]: https://apireference.aspose.com/words/cpp/class/aspose.words.saving.save_output_parameters/
[8]: https://apireference.aspose.com/words/cpp/class/aspose.words.document/
[9]: https://apireference.aspose.com/words/cpp/class/aspose.words.saving.pdf_save_options/
[10]: https://apireference.aspose.com/words/cpp/class/aspose.words.saving.pdf_save_options/#a38c73e85ecd0c278a118e2cbbd599c05
[11]: https://apireference.aspose.com/words/cpp/class/aspose.words.saving.save_output_parameters/
[12]: https://apireference.aspose.com/words/cpp/class/aspose.words.document/
[13]: https://apireference.aspose.com/words/cpp/class/aspose.words.saving.save_output_parameters/
[14]: https://apireference.aspose.com/words/cpp/class/aspose.words.saving.pdf_save_options/#a751585132e8e03d2b66955dd808363bc
[15]: https://apireference.aspose.com/words/cpp/class/aspose.words.saving.pdf_save_options/#a9fc1a7d41317f55417a099a0d97fcaf1
[16]: https://docs.aspose.com/display/wordscpp/Product+Overview
[17]: http://forum.aspose.com
[18]: https://blog.aspose.com/2020/01/02/convert-word-doc-docx-to-pdf-in-csharp-net-core/
[19]: https://blog.aspose.com/2020/02/20/convert-word-doc-docx-to-pdf-in-java-programmatically/






---
title: 'Convert DOCX to DOC or DOC to DOCX using C++'
seoTitle: "Convert DOCX to DOC or DOC to DOCX using C++"
description: "Convert DOCX to DOC and DOC to DOCX format using C++. Bulk convert DOCX and DOC files with ease within your C++ applications."
date: Mon, 28 Jun 2021 21:49:51 +0000
draft: false
url: /2021/06/28/convert-docx-to-doc-or-doc-to-docx-using-cpp/
author: Muhammad Ahmad
summary: 'Microsoft Word documents are available in two formats, [DOC][1] and [DOCX][2]. DOC is an older format, and DOCX is its successor. You can convert DOCX files to DOC format and vice-versa. In this article, you will learn how to convert a DOCX file to DOC format and a DOC file to DOCX format. You will also see how to perform these conversions in bulk.'
tags: ['Batch Convert DOC to DOCX C++', 'Batch Convert DOCX to DOC C++', 'Convert DOC to DOCX C++', 'Convert DOCX to DOC C++']
categories: ['Aspose.Words Product Family']
---



{{< figure align=center src="images/Convert-DOCX-to-DOC-to-DOCX.png" alt="Convert DOCX to DOC or DOC to DOCX using C++">}}


Microsoft Word documents are available in two formats, [DOC][3] and [DOCX][4]. DOC is an older format, and DOCX is its successor. You can convert DOCX files to DOC format and vice-versa. In this article, you will learn how to convert a DOCX file to DOC format and a DOC file to DOCX format. You will also see how to perform these conversions in bulk. To explore these scenarios in detail, please see the following sections:

*   [C++ API for Converting DOCX to DOC and DOC to DOCX Format][5]
*   [Converting DOCX File to DOC Format using C++][6]
*   [Batch Convert DOCX Files to DOC Format using C++][7]
*   [Convert DOC File to DOCX Format using C++][8]
*   [Batch Convert DOC Files to DOCX Format using C++][9]

## C++ API for Converting DOCX to DOC and DOC to DOCX Format {#CPP-API-for-Converting-DOCX-to-DOC-and-DOC-to-DOCX-Format}

[Aspose.Words for C++][10] is a native C++ library that allows you to create, read, and modify Microsoft Word documents. Furthermore, it also supports converting DOCX files to DOC format and DOC files to DOCX format. You can either install the API through [NuGet][11] or download it directly from the [Downloads][12] section.

```
PM> Install-Package Aspose.Words.Cpp
```

## Converting DOCX File to DOC Format using C++ {#Converting-DOCX-File-to-DOC-Format-using-CPP}

You can convert a DOCX file to DOC format by following the steps given below.

*   Create an instance of the [LoadOptions][13] class.
*   Set the load format as DOCX using [LoadOptions->set\_LoadFormat(Aspose::Words::LoadFormat value)][14] method.
*   Load the source DOCX file using the [Document][15] class.
*   Save the converted DOC file using [Document->Save(System::String fileName, Aspose::Words::SaveFormat saveFormat)][16] method.

The following sample code shows how to convert a DOCX file to a DOC file using C++.

{{< gist aspose-com-gists dd9e06fbbc3c60b11d00879b0b26ff62 "Convert-DOCX-to-DOC.cpp" >}}

## Batch Convert DOCX Files to DOC Format using C++ {#Batch-Convert-DOCX-Files-to-DOC-Format-using-CPP}

If you have hundreds of DOCX files that you need to convert to DOC format, you can easily convert them by executing the program once. In this example, we will use the boost library to iterate through the files in the directory. The following are the steps to batch convert DOCX files to DOC format.

*   Iterate through the files in the directory.
*   Create an instance of the [LoadOptions][17] class.
*   Set the load format as DOCX using [LoadOptions->set\_LoadFormat(Aspose::Words::LoadFormat value)][18] method.
*   Load the DOCX files using the [Document][19] class.
*   Change the extension to DOC in the filename.
*   Save the converted DOC file using the [Document->Save(System::String fileName, Aspose::Words::SaveFormat saveFormat)][20] method.

The following sample code demonstrates how to convert DOCX files to DOC format in bulk using C++.

{{< gist aspose-com-gists dd9e06fbbc3c60b11d00879b0b26ff62 "Convert-DOCX-to-DOC-Batch.cpp" >}}

## Convert DOC File to DOCX Format using C++ {#Convert-DOC-File-to-DOCX-Format-using-CPP}

The following are the steps to convert a DOC file to a DOCX file.

*   Create an instance of the [LoadOptions][21] class.
*   Set the load format as DOC using [LoadOptions->set\_LoadFormat(Aspose::Words::LoadFormat value)][22] method.
*   Load the source DOC file using the [Document][23] class.
*   Save the converted DOCX file using [Document->Save(System::String fileName, Aspose::Words::SaveFormat saveFormat)][24] method.

The following sample code shows how to convert a DOC file to a DOCX file using C++.

{{< gist aspose-com-gists dd9e06fbbc3c60b11d00879b0b26ff62 "Convert-DOC-to-DOCX.cpp" >}}

## Batch Convert DOC Files to DOCX Format using C++ {#Batch-Convert-DOC-Files-to-DOCX-Format-using-CPP}

In order to convert DOC files to DOCX format in bulk, use the steps given below.

*   Iterate through the files in the directory.
*   Create an instance of the [LoadOptions][25] class.
*   Set the load format as DOC using [LoadOptions->set\_LoadFormat(Aspose::Words::LoadFormat value)][26] method.
*   Load the DOC files using the [Document][27] class.
*   Change the extension to DOCX in the filename.
*   Save the converted DOCX file using the [Document->Save(System::String fileName, Aspose::Words::SaveFormat saveFormat)][28] method.

The following sample code demonstrates how to convert DOC files to DOCX format in bulk using C++.

{{< gist aspose-com-gists dd9e06fbbc3c60b11d00879b0b26ff62 "Convert-DOC-to-DOCX-Batch.cpp" >}}

## Get a Free License

You can try the API without evaluation limitations by requesting [a free temporary license][29].

## Conclusion

In this article, you have learned how to convert a DOCX file to DOC format and a DOC file to DOCX format using C++. Furthermore, you have seen how to perform these conversions in bulk using the boost library. Aspose.Words for C++ provides a bunch of additional features for automating your Word-related tasks. You can explore the API in detail by visiting the [official documentation][30]. In case of any questions, please feel free to reach us on our [free support forum][31].

## See Also

*   [Working with Table of Contents in Word Documents using C++][32]
*   [Split MS Word Documents using C++][33]




[1]: https://docs.fileformat.com/word-processing/doc/
[2]: https://docs.fileformat.com/word-processing/docx/
[3]: https://docs.fileformat.com/word-processing/doc/
[4]: https://docs.fileformat.com/word-processing/docx/
[5]: #CPP-API-for-Converting-DOCX-to-DOC-and-DOC-to-DOCX-Format
[6]: #Converting-DOCX-File-to-DOC-Format-using-CPP
[7]: #Batch-Convert-DOCX-Files-to-DOC-Format-using-CPP
[8]: #Convert-DOC-File-to-DOCX-Format-using-CPP
[9]: #Batch-Convert-DOC-Files-to-DOCX-Format-using-CPP
[10]: https://products.aspose.com/words/cpp
[11]: https://www.nuget.org/packages/Aspose.Words.Cpp
[12]: https://downloads.aspose.com/words/cpp
[13]: https://apireference.aspose.com/words/cpp/class/aspose.words.loading.load_options
[14]: https://apireference.aspose.com/words/cpp/class/aspose.words.loading.load_options#a90d031c6751e7b2706001bf11a1629cd
[15]: https://apireference.aspose.com/words/cpp/class/aspose.words.document
[16]: https://apireference.aspose.com/words/cpp/class/aspose.words.document#a1355bc15bd6da23c7bf65f3fcf0fb050
[17]: https://apireference.aspose.com/words/cpp/class/aspose.words.loading.load_options
[18]: https://apireference.aspose.com/words/cpp/class/aspose.words.loading.load_options#a90d031c6751e7b2706001bf11a1629cd
[19]: https://apireference.aspose.com/words/cpp/class/aspose.words.document
[20]: https://apireference.aspose.com/words/cpp/class/aspose.words.document#a1355bc15bd6da23c7bf65f3fcf0fb050
[21]: https://apireference.aspose.com/words/cpp/class/aspose.words.loading.load_options
[22]: https://apireference.aspose.com/words/cpp/class/aspose.words.loading.load_options#a90d031c6751e7b2706001bf11a1629cd
[23]: https://apireference.aspose.com/words/cpp/class/aspose.words.document
[24]: https://apireference.aspose.com/words/cpp/class/aspose.words.document#a1355bc15bd6da23c7bf65f3fcf0fb050
[25]: https://apireference.aspose.com/words/cpp/class/aspose.words.loading.load_options
[26]: https://apireference.aspose.com/words/cpp/class/aspose.words.loading.load_options#a90d031c6751e7b2706001bf11a1629cd
[27]: https://apireference.aspose.com/words/cpp/class/aspose.words.document
[28]: https://apireference.aspose.com/words/cpp/class/aspose.words.document#a1355bc15bd6da23c7bf65f3fcf0fb050
[29]: https://purchase.aspose.com/temporary-license
[30]: https://docs.aspose.com/words/cpp/
[31]: https://forum.aspose.com/c/words/8
[32]: https://blog.aspose.com/2021/05/11/working-with-table-of-contents-in-word-documents-using-cpp/
[33]: https://blog.aspose.com/2021/02/26/split-ms-word-documents-using-cpp/






---
title: 'Convert PUB to Word Document (DOC/DOCX) using C++'
seoTitle: "Convert PUB to Word Document (DOC/DOCX) using C++"
description: "Convert Microsoft Publisher (PUB) files to Microsoft Word (DOC/DOCX) files using Aspose.PUB for C++ and Aspose.PDF for C++ APIs."
date: Wed, 28 Jul 2021 18:24:33 +0000
draft: false
url: /2021/07/28/convert-pub-to-word-document-doc-docx-using-cpp/
author: Muhammad Ahmad
summary: 'Microsoft Publisher ([PUB)][1] files are used to create professional documents and marketing materials such as brochures, newsletters, and posters. There might be scenarios where you need to convert the PUB file to a Word document in [DOC][2] and [DOCX][3] format. For such cases, this article will teach you **how to convert PUB files to Word format using C++**.'
tags: ['Convert PUB to DOC using C++', 'Convert PUB to DOCX using C++', 'Convert PUB to Word Format using C++', 'PUB to DOCX C++']
categories: ['Aspose.PDF Product Family', 'Aspose.PUB Product Family']
---



{{< figure align=center src="images/PUB-to-Word.jpg" alt="DOCX) using C++">}}


Microsoft Publisher ([PUB)][4] files are used to create professional documents and marketing materials such as brochures, newsletters, and posters. There might be scenarios where you need to convert the PUB file to a Word document in [DOC][5] and [DOCX][6] format. For such cases, this article will teach you **how to convert PUB files to Word format using C++**.

*   [C++ APIs for Converting PUB Files to Word Format][7]
*   [Convert PUB Files to Word DOC/DOCX Files using C++][8]

## C++ APIs for Converting PUB Files to Word Format {#CPP-APIs-for-Converting-PUB-Files-to-Word-Format}

We will perform this conversion using the [Aspose.PUB for C++][9] and [Aspose.PDF for C++][10] APIs. The former is an API for working with Microsoft Publisher (PUB) files, whereas the latter is an API for creating, reading, and updating PDF files. We will use the Aspose.PUB for C++ API to convert PUB files to PDF format and Aspose.PDF for C++ API to convert the generated PDF files to Word files. You can either install the APIs through NuGet or download them directly from the [Downloads][11] section.

```
PM> Install-Package Aspose.PUB.Cpp
PM> Install-Package Aspose.PDF.Cpp
```

## Convert PUB Files to Word DOC/DOCX Files using C++ {#Convert-PUB-Files-to-Word-DOC-DOCX-Files-using-CPP}

The following are the steps to convert PUB files to Word documents in DOC or DOCX format.

*   Load the PUB file using the [PubFactory::CreateParser(System::String fileName)][12] method.
*   Convert the PUB file to PDF format using the [ConvertToPdf(System::SharedPtr<Document> doc, System::String fileName)][13] method.
*   Load the generated PDF file using the [Document][14] class.
*   Create an instance of the [DocSaveOptions][15] class.
*   Set the format to [DocFormat::DocX][16] using the [DocSaveOptions->set\_Format(DocSaveOptions::DocFormat value)][17] method.
*   Save the Word file using the [Document->Save(System::String outputFileName, System::SharedPtr<SaveOptions> options)][18] method.

The following sample code shows how to convert a PUB file to a Word document using C++.

{{< gist aspose-com-gists df85ab10987edad6def4555567c0ebb1 "PUB_To_Word.cpp" >}}

## Get a Free License

You can try the API without evaluation limitations by requesting [a free temporary license][19].

## Conclusion

In this article, you have learned how to convert PUB files to Word format using C++. To achieve this, we used the Aspose.PUB for C++ and Aspose.PDF for C++ APIs. You can learn more about these APIs by exploring their official documentation. In case of any queries, please feel free to reach us at our [free support forum][20].

*   [Aspose.PUB for C++ Documentation][21]
*   [Aspose.PDF for C++ Documentation][22]

## See Also

*   [Convert PUB to Image using C++][23]




[1]: https://en.wikipedia.org/wiki/PUB_(file_type)
[2]: https://docs.fileformat.com/word-processing/doc/
[3]: https://docs.fileformat.com/word-processing/docx/
[4]: https://en.wikipedia.org/wiki/PUB_(file_type)
[5]: https://docs.fileformat.com/word-processing/doc/
[6]: https://docs.fileformat.com/word-processing/docx/
[7]: #CPP-APIs-for-Converting-PUB-Files-to-Word-Format
[8]: #Convert-PUB-Files-to-Word-DOC-DOCX-Files-using-CPP
[9]: https://products.aspose.com/pub/cpp/
[10]: https://products.aspose.com/pdf/cpp
[11]: https://downloads.aspose.com/total
[12]: https://apireference.aspose.com/pub/cpp/class/aspose.pub.pub_factory#a88c04c4c35d45ee8febc7e1554d03c4b
[13]: https://apireference.aspose.com/pub/cpp/class/aspose.pub.i_pdf_converter#acdea381bc8f2a2799e73a039b09ecdb5
[14]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.document
[15]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.doc_save_options
[16]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.doc_save_options#a6db3d3814fe7159c59e848d94e07ed57
[17]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.doc_save_options#afc19c9ecf428c6cb4bc3650e4279af1c
[18]: https://apireference.aspose.com/pdf/cpp/class/aspose.pdf.document#a6383c010776212483f51cc41235924db
[19]: https://purchase.aspose.com/temporary-license
[20]: https://forum.aspose.com/
[21]: https://docs.aspose.com/pub/cpp/
[22]: https://docs.aspose.com/pdf/cpp/
[23]: https://blog.aspose.com/2021/07/23/convert-pub-to-image-using-cpp/






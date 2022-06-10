---
title: 'Convert PDF to DOC and DOCX in C++'
date: Tue, 05 Nov 2019 08:35:01 +0000
draft: false
url: /2019/11/05/convert-pdf-to-doc-and-docx-in-c/
author: Kashif Iqbal
summary: ''
tags: ['PDF', 'PDF to Word Conversion', 'c++ library', 'convert PDF files']
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/aspose_pdf-for-cpp-128x128.png" alt="aspose-pdf-for-cpp">}}


[Aspose.PDF for C++][1] API lets you read and convert PDF documents to Microsoft Word's [DOC][2] and [DOCX][3] file formats. C++ is one of the widely-used programming languages for writing fast and interoperable code that can be executed on a number of platforms. C++ application developers can use Aspose.PDF for C++ to write programs that can manipulate PDF documents without the need of installing any other software on end-user machines.

In this post, we will demonstrate the powerful features of Aspose.PDF for C++ API to read and [convert PDF files][4] to DOC and DOCX file formats.

## Convert PDF to DOC

Aspose.PDF for C++ SDK lets you read a PDF file and [convert it to Microsoft Word Binary file format][5] (.doc) with just a couple of lines. The Document class of the API lets you read a PDF file from disc or stream, use the Save method for saving it in different file formats. Use the [SaveFormat][6] enumeration to specify the output file format as shown in the code sample below.

```
auto doc = MakeObject<Document>(u"..\\Data\\Document\\input.pdf");
doc->Save(u"..\\Data\\Document\\input_out.doc", SaveFormat:: Doc);
```

## Convert PDF to DOCX

DOCX is the modern Word Documents file format that is based on Office Open XML file format specifications. Aspose.PDF for C++ can [convert PDF files to DOCX][7] with the same simplicity as it converts to DOC file format. This is as illustrated in the following sample code.

```
auto doc = MakeObject<Document>(u"..\\Data\\Document\\input.pdf");
doc->Save(u"..\\Data\\Document\\input_out.docx", SaveFormat::DocX);
```

In a nutshell, the API lets you convert PDF files to several other file formats without you being worried about the underlying document architecture of source and output file formats. Want to try it out? Download your free copy of the [Aspose.PDF for C++ API][8] and get started in no time by following the detailed [developer guid][9]e from API documentation. In case of any queries, feel free to write to us on [Aspose.PDF forum][10] to get further assistance.




[1]: https://products.aspose.com/pdf/cpp
[2]: https://wiki.fileformat.com/word-processing/doc/
[3]: https://wiki.fileformat.com/word-processing/docx/
[4]: https://docs.aspose.com/display/pdfcpp/Convert+PDF+Files
[5]: https://docs.aspose.com/display/pdfcpp/Convert+PDF+to+DOC+and+DOCx+in+CPP#ConvertPDFtoDOCandDOCxinCPP-ConvertPDFtoDOC
[6]: https://apireference.aspose.com/cpp/pdf/namespace/aspose.pdf/#a53326a8c074ab80acf467385f9350fc2
[7]: https://docs.aspose.com/display/pdfcpp/Convert+PDF+to+DOC+and+DOCx+in+CPP#ConvertPDFtoDOCandDOCxinCPP-ConvertPDFtoDOCX
[8]: https://downloads.aspose.com/pdf/cpp
[9]: https://docs.aspose.com/display/pdfcpp
[10]: https://forum.aspose.com/c/pdf





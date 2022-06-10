---
title: 'Convert a Document using Aspose.Words'
seoTitle: "Convert a Document using Aspose.Words for .NET, Java, C++"
description: "Aspose.Words allows you the ability to convert a document from one of most popular formats to another without installing other applications or tools."
date: Fri, 03 Jul 2020 08:27:26 +0000
draft: false
url: /2020/07/03/convert-a-document-using-aspose.words/
author: Mary Gerasimova
summary: ''
tags: ['Convert a Document Cloud', 'Convert a document', 'Convert a document Aspose.Words', 'Convert documents from one format to another']
categories: ['Aspose.Words Product Family']
---



{{< figure align=center src="images/aspose.words_-150x150-1-e1594387398675.png" alt="Aspose.Words">}}


Converting documents from one format to another is one of the main features of Aspose.Words. Conversion in Aspose.Words consists of opening a document in one of the supported load formats and then saving it in another format.

Aspose.Words supports almost all common conversion combinations, for example:

*   DOC, DOCX, RTF to PDF or XPS,
*   DOC or DOCX to JPEG, TIFF, PNG,
*   DOCX to Markdown or HTML,
*   PDF to DOC, DOCX, or other Word formats,
*   and others.

Please note that this is not a complete list of possible conversions. You can check out [LoadFormat][1] that specifies all load or import formats and [SaveFormat][2] that specifies all save or export formats supported by Aspose.Words.

## How to Convert a Document

First, you need to load a document into Aspose.Words. Then you need to save this document in the required format. Follow these two simple steps and you will find out how easily Aspose.Words allows you to convert documents.

Note that you can specify additional options when saving a document to get the desired result. We will also discuss it below.

### How to Load a Document

To load a document pass the file name or the stream into one of the [Document][3] constructors. The format of the loaded document is determined automatically most of the times.

The following example shows how to load a document from a file:

```
// Load the document from the absolute path on disk.  
Document doc = new Document(dataDir + "TestDocument.docx");
```

### How to Save a Document

To save your document, use one of the Save methods. Aspose.Words automatically determines the desired save format from the file extension. You can save a document both to a file or a stream. For example, you can save a DOCX document as a PDF file.

The following example shows how to save a document to a file:

```
// Save the document as a PDF file.  
doc.Save(dataDir + "Document.pdf");
```

## Specify Advanced Conversion Options

When converting a document, you can set some advanced properties. Aspose.Words provides you with the [SaveOptions][4] class, which allows you to control the process of saving your document in the required format more precisely. Each save format has a corresponding class that holds the save options for this save format. For example, there is [HtmlSaveOptions][5] for saving to HTML/MHTML/EPUB format, or [PdfSaveOptions][6] for saving to PDF. You can read more about advanced properties in the article [‘Specify Save Options’][7] in the Aspose.Words documentation.

The following example shows how to convert a document from DOCX to PDF and set Aspose.Words to embed full fonts in the output document:

```
// Load the document from the file.
Document doc = new Document(dataDir + "TestDocument.docx");

// Aspose.Words embeds full fonts by default when EmbedFullFonts is set to true.
// The property below can be changed each time a document is rendered.
PdfSaveOptions options = new PdfSaveOptions();
options.EmbedFullFonts = true;

// The output PDF will be embedded with all fonts found in the document.
doc.Save(dataDir + "TestDocument.EmbedFullFonts.pdf", options);
```

## Variations of Conversions Supported by Aspose.Words

As mentioned above, Aspose.Words allows you to convert a document from one of most popular formats to another. This means that you can solve most of your conversion tasks using only Aspose.Words without installing special applications or tools. For example, you can easily and reliably convert a document from Microsoft Word formats such as DOC or DOCX to PDF or HTML, or from PDF or HTML to Markdown.

Study the ‘[Converting a Document][8]’ documentation section for more Aspose.Words conversion examples.

## See Also

To understand this question in more detail, look at the following articles in the Aspose blog:

*   [C# Convert Word Document to PDF][9]
*   [C# Create, Edit or Convert MS Word Documents][10]
*   [C#, Java Convert Word (DOC, DOCX) to Byte Array][11]
*   [Java Convert Word DOC/DOCX to PDF][12]
*   [C++ Convert Word DOC or DOCX to PDF][13]
*   [C++ Convert Word Document to Multipage TIFF Image][14]




[1]: https://apireference.aspose.com/words/net/aspose.words/loadformat
[2]: https://apireference.aspose.com/words/net/aspose.words/saveformat
[3]: https://apireference.aspose.com/net/words/aspose.words/document/constructors/main
[4]: https://apireference.aspose.com/words/net/aspose.words.saving/saveoptions
[5]: https://apireference.aspose.com/words/net/aspose.words.saving/htmlsaveoptions
[6]: https://apireference.aspose.com/words/net/aspose.words.saving/pdfsaveoptions
[7]: https://docs.aspose.com/display/wordsnet/Specify+Save+Options
[8]: https://docs.aspose.com/display/wordsnet/Converting+a+Document
[9]: https://blog.aspose.com/2020/01/02/convert-word-doc-docx-to-pdf-in-csharp-net-core/
[10]: https://blog.aspose.com/2020/01/08/csharp-word-automation-create-edit-process-word-documents/
[11]: https://blog.aspose.com/2019/12/09/convert-worddoc-docx-to-byte-array/
[12]: https://blog.aspose.com/2020/02/20/convert-word-doc-docx-to-pdf-in-java-programmatically/
[13]: https://blog.aspose.com/2020/04/10/convert-word-doc-or-docx-to-pdf-in-cpp/
[14]: https://blog.aspose.com/2019/11/07/aspose-words-for-cpp-19-10-released/






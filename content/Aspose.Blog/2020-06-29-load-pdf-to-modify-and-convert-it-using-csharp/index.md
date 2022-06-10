---
title: 'Load a PDF File to Further Modify and Convert It using C#'
seoTitle: "Load PDF and Convert It to Popular Formats using C#"
description: "Aspose.Words provides the ability to load a PDF document for its further modification. You can save such a PDF in any supported format."
date: Mon, 29 Jun 2020 18:10:51 +0000
draft: false
url: /2020/06/29/load-pdf-to-modify-and-convert-it-using-csharp/
author: Nazim Faour
summary: ''
tags: ['Convert PDF to DOCX in Csharp', 'Convert PDF to HTML Csharp', 'Load PDF Csharp']
categories: ['Aspose.Words Product Family']
---

In many cases, while working with a PDF document, you need to change it: copy, paste, drag and drop specific PDF content such as text, images, tables, and diagrams. It's fine to perform these options manually inside the same PDF file as long as you want to work with small parts of your document. But what if you want to perform the editing options in more complex scenarios such as creating a digital signature, merging multiple PDF documents, or reprocessing all the text in a PDF file?

**Aspose.Words** answers the question with a fast and accurate tool that allows you to load, edit, and convert PDF to any supported file formats such as DOCX, HTML, Markdown, and others. This article will guide you through the usage of these options both programmatically using C# and online.

## Features of Loading a PDF Document using C#

Usually, PDFs are used only for viewing, but sometimes you may need to edit or add something new to the existing PDF document.

Aspose.Words provides additional options to work with PDF documents such as:

*   Convert PDF to multiple formats and extract data.
*   [Print PDF documents][1] with a variety of printing options.
*   Encrypt and decrypt PDF as well as modify passwords, and others.

In addition to loading a PDF document, you can create PDF documents programmatically in C# and manage the PDF content such as:

*   Add, update, delete text and images.
*   Insert text and image in headers and footers.
*   Manipulate, export, and import annotations.
*   Add, modify, and remove bookmarks.
*   Add tables, graph objects during PDF generation, and others.

## Convert from PDF to the Desired Format using C#

One of the main features of Aspose.Words is the ability to easily and reliably [convert documents][2] [from one file format][3] to [another][4]. In Aspose.Words, converting a PDF document format to another format, such as DOCX, is a very simple process and can be accomplished with few lines of code. You can convert PDF to DOCX programmatically in C# by implementing the following conversion steps:

1.  Load a PDF document.
2.  Save the result to the target file format.

```
**Note:** You can apply some additional options when loading or saving a document.
```

Let’s describe the process of converting a PDF document into a DOCX file format in C# by going through the previous steps with all necessary programming details.

### Load a PDF Document

Most tasks that you want to perform with Aspose.Words will require you to load a document as a first step of the conversion process. When you load a PDF document into Aspose.Words, it builds its [DOM (Document Object Model)][5], and all document elements and formatting are simply loaded into memory. Use one of the [document constructors][6] to either create a blank document or load your PDF document. You can create a blank document with any necessary content or load your document from a stream, as it’s explained in the ['Creating or Loading a Document'][7] article.

The following example shows how to load a PDF document from a file in C#:

```
// Load your PDF document into a Document object using one of its constructors
// and the path to your file.
Document doc = new Document(@"C:\\DocumentName.pdf");
```

### Save a Document in Any Supported Format

Most tasks that you want to perform with Aspose.Words will require you to [save a document][8] as a final step. Aspose.Words supports many different save or export formats that are listed in the [SaveFormat][9] enumeration. Use one of the [Save][10] methods to save the result to a local file, for example, in the DOCX file format.

To achieve that programmatically in C#, invoke the Document.Save method on the **Document** object and specify the desired output format as DOCX by entering your file name with the “.docx” extension:

```
// Save your document as a DOCX file.
doc.Save(dataDir + "DocumentName.docx");
```

Congratulations, you have successfully managed to convert your PDF file to DOCX.

### Apply Additional Options

You can apply different [PDF save options][11] or [PDF load options][12], and here are a few examples, such as digital signatures, page range, and document open password. Let's learn more about them.

#### Add and Verify Digital Signatures

Aspose.Words allows you to sign a PDF document using the [DigitalSignatureDetails][13] PDF save option property. You need to upload a digital certificate from disk or from a certificate store and pass it to a new instance of the X509Certificate2 class.

The following code example shows how to sign a PDF document in C#:

```
// The path to the documents directory.
**string** dataDir = RunExamples.GetDataDir\_LoadingAndSaving();

// Create a simple document from scratch.
Document doc = **new** Document();
DocumentBuilder builder = **new** DocumentBuilder(doc);

// Load the certificate from disk.
// The other constructor overloads can be used to load certificates from different locations.
X509Certificate2 cert = **new** X509Certificate2(dataDir + "signature.pfx", "signature");

// Pass the certificate and details to the save options class to sign with.
PdfSaveOptions options = **new** PdfSaveOptions();
options.DigitalSignatureDetails = **new** PdfDigitalSignatureDetails();
dataDir = dataDir + "Document.Signed\_out.pdf";

// Save the document as PDF.
doc.Save(dataDir, options);
```

#### Set Page Range

To set the page range of loading your PDF document, you will need to use the [PageIndex][14] property to specify the index of the start page and the [PageCount][15] PDF load option property to set the total number of pages to load starting from the specified index:

```
**var** loadOptions = **new** PdfLoadOptions { PageIndex = 2, PageCount = 4 };  
**var** doc = **new** Document("YourDocumentName.pdf", loadOptions);
```

#### Open Protected PDF with Password

You can open an encrypted PDF document by specifying the password value directly in the PDF load options:

```
**var** loadOptions = **new** PdfLoadOptions { Password = "123456" };  
**var** doc = **new** Document("YourDocumentName.pdf", loadOptions);
```

## PDF Online Converter

If you’re not a programmer, then it’s better to use the online PDF converter. As a first step, all you have to do to convert PDF online is to point your Web browser to the following page on the Aspose Website at the [file converter tool][16].

Let’s guide you through the online conversion process step-by-step:

1.  Drag & drop or select a PDF file to upload by clicking on the button “Drop or Upload your files” as shown in the picture below.![](https://blog.aspose.com/wp-content/uploads/sites/2/2020/06/Drop-or-Upload-your-files.png)
2.  Select DOCX file format from the drop-down list, or choose a different file format.
3.  Click on the button "Convert" to convert your PDF file as shown in the picture below.![Convert your PDF][17]
4.  Click on the button “DOWNLOAD NOW” to download the conversion result as a DOCX file. Also, you can view the conversion result on **Aspose File Viewer** by clicking on the button “VIEW RESULTS”  as shown in the picture below.![View results][18]
5.  Congratulations, you have successfully managed to load, convert and save your PDF file to DOCX with our online file converter.

## See Also

If you want to achieve the opposite direction and load a Word document to PDF then you can read the following article: [Convert Word Document to PDF Programmatically in C# .NET – A Complete Guide][19].




[1]: https://docs.aspose.com/display/wordsnet/Print+a+Document+Programmatically+or+Using+Dialogs
[2]: https://docs.aspose.com/display/wordsnet/Converting+a+Document
[3]: https://apireference.aspose.com/net/words/aspose.words/loadformat
[4]: https://apireference.aspose.com/words/net/aspose.words/saveformat
[5]: https://docs.aspose.com/display/wordsnet/Aspose.Words+Document+Object+Model
[6]: https://apireference.aspose.com/words/net/aspose.words/document/constructors/main
[7]: https://docs.aspose.com/display/wordsnet/Creating+or+Loading+a+Document
[8]: https://docs.aspose.com/display/wordsnet/Saving+a+Document
[9]: http://www.aspose.com/api/net/words/aspose.words/saveformat
[10]: https://apireference.aspose.com/words/net/aspose.words/document/methods/save/index
[11]: https://apireference.aspose.com/words/net/aspose.words.saving/pdfsaveoptions/properties/index
[12]: https://apireference.aspose.com/
[13]: https://apireference.aspose.com/words/net/aspose.words.saving/pdfsaveoptions/properties/digitalsignaturedetails
[14]: https://apireference.aspose.com/
[15]: https://apireference.aspose.com/
[16]: https://products.aspose.app/words/conversion
[17]: https://blog.aspose.com/wp-content/uploads/sites/2/2020/06/convert-your-PDF.png
[18]: https://blog.aspose.com/wp-content/uploads/sites/2/2020/06/download-the-conversion-result.png
[19]: https://blog.aspose.com/2020/01/02/convert-word-doc-docx-to-pdf-in-csharp-net-core/






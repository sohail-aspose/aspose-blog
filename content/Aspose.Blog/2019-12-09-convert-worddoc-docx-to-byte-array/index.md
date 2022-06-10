---
title: 'Convert Word (DOC, DOCX) to Byte Array'
date: Mon, 09 Dec 2019 08:18:14 +0000
draft: false
url: /2019/12/09/convert-worddoc-docx-to-byte-array/
author: Muzammil Khan
summary: ''
tags: ['Aspose.Words for .NET', 'Aspose.Words for Java', 'C#', 'Convert DOC to Byte Array', 'Convert Document to Byte Array', 'conversion', 'convert document', 'java']
categories: ['Aspose.Words Product Family', 'Aspose.Total Product Family']
---



{{< figure align=center src="images/aspose.words_logo.png" alt="Convert Word (DOC, DOCX) to Byte Array C# Java">}}


[Aspose.Words API][1] provides the simplest way to convert a Microsoft Word [DOC][2] or [DOCX][3] document to a byte array in C# and Java.

The conversion of a Word document to a byte array is helpful when storing documents in the database and/ or then retrieving them from the database.

[Aspose.Words API][4] provides the functionality to manipulate Microsoft Word files without using Microsoft Word. If you do not have Aspose.Words API installed, please follow the instructions given on [installation][5] page for .NET and [installation][6] page for using with Java.

## Convert a Word Document to a Byte Array using C#

[Aspose.Words for .NET][7] can be used to convert a Document object to obtain a byte array representing the Document in any .NET application.  
The following code snippet demonstrates the conversion of a DOC file to a byte array.

```
// Load the document from disk.
Document doc = new Document("Sample.doc");

// Create a new memory stream.
MemoryStream outStream = new MemoryStream();
// Save the document to stream.
doc.Save(outStream, SaveFormat.Docx);

// Convert the document to byte form.
byte[] docBytes = outStream.ToArray();

// The bytes are now ready to be stored/transmitted.

// Now reverse the steps to load the bytes back into a document object.
MemoryStream inStream = new MemoryStream(docBytes);

// Load the stream into a new document object.
Document loadDoc = new Document(inStream);
// Save the document.
loadDoc.Save("loadDoc.docx",SaveFormat.Docx);
```

## Convert a Word Document to a Byte Array using Java

The following code snippet demonstrates the conversion of a DOC file to a byte array using [Aspose.Words for Java][8] API.

```
// Load the document.
Document doc = new Document("Sample.doc");

// Create a new memory stream.
ByteArrayOutputStream outStream = new ByteArrayOutputStream();
// Save the document to stream.
doc.save(outStream, SaveFormat.DOCX);

// Convert the document to byte form.
byte[] docBytes = outStream.toByteArray();

// The bytes are now ready to be stored/transmitted.

// Now reverse the steps to load the bytes back into a document object.
ByteArrayInputStream inStream = new ByteArrayInputStream(docBytes);

// Load the stream into a new document object.
Document loadDoc = new Document(inStream);
// Save the document.
loadDoc.save("loadDoc.docx",SaveFormat.Docx);
```

## See Also

*   [Convert Word DOCX/DOC to PDF in C# .NET – A Complete Guide][9]
*   [Convert Word DOC/DOCX to PDF in Java][10]




[1]: https://products.aspose.com/words
[2]: https://wiki.fileformat.com/word-processing/doc/
[3]: https://wiki.fileformat.com/word-processing/docx/
[4]: https://docs.aspose.com/display/wordsnet/Home
[5]: https://docs.aspose.com/display/wordsnet/Installation
[6]: https://docs.aspose.com/display/wordsjava/Installation
[7]: https://docs.aspose.com/display/wordsnet/Home
[8]: https://docs.aspose.com/display/wordsjava/Home
[9]: https://blog.aspose.com/2020/01/02/convert-word-doc-docx-to-pdf-in-csharp-net-core/
[10]: https://blog.aspose.com/2020/02/20/convert-word-doc-docx-to-pdf-in-java-programmatically/





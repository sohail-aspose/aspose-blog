---
title: 'Exceptions Thrown by Document Constructors Got Better'
date: Thu, 01 Feb 2007 10:47:00 +0000
draft: false
url: /2007/02/01/exceptions-thrown-by-document-constructors-got-better/
author: Romank
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---

According to many customers' requests, we have improved design and documentation related to exceptions thrown by the Document class constructors. This is a new improvement introduced in Aspose.Words for .NET 4.1

The _Document_ class represents a Microsoft Word document in Aspose.Words and a document is loaded from a file or stream using one of the Document constructors.

First, Aspose.Words automatically detects the format of the file (DOC, RTF, HTML or WordML) and then proceeds to load the document appropriately. When loading, the document is checked and validated against inconsistencies and corruption. Unfortunately, it is a fact of life that a lot of documents exist out there with different degrees of data corruption. Things like the unexpected number of cells, missing pieces and so on do occur quite often. Over the time, Aspose.Words matured to recognize and correct any inconsistencies in documents, but still, it cannot always finish loading a document successfully and therefore throws an exception.

In previous Aspose.Words versions, the type of the exception thrown when a document could not be loaded was not strictly specified. If the corruption was explicitly detected by Aspose.Words code, it would throw InvalidOperationException. But if the corruption was detected implicitly (e.g access to an element in an array using an invalid index), then an IndexOutOfRangeException would be thrown. Therefore, it was a strictly "all or nothing" situation for developers using Aspose.Words. If the document constructor throws, then it just means it cannot be loaded for whatever reason.

Our customers have repeatedly asked for a feature that would allow to distinguish some kinds of errors during document load so they can take different actions in their exception handling code. Recently, I was working on a project where Aspose.Words had to process thousands of files, some of the files were in the pre-Word 97 DOC format (not supported by Aspose.Words), some of the files were corrupted, some of the files were non DOC documents at all, although they had the DOC extension. The project had to sort unsupported and corrupted documents separately from the rest of the documents that would load normally and that was not possible and I had to redesign the exceptions.

The exceptions have now got organized as follows:

*   _UnsupportedFileFormatException_ \- thrown when Aspose.Words cannot recognize the file format, or recognizes it, but does not support (for example pre-Word97).
*   _FileCorruptedException_ \- thrown when the document appears to be corrupted such that Aspose.Words cannot load it.
*   _PleaseReportException_ \- thrown when the document is most likely valid but contains some undocumented or unusual structures that we would like you to send the document to us for a fix.

Depending on whether you load from a file or from the stream, there could be other arguments or .NET exceptions thrown, for a complete specification see _Document Constructors_.

After the work was done, I was happy to find that what we've done went well along with the guidelines in a recent post by Krzysztof Cwalina, How to Design Exception Hierarchies.

A few days ago I posted a question about exception documentation in the public API.

Here is an example of how the new exception classes can be used:

```
try
{
Console.WriteLine(“Processing file “ + file);
TestUtil.OpenSaveOpen(file);
}

catch (UnsupportedFileFormatException e)
{

// Catch unsupported file format exception because we want to move such files out of the main test dir. I think it is a good example of why you would need a separate exception class – to handle just this exception in a special way.
Console.WriteLine(“Unsupported file format. Moving file ‘” + file + “‘. “ + e.Message);
File.Move(file, @”C:\GoogleProof\Unsupported\” + Path.GetFileName(file));
}
catch (Exception e)
{
// Just log the error and let the program continue, we have to process heaps more other files and directories.
Console.Error.WriteLine(“File ‘” + file + “‘. “ + e.ToString());
}
```









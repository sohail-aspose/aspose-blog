---
title: 'Import Plain Text from .TXT to Word Document in C# and Java'
date: Wed, 04 Jul 2012 12:30:29 +0000
draft: false
url: /2012/07/04/import-plain-text-from-.txt-to-word-in-csharp-and-java/
author: Adam Skelton
summary: ''
tags: ['altchunk', 'chunk', 'release', 'rendering', 'signature line', 'txt']
categories: ['Aspose.Words Product Family']
---



{{< figure align=center src="images/aspose.words-logo2.jpg" alt="">}}


We have just released this month’s improvements to Aspose.Words for .NET and Java. This month’s releases incude more than 120 improvements to many areas of our component.

You can immediately download our latest Aspose.Words release from the following links:

*   [Aspose.Words for .NET 11.5.0][1]
*   [Aspose.Words for Java 11.5.0][2]

As usual, if you have any queries about the new release or our components, in general, we are glad to answer them in on our [support forums][3].

Here is a look at the biggest features included in this month's release:

## Import Text from Plain Text Formats

We are proud to announce that Aspose.Words now supports directly importing plain text format (.txt) into a new Aspose.Words **Document** **object**.

In previous versions of Aspose.Words this format was not directly supported during import but could still be achieved manually by reading the text and inserting it using **DocumentBuilder**. The reason plain text was not supported until now is due to the format being difficult to load in useful and reliable way, more specifically:

*   The different encoding used in text files can make it hard to auto-detect text files when no **LoadFormat** is specified.
*   Aspose.Words needs to have a smart way of parsing a text file so blocks of texts are imported into Aspose.Words as the types of nodes they most closely represent. For example, lines that start with 1), 2), 3) in plain text format are imported into Aspose.Words as a proper numbered list.

The new text import engine supports these features and more. It can be used by simply calling the document constructor with the appropriate string path or stream to a text file:

```
Document doc = new Document("MyTextFile.txt");
```

### Example

Here is an example of this feature in action:

#### **Source Text File:**



{{< figure align=center src="images/sample_input-1024x565.jpg" alt="Import text from txt to Word">}}


In the screen above you can see the lists in the text file are imported as real word lists. The paragraphs that start with spacing are imported with hanging indent to mimic the look of the text file.

## Support for AltChunk Content

AltChunks are a feature new to OOXML documents. They act a bit like the traditional INCLUDETEXT field in the way that they allow you to insert content from external sources and insert them into the document, however, they also provide more advanced features.

Until now documents containing AltChunk had that particular content skipped which resulted in the content going missing during conversion. Now, these documents are converted without any problems.

Currently, AltChunk is supported during conversions but there is no public API to work with this feature. If you have a requirement to working with AltChunk then please let us know. We are always adding new features and functionality to Aspose components.

## Rendering of Digital Signatures Lines

A signature line allows a digital signature to be added in visual form to any position in the document. This feature has been hotly requested from our customers after we added support for signature lines in Aspose.Words 11.3.0. During initial support the signature lines were only retained during conversion to other word formats that supported signature lines. If the document was converted to other formats such as DOC or PDF the visual aspects of the signature would be lost.

Starting in Aspose.Words 11.5.0 rendering of signature lines is fully supported during conversion to all formats. This includes formats that do not natively support signature line. In such a case the signature line object is converted to a regular image.




[1]: http://downloads.aspose.com/words/net
[2]: http://downloads.aspose.com/words/java
[3]: http://forum.aspose.com





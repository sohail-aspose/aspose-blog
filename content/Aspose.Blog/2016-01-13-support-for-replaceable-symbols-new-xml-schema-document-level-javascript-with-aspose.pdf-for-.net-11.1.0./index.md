---
title: 'Support for Replaceable Symbols, a New XML Schema and Document-level JavaScript for PDF Documents'
date: Wed, 13 Jan 2016 18:24:59 +0000
draft: false
url: /2016/01/13/support-for-replaceable-symbols-new-xml-schema-document-level-javascript-with-aspose.pdf-for-.net-11.1.0./
author: Codewarior
summary: ''
tags: ['Nayyer Shahbaz']
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/aspose_pdf-for-net.jpg" alt="aspose-pdf-for-net">}}


Aspose.PDF for .NET is among one of the top API's being used by developers across the globe for PDF file creation as well as manipulation. The ease of use, lightweight architecture, compatibility with almost all VisualStudio versions, .NET Frameworks, and almost all versions of Windows, are some of the features which have made this API favorite among developers. With every new release, we provide a bunch of new features and enhancements to cope with the requirements of our customers with an intent to make our API more robust to cater as many possible scenarios as we can. A new release of [Aspose.PDF for .NET 11.1.0][1] has already hit the download section and provides new features and enhancements already requested by our customers. Among these new features, there have been fixes towards various exceptions and bugs reported against earlier release versions.

## Replaceable symbols using TextFragment

Replaceable symbols are special symbols in a text string that can be replaced with corresponding content at run time.

When adding TextFragment to paragraphs collection of PDF documents, it does not support line feed inside the text. However in order to add text with a line feed, please use TextFragment with TextParagraph:

*   use "\\r\\n" or Environment.NewLine in TextFragment instead of single "\\n";
*   create TextParagraph object. It will add text with line splitting;
*   add the TextFragment with TextParagraph.AppendLine;
*   add the TextParagraph with TextBuilder.AppendParagraph.

{{< gist aspose-pdf 7e1330795d76012fcb04248bb81d45b3 "Examples-CSharp-AsposePDF-Text-RenderingReplaceableSymbols-RenderingReplaceableSymbols.cs" >}}

Please visit the following link for further details on [Rendering Replaceable Symbols during PDF creation.][2]

## Aspose.PDF for .NET XML Schema for DOM Approach

The Document Object Model (DOM) of the Aspose.PDF namespace is created using XML Schema Document (XSD) which can be found here: Aspose.PDF XML schema(DOM).xsd. This schema can be used to know the detailed information of all the elements and attributes that are supported by Aspose.PDF for .NET.

## Using Roman Numbers in TOC Entries

Headings are important parts of any document. Writers always try to make headings more prominent and meaningful to its readers. If there are more than one headings in a document, a writer has several options to organize these headings. One of the most common approaches to organize headings is to write headings in Numbering Style. Aspose.PDF for .NET supports following heading styles.

<figure class="wp-block-table"><table class=""><tbody><tr><td>**Heading Types</strong></td><td><strong>Description**</td></tr><tr><td>NumeralsArabic</td><td>Arab type,for example, 1,1.1,...</td></tr><tr><td>NumeralsRomanUppercase</td><td>Roman upper type, for example, I,I.II, ...</td></tr><tr><td>NumeralsRomanLowercase</td><td>Roman lower type, for example, i,i.ii, ...</td></tr><tr><td>LettersUppercase</td><td>English upper type, for example, A,A.B, ...</td></tr><tr><td>LettersLowercase</td><td>English lower type, for example, a,a.b, ...</td></tr></tbody></table></figure>

{{< gist aspose-pdf 7e1330795d76012fcb04248bb81d45b3 "Examples-CSharp-AsposePDF-Headings-ApplyNumberStyle-ApplyNumberStyle.cs" >}}

Further details can be found on [How to Apply Numbering Style in Heading.][3]

## Add Document-Level JavaScript

A new property named JavaScript is added in Document class which has JavaScript collection type and provides access to JAvaScript scenarios by its key. The JavaScript collection has the following properties and methods:

*   string this\[string key\] { get; set; } - Gets or sets JavaScript by its name
*   IList Keys - provides list of existing keys in JavaScript collection
*   bool Remove(string key) - removes JavaScript by its key.

```
Document doc = new Document();
doc.Pages.Add();
doc.JavaScript["func1"] = "function func1() { hello(); }";
doc.JavaScript["func2"] = "function func2() { hello(); }";
doc.Save("c:/PDFtest/39455_js.PDF");
Document doc1 = new Document("c:/PDFtest/39455_js.PDF");
IList keys = doc1.JavaScript.Keys;
Console.WriteLine("=============================== ");
foreach (string key in keys)
{
    Console.WriteLine(key + " ==> " + doc1.JavaScript[key]);
}

doc1.JavaScript.Remove("func1");
Console.WriteLine("Key 'func1' removed ");
Console.WriteLine("=============================== ");
```

## Miscellaneous Fixes

As well as the enhancements and features discussed above, there have been specific improvements regarding Footnote rendering, TOC rendering, PDF to HTML, HTML to PDF conversion features. Among these fixes, the PCL to PDF, SVG to PDF, PDF to Excel, PDF to DOC, PDF to TIFF, XML to PDF, TIFF to PDF conversion, conversion of PDF to PDF/A compliant documents, text replacement, rendering PDF files to XPS format are also improved. Please download and try the latest release of [Aspose.PDF for .NET 11.1.0][4].




[1]: https://downloads.aspose.com/pdf/net
[2]: https://docs.aspose.com/display/pdfnet/Replace+Text+in+a+PDF+Document#ReplaceTextinaPDFDocument-RenderingReplaceableSymbolsduringPDFcreation
[3]: https://docs.aspose.com/display/pdfnet/Working+with+Headings
[4]: https://downloads.aspose.com/pdf/net





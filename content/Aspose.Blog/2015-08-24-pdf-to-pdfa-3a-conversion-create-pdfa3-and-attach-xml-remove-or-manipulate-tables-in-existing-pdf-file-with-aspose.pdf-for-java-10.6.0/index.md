---
title: 'Convert PDF to PDF/A-3a, Create PDF/A_3a and Attach XML to PDF in Java'
date: Mon, 24 Aug 2015 06:14:35 +0000
draft: false
url: /2015/08/24/pdf-to-pdfa-3a-conversion-create-pdfa3-and-attach-xml-remove-or-manipulate-tables-in-existing-pdf-file-with-aspose.pdf-for-java-10.6.0/
author: Codewarior
summary: ''
tags: ['Nayyer Shahbaz', 'attach xml to pdf java', 'convert pdf to pdfa', 'convert pdf to pdfa java', 'java convert pdf to pdf/a', 'manipulate table in pdf', 'remove table from pdf java']
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/aspose-Pdf-for-Java_100.png" alt="Aspose.Pdf for .NET logo">}}


In every new release, we closely analyze our customers' requirements and focus even towards minor details, so that we come up with features which produce remarkable outputs and bring ease to their life by eliminating the hassle of writing huge lines of code. All this can be accomplished using a single API instead of numerous components/softwares. Empowering the API with new rich features and enhancements, a new release of [Aspose.PDF for Java 10.6.0][1] has been published. This version contains some amazing new features which enrich the API to create stunning applications with a vast variety of PDF creation as well as manipulation features. Astonish your customers through your applications by providing stunningly amazing features for PDF file creation/manipulation and surprise them with resultant files with great fidelity. The ease of use, extensive documentation, and free technical support are some of the salient features of our API's and we always strive to meet our customer's expectations because we believe customer satisfaction is our Quality. Indeed we have taken the responsibility of harder parts and provide you the APIs which provide out of the box features and have incredible capabilities to generate the output with even a couple of code lines. Like always, the new release is also empowered with some new features and enhancements.

## Convert PDF to PDF/A-3 with Compliance-level (3a, 3b)

[PDF to PDF/A conversion][2] and PDF/A compliance validation features have been supported by our API for quite some time and from time to time, we introduce modifications so that new enhancements are provided in these functionalities. The following code lines can help in converting PDF files to PDF/A\_3a compliant format.

{{< gist aspose-pdf 474c352a71ac9477aa0d604fd32e1c6a "Examples-src-main-java-com-aspose-pdf-examples-NewDocumentObject-docconversion-ConvertPDFToPDFAFormat-PDFToPDFA3aConversion.java" >}}

## Create PDF/A-3 and Attach XML File

Aspose.PDF for Java offers the feature to convert PDF files to PDF/A format and it also supports the capabilities of adding files as an attachment to PDF document. In case you have a requirement to attach files to PDF/A compliance format, then we recommend using PDF\_A\_3A value from com.aspose.pdf.PdfFormat enumeration, as according to [this post in Adobe community][3], PDF/A\_3a is the format that provides the feature to attach any file format as an attachment to PDF/A complaint file. However, once the file is attached, you should convert it into Pdfa-3a format again, in order to fix metadata. Please take a look at the following code snippet.

{{< gist aspose-pdf 474c352a71ac9477aa0d604fd32e1c6a "Examples-src-main-java-com-aspose-pdf-examples-NewDocumentObject-docconversion-ConvertPDFToPDFAFormat-CreatePDFA3AndAttachXMLFile.java" >}}

## Manipulate Tables in an Existing PDF Document

One of the earliest features supported by Aspose.PDF for Java is its capabilities of [Working with Tables][4] and it provides great support for adding tables in PDF files being generated from scratch or any existing PDF files. You also get the capability to dynamically create tables and place them inside PDF file. Starting this release, a new feature of searching and parsing simple tables that already exist in PDF document has been provided. A new class named com.aspose.pdf.TableAbsorber provides these capabilities. The usage of TableAbsorber is very much similar to the existing TextFragmentAbsorber class.

{{< gist aspose-pdf 474c352a71ac9477aa0d604fd32e1c6a "Examples-src-main-java-com-aspose-pdf-examples-NewDocumentObject-tables-ManipulateTablesInExistingPDF-.java" >}}

Features related to this functionality which still need implementation.

*   One of the customers has requested to fetch the data based on the blocks of table or borders (as given in the diagram) and colors as well.
*   Currently, TableAbsorber cannot recognize the table cell background color now. However, we expect to make this improvement in this future and a separate ticket is already created in our issue tracking system.
*   Another customer wants to get the contents of the column in the table. Currently, TableAbsorber cannot recognize tables without borders, but conversion to XLS works well in such cases. However, conversion to XLS is a workaround. An enhancement ticket has been logged to improve TableAbsorber for working with such table types.
*   A Customer wants to update the table in existing PDF dynamically. Including deleting / insertion of rows. This request is a bit difficult to implement and the current implementation of TableAbsorber cannot fulfill such requirements.
*   If you have a requirement of looking for text property in com.aspose.pdf.cells or BaseParagraph types, (such types are designed for adding new contents on the page), you must cast BaseParagraph to one of the inherited types. For example, the next code must help:

```
<code>for(com.aspose.pdf.Row row : (Iterable)table.getRows()) {
TextFragment updatedfragment = (com.aspose.pdf.TextFragment) row.getCells().get_Item(1).getParagraphs().get_Item(1);     
String text;     
if (updatedfragment != null)         
text = updatedfragment.getText(); } </code> 
```

## Remove Tables from Existing PDF

Aspose.Pdf for Java offers the capabilities to insert/create a table inside PDF document while it is being generated from scratch or you can also add the table object in any existing PDF document. However, you may have a requirement to Manipulate Tables in existing PDF where you can update the contents in existing table cells. However, you may come across a requirement to remove table objects from an existing PDF document. Please note that in order to remove the tables, we need to use TableAbsorber class to get hold of tables in existing PDF and then replace the table cell contents with blank characters and in order to remove the border, certain page region is redacted. The following code snippet shows the steps to delete table from the existing PDF document.

{{< gist aspose-pdf 474c352a71ac9477aa0d604fd32e1c6a "Examples-src-main-java-com-aspose-pdf-examples-NewDocumentObject-tables-RemoveTablesFromExistingPDF-.java" >}}

## Miscellaneous Fixes

As well as the enhancements and features discussed above, there have been specific improvements for PDF to HTML and HTML to PDF conversion features with better support for HTML5. Among these fixes, the PCL to PDF, SVG to PDF, PDF to Excel, PDF to DOC, PDF to TIFF and TIFF to PDF conversion, conversion of PDF to PDF/A compliant documents, text replacement, Filling of signature field with an image, flattening of PDF and rendering of PDF to XPS format, FloatingBox rendering, FootNote, EndNote and rendering of non-English (specifically Arabic) contents are also improved. Please download and try the latest release of [Aspose.PDF for Java 10.6.0][5].




[1]: https://downloads.aspose.com/pdf/java
[2]: https://docs.aspose.com/display/pdfjava/Convert+PDF+to+other+Formats
[3]: https://forums.adobe.com/thread/868219
[4]: https://docs.aspose.com/display/pdfjava/Working+with+Tables+-+DOM
[5]: https://downloads.aspose.com/pdf/java





---
title: 'OpenXPS Rendering, HTML Improvements and Many More Goodies in Aspose.Words 13.6.0'
date: Thu, 04 Jul 2013 13:46:32 +0000
draft: false
url: /2013/07/04/openxps-rendering-html-improvements-and-many-more-goodies-in-aspose.words-13.6.0/
author: Adam Skelton
summary: ''
tags: ['CustomXml', 'Html 5', 'OpenXps', 'SDT', 'XPS', 'document', 'import', 'structured document tags']
categories: ['Aspose.Words Product Family']
---



{{< figure align=center src="images/aspose.words_-150x150-1-e1594387398675.png" alt="Aspose.Words">}}


Aspose.Words has gained more than 600 new features and bug fixes this year so far, with many more coming with each monthly release. This month’s release includes a further 100+ improvements to Aspose.Words for .NET and Java.

You can download the latest release of Aspose.Words from the following links:

*   [Aspose.Words for .NET 13.6.0][1]
*   [Aspose.Words for Java 13.6.0][2]

Here is a look at the biggest features in this month’s release:

## Support for OpenXps Format

The [Open XML Paper Specification][3] (called OpenXPS for short) is an XML-based fixed document format often used in rendering and printing. The format is heavily based on and succeeds the existing XPS format and was standardized as an open document standard format by Ecma International in mid-2009.

Aspose.Words already supports the XPS format and provides high fidelity conversions from other documents to the XPS format. Support for OpenXPS was the next step as the format can now be widely adopted by many organisations now that it is standardized. It also appears as the default format used by Microsoft XPS Document Writer on the Windows 8 operating system.

To save a document in the OpenXPS format simply specify an output file name with the extension ".oxps" or use the new **SaveFormat.OpenXps** enumeration with either the appropriate overload of the **Document.Save** method or with the **XpsSaveOptions** class.

## Import of Malformed HTML Documents Improved

We have finished integration of a new HTML parser in both Aspose.Words for .NET and Java which conforms to the HTML 5 standards. This means that HTML documents loaded into Aspose.Words are now properly read and interpreted compared to the old parser which did not conform to HTML 5 standards and thus would sometimes result in incorrectly loaded documents or errors.

This new parser was the key to closing many previously reported bugs that stemmed from loading of malformed HTML into Aspose.Words. These files can now be successfully loaded by Aspose.Words and any inconsistencies with the file data skipped. This fix benefits anyone using Aspose.Words for loading or saving HTML documents in general as HTML parsing is improved all round.

## Support for Data Binding to Custom XML

In last month’s blog post we reported progress on the next version of the Structured Document Tag API. This month’s release includes further improvements to the API, including the hotly requested feature _Data Binding to Custom XML properties_. This involves a structured document tag in the document to link and display information from xml data inside the document. This feature is now supported so that the correct values show when saving or rendering a document. The API to add new links or edit existing ones is planned so stay tuned.




[1]: https://products.aspose.com/words/net
[2]: https://products.aspose.com/words/java
[3]: http://en.wikipedia.org/wiki/Open_XML_Paper_Specification





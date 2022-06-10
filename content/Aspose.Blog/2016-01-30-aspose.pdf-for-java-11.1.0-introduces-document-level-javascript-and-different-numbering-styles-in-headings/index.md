---
title: 'Support of Document-Level JavaScript and Different Numbering Styles in Headings in PDF Documents'
date: Sat, 30 Jan 2016 18:56:38 +0000
draft: false
url: /2016/01/30/aspose.pdf-for-java-11.1.0-introduces-document-level-javascript-and-different-numbering-styles-in-headings/
author: Tilal Ahmad
summary: ''
tags: ['Add document level JavaScript to PDF', 'Roman Numbers for TOC in PDF']
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/aspose_pdf-for-java2.jpg" alt="">}}


We are pleased to announce new version of Aspose.PDF for Java. Aspose.PDF for Java 11.1.0 includes all the features and enhancements introduced in Aspose.PDF for .NET 11.1.0. Now it supports Roman numbers style for heading in PDF documents and allows to add document level JavaScript.

Along with the above-stated enhancements, this release fixes a number of issues reported by our customers in the previous release. Some of these are PDF to PDFA, PDF to TIFF, PDF to PNG, HTML to PDF, PDF to HTML and TimeZone issue. Please check release notes of Aspose.PDF for Java 11.1.0 for the complete list.

The following sections describe some details regarding these newly added features/enhancements.

## Using Roman Numbers in TOC Entries

Headings are important parts of any document. Writers always try to make headings more prominent and meaningful to its readers. If there are more than one headings in a document, a writer has several options to organize these headings. One of the most common approaches to organize headings is to write headings in Numbering Style. Aspose.PDF for Java supports the following heading styles. Further details can be found on [How to Apply Numbering Style in Heading.][1]

<figure class="wp-block-table"><table class=""><tbody><tr><td>**Heading Types</strong></td><td><strong>Description**</td></tr><tr><td>NumeralsArabic</td><td>Arab type,for example, 1,1.1,…</td></tr><tr><td>NumeralsRomanUppercase</td><td>Roman upper type, for example, I,I.II, …</td></tr><tr><td>NumeralsRomanLowercase</td><td>Roman lower type, for example, i,i.ii, …</td></tr><tr><td>LettersUppercase</td><td>English upper type, for example, A,A.B, …</td></tr><tr><td>LettersLowercase</td><td>English lower type, for example, a,a.b, …</td></tr></tbody></table></figure>

## Add Document Level JavaScript

A new property named JavaScript is added in Document class which has JavaScript collection type and provides access to JAvaScript scenarios by its key.

```
//Add Document level JavaScript
Document doc = new Document();
doc.getPages().add();
doc.getJavaScript().set_Item(“func1″,”function func1() { hello(); }”);
doc.getJavaScript().set_Item(“func2”, “function func2() { hello(); }”);
doc.save(“E:/data/Doucment_level_js.pdf”);
//Remove Document level JavaScript by key
Document doc1 = new Document(“E:/data/Doucment_level_js.pdf”);
doc1.getJavaScript().remove(“func1”);
System.out.println(“Key ‘func1’ removed “);
doc1.save(“E:/data/Document_level_js_remove.pdf”);
```

## Aspose.PDF for Java Resources

The following resources will help you work with Aspose.Pdf for Java:

*   [Home page for Aspose.PDF for Java][2]
*   [Download Aspose.PDF for Java][3]
*   [Aspose.PDF product family forum][4] – Post your technical questions and queries, or any other problem you faced while running Aspose.PDF APIs.
*   [Aspose.PDF for Java online documentation][5] – help documentation and API reference documents.
*   [Enable Blog Subscription][6] – Do not limit yourself, you can keep yourself updated with the latest news on Aspose.PDF APIs, new features, fixes and other API related topics by subscribing to Aspose.PDF blog.
*   [Aspose.PDF for Java Examples][7] – Source code examples.




[1]: http://docs.aspose.com/display/pdfjava/Apply+Numbering+Style+in+Heading
[2]: https://products.aspose.com/pdf/java
[3]: https://downloads.aspose.com/pdf/java
[4]: http://forum.aspose.com
[5]: http://docs.aspose.com/display/pdfjava/Home
[6]: https://blog.aspose.com/
[7]: https://github.com/asposepdf/Aspose_Pdf_JAVA





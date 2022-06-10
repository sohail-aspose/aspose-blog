---
title: 'Support for Index Fields in Aspose.Words 13.5.0'
date: Sun, 23 Jun 2013 12:54:01 +0000
draft: false
url: /2013/06/23/support-for-index-fields-as-well-as-many-other-improvements-in-aspose.words-13.5.0/
author: Adam Skelton
summary: ''
tags: ['API', 'Index', 'SDT', 'Word', 'content controls', 'field', 'field update', 'pdf size', 'structured document tags']
categories: ['Aspose.Words Product Family']
---



{{< figure align=center src="images/aspose.words_-150x150-1-e1594387398675.png" alt="Aspose.Words">}}


This month’s release of Aspose.Words for .NET and Java contains 132 new features, bug fixes and general improvements to Aspose.Words.

You can immediately download the latest Aspose.Words release from the following links:

*   [Aspose.Words for .NET 13.5.0][1]
*   [Aspose.Words for Java 13.5.0][2]

Here is a closer look at just a few of the great features this update provides for you.

## Support for Updating INDEX Field by the Field Engine

An INDEX field in a Microsoft Word Document is an alphabetical look up list of interesting keywords in the document and the page number they are found on. Index entries are marked using index entry fields (the XE field).



{{< figure align=center src="images/IndexFieldWord.png" alt="An index field in a Microsoft Word document" caption="A document with a short paragraph containing index entry fields and the generated index in the next section.">}}


Starting with this release, Aspose.Words supports updating this field and can build the contents of the index field from scratch. Simply call **Document.UpdateFields** to update all fields in the document including the INDEX field.

## Work on the Structured Document Tag API v2 Commences

The second round of improvements to the Structured Document Tag API has begun. These improvements are to provide new features when working with structured documents tags that we couldn’t quite squeeze into the release of the first API.

This month release includes several new SDT features, including _Data Binding of Structured Document Tags to Document Properties_. This feature involves special structured document tags that are linked to a document property. Aspose.Words now supports these types of structured document tags so the correct value is used.

Keep an eye out for more SDT features and improvements in the next few releases as work on the API continues.

## Improved Font Embedding Behavior to Decrease Output File Size

In the previous few releases of Aspose.Words there have been improvements to reduce the file size of the documents created by Aspose.Words, especially in the domain of PDF output. Our developers have continued this work by improving on an existing option so that the types of fonts that are embedded when saving to PDF can be furthered controlled. This can result in a smaller PDF sizes which is useful feature for those who must produce rendered documents that are small as possible.




[1]: https://products.aspose.com/words/net
[2]: https://products.aspose.com/words/java





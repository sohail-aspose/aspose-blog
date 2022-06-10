---
title: 'Custom XML Parts in the API and Other Goodies in Aspose.Words 10.4'
date: Wed, 31 Aug 2011 10:28:41 +0000
draft: false
url: /2011/08/31/custom-xml-parts-in-the-api-and-other-goodies-in-aspose.words-10.4/
author: Romank
summary: ''
tags: ['Work with Custom XML Parts', 'customer XML data storage', 'customer XML parts']
categories: ['Aspose.Words Product Family']
---



{{< figure align=center src="images/aspose.words-logo2.jpg" alt="ASpose.Words icon">}}


In this post, I am going to tell you what we've been busy with during August 2011 and how this work resulted in the Aspose.Words 10.4.0 release.

We continue to maintain the code of our .NET and Java products in sync by using autoporting so you continue to get the same set of features and fixes in both products on the same day.

As usual, you can download Aspose.Words from:

*   [Aspose.Words for .NET 10.4.0][1]
*   [Aspose.Words f or Java 10.4.0][2]

## Custom XML Data Storage in the Public API

Custom XML Data Storage (or Custom XML Parts) are basically user-defined XML files that are stored inside an OOXML package. Aspose.Words has been known to support Custom XML Parts for some time already by preserving them during open/save operations.

What's new in this release is that you can now programmatically access, create, extract or delete Custom XML Parts using Aspose.Words. The following public members were added to Aspose.Words:

*   **Document.CustomXmlParts** - this property is your starting point to access Custom XML Data inside a document.
*   class **CustomXmlPart**
*   class **CustomXmlPartCollection**
*   class **CustomXmlSchemaCollection**

_Useful fact 1:_ Did you know that Custom XML Parts can be stored not only in OOXML documents. Microsoft Word binary DOC documents also support Custom XML Parts and Aspose.Words supports Custom XML Parts both in DOCX and DOC documents.

_Useful fact 2:_ In the following releases we are going to implement SDT (Content Controls) binding to Custom XML Data and support it in the public API and also in conversions and rendering.

## Custom Parts in the Public API

In addition to the well-known Custom XML Data Storage Parts described above, the ISO/IEC 29500 standard allows for "custom parts" to exist in an OOXML package. If some part has an explicit relationship to another part, and that relationship is not defined in ISO/IEC 29500, then this is considered an "unknown relationship". Unknown relationships are allowed and thus such custom parts are allowed. There is a bit more info about this in Doug Mahugh's post Arbitrary content in an OPC package. While Doug calls these parts "arbitrary content" or "payload part", we use the term "custom part" in Aspose.Words.

It is important to note that Custom Parts are somewhat obscure and the standard does not recommend using them. The standard recommends using Custom XML Data Storage Parts instead. But one of the most important differences between Custom XML Part and a Custom Part is that the former has to be XML while the latter can be any content.

While implementing support for Custom XML Parts in Aspose.Words we decided to implement support for Custom Parts too. Aspose.Words supports Custom Parts in the following ways:

*   Custom Parts that are related to the OOXML package itself are supported only. Custom parts that are related to other parts are ignored.
*   Aspose.Words preserves Custom Parts during DOCX open/save.
*   Public members **Document.PackageCustomParts**, **CustomPart**, **CustomPartCollection** allow to accessing, creating, extracting and deleting custom parts.

## Unified API for Loss of Fidelity Warnings

Many customers have requested this feature. You wanted to be able to find out if some data or formatting was lost during document conversion. The use case is that you have an important DOCX document to convert to PDF and you need to make sure it comes out correctly (e.g. looks like it was done by Microsoft Word). While Aspose.Words does this job very well, it sometimes can produce output that looks not the way you expected. Maybe it was a complex text wrapping option, maybe it was Right-to-Left text or something else that Aspose.Words does not yet support well. If any case, what you want is a list of all such issues that were encountered in the document. You don't want to hear "your system produces ugly PDF documents" from an angry customer of yours. You want an advance warning saying "converting this document has issues here and there" so you can decide what to do, for example, abort conversion or warn the customer.

We've been discussing the design for this feature for some time at Aspose because this API needs to be the same across all Aspose components. I am happy to announce that this Unified Load and Save Warnings API is now becoming available in Aspose.Words.

In Aspose.Words 10.4 we've added the following public members:

*   **LoadOptions.WarningCallback** property
*   **SaveOptions.WarningCallback** property
*   **IWarningCallback** interface
*   **WarningInfo** class
*   **WarningType** enum

By default, Aspose.Words does not collect any warnings. But if you implement the IWarningCallback interface and set the WarningCallback property in LoadOptions or SaveOptions, then Aspose.Words will call your method when it encounters conversion issues found in a document.

_Note:_ In Aspose.Words 10.4 there will be NO IWarningCallback warnings issued to you. We have created the infrastructure and the API, but the work of actually adding the warnings is now in progress. We expect to add all warnings to all format conversions in the next few releases.

## Fixes in the Field Update and Rendering Engines

You continue sending us useful test documents that feature either unusual or advanced formatting combinations and we continue analyzing them and improving Aspose.Words accordingly. This month's release almost entirely consists of such improvements or fixes. It includes better handling of the date/time formatting in fields, "clear" tab stops in styles, culture-specific decimal tab and many others. Looking forward to more of your documents.

## Samples and Demos on Linux

Demos are projects that are included in the Aspose.Words download. Samples are projects that are provided in a separate download. This month we tested and retested all of these projects to make sure they run smoothly on Linux. We tested both Aspose.Words for Java samples and Aspose.Words for .NET samples that you can run with Mono.

There is one known issue left: we use a Microsoft Access .mdb database in some of our sample projects and it proved difficult to find a suitable free database driver for .MDB that would work on Linux. We are probably going to replace .MDB in the samples with something else soon.

## Advances in Rendering to Graphics on Java

We were also busy working on finalizing the "rendering to graphics" feature in Aspose.Words for Java. This feature is now more complete. Here is what's new in Aspose.Words for Java 10.4:

*   **ShapeBase.getShapeRenderer**, **DrawingML.getShapeRenderer** methods, and the **ShapeRenderer** class to export individual shapes as images.
*   **Document.renderToScale**, **Document.renderToSize**, **ShapeRenderer.renderToScale**, **ShapeRenderer.renderToSize** methods to easily create images or thumbnails of a desired size.
*   **SaveFormat.TIFF** is now available and can be used in **Document.save**to convert document pages into TIFF images, including multi-frame TIFF. The compression can be specified using **ImageSaveOptions.setTiffCompression**, but due to JAI limitations color images can only be saved in the uncompressed mode, switching compression on will produce 1bpp output.
*   Fidelity improvements in line, arrows, brushes, gradients and text rendering to Graphics and images.

## Printing on Java

I was not supposed to say this right now, but yes, we have implemented the **Document.Print** methods and also the **AsposeWordsPrintDocument**class to allow printing of documents. This feature was available in Aspose.Words for .NET and it is finally coming to Aspose.Words for Java.

The reason I did not want to say this is because this feature is not "release ready" in the current 10.4 release. The printed document margins, page size, and orientation are not respected correctly. The documentation and code examples are also not complete. Everything will be in the proper shape by the end of September. In the meantime, you can just play with printing and plan on using it.

That's all from me now. See you next time.




[1]: https://downloads.aspose.com/words/net
[2]: https://downloads.aspose.com/words/java





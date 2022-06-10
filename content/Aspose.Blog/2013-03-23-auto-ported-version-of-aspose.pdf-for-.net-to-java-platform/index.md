---
title: 'Autoporting Aspose.Pdf for .NET to Java'
date: Sat, 23 Mar 2013 23:52:23 +0000
draft: false
url: /2013/03/23/auto-ported-version-of-aspose.pdf-for-.net-to-java-platform/
author: Codewarior
summary: ''
tags: ['Nayyer Shahbaz']
categories: ['Aspose.PDF Product Family']
---

In July 2011, we introduced Aspose.Pdf for .NET 6.0.0,  which merged the APIs for Aspose.Pdf for .NET and Aspose.Pdf.Kit for .NET into one. That release also introduced a new [Document Object Model][1] (DOM) approach to create new and manipulate existing PDF files. Prior to the new DOM, the Aspose.Pdf for .NET DOM could deal with individual objects when creating PDF files, but did not have any feature for dealing with individual objects inside existing PDFs. Furthermore, prior to version 6.0.0,  Aspose.Pdf for .NET and Aspose.Pdf.Kit for .NET were two separate products and customers had to use one for generating new document and another for manipulating existing PDF files.

Our customers have used the merged Aspose.Pdf for .NET API for over a year and from their feedback, they are happy having document generation and manipulation in a single product. The new DOM structure introduced under the Aspose.Pdf namespace has had lots of positive feedback on its capabilities as compared to legacy approaches. We still support the code-base of legacy products, but the new DOM structure is better better in terms of performance and offers some great features including:

*   Creating PDF Portfolios
*   Embedding fonts in existing PDF file
*   [Conversion of PDF for DOC][2]
*   Conversion of PDF to HTML
*   Conversion of XPS to PDF
*   Conversion of SVG to PDF
*   Convert CGM image to PDF
*   Get the resolution and dimensions of embedded images

## Porting Aspose.Pdf for .NET to Java

There has been a huge demand for the above features in Aspose.Pdf for Java and Aspose.Pdf.Kit for Java. In recent releases, we have introduced some useful features but the .NET version is still much more powerful than the Java one. So instead of continuing to provide the same product on different platforms with a different set of features and capabilities, we have decided to keep the products identical. To serve our Java customers with the same set of features that are available in Aspose.Pdf for .NET, we have worked hard to port the current Aspose.Pdf for .NET code-base to Java. The new, autoported, release will be a merged API (Aspose.Pdf for Java, Aspose.Pdf.Kit for Java and DOM API) so our Java customers will get the power of PDF generation, as well as manipulation, with a single API.

## Impact of Migration

We are well aware that change comes with a cost and for product developers, the first question that comes to mind is how much work/effort is required to migrate the existing code-base and make it compatible with the new product. Program Managers and product leads are more concerned about the time required for this migration because most of the time, they are under tight schedules and are usually not prepared for such surprises. So keeping all that in mind, we have tried our level best to keep the existing code modification to a minimum so that our customers don't get lost while switching between two versions.

## Structure of the Autoported Merged API

The version numbering of the new autoported version of Aspose.Pdf for Java will start from 4.0.0. In the first release there will be two JAR files: one will the be same as the current Aspose.Pdf for Java, and the other jar file will be the version that has been autoported from Aspose.Pdf for .NET. All the classes and enumerations of the new DOM structure will be under the **com.aspose.pdf** package and the classes and enumerations related to Aspose.Pdf.Kit for Java will be available under the **com.aspose.pdf.facades** package. In future releases, there will be a single JAR with all sets of functionality.

Aspose.Pdf.Kit for Java users can quickly migrate to the autoported version by removing references to aspose-pdf-kit-x.x.x.jar from their code and adding a reference to the new JAR file into the application class-path. Then update the package reference from **com.aspose.pdf.kit** to **com.aspose.pdf.facades**. However, the time required to learn and implement the new DOM depends on your needs and understanding of the new structure.

Please stay tuned for more blogs on this topic, as they will help you to better understand and migrate your code to the merged Aspose.Pdf for Java API.




[1]: http://en.wikipedia.org/wiki/Document_Object_Model
[2]: https://www.aspose.cloud/templates/aspose/App_Themes/V3/images/total/272x272/aspose_total-for-net.png





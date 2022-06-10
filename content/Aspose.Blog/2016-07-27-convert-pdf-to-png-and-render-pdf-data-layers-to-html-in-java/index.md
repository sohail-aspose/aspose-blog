---
title: 'Convert PDF to PNG and Render PDF Data Layers to HTML in Java'
date: Wed, 27 Jul 2016 16:47:27 +0000
draft: false
url: /2016/07/27/convert-pdf-to-png-and-render-pdf-data-layers-to-html-in-java/
author: Tilal Ahmad
summary: ''
tags: ['Convert PDF to PNG images in Java', 'PDF to HTML', 'PDF to PNG', 'Render PDF Data Layers to HTML in Java']
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/aspose_pdf-for-java2.jpg" alt="">}}


We are pleased to announce [Aspose.PDF for Java 11.7.0][1] release. This version includes PDF to PNG conversion performance enhancement in addition to the improvements/enhancements made in its equivalent .NET version. We have also fixed a number of issues in this release. Some of these are PDF to HTML, HTML to PDF, SVG to PDF, PDF to PDF/A, PDF to DOC(X), and PDF to Image. Please check release notes of Aspose.PDF for Java 11.7.0 for a complete list of bug fixed.

The following sections describe some details regarding these newly added enhancements.

## Rendering PDF Layers to HTML Separately

A PDF document can contain different data layers and you can have the requirement to render each layer separately as an HTML Layer element. We have introduced this feature in the current release, we need to set **ConvertMarkedContentToLayers** property to control the [layers rendering in PDF to HTML conversion][2] as following.

{{< gist aspose-pdf 474c352a71ac9477aa0d604fd32e1c6a "Examples-src-main-java-com-aspose-pdf-examples-AsposePdfExamples-DocumentConversion-PDFToHTMLRenderPDFDataLayersAsSeparateHTMLLayerElement-.java" >}}

## AutoFitToWindows Value in ColumnAdjustment Type Enum

We have introduced a new value AutoFitToWindows in ColumnAdjustment Type Enum in the current release. It will [adjust table columns to fit windows][3].

{{< gist aspose-pdf 474c352a71ac9477aa0d604fd32e1c6a "Examples-src-main-java-com-aspose-pdf-examples-AsposePdfExamples-Tables-AddTableInExistingPDFDocument-SetAutoFitToWindowPropertyInColumnAdjustmentTypeEnumeration.java" >}}

## Dash Line style of Graph objects

Sometimes we could have the requirement to create a [Graph Object with dashed line][4]. Now, we can easily achieve the requirement with GraphInfo object, as follows.

{{< gist aspose-pdf 474c352a71ac9477aa0d604fd32e1c6a "Examples-src-main-java-com-aspose-pdf-examples-NewDocumentObject-graphs-AddLineObjectToPDF-.java" >}}

## Enhancements

Following is a list of improvements included in this release.

*   Improved XPS to PDF conversion performance
*   Improved PDF to PNG conversion performance

## Aspose.PDF for Java Resources

The following resources will help you work with Aspose.Pdf for Java:

*   [Home Page for Aspose.PDF for Java][5]
*   [Download Aspose.PDF for Java][6]
*   [Aspose.PDF product family forum][7] – Post your technical questions and queries, or any other problem you faced while running Aspose.PDF APIs.
*   [Aspose.PDF for Java online documentation][8] – help documentation and API reference documents.
*   [Enable Blog Subscription][9] – Do not limit yourself, you can keep yourself updated with the latest news on Aspose.PDF APIs, new features, fixes and other API related topics by subscribing to our blog.
*   [Aspose.PDF for Java Examples][10] – We have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: https://downloads.aspose.com/pdf/java
[2]: https://docs.aspose.com/display/pdfjava/Convert+PDF+to+HTML+format#ConvertPDFtoHTMLformat-PDFtoHTML-RenderPDFdatalayersasaseparateHTMLLayerElement
[3]: https://docs.aspose.com/display/pdfjava/Add+Table+in+Existing+PDF+Document#AddTableinExistingPDFDocument-AutoFitToWindowpropertyinColumnAdjustmentTypeenumeration
[4]: https://docs.aspose.com/
[5]: http://products.aspose.com/pdf/java
[6]: http://downloads.aspose.com/pdf/java
[7]: http://forum.aspose.com
[8]: http://docs.aspose.com/display/pdfjava/Home
[9]: https://blog.aspose.com/
[10]: https://github.com/asposepdf/Aspose_Pdf_JAVA





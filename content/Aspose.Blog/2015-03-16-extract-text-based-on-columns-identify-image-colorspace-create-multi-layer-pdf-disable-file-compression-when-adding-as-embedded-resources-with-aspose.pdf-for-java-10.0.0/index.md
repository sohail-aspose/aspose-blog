---
title: 'Extract Text Based on Columns, Identify Image Colorspace, Create multi-layer PDF, Disable File Compression when Adding as Embedded Resources with Aspose.PDF for Java 10.0.0'
date: Mon, 16 Mar 2015 13:22:29 +0000
draft: false
url: /2015/03/16/extract-text-based-on-columns-identify-image-colorspace-create-multi-layer-pdf-disable-file-compression-when-adding-as-embedded-resources-with-aspose.pdf-for-java-10.0.0/
author: Codewarior
summary: ''
tags: ['Nayyer Shahbaz', 'Create a multi-layer PDF in Java', 'Extract text based on columns in PDF in Java', 'Identify image colorspace in PDF']
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/aspose-Pdf-for-Java_100.png" alt="Aspose.Pdf for Java logo">}}


The new release of [Aspose.PDF for Java 10.0.0][1] has been published and like previous versions, this release contains some new and great features which have already been supported in its sibling (Aspose.PDF for .NET). The following are the details of new features and enhancements introduced with this release.

## Identify if Image in PDF is Colored or Black & White

A PDF file may consist of Text, Image, Attachment, Graph, Annotations, and other elements and Aspose.PDF for Java provides the feature to add as well as manipulate the image in an existing PDF file. Different types of compression can be applied over images to reduce their size. The type of compression being applied over image depends upon the ColorSpace of source image i.e. if the image is Color (RGB), then apply JPEG2000 compression, and if it is Black & White, then JBIG2/JBIG2000 compression should be applied. Therefore identifying each image type and using an appropriate type of compression will create the best/optimized output. We may come across a requirement to determine image Color space and apply appropriate compression for the image to reduce PDF file size. Please visit the following link for related information on Identify if image inside PDF is Colored or Black & White.

The following code snippet shows the steps to Identify if the image inside PDF is Colored or Black & White.

{{< gist aspose-pdf 474c352a71ac9477aa0d604fd32e1c6a "Examples-src-main-java-com-aspose-pdf-examples-NewDocumentObject-images-IdentifyIfImageInsidePDFIsColoredOrBlackAndWhite-.java" >}}

## Extract text based on columns

In case we have a PDF document with more than one column (multi-column) PDF document and we need to extract the page contents while honoring the same layout, then Aspose.PDF for .NET is the right choice to accomplish this requirement. One approach is to reduce the font size of contents inside PDF documents and then perform text extraction. For further details, please visit [Extract text based+on columns][2].

The following code snippet can be used to fulfill this requirement.

{{< gist aspose-pdf 474c352a71ac9477aa0d604fd32e1c6a "Examples-src-main-java-com-aspose-pdf-examples-NewDocumentObject-text-ExtractTextBasedOnColumns-ExtractTextBasedOnColumns.java" >}}

In this new release, we also have introduced several improvements in TextAbsorber and in the internal text formatting mechanism. So now during the text extraction using ‘Pure’ mode, you may call setScaleFactor(..) method and it can be another approach to extract text from a multi-column PDF document besides the above stated approach. This scale factor may be set to adjust the grid which is used for the internal text formatting mechanism during text extraction. Specifying the ScaleFactor values between 1 and 0.1 (including 0.1) has the same effect as font reduction.

Specifying the ScaleFactor values between 0.1 and -0.1 is treated as zero value, but it makes the algorithm to calculate scale factor needed during extracting text automatically. The calculation is based on average glyph width of the most popular font on the page, but we cannot guarantee that in extracted text no string of column reaches the start of the next column. Please note that if ScaleFactor value is not specified, the default value of 1.0 will be used. It means no scaling will be carried out. If the specified ScaleFactor value is more than 10 or less than -0.1, the default value of 1.0 will be used.

We propose the usage of auto-scaling (ScaleFactor = 0) when processing large number of PDF files for text content extraction. Or manually set redundant reducing of grid width ( about ScaleFactor = 0.5). However you must not determine whether scaling is necessary for concrete document or not. If You set redundant reducing of grid width for the document (that doesn't need in it), the extracted text content will remain fully adequate. Please take a look over the following code snippet.

{{< gist aspose-pdf 474c352a71ac9477aa0d604fd32e1c6a "Examples-src-main-java-com-aspose-pdf-examples-NewDocumentObject-text-ExtractTextBasedOnColumns-UsingSetScaleFactorMethod.java" >}}

## Create Multi-layer PDF file

Layers can be used in PDF documents in many ways. You might have a multi-lingual file that you want to distribute and want the text in each language to appear on different layers, with the background design appearing on a separate layer. You might also create documents with animation that appears on a separate layer. One example could be to add a license agreement to your file, and you don’t want a user to view the content until they agree to the terms of the agreement.

{{< gist aspose-pdf 474c352a71ac9477aa0d604fd32e1c6a "Examples-src-main-java-com-aspose-pdf-examples-NewDocumentObject-AddLayersToPDFFile-.java" >}}

As well as the enhancements and features discussed above, there have been numerous fixes related to recently introduced PDF to DOC conversion, PDF to Excel conversion, PDF to HTML conversion, PDF to PDF/A conversion, XPS to PDF conversion, PDF to TIFF conversion, text replacement, text extraction, rendering PDF files to XPS and creating TOCs in PDF files. Please download and try the latest [Aspose.PDF for .NET 10.0.0][3] release.




[1]: https://downloads.aspose.com/pdf/java
[2]: https://docs.aspose.com/display/pdfjava/Extract+Text+from+PDF#ExtractTextfromPDF-Extracttextbasedoncolumns
[3]: https://downloads.aspose.com/pdf/java





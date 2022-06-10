---
title: 'Support of PDF/A_2U standard and Improved PDF Optimization in Aspose.Pdf for Java 16.12.0'
date: Thu, 12 Jan 2017 07:22:48 +0000
draft: false
url: /2017/01/12/support-pdfa_2u-standard-improved-pdf-optimization-aspose.pdf-java-16.12.0/
author: Tilal Ahmad
summary: ''
tags: []
categories: ['Aspose.PDF Product Family']
---

[![][1]](http://blog.aspose.com/wp-content/uploads/sites/2/2017/03/aspose-Pdf-for-Java.png)The new version of [Aspose.Pdf for Java, 16.12.0][2], has been released. As Java version of Aspose.Pdf is ported version of Aspose.Pdf for .NET, so it includes all the enhancements and improvements from the corresponding .NET version(16.12.0) along with the fixes of the bugs reported in previous versions of Aspose.Pdf for Java reported by our valued customers that makes it more stable and reliable release as compared to previous releases. We have improved PDF to DOCX, PDF to PPTX feature, PDF to PDFA standard conversion along with many other bug fixes. Please check the detailed release notes of Aspose.Pdf for Java 16.12.0, in order to get an idea about the new features/enhancements and improvements made in this release of Aspose.Pdf for Java.

Furthermore, If you are planning to upgrade the API from any previous version, we strongly recommend you to check the Public API Changes section of current release and other intermediate releases from release notes pages, to know what has been changed since your current revision of the API.

The following sections describe some details regarding these newly added features/enhancements.

## Support of PDF/A\_2U standard

We have introduced new PDFA standard, PDF/A\_2U, in Aspose.Pdf for Java 16.12.0. We have included a new value PDF\_A\_2U in PdfFormt enum. Please check following code snippet for new feature.

```
 String inFile = "Input.pdf";
String outFile = "Output.pdf";
String outLog = "log.xml";
Document doc = new Document(inFile);
PdfFormatConversionOptions opts = new PdfFormatConversionOptions(outLog, PdfFormat.PDF_A_2U, ConvertErrorAction.Delete);
doc.convert(opts);
doc.save(outFile); 
```

## PDF optimization feature improved

In this release we have improved the PDF optimization feature with introduction of some new properties in OptimizationOption class. Mainly resizing of the embedded images reduces the PDF file size, ResizeImages and MaxResolution properties for the purpose along with RemovePrivateInfo:

```
 Document document = new Document("input.pdf");
OptimizationOptions optimizationOptions =new OptimizationOptions();
optimizationOptions.setLinkDuplcateStreams(true);
optimizationOptions.setRemoveUnusedObjects(true);
optimizationOptions.setRemoveUnusedStreams(true);
optimizationOptions.setCompressImages(true);
optimizationOptions.setResizeImages(true);
optimizationOptions.setRemovePrivateInfo(true);
optimizationOptions.setImageQuality(50);
optimizationOptions.setMaxResoultion(75);
document.optimizeResources(optimizationOptions);
.... 
```

## Rendering a specific PDF page region to image

We have a requirement to render a specific PDF page region to image. We have introduced following new methods in ImageDevice and TiffDevice classes..

**getCropRectangle()**

**setCroptRectangle(com.aspose.pdf.Rectangle)**

```
 Document document = new Document("Input.pdf");
JpegDevice jpegDevice = new JpegDevice();
com.aspose.pdf.Rectangle rectangle = new com.aspose.pdf.Rectangle(200, 100, 400, 300);
jpegDevice.setCropRectangle(rectangle);
jpegDevice.process(document.getPages().get_Item(1), "Output.jpg"); 
```

## Aspose.Pdf for Java Resources

The following resources will help you work with Aspose.Pdf for Java:

*   [Home page for Aspose.Pdf for Java][3]
*   [Download Aspose.Pdf for Java][4]
*   [Pdf product family forum][5]– Post your technical questions and queries, or any other problem you faced while running Aspose.Pdf APIs.
*   Pdf for Java online documentation– help documentation and API reference documents.
*   [Enable Blog Subscription][6]– Do not limit yourself, you can keep yourself updated with the latest news on Aspose.Pdf APIs, new features, fixes and other API related topics by subscribing to Aspose.Pdf blog.
*   [Aspose.Pdf for Java Examples][7]– We have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: http://blog.aspose.com/wp-content/uploads/sites/2/2017/03/aspose-Pdf-for-Java.png
[2]: http://downloads.aspose.com/pdf/java/new-releases/aspose.pdf-for-java-16.12.0/
[3]: https://www.aspose.com/templates/aspose/App_Themes/V3/images/words/272x272/aspose_words-for-net.png
[4]: http://www.aspose.com/community/files/72/java-components/aspose.pdf-for-java/default.aspx
[5]: http://www.aspose.com/community/forums/aspose.pdf-product-family/20/showforum.aspx
[6]: https://blog.aspose.com/
[7]: https://github.com/asposepdf/Aspose_Pdf_JAVA





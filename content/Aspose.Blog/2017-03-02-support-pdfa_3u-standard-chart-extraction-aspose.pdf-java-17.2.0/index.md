---
title: 'Support of PDFA_3U Standard and Chart Extraction in Aspose.Pdf for Java 17.2.0'
date: Thu, 02 Mar 2017 03:24:38 +0000
draft: false
url: /2017/03/02/support-pdfa_3u-standard-chart-extraction-aspose.pdf-java-17.2.0/
author: Tilal Ahmad
summary: ''
tags: []
categories: ['Aspose.PDF Product Family']
---

[![][1]](http://blog.aspose.com/wp-content/uploads/sites/2/2017/03/aspose-Pdf-for-Java.png)The new version [Aspose.Pdf for Java, 17.2.0][2] has been released. This version includes support of PDFA\_3U standard, extraction of Graph Charts from PDF document and enhancement in PDF to TIFF conversion. As Aspose.Pdf for Java is auto ported version of Aspose.Pdf for .NET, so it includes all the enhancements and improvements introduced in its corresponding version of [Aspose.Pdf for  .NET version(17.2.0)][3] along with enhancements and improvements introduced in this version. Please check the detailed [release notes of Aspose.Pdf for Java 17.2.0][4], in order to get an idea about the new features/enhancements and improvements made in this release of Aspose.Pdf for Java.

Furthermore, If you are planning to upgrade the API from any previous version, we strongly recommend you to check the [Public API Changes section of current release][5] and other intermediate releases from release notes pages, to know what has been changed since your current revision of the API.

The following sections describe some details regarding these newly added features/enhancements.

## PDF to PDFA\_3U Conversion

We have introduced [support of PDFA\_3U][6] in this release. You can convert PDF to PDFA\_3U standard using following code snippet.

```
Document doc = new Document("inFile.pdf"); 
PdfFormatConversionOptions opts = new PdfFormatConversionOptions("outLog.txt", PdfFormat.PDF_A_3U, ConvertErrorAction.Delete);
doc.convert(opts);
doc.save("outFile.pdf"); 
```

## Chart extraction as image

Some of our customers asked for support of [Charts extraction from PDF document as image][7]. Chart object is placed as Marked Content object in PDF document. We have implemented a new method extractMarkedContentAsImage() in Aspose.Pdf for Java 17.2.0 to extract Marked Contents as image. Please check following code snippet to extract Chart objects.

```
//Open document
Document document = new Document("sample.pdf");
//instantiate PdfExtractor
PdfExtractor pdfExtractor = new PdfExtractor();
//Extract Chart objects as image in a folder
pdfExtractor.extractMarkedContentAsImages(document.getPages().get_Item(1), "C:/Temp/Charts_page_1");
document.close(); 
```

## PDF to Pixelated TIFF image

While converting PDF to compressed TIFF, customers requested [Pixelated TIFF output support][8]. We have implemented a new option Pixelated in com.aspose.pdf.devices.TiffSettings.IndexedConversionType class. Now it has two values: Pixelated and Simple. Simple is the default style of black and white conversion. Please find sample code as below:

```
//Open document
com.aspose.pdf.Document pdfDocument = new com.aspose.pdf.Document("Input.pdf");
//Create stream object to save the output image
java.io.OutputStream imageStream = new java.io.FileOutputStream("Image.tiff");
//Create Resolution object
com.aspose.pdf.devices.Resolution resolution = new com.aspose.pdf.devices.Resolution(300);
//instantiate TiffSettings object
com.aspose.pdf.devices.TiffSettings tiffSettings  = new com.aspose.pdf.devices.TiffSettings();
//set the compression of resultant TIFF image
tiffSettings.setCompression(com.aspose.pdf.devices.CompressionType.CCITT4);
//set the color depth for resultant image
tiffSettings.setDepth(com.aspose.pdf.devices.ColorDepth.Format4bpp);
//skip blank pages while rendering PDF to TIFF
tiffSettings.setSkipBlankPages(true);
//set image brightness
//tiffSettings.setBrightness(.5f);
//set IndexedConversion Type, default value is simple
tiffSettings.setIndexedConversionType(IndexedConversionType.Pixelated);
//Create TiffDevice object with particular resolution
com.aspose.pdf.devices.TiffDevice   tiffDevice = new com.aspose.pdf.devices.TiffDevice(2480, 3508,resolution,tiffSettings);
//Convert a particular page (Page 1) and save the image to stream
tiffDevice.process(pdfDocument,1,1,imageStream);
//Close the stream
imageStream.close(); 
```

## Improvements

In addition to above stated enhancements and improvements, this version also includes some other important bug fixes as well. There have been specific improvements regarding PDF to PDFA conversion, HTML to PDF, PCL to PDF and PDF to PPTX conversion. Please check [release notes of Aspose.Pdf for Java 17.2.0][9] for complete list of bug fixed.

## Aspose.Pdf for Java Resources

The following resources will help you work with Aspose.Pdf for Java:

*   [Home page for Aspose.Pdf for Java][10]
*   [Download Aspose.Pdf for Java][11]
*   [Pdf product family forum][12]– Post your technical questions and queries, or any other problem you faced while running Aspose.Pdf APIs.
*   Pdf for Java online documentation– help documentation and API reference documents.
*   [Enable Blog Subscription][13]– Do not limit yourself, you can keep yourself updated with the latest news on Aspose.Pdf APIs, new features, fixes and other API related topics by subscribing to Aspose.Pdf blog.
*   [Aspose.Pdf for Java Examples][14]– We have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: http://blog.aspose.com/wp-content/uploads/sites/2/2017/03/aspose-Pdf-for-Java.png
[2]: https://downloads.aspose.com/pdf/java/new-releases/aspose.pdf-for-java-17.2.0/
[3]: https://blog.aspose.com/2017/02/10/enhanced-watermark-annotation-footnote-aspose.pdf-.net-17.2.0/
[4]: https://docs.aspose.com/display/pdfjava/Aspose.Pdf+for+Java+17.2.0+Release+Notes
[5]: https://docs.aspose.com/display/pdfjava/Aspose.Pdf+for+Java+17.2.0+Release+Notes
[6]: https://docs.aspose.com/display/pdfjava/Convert+PDF+to+other+Formats#ConvertPDFtootherFormats-PDFtoPDF/A_3UConversion
[7]: https://docs.aspose.com/
[8]: https://docs.aspose.com/display/pdfjava/Convert+PDF+Page+to+Image#ConvertPDFPagetoImage-ConvertPDFPagestoPixelatedTIFFImages
[9]: https://docs.aspose.com/display/pdfjava/Aspose.Pdf+for+Java+17.2.0+Release+Notes
[10]: https://www.aspose.com/templates/aspose/App_Themes/V3/images/words/272x272/aspose_words-for-net.png
[11]: http://www.aspose.com/community/files/72/java-components/aspose.pdf-for-java/default.aspx
[12]: http://www.aspose.com/community/forums/aspose.pdf-product-family/20/showforum.aspx
[13]: https://blog.aspose.com/
[14]: https://github.com/asposepdf/Aspose_Pdf_JAVA





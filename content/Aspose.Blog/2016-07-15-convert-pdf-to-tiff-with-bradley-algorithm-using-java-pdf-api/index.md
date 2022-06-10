---
title: 'Convert PDF to TIFF with Bradley Algorithm using Java'
date: Fri, 15 Jul 2016 04:20:29 +0000
draft: false
url: /2016/07/15/convert-pdf-to-tiff-with-bradley-algorithm-using-java-pdf-api/
author: Tilal Ahmad
summary: ''
tags: []
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/aspose_pdf-for-java.jpg" alt="">}}


[Aspose.PDF for Java 11.6.0][1] has been released. We are pleased to announce that this version of Aspose.PDF for Java includes same features and enhancements introduced in Aspose.PDF for .NET 11.6.0. Some of these are support of Bradley algorithm in PDF to TIFF conversion, improved text extraction, Adding image with filter type and support of different styles of  page number in Page number stamp.

The following sections describe some details regarding these newly added enhancements.

## PDF to TIFF - Use Bradley Algorithm

We received a requirement to convert a PDF document to TIFF using Bradley algorithm, The feature was implemented in Aspose.PDF for .NET version at first place and now it is also available in Java version of Aspose.PDF.

```
String outputImageFile = "OutputFile.tif";
String outputBinImageFile = "OutputFile_binary.tif";
//open document
com.aspose.pdf.Document pdfDocument = new com.aspose.pdf.Document("Input.pdf");
//create Resolution object
Resolution resolution = new Resolution(300);
//create TiffSettings object
TiffSettings tiffSettings = new TiffSettings();
tiffSettings.setCompression(CompressionType.LZW);
tiffSettings.setDepth(com.aspose.pdf.devices.ColorDepth.Format1bpp);
//create TIFF device
TiffDevice tiffDevice = new TiffDevice(resolution, tiffSettings);
//convert a particular page and save the image to stream
tiffDevice.process(pdfDocument, outputImageFile);
InputStream inStream = new FileInputStream(outputImageFile);
OutputStream outStream = new FileOutputStream(outputBinImageFile);
tiffDevice.binarizeBradley(inStream, outStream, 0.1);
inStream.close();
outStream.close();
```

## Custom Page Number Style

Now we can add page number in existing PDF document, with different Page number styles such as I, II, III, or A, B, C instead of just the typical 1, 2, 3. In order to accomplish this requirement, NumberingStyle property has been introduced, which accepts the values from NumberingStyle enumeration. Specified below are values offered in this enumeration.

*   LettersLowercase
*   LettersUppercase
*   NumeralsArabic
*   NumeralsRomanLowercase
*   NumeralsRomanUppercase

### DOM Approach```
Document doc = new Document("input.pdf");
PageNumberStamp pst = new PageNumberStamp();
PageLabel label1 = new PageLabel();
label1.setNumberingStyle(NumberingStyle.NumeralsRomanUppercase);
label1.setStartingValue(1);
doc.getPageLabels().updateLabel(0, label1);
pst.setNumberingStyle(NumberingStyle.NumeralsRomanUppercase);
for (Page page : (Iterable<Page>) doc.getPages())
{
pst.put(page);
}
doc.save("output.pdf");
```

### Facades Approach```
com.aspose.pdf.facades.PdfFileStamp pst = **new** PdfFileStamp();
pst.bindPdf("input.pdf");
pst.setNumberingStyle(NumberingStyle.NumeralsRomanUppercase);
pst.addPageNumber("#");
pst.save("output.pdf");
```

## Adding Image with Filter Type

Sometime customer has requirement to decrease PDF size after adding image into PDF document and he can use OptimizationOptions to compress the PDF. In this release we have introduced an ImageFilterType property to achieve this goal when adding image to PDF. The user has to use Jpeg2000 decoder to add image on the page (decrease the size of image up to 30% compare with old one) as following.

```
....
//get the page where image needs to be added
Page page = pdfDocument.getPages().get_Item(1);
//load image into stream
InputStream image = new FileInputStream("image.png");
//add image to Images collection of Page Resources
page.getResources().getImages().addWithImageFilterType(image, ImageFilterType.Jpeg2000);
//using GSave operator: this operator saves current graphics state
page.getContents().add(new Operator.GSave());
....
```

## Improved Text Extraction

We have introduced a new field MemorySaving in TextFormattingMode class, it skips the non-text commands and consumes less memory, but please note performance rise is insignificant.

```
Document pdfDocument = new Document(inFile);
//create TextAbsorber object to extract text
TextAbsorber textAbsorber = new TextAbsorber(new TextExtractionOptions(TextExtractionOptions.TextFormattingMode.MemorySaving));
//accept the absorber for all the pages
pdfDocument.getPages().accept(textAbsorber);
//get the extracted text
String extractedText = textAbsorber.getText();
```

## Miscellaneous Fixes

This version also includes some important bug fixes along with above stated enhancements. There have been specific improvements regarding printing, XPS to PDF, HTML to PDF, PDF to HTML, PDF to PDF/A, PDF to Image, Html text rendering and some other. Please check release notes of [Aspose.PDF for Java 11.6.0][2] for complete list of bug fixed.

## Aspose.PDF for Java Resources

The following resources will help you work with Aspose.Pdf for Java:

*   [Home page for Aspose.PDF for Java][3]
*   [Download Aspose.PDF for Java][4]
*   [Aspose.PDF product family forum][5] – Post your technical questions and queries, or any other problem you faced while running Aspose.PDF APIs.
*   [Aspose.PDF for Java documentation][6] – help documentation and API reference documents.
*   [Enable Blog Subscription][7] – Do not limit yourself, you can keep yourself updated with the latest news on Aspose.PDF APIs, new features, fixes and other API related topics by subscribing to Aspose.PDF blog.
*   [Aspose.PDF for Java Examples][8] – We have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: https://downloads.aspose.com/pdf
[2]: http://www.aspose.com/downloads/pdf/java/new-releases/aspose.pdf-for-java-11.6.0/
[3]: https://www.aspose.com/templates/aspose/App_Themes/V3/images/words/272x272/aspose_words-for-net.png
[4]: https://downloads.aspose.com/pdf
[5]: http://www.aspose.com/community/forums/aspose.pdf-product-family/20/showforum.aspx
[6]: https://docs.aspose.com/pdf/java
[7]: https://blog.aspose.com/
[8]: https://github.com/asposepdf/Aspose_Pdf_JAVA





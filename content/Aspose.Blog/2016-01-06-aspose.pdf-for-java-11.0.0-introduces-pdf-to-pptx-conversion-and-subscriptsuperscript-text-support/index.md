---
title: 'Convert PDF to PPTX and Add Subscript/Superscript Text in PDF using Java'
date: Wed, 06 Jan 2016 04:20:04 +0000
draft: false
url: /2016/01/06/aspose.pdf-for-java-11.0.0-introduces-pdf-to-pptx-conversion-and-subscriptsuperscript-text-support/
author: Tilal Ahmad
summary: ''
tags: ['Aspose.Products', 'Add Subscript or Superscript Text in PDF in Java', 'Convert PDF to PPTX']
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/aspose_pdf-for-java1.jpg" alt="">}}


We are pleased to announce a new release of [Aspose.PDF for Java 11.0.0][1] and now it is available in the Aspose download section. It is the auto-ported version of its counterpart i.e Aspose.PDF for .NET 11.0.0, so it includes the same features and enhancements. It includes PDF to PPTX conversion and subscript/superscript text support along with many other features and enhancements, we also have made significant progress in terms of bug fixing of issues reported against earlier released versions in this new release.

As well as the enhancements and features discussed above, there has been a specific improvement for printing features, using font files from Windows on Linux, PDF to HTML and HTML to PDF. Some other fixes are the PCL to PDF, PDF to PNG, PDF to TIFF, conversion of PDF to PDF/A compliant documents and flattening of PDF. Please check release notes of Aspose.PDF for Java 11.0.0 for the complete list.

The following sections describe some details regarding these newly added features/enhancements.

## PDF to PPTX Conversion

We have an API named [Aspose.Slides][2] which offers the feature to create as well as manipulate PPT/PPTX presentations. This API also provides the feature to convert PPT/PPTX files to PDF format. Recently many of our customers requested a feature to transform PDF files to PPTX format, and we are pleased to share that this new release of Aspose.PDF for Java offers this great feature. In this version of Aspose.PDF for Java, we have introduced a feature to transform PDF documents into PPTX format. During this conversion, the individual pages of the PDF file are converted to separate slides in the PPTX file. So in order to accomplish this requirement, you only need to instantiate an object of PptxSaveOptions class and pass it as the second argument to Document.save(..) method. For further details, please take a look over [Convert PDF to PPTX][3].

## Support of Superscript in TextState

In order to accomplish this requirement, you may consider setting TextState.Superscript and TextState.Subscript properties of TextSegment and TextFragment objects. Please take a look at the following code snippet.

```
Document document = new Document();
com.aspose.pdf.Page page = document.getPages().add();
//Superscript example
TextFragment fragment1 = new TextFragment();
TextSegment seg11 = new TextSegment(“8”);
fragment1.getSegments().add(seg11);
TextSegment seg12 = new TextSegment(“th”);
fragment1.getSegments().add(seg12);
seg12.getTextState().setSuperscript(true);
TextSegment seg13 = new TextSegment(” M”);
fragment1.getSegments().add(seg13);
TextSegment seg14 = new TextSegment(“lle”);
fragment1.getSegments().add(seg14);
seg14.getTextState().setSuperscript(true);
TextSegment seg15 = new TextSegment(” Blip”);
fragment1.getSegments().add(seg15);
TextSegment seg16 = new TextSegment(“42”);
seg16.getTextState().setSuperscript(true);
fragment1.getSegments().add(seg16);
TextSegment seg17 = new TextSegment(” x”);
fragment1.getSegments().add(seg17);
TextSegment seg18 = new TextSegment(“2n”);
seg18.getTextState().setSuperscript(true);
fragment1.getSegments().add(seg18);
page.getParagraphs().add(fragment1);
//Subscript example
TextFragment fragment2 = new TextFragment();
TextSegment seg21 = new TextSegment(“C”);
fragment2.getSegments().add(seg21);
TextSegment seg22 = new TextSegment(“2”);
fragment2.getSegments().add(seg22);
seg22.getTextState().setSubscript(true);
TextSegment seg23 = new TextSegment(“H”);
fragment2.getSegments().add(seg23);
TextSegment seg24 = new TextSegment(“5”);
fragment2.getSegments().add(seg24);
seg24.getTextState().setSubscript(true);
TextSegment seg25 = new TextSegment(“OH + 3O”);
fragment2.getSegments().add(seg25);
TextSegment seg26 = new TextSegment(“2”);
seg26.getTextState().setSubscript(true);
fragment2.getSegments().add(seg26);
TextSegment seg27 = new TextSegment(” —> 2CO”);
fragment2.getSegments().add(seg27);
TextSegment seg28 = new TextSegment(“2”);
seg28.getTextState().setSubscript(true);
fragment2.getSegments().add(seg28);
TextSegment seg29 = new TextSegment(” + 3H”);
fragment2.getSegments().add(seg29);
TextSegment seg210 = new TextSegment(“2”);
seg210.getTextState().setSubscript(true);
fragment2.getSegments().add(seg210);
TextSegment seg211 = new TextSegment(“O;”);
fragment2.getSegments().add(seg211);
page.getParagraphs().add(fragment2);
document.save(myDir+"superscript_test.pdf");
```

You can set TextState.FontSize and TextState.LineSpacing for TextSegment or TextFragment objects as normal when setting Superscript property. However, if you need to set specific font (e.g. Arial) and superscript, please try using the following code snippet.

```
TextFragment fragment1 = new TextFragment();
TextSegment seg11 = new TextSegment(“8”);
seg11.getTextState().setFont(FontRepository.findFont(“Arial”));
fragment1.getSegments().add(seg11);
TextSegment seg12 = new TextSegment(“th”);
seg12.getTextState().setFont(FontRepository.findFont(“Arial”));
seg12.getTextState().setSuperscript(true);
fragment1.getSegments().add(seg12);
```

In the above-specified code snippet, the font information is set for TextSegement object because setting the font for TextFragment leads to the unification of text segments properties, and individual properties of segments will be lost. So following code snippet cannot be used.

```
TextFragment fragment1 = new TextFragment(); 
fragment1.getTextState().setFont(FontRepository.findFont("Arial"));
```

Also please note that we use following values for glyph transformation: **superscript/subscript size 58.3%, subscript position -33.3%, superscript position +33.3%**. These values match to [default values of Adobe products.][4] However, if you have a requirement to modify these glyph transformation parameters, please feel free to contact and we may consider implementing a separate enhancement.

## Aspose.Pdf for Java Resources

The following resources will help you work with Aspose.PDF for Java:

*   [Home page for Aspose.PDF for Java][5]
*   [Download Aspose.PDF for Java][6]
*   [Aspose.PDF product family forum][7] – Post your technical questions and queries, or any other problem you faced while running Aspose.PDF APIs.
*   [Aspose.PDF for Java online documentation][8] – help documentation and API reference documents.
*   [Enable Blog Subscription][9] – Do not limit yourself, you can keep yourself updated with the latest news on Aspose.PDF APIs, new features, fixes and other API related topics by subscribing to Aspose.PDF blog.
*   [Aspose.PDF for Java Examples][10] – We have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: https://downloads.aspose.com/pdf/java
[2]: https://products.aspose.com/slides/java
[3]: http://docs.aspose.com/display/pdfjava/Convert+PDF+to+PPTX
[4]: https://en.wikipedia.org/wiki/Subscript_and_superscript#Desktop_publishing
[5]: https://products.aspose.com/pdf/java
[6]: https://downloads.aspose.com/pdf/java
[7]: http://forum.aspose.com
[8]: http://docs.aspose.com/display/pdfjava/Home
[9]: https://blog.aspose.com/category/pdf/
[10]: https://github.com/asposepdf/Aspose_Pdf_JAVA





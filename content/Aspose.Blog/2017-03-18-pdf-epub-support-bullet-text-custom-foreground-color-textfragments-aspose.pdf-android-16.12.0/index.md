---
title: 'Convert PDF Files to EPUB in Android using Java'
date: Sat, 18 Mar 2017 18:00:14 +0000
draft: false
url: /2017/03/18/pdf-epub-support-bullet-text-custom-foreground-color-textfragments-aspose.pdf-android-16.12.0/
author: Codewarior
summary: ''
tags: ['Nayyer Shahbaz']
categories: ['Aspose.PDF Product Family']
---

We are pleased to announce that the capability of converting PDF files to EPUB format, the functionality of adding bullet text inside PDF document, and the leverage of setting foreground color for text inside PDF document has been provided in the recent release of Aspose.PDF for Android 16.12.0. Starting this release, we also have adopted a new mechanism for version numbering i.e. Year.Month.BuildNumber, as it provides better mechanism to keep track of product release in accordance to specific month of a year and this approach, is being followed across the board for all the products.

## Convert PDF to EPUB in Android

EPUB (short for electronic publication) is a free and open e-book standard from the International Digital Publishing Forum (IDPF). Files have the extension .epub and we have been receiving lots of requests from our customers regarding the support for this format. The conversion of PDF file to EPUB format is made possible with the introduction of EpubSaveOptions class. The following code snippet shows the steps to create a PDF document from the beginning where sample TextFragment is placed inside PDF document and then files is saved in EPUB format.

```
 //generate a new document
com.aspose.pdf.Document pdfDocument = new com.aspose.pdf.Document();
com.aspose.pdf.Page p = pdfDocument.getPages().add();
com.aspose.pdf.TextFragment tf = new com.aspose.pdf.TextFragment("Hello World!");
p.getParagraphs().add(tf);
//reload the document after generation
java.io.ByteArrayOutputStream baos = new java.io.ByteArrayOutputStream();
pdfDocument.save(baos);
pdfDocument = new com.aspose.pdf.Document(new java.io.ByteArrayInputStream(baos.toByteArray()));
//convert into epub using SaveFormat
pdfDocument.save("epub_out.epub", com.aspose.pdf.SaveFormat.Epub);
```

In case you need to convert any existing PDF file, you simply need to load the file in Document object, instantiate EpubSaveOptions instance and pass this object as second argument to Save(..) method of Document object. Please take a look over the following code snippet.

```
String inFile = "input.pdf";
String outFile = "epub_test_out.epub";
// load a source PDF file
com.aspose.pdf.Document pdfDocument = new com.aspose.pdf.Document(inFile);
// instantiate EpubSaveOptions object
com.aspose.pdf.EpubSaveOptions options = new com.aspose.pdf.EpubSaveOptions();
// specify the content recognition mode as Flow
options.ContentRecognitionMode = com.aspose.pdf.EpubSaveOptions.RecognitionMode.Flow;
// save the file in EPUB format
pdfDocument.save(outFile, options);
```

You may consider visiting the following link for further details on [Converting a PDF File to EPUB format.][1]

## Setting RGB Color as Text Foreground Color

Aspose.PDF for Android provides the capabilities to add as well as manipulate text inside PDF file. While adding text, we can set formatting for text objects and also we can use setForegroundColor(..) method of TextSegment class, which takes Color object as an argument. Please take a look over following code snippet.

```
//Instantiate Pdf object by calling its empty constructor
Document doc = new Document();
//Create a section in the Pdf object
Page page = doc.getPages().add();
TextFragment fragment = new TextFragment("");
TextSegment segment = new TextSegment("Different RGB color to the text:");
TextState ts = new TextState();
ts.setFontSize(12.0f);
ts.setFont(FontRepository.findFont("Arial"));
ts.setHorizontalAlignment(HorizontalAlignment.Center);
ts.setForegroundColor(new Color(125, 125, 125));
segment.setTextState(ts);
TextSegment segment1 = new TextSegment("255,0,0/ ");
TextState ts1 = new TextState();
ts1.setFontSize(12.0f);
ts1.setFont(FontRepository.findFont("Arial"));
ts1.setHorizontalAlignment(HorizontalAlignment.Center);
ts1.setForegroundColor(new Color(255, 0, 0));
segment1.setTextState(ts1);
TextSegment segment2 = new TextSegment("0,255,0/ ");
TextState ts2 = new TextState();
ts2.setFontSize(12.0f);
ts2.setFont(FontRepository.findFont("Arial"));
ts2.setHorizontalAlignment(HorizontalAlignment.Center);
ts2.setForegroundColor(new Color(0, 255, 0));
segment2.setTextState(ts2);
TextSegment segment3 = new TextSegment("0,0,255/ ");
TextState ts3 = new TextState();
ts3.setFontSize(12.0f);
ts3.setFont(FontRepository.findFont("Arial"));
ts3.setHorizontalAlignment(HorizontalAlignment.Center);
ts3.setForegroundColor(new Color(0, 0, 255));
segment3.setTextState(ts3);
TextSegment segment4 = new TextSegment("#00156E");
TextState ts4 = new TextState();
ts4.setFontSize(12.0f);
ts4.setFont(FontRepository.findFont("Arial"));
ts4.setHorizontalAlignment(HorizontalAlignment.Center);
ts4.setForegroundColor(com.aspose.pdf.Color.parse("#00156E").toRgb());
segment4.setTextState(ts4);
fragment.getSegments().add(segment);
fragment.getSegments().add(segment1);
fragment.getSegments().add(segment2);
fragment.getSegments().add(segment3);
fragment.getSegments().add(segment4);
page.getParagraphs().add(fragment);
doc.save("resultantfile.pdf");
```

## Add Bullet Text in PDF Document

A PDF file is comprised of Text, Images, Attachments, Annotations, Graphs, Headings etc. During the content rendering inside PDF file, we often come across a requirement where we need to add contents in bullet format. This requirement can be accomplished using Aspose.PDF for Android and in order to fulfill this requirement, we need to create Dash and Bullet text and then we need to create string objects to represent Bullet and Dash characters. After that, we need to add the TextFragment objects to paragraphs collection of page instance and finally save the PDF document.

```
 //Input data:
List bulletList = new java.util.ArrayList(2);
bulletList.add("Things we do out of:");
bulletList.add("Tend to have errors related to inattention, slips, or lapses of memory");
List dashList = new java.util.ArrayList(3);
dashList.add("Habit or routine (Tasks done successfully 50 times)");
dashList.add("Not thinking (Requires less than 7-15 discrete steps)");
dashList.add("Using little or no conscious thought");
String bullet = new String(new char[]{8226, 32});
String dash = new String(new char[]{32, 32, 32, 32, 32, 8211, 32});
//Instantiate Pdf object by calling its empty constructor
Document doc = new Document();
//Create a section in the Pdf object
Page page = doc.getPages().add();
//Create the first bullet text line
TextFragment bulletFragment = new TextFragment(bullet + bulletList.get(0));
bulletFragment.getTextState().setFont(FontRepository.findFont("Arial"));
page.getParagraphs().add(bulletFragment);
//Create dash text
for (int i = 0; i < dashList.size(); i++) 
{ 
    TextFragment dashFragment = new TextFragment(dash + dashList.get(i)); 
    bulletFragment.getTextState().setFont(FontRepository.findFont("Arial")); 
    page.getParagraphs().add(dashFragment); 
    }
//Create the second bullet text line
bulletFragment = new TextFragment(bullet + bulletList.get(1));
bulletFragment.getTextState().setFont(FontRepository.findFont("Arial"));
page.getParagraphs().add(bulletFragment);
doc.save(Environment.getExternalStorageDirectory().getAbsolutePath()+"/Bullet_Text_output.pdf"); 
```

Apart from above-stated features, in this release we also have worked significantly on performance improvement, handling different documents to avoid unexpected behaviors, have greatly improved the PDF to raster images conversion and text extraction capabilities. Like we always have emphasized on using latest release versions of our API's, so we recommended you to please get the chance to download and start evaluating the new release of [Aspose.PDF for Android 16.12.0][2].




[1]: https://docs.aspose.com/display/pdfjava/Convert+PDF+to+other+Formats#ConvertPDFtootherFormats-ConvertPDFtoEPUBformat
[2]: https://downloads.aspose.com/pdf/android/new-releases/aspose.pdf-for-android-16.12.0/





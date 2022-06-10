---
title: 'Convert Word to PCL using C++ with Aspose.Words for C++ 19.5'
date: Wed, 15 May 2019 07:37:11 +0000
draft: false
url: /2019/05/15/convert-word-to-pcl-using-cpp-with-aspose.words-for-cpp/
author: Awais Hafeez
summary: ''
tags: ['Word to PCL in Cplusplus', 'Word to PCL in Cpp']
categories: ['Aspose.Words Product Family']
---

Guys, lets check out what's new for you in [Aspose.Words for C++ 19.5][1] release.

## Convert Word to PCL in C++

Aspose.Words for C++ now provides support to save Word document to [PCL (][2]_[Printer Command Language][3]_[)][4]. Aspose.Words can save documents to PCL 6 (_PCL 6 Enhanced or PCL XL_) format. PclSaveOptions class can be used to specify additional options when saving a document into the PCL format. The following code example shows how to save the document to PCL using save options.

{{< gist aspose-com-gists 518f03cac02abb105e02f55edb7de9f9 "cpp-Loading-and-Saving-ConvertDocumentToPCL-ConvertDocumentToPCL.cpp" >}}

## Additional Text Positioning in Word to PDF

We have added a [AdditionalTextPositioning][5] member in PdfSaveOptions class which can be used to specify whether to write additional text positioning operators or not. If you set it to true, then additional text positioning operators are written to the output PDF. This may help to overcome issues with inaccurate text positioning with some printers. The downside is the increased PDF document size.

{{< gist aspose-com-gists 518f03cac02abb105e02f55edb7de9f9 "cpp-Rendering-Printing-WorkingWithPdfSaveOptions-AdditionalTextPositioning.cpp" >}}

## Predefined Font FallBack Settings for Google Noto Fonts

We have added a new [LoadNotoFallbackSettings][6] member to FontFallbackSettings class that loads predefined fallback settings which uses Google Noto fonts. Google Noto are free fonts licensed under SIL OFL and can be downloaded from here (https://www.google.com/get/noto/). Sample usage code is as follows:

{{< gist aspose-com-gists 518f03cac02abb105e02f55edb7de9f9 "cpp-Rendering-Printing-SetFontSettings-SetPredefinedFontFallbackSettings.cpp" >}}

## Specify Unit of Measure to OpenDocument

We now provide a [MeasureUnit option in OdtSaveOptions][7] class to specify units of measure that can be applied to document content. Open Office uses centimeters when specifying lengths, widths and other measurable formatting and content properties in documents whereas MS Office uses inches. You can use OdtSaveOptions.MeasureUnit property to specify the unit of measure to apply to document content. The following code example shows how to use this property.

{{< gist aspose-com-gists 518f03cac02abb105e02f55edb7de9f9 "cpp-Programming-Documents-Document-WorkingWithSaveOptions-SetMeasureUnitForODT.cpp" >}}

## Prevent Embedding Fonts while saving Document into HtmlFixed

By default, Aspose.Words embed the fonts into the HtmlFixed file format. You can set the value of [HtmlFixedSaveOptions.UseTargetMachineFonts][8] property as true to prevent fonts from embedding into the HtmlFixed document. When the value of this property is true, the fonts from the target machine will be used to display the document.

{{< gist aspose-com-gists 518f03cac02abb105e02f55edb7de9f9 "cpp-Loading-and-Saving-SaveOptionsHtmlFixed-UseFontFromTargetMachine.cpp" >}}

## Write all CSS Declarations of HtmlFixed Document into Single File

By default, Aspose.Words saves "@font-face" rules of HtmlFixed documents into a separate file "fontFaces.css" while other CSS declarations are written to "styles.css". You can change this behavior by setting the value of [HtmlFixedSaveOptions.SaveFontFaceCssSeparately][9] property to false. This saves all CSS rules and declarations into the same file "styles.css". Below code example shows how to save all CSS rules and declarations into one file.

{{< gist aspose-com-gists 518f03cac02abb105e02f55edb7de9f9 "cpp-Loading-and-Saving-SaveOptionsHtmlFixed-WriteAllCSSrulesinSingleFile.cpp" >}}

## How to Align Chart Label

If you want to set a text alignment for multi-line labels, you can simply achieve this by setting the value of [ChartAxis.TickLabelAlignment][10] property. The following code example shows how to tick label alignment.

{{< gist aspose-com-gists 518f03cac02abb105e02f55edb7de9f9 "cpp-Programming-Documents-Charts-WorkingWithChartAxis-TickMultiLineLabelAlignment.cpp" >}}

## See Also Useful Links

The resources, you may need to accomplish your tasks:

*   [Aspose.Words for C++ Online Documentation][11] - up-to-date documentation containing Programmer's Guide, Knowledge Base, and much more.
*   [Aspose.Words for C++ Product Page][12]
*   [Install Aspose.Words for C++ NuGet Package][13]
*   [Aspose.Words for C++ API Reference Guide][14] - detailing the publicly exposed classes, methods, properties, constants & interfaces.
*   [Download Examples at GitHub Repository][15] - we have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.[](https://helpdesk.aspose.com/)

Keeping the Aspose tradition, you are welcome to shape the upcoming releases of Aspose.Words for C++ API by posting your suggestions and concerns in the [Aspose.Words for C++ support forum][16].




[1]: https://downloads.aspose.com/words/cpp/new-releases/aspose.words-for-c---19.5/
[2]: https://docs.aspose.com/display/wordscpp/Printer+Command+Language+-+PCL
[3]: https://docs.aspose.com/display/wordscpp/Printer+Command+Language+-+PCL
[4]: https://docs.aspose.com/display/wordscpp/Printer+Command+Language+-+PCL
[5]: https://apireference.aspose.com/cpp/words/class/aspose.words.saving.pdf_save_options/#af15683a0a3ac4d21bf1288061e7f1cad
[6]: https://apireference.aspose.com/cpp/words/class/aspose.words.fonts.font_fallback_settings/#a5b8a35a3bc12d26d315142d753b7e8b1
[7]: https://apireference.aspose.com/cpp/words/class/aspose.words.saving.odt_save_options/#af8880fb7b66abebab8d949c1003cd196
[8]: https://apireference.aspose.com/cpp/words/class/aspose.words.saving.html_fixed_save_options/#a5b5f0685d5c7a4936a16f0c6b908629c
[9]: https://apireference.aspose.com/cpp/words/class/aspose.words.saving.html_fixed_save_options/#a04a08dc612a8f5909724ab7f179e447c
[10]: https://apireference.aspose.com/cpp/words/class/aspose.words.drawing.charts.chart_axis/#ad0dbf98f9f5f091d2407e67aca7e78e0
[11]: https://docs.aspose.com/display/wordscpp/Home
[12]: https://products.aspose.com/words/cpp
[13]: https://www.nuget.org/packages/Aspose.Words.Cpp/
[14]: https://apireference.aspose.com/cpp/words
[15]: https://github.com/aspose-words/Aspose.words-for-C
[16]: https://forum.aspose.com/c/words





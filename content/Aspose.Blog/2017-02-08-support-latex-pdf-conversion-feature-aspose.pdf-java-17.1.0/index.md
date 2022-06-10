---
title: 'Convert Latex to PDF Conversion in Java using Aspose.PDF for Java 17.1.0'
date: Wed, 08 Feb 2017 14:18:38 +0000
draft: false
url: /2017/02/08/support-latex-pdf-conversion-feature-aspose.pdf-java-17.1.0/
author: Tilal Ahmad
summary: ''
tags: ['Convert Latex to PDF in Java', 'Java PDF API', 'TeX to PDF in Java']
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/aspose-Pdf-for-Java.png" alt="">}}


We are pleased to announce a new release of [Aspose.PDF for Java, 17.1.0][1]. This version includes a new feature to convert Latex file to PDF document along with all the enhancements and improvements introduced in its corresponding version of [Aspose.PDF for .NET (17.1.0)][2]. We have improved TIFF to PDF conversion performance, PDF to PDFA, PDF to DOC/DOCX and HTML to PDF conversion feature along with many other bug fixes in this version. Please check the detailed [release notes of Aspose.PDF for Java 17.1.0][3], in order to get an idea about the new features/enhancements and improvements made in this release of Aspose.Pdf for Java.

Furthermore, If you are planning to upgrade the API from any previous version, we strongly recommend you to check the [Public API Changes section of current release][4] and other intermediate releases from release notes pages, to know what has been changed since your current revision of the API.

The following sections describe some details regarding these newly added features/enhancements.

## Latex to PDF Conversion

This version has introduced Latex to the PDF conversion feature. We included a LatexLoadOptions class to load Latex files in Aspose.PDF DOM and render it to PDF file. Please check the following code snippet for converting the TEX file to PDF. ([Read more][5]

```
//Instantiate Latex Load option object
LatexLoadOptions Latexoptions = new LatexLoadOptions();
//Create Document object
com.aspose.pdf.Document doc = new com.aspose.pdf.Document("samplefile.tex", Latexoptions);
//Save the output in PDF file
doc.save("TeXToPDF_out.pdf");
```

## Add Break Text for Table Broken in Two Pages

Sometimes it is required to show some text at the bottom of the page to inform users for table broken in two pages. We have included BreakText property in Table class for this purpose in this version.

```
String outFile = "Table.pdf";
com.aspose.pdf.Document doc = new com.aspose.pdf.Document();
Page page = doc.getPages().add();
com.aspose.pdf.Table tab = new com.aspose.pdf.Table();
tab.setAlignment(HorizontalAlignment.Center);
tab.setDefaultCellBorder(new com.aspose.pdf.BorderInfo(com.aspose.pdf.BorderSide.All, 0.1f));
tab.getMargin().setTop(10);

for (int i = 1; i <= 200; i++)

{ com.aspose.pdf.Row row1 = tab.getRows().add(); row1.getCells().add("row - " + i); }
tab.setBreakText(new TextFragment("To be continued on next page"));
tab.setRepeatingRowsCount(1);
page.getParagraphs().add(tab);
doc.save(outFile); 
```

## Other Features

*   [Reference a Single Image Multiple Times][6]
*   [Set Different TabLeaderTypes for different TOC Levels][7]
*   [Add text inside Graph Object][8]

## Aspose.PDF for Java Resources

The following resources will help you work with Aspose.PDF for Java:

*   [Home page for Aspose.PDF for Java][9]
*   [Download Aspose.PDF for Java][10]
*   [Support forum][11]– Post your technical questions and queries, or any other problem you faced while running Aspose.PDF APIs.
*   [Pdf for Java online documentation][12]– help documentation and API reference documents.
*   [Enable Blog Subscription][13]– Do not limit yourself, you can keep yourself updated with the latest news on Aspose.PDF APIs, new features, fixes and other API related topics by subscribing to Aspose.PDF blog.
*   [Aspose.PDF for Java Examples][14] – We have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: https://downloads.aspose.com/pdf/java/new-releases/aspose.pdf-for-java-17.1.0/
[2]: https://blog.aspose.com/2017/01/17/support-reference-single-image-multiple-times-add-text-inside-graph-object-aspose.pdf-.net-17.1.0/
[3]: https://docs.aspose.com/display/pdfjava/Aspose.Pdf+for+Java+17.1.0+Release+Notes
[4]: https://docs.aspose.com/display/pdfjava/Aspose.Pdf+for+Java+17.1.0+Release+Notes
[5]: https://docs.aspose.com/display/pdfjava/Convert+a+File+to+PDF+Format#ConvertaFiletoPDFFormat-ConvertTeXfiletoPDFformat)
[6]: https://docs.aspose.com/
[7]: https://docs.aspose.com/display/pdfjava/Manipulate+PDF+Document#ManipulatePDFDocument-SetdifferentTabLeaderTypefordifferentTOCLevels
[8]: https://docs.aspose.com/
[9]: http://www.aspose.com/java/pdf-component.aspx
[10]: http://www.aspose.com/community/files/72/java-components/aspose.pdf-for-java/default.aspx
[11]: http://www.aspose.com/community/forums/aspose.pdf-product-family/20/showforum.aspx
[12]: http://docs.aspose.com/display/pdfjava/Home
[13]: https://blog.aspose.com/
[14]: https://github.com/asposepdf/Aspose_Pdf_JAVA





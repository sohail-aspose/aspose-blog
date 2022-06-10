---
title: 'Wrap Lines, Calculate Text Index in TextFragment and Set TOC Line Style in PDF'
date: Wed, 02 Nov 2016 05:31:09 +0000
draft: false
url: /2016/11/02/33860/
author: Tilal Ahmad
summary: ''
tags: ['Calculate Text Index in PDF', 'Calculate Text Index in Text Fragment', 'Wrap Lines in PDF']
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/aspose-Pdf-for-Java.png" alt="Wrap Lines, Calculate Text Index in TextFragment and Set TOC Line Style in PDF">}}


We are pleased to announce [Aspose.PDF for Java 16.10.0][1] release. This version of Aspose.Pdf for Java includes the same features and enhancements introduced in Aspose.PDF for .NET 16.10.0 along with a number of fixes of the bugs reported in older versions of Aspose.Pdf for Java. These enhancements and improvements add further value to API stability and prove it more reliable API for PDF document processing. Some of the new features of this release are the support of Warp Lines, None Line style of TOC element and calculation of text index in TextFragment. Please check the detailed [release notes][2] to get an idea about the issues fixed in this revision of Aspose.Pdf for Java.

Please note if you are planning to upgrade the API from any previous version, we strongly suggest you to check the [Public API Changes section of current release][3] and other intermediate releases, to know what has been changed since your current revision of the API.

The following sections describe some details regarding these newly added enhancements.

## Set TOC Line Style to None

Some customers have a business requirement to create TOC elements without any line style. So we have introduced a new LiesDash property in TocInfo class to set the TOC dash line style to none in Aspose.Pdf for .NET 16.10.0. Please check following code snippet to set LineDash value to None from TabLeaderType enum:

```
....

//Create object to represent TOC information

TocInfo tocInfo = new TocInfo();

TextFragment title = new TextFragment("Table Of Contents");

title.getTextState().setFontSize(20);

title.getTextState().setFontStyle(FontStyles.Bold);

//Set the title for TOC

tocInfo.setTitle(title);

//Set TOC line dash style

tocInfo.setLineDash(TabLeaderType.None);

tocPage.setTocInfo(tocInfo);
```

## Support of Wrap line in New Generator

We have introduced the Wrap line feature in the TextFragment class of the new generator. We can use this feature in all the Objects those support Paragraph object e.g. Page, Table object. We can accomplish this task by setting the desired value of setWrapLinesCount property of TextFragment object as following:

```
TextFragmentAbsorber absorber = new TextFragmentAbsorber("Windows");

Document doc = new Document("SimpleInput.pdf");

doc.getPages().get_Item(1).accept(absorber);

for (TextFragment textFragment : (Iterable<TextFragment>) absorber.getTextFragments())

{

int position = textFragment.getSegments().get_Item(1).getStartCharIndex();

System.out.println("Starting position of "+textFragment.getText()+ " word is "+position+ " in the text show operator.");

}
```

## Calculation of Text index in TextFragment

One of the customers has the requirement to calculate the text index in TextFragment. Please note PDF document does not contain any definition of "line". PDF operates with text segments (text show operators) that are absolutely positioned on the page anywhere. Mostly PDF text segment represents one line in the text. But sometimes it may represent a part of the line. Therefore often index of the fragment in the physical text segment will be also an index in the line.

We have added two read-only properties StartCharIndex and EndCharIndex in TextSegment Class. These properties get the starting / ending character index of the current segment in the show text operator (Tj, TJ) segment. Please consider the following code to get text Index in TextFragment.

```
TextFragmentAbsorber absorber = new TextFragmentAbsorber("Windows");

Document doc = new Document("SimpleInput.pdf");

doc.getPages().get_Item(1).accept(absorber);

for (TextFragment textFragment : (Iterable<TextFragment>) absorber.getTextFragments())

{

int position = textFragment.getSegments().get_Item(1).getStartCharIndex();

System.out.println("Starting position of "+textFragment.getText()+ " word is "+position+ " in the text show operator.");

}
```

## Miscellaneous fixes

We have improved PDF to PDFA conversion features in this release by fixing a number of related issues. This version also includes some other important bug fixes along with above-stated enhancements. Please check release notes of Aspose.PDF for Java 16.10.0 for a complete list of bug fixed.

## Aspose.PDF for Java Resources

The following resources will help you work with Aspose.Pdf for Java:

*   [Home page for Aspose.PDF for Java][4]
*   [Download Aspose.PDF for Java][5]
*   [Aspose.PDF product family forum][6] – Post your technical questions and queries, or any other problem you faced while running Aspose.Pdf APIs.
*   [Aspose.PDF for Java online documentation][7] – help documentation and API reference documents.
*   [Enable Blog Subscription][8] – Do not limit yourself, you can keep yourself updated with the latest news on Aspose.Pdf APIs, new features, fixes and other API related topics by subscribing to Aspose.Pdf blog.
*   [Aspose.PDF for Java Examples][9] – We have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: https://downloads.aspose.com/pdf/java
[2]: https://docs.aspose.com/display/pdfjava/Aspose.Pdf+for+Java+16.10.0+Release+Notes
[3]: https://docs.aspose.com/display/pdfjava/Aspose.Pdf+for+Java+16.10.0+Release+Notes
[4]: https://products.aspose.com/pdf/java
[5]: https://downloads.aspose.com/pdf/java
[6]: https://forum.aspose.com/
[7]: http://docs.aspose.com/display/pdfjava/Home
[8]: https://blog.aspose.com/
[9]: https://github.com/aspose-pdf/Aspose.PDF-for-Java





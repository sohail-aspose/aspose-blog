---
title: 'TOC Indentation without Numbers and Image Optimization in PDF using Java'
date: Mon, 03 Oct 2016 03:03:13 +0000
draft: false
url: /2016/10/03/aspose.pdf-for-java-11.9.0-introduces-toc-indentation-without-numbers-and-enhances-pdf-optimization-process/
author: Tilal Ahmad
summary: ''
tags: []
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/aspose_pdf-for-java1.jpg" alt="">}}


We are pleased to announce [Aspose.PDF for Java 11.9.0][1] has been released. It includes two enhancements, to add TOC indentation without numbering and PDF optimization. In addition to above enhancements, this version consist of some other important bug fixes as well. There have been specific improvements regarding PDF to PDFA, PDF to HTML, HTML to PDF and PDF to Images. Please check [release notes of Aspose.PDF for Java 11.9.0][2] for complete list of bug fixed.

The following sections describe some details regarding these enhancements/Improvements:

## Add TOC Indentation without Numbers in Java

**TOC indentation:** One of the customer has requirement to add TOC entries without numbering styles and add indentation to headings. We have implemented indentation without numbers and now able to use **setIndentation()** method to set indentation characters. But please take into account that, this is one of auto sequencing type with "**None**" NumberingStyle parameter.**final**

```
final com.aspose.pdf.TocInfo tocInfo = new com.aspose.pdf.TocInfo();

....

tocInfo.setLevelIndentation(4);

....

final com.aspose.pdf.Heading heading2 = new com.aspose.pdf.Heading(level++);

heading2.setAutoSequence(true);

heading2.setStyle(NumberingStyle.None);

....
```

## Image Manipulation in PDF Optimization

During PDF optimization, sometimes it is required to change image resolution and image dimensions. Till last release this requirement was fulfilled by iterating through Page resources and using replace method of Image class. However we have implemented additional optimization methods to process optimization in one place.

**optimizeOptions.setResolution(100)**: - we will update all the images resolution to the requested value.  
**optimizeOptions.setMaximumImageDimension(2500)**: - we will specifies the maximum image dimension. If the image width or height of the existing image is greater than this value - the image size will be proportionally reduced.

```
Document doc = new Document(myDir+"input.pdf");

OptimizationOptions optimizeOptions = new OptimizationOptions();

optimizeOptions.setRemoveUnusedObjects(true);

optimizeOptions.setLinkDuplcateStreams(true);

optimizeOptions.setRemoveUnusedStreams(true);

optimizeOptions.setCompressImages(true);

optimizeOptions.setImageQuality(60);

optimizeOptions.setResolution(100);

optimizeOptions.setMaximumImageDimension(2500);

doc.optimizeResources(optimizeOptions);

doc.save(myDir + "output.pdf");
```

## Public API Changes

The major API change in this release is the legacy engine (package **aspose.pdf.\***) moved from the build to another jar file (**aspose.pdf.legacy-11.9.0.jar**) with deleting all the methods bind with it. **License** and **AssemblyConstants** classes for the legacy jar moved into the **com.aspose.pdf.legacy** package. All the other classes from the package **aspose.pdf.\*** are not changed. Please check [Public API Changes section][3] in release notes for complete details of Public API changes of this release.

## Aspose.PDF for Java Resources

The following resources will help you work with Aspose.Pdf for Java:

*   [Home page for Aspose.PDF for Java][4]
*   [Download Aspose.PDF for Java][5]
*   [Aspose.PDF product family forum][6] – Post your technical questions and queries, or any other problem you faced while running Aspose.PDF APIs.
*   [Aspose.PDF for Java online documentation][7] – help documentation and API reference documents.
*   [Enable Blog Subscription][8] – Do not limit yourself, you can keep yourself updated with the latest news on Aspose.PDF APIs, new features, fixes, and other API related topics by subscribing to Aspose.PDF blog.
*   [Aspose.PDF for Java Examples][9] – We have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: http://www.aspose.com/downloads/pdf/java/new-releases/aspose.pdf-for-java-11.9.0/
[2]: http://docs.aspose.com/display/pdfjava/Aspose.Pdf+for+Java+11.9.0+Release+Notes
[3]: http://docs.aspose.com/display/pdfjava/Aspose.Pdf+for+Java+11.9.0+Release+Notes
[4]: https://www.aspose.com/templates/aspose/App_Themes/V3/images/words/272x272/aspose_words-for-net.png
[5]: http://www.aspose.com/community/files/72/java-components/aspose.pdf-for-java/default.aspx
[6]: http://www.aspose.com/community/forums/aspose.pdf-product-family/20/showforum.aspx
[7]: http://docs.aspose.com/display/pdfjava/Home
[8]: https://blog.aspose.com/
[9]: https://github.com/asposepdf/Aspose_Pdf_JAVA





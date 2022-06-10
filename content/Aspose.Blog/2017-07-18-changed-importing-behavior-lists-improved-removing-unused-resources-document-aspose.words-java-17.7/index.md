---
title: 'Remove Unused Resources in Word Document in Java'
date: Tue, 18 Jul 2017 06:39:53 +0000
draft: false
url: /2017/07/18/changed-importing-behavior-lists-improved-removing-unused-resources-document-aspose.words-java-17.7/
author: Tilal Ahmad
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---



{{< figure align=center src="images/aspose-Words-for-Java-1.png" alt="">}}


We have released new version of [Aspose.Words for Java, 17.7][1]. It includes new features, enhancements and fixes of Java platform along with auto porting of its corresponding .NET version functionality i.e. Aspose.Words for .NET 17.7. Some of the new improvements are to display document title in window title bar of PDF document, removing unused resources from document and improved logic of lists import in document joining/appending. Please check the detailed [release notes of this version][2] to get an idea about the new features/enhancements and fixes made in this release.

Furthermore, if you are planning to upgrade the API from any previous version, we strongly recommend you to check the [Public API Changes section of current release][3] and other intermediate releases from [release notes folder][4], to know what has been changed since your current revision of the API.

The following sections describe some details regarding these newly added features/enhancements.

## Removal of Unused Resources from Document using Java

We have added a new cleanup method in Document class in Aspose.Words for .NET 17.7 to [remove unused styles and lists from the document][5]. Now you can remove only lists or styles or both from document. Please note Document.RemoveUnusedResources method is now obsolete.



## Display Document Title in Window Title Bar of PDF

We have introduced a new feature in Aspose.Words for .NET 17.7 to control behavior of how [document title is presented in output PDF document][6]. A new property DisplayDocTitle is included in PdfSaveOptions class. This property is used to specify whether windows title bar should display the document title, taken from the Title entry of the document information dictionary.

{{< gist aspose-com-gists aa75ee5112aca57022c741270ff8cbc4 "Examples-src-main-java-com-aspose-words-examples-loading_saving-DisplayDocTitleInWindowTitlebar-DisplayDocTitleInWindowTitlebar.java" >}}

## Improved Behavior of List Import in Document Joining/Appending

We have improved the List import behavior in this release. Previously, list definitions were copied with a new identifier while importing. Now Aspose.Words reuses identical list definitions in the destination. Equality of list definitions in the source and destination is determined by their identifiers. Also Aspose.Words preserves list definition identifiers from the source when equal list definition cannot be found in the destination. This is how MS Word behaves.

## Change in AspectRatioLock Default Value of Image

We have changed [Shape.AspectRatioLocked default value of ShapeType.Image][7] to mimic MS Word behavior. Now AspectRatioLocked default value for ShapeType.Image is “true” and false for other types of Shapes.

{{< gist aspose-com-gists aa75ee5112aca57022c741270ff8cbc4 "Examples-src-main-java-com-aspose-words-examples-programming_documents-document-DocumentBuilderSetImageAspectRatioLocked-DocumentBuilderSetImageAspectRatioLocked.java" >}}

## Other Improvements

There are 104 improvements and fixes in this regular monthly release. The most notable are:

*   Performance of saving to PDF is improved.
*   The proper algorithm for rendering of shapes with automatic size textboxes (i.e. closest to MS Word output) implemented.
*   The rendered PDF documents can now show the document title in the title bar of the viewer. This is controlled by “PdfSaveOptions.DisplayDocTitle” property.
*   Improved font rendering in PDF documents for Adobe Illustrator limitations.
*   Improved rendering of fonts with simulated bold style.
*   Vertical text rendering in DrawingML textboxes improved.
*   Problem with rendering of numbers on horizontal axis in DrawingML Charts fixed.
*   Implemented support for "Wrap trailing spaces to next line" option.
*   Implemented support for footnote continuation notices.
*   Improved text wrapping logic for "2013 and later" documents.
*   Improved non-breaking space width calculation.
*   Improved Asian text justification logic.

## Aspose.Words for Java Resources

The following resources will help you work with Aspose.Words for Java:

*   [Home page for Aspose.Words for Java][8]
*   [Download Aspose.Words for Java][9]
*   [Install Aspose.Words for Java from Maven][10]
*   Aspose.Words product family forum – Post your technical questions and queries, or any other problem you faced while running Aspose.Words APIs.
    *   [Free Support Forum][11]
    *   [Paid Support Forum][12]
*   [Aspose.Words for Java online documentation][13] – Help documentation.
*   [Aspose.Words for Java online API reference][14] - API reference documents.
*   [Enable Blog Subscription][15] – Do not limit yourself, you can keep yourself updated with the latest news on Aspose.Words, APIs, new features, fixes and other API related topics by subscribing to Aspose.Words blog.
*   [Aspose.Words for Java Examples][16] – We have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: https://downloads.aspose.com/words/java/new-releases/aspose.words-for-java-17.7/
[2]: https://docs.aspose.com/display/wordsjava/Aspose.Words+for+Java+17.7+Release+Notes
[3]: https://docs.aspose.com/display/wordsjava/Aspose.Words+for+Java+17.7+Release+Notes
[4]: https://docs.aspose.com/display/wordsjava/Release+Notes
[5]: https://docs.aspose.com/display/wordsjava/Working+with+Document#WorkingwithDocument-RemoveUnusedStylesandListsfromDocument
[6]: https://docs.aspose.com/display/wordsjava/Working+with+Document#WorkingwithDocument-DisplaytheDocumentTitleinWindowTitlebarofPDFdocument
[7]: https://docs.aspose.com/display/wordsjava/Working+with+Images#WorkingwithImages-LockAspectRatioofImage
[8]: https://www.aspose.com/products/words/java
[9]: https://downloads.aspose.com/words/java
[10]: http://maven.aspose.com/repository/simple/ext-release-local/com/aspose/aspose-words/
[11]: https://forum.aspose.com/c/words
[12]: https://helpdesk.aspose.com/
[13]: https://docs.aspose.com/display/wordsjava/Home
[14]: https://apireference.aspose.com/java/words
[15]: https://blog.aspose.com/category/aspose-products/aspose-words-product-family/
[16]: https://github.com/aspose-words/Aspose.Words-for-Java





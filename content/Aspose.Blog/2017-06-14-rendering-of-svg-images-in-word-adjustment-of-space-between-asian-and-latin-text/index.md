---
title: 'Improved Rendering of SVG Images and Automatic Adjustment of Space between Asian and Latin Text/Numbers in Word'
date: Wed, 14 Jun 2017 13:02:42 +0000
draft: false
url: /2017/06/14/rendering-of-svg-images-in-word-adjustment-of-space-between-asian-and-latin-text/
author: Tilal Ahmad
summary: ''
tags: []
categories: ['Aspose.Words Product Family']
---



{{< figure align=center src="images/aspose-Words-for-Java-1.png" alt="">}}


We are pleased to announce new release [Aspose.Words for Java 17.6][1]. As Aspose.Words for Java is auto-ported from Aspose.Words for .NET, this month release includes all the new features, enhancements and fixes introduced in its corresponding version .NET version i.e Aspose.Words for .NET 17.6. Some of the new features are the support of automatically adjust space between Asian and Latin Text/Numbers and import of HTML form field tags as Content Control tags (SDT). Please check the [detailed release notes of this version][2] to get an idea about the new features/enhancements and fixes made in this release.

Furthermore, if you are planning to upgrade the API from any previous version, we strongly recommend you to check the [Public API Changes section of current release][3] and other intermediate releases from [release notes folder][4], to know what has been changed since your current revision of the API.

The following sections describe some details regarding these newly added features/enhancements.

## Improved rendering of SVG images

We have improved the SVG image rendering technique in this version. Earlier, upon inserting the SVG image into the document, it is converted to meta-file (EMF) using GDI/+. We have noticed that GDI/+ is not working as expected in the multithreading approach, an exception occurs in GDI/+. To prevent problems with multi-threading, we have switched to our own EMF renderer instead of GDI/+.

## Automatically Adjust Space between East Asian and Latin Text/Number

We have implemented a new feature in this release to [automatically adjust space between East Asian and Latin text and Numbers and East Asian text][5].  We have added two public properties in ParagraphFormat class AddSpaceBetweenFarEastAndAlpha and AddSpaceBetweenFarEastAndDigit to achieve this. Gets or Sets flag indicating whether inter-character spacing is automatically adjusted. 

{{< gist aspose-words b37032675133885c4c91814fb3d51a25 "Examples-src-main-java-com-aspose-words-examples-programming_documents-document-DocumentBuilderSetSpacebetweenAsianandLatintext.java" >}}

## Import HTML Form Fields Tags as Content Control Tags(SDT)

Some of our customers have the requirement to [import HTML form fields as content control tags(SDT) in HTML to DOCX conversion][6]. We have introduced this new feature in Aspose.Words for Java 17.6. Now you can import <input> and <select> elements as content control (SDT) during HTML to DOCX conversion.  Please check the following sample code snippet for detail:

{{< gist aspose-com-gists aa75ee5112aca57022c741270ff8cbc4 "Examples-src-main-java-com-aspose-words-examples-loading_saving-LoadAndSaveHtmlFormFieldasContentControlinDOCX.java" >}}

## Other Improvements

We have 95 improvements and fixes in the current release. In addition to the above features and enhancements following are some of the notable improvements of this release:

*   Performance and memory optimizations caused by shrinking and optimizing the storage of internal unsigned types.
*   Throw warnings when an external resource in HTML could not be loaded.
*   Track changes view settings in LibreOffice.
*   Added ability to reference data from parent region in child regions.
*   Implemented support for distributed paragraph alignment.
*   Improved handling of justified alignment in Asian text.
*   Improved line height calculation for inline images in Asian text
*   Improved handling of hidden paragraph breaks around text frames
*   Improved text wrapping of sections breaks around floating objects
*   Improved Aps logical structure generation for repeated header rows
*   Improved rendering of PDF logical structure of Table headers.
*   Character offsets in META\_EXTTEXTOUT records are now taken into account while rendering multi-byte encoding metafiles.

## Aspose.Words for Java Resources

The following resources will help you work with Aspose.Words for Java:

*   [Home page for Aspose.Words for Java][7]
*   [Download Aspose.Words for Java][8]
*   [Install Aspose.Words for Java from Maven][9]
*   Aspose.Words product family forum – Post your technical questions and queries, or any other problem you faced while running Aspose.Words APIs.
    *   [Free Support Forum][10]
    *   [Paid Support Forum][11]
*   [Words for Java online documentation][12]– Help documentation.
*   [Words for Java online API reference][13] - API reference documents.
*   [Enable Blog Subscription][14]– Do not limit yourself, you can keep yourself updated with the latest news on Aspose.Words, APIs, new features, fixes and other API related topics by subscribing to Aspose.Words blog.
*   [Aspose.Words for Java Examples][15] – We have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: https://downloads.aspose.com/words/java/new-releases/aspose.words-for-java-17.6/
[2]: https://docs.aspose.com/display/wordsjava/Aspose.Words+for+Java+17.6+Release+Notes
[3]: https://docs.aspose.com/display/wordsjava/Aspose.Words+for+Java+17.6+Release+Notes
[4]: https://docs.aspose.com/display/wordsjava/Aspose.Words+for+Java
[5]: https://docs.aspose.com/display/wordsjava/Using+DocumentBuilder+to+Modify+a+Document#UsingDocumentBuildertoModifyaDocument-AutomaticallyAdjustSpacebetweenAsianandLatintext,Numbers
[6]: https://docs.aspose.com/display/wordsjava/Saving+a+Document#SavingaDocument-SaveHTMLtagsInputandSelectasContentControl
[7]: https://www.aspose.com/products/words/java
[8]: https://downloads.aspose.com/words/java
[9]: http://maven.aspose.com/repository/simple/ext-release-local/com/aspose/aspose-words/17.6/
[10]: https://forum.aspose.com/c/words
[11]: https://helpdesk.aspose.com/
[12]: https://docs.aspose.com/display/wordsjava/Home
[13]: https://apireference.aspose.com/java/words
[14]: https://blog.aspose.com/category/aspose-products/aspose-words-product-family/
[15]: https://github.com/aspose-words/Aspose.Words-for-Java





---
title: 'Print OneNote Documents using Java with Aspose.Note for Java'
date: Tue, 25 Jul 2017 10:58:27 +0000
draft: false
url: /2017/07/25/print-onenote-documents-aspose.note-java-17.3/
author: Kashif Iqbal
summary: ''
tags: []
categories: ['Aspose.Note Product Family']
---



{{< figure align=center src="images/aspose_note-for-java.png" alt="Aspose.Note for Java">}}


We are pleased to announce the release of [Aspose.Note for Java][1] 17.3. It includes new feature of adding hyperlinks to images in the document. It also provides the capability of printing documents to printer. We have also fixed several bugs reported to us by our valued customers. For a complete list of what is new and fixed, please visit the [release notes][2] section of Aspose.Note for Java 17.3.

## Add Hyperlink to Images in OneNote

This release enhances the feature of working with images in the Microsoft OneNote document. It provides the capability to [add hyperlink to images][3] in a page. The setHyperlink can be used to set hyperlink to an image as shown in the code sample below. This feature can be used with new images as well as existing images in the document.

```
Document document = new Document();
Page page = new Page(document);
Image image = new Image(document, dataDir + "image1.jpg");
image.setHyperlinkUrl( "http://www.aspose.com");
page.appendChild(image);
document.appendChild(page);
document.save(dataDir + "HyperlinkToImage_out.one"); 
```

## Printing OneNote Documents using Java

You can now [print OneNote documents][4] to printer using Aspose.Note for Java API. The API supports printing document to output printer as well as virtual printers. It also facilitates to set additional printer settings using the PrintOptions class.

## Optimized File Size and Saving Time

We have also worked to improve the file size and saving time for documents with large number of [page versions][5]. With this improvement, the file size and document saving time is reduced. This surely helps improve the overall API performance in terms of efficiency and effectiveness.

## API Resources

*   [Documentation][6]– Visit our documentation section for getting started with the API in no time
*   [API Reference Guide][7]– Gives detailed information about all the namespaces, classes and methods of the API
*   [Forum Support][8]– Post your queries on Aspose.Note forum to get assistance from our technical support team
*   [GitHub Examples][9]– Try the ready-to-use examples of the API by downloading from our GitHub repository




[1]: https://products.aspose.com/note/java
[2]: https://docs.aspose.com/note/java/aspose-note-for-java-17-3-release-notes/
[3]: https://docs.aspose.com/note/java/working-with-images/#WorkingwithImages-LinkanImagetoHyperlink
[4]: https://docs.aspose.com/note/java/printing-documents/
[5]: https://blog.aspose.com/2016/09/16/page-history-modifications-supported-with-aspose.note-for-java-2.5.0/
[6]: https://docs.aspose.com/note/java/
[7]: https://apireference.aspose.com/note/java
[8]: https://forum.aspose.com/c/note
[9]: https://github.com/aspose-note/Aspose.Note-for-Java





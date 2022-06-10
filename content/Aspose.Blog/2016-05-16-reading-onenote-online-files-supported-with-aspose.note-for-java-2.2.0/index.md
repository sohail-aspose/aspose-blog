---
title: 'Read OneNote Online Files using Aspose.Note for Java'
date: Mon, 16 May 2016 15:45:25 +0000
draft: false
url: /2016/05/16/reading-onenote-online-files-supported-with-aspose.note-for-java-2.2.0/
author: Kashif Iqbal
summary: ''
tags: []
categories: ['Aspose.Note Product Family']
---



{{< figure align=center src="images/aspose_note-for-java1.png" alt="">}}


We are pleased to announce the release of [Aspose.Note for Java 2.2.0][1]. This month’s release introduces new features and enhancements along with bug fixes that were reported in our last month’s release. Specifically, the API now supports Microsoft OneNote online file format. In addition, it provides support for adding alternate text for images as well as set different page splitting algorithms. For a detailed list of what is new and fixed, please visit our product release notes section in Aspose.Note for Java documentation.

## Java OneNote API - New Features and Enhancements

**Support for OneNote Online (SharePoint) File Format:** This month’s release of Aspose.Note for Java supports OneNote online file format, known as OneNote SharePoint file format. However, this feature comes with some limitations due to the lack of available specifications for reading such contents. These limitations are:

*   Hand written drawings are not supported
*   Embedded Files/Images are also not supported

However, we are investigating all possible methods for supporting these and hope to include these in one of nearest releases.

**Support for Adding Alternative Text for Image:** This month’s release also provides an enhancement where [alternative text][2] can be added for image. This can be achieved by setting the AlternativeText property of the Image class using the _setAlternativeText_ method as shown in the following code sample.

{{< gist aspose-com-gists 952261680cb5075c778c0ae67a69bd14 "Examples-src-main-java-com-aspose-note-examples-images-InsertanImage-InsertImage.java" >}}

**Setting Page Splitting Algorithm:** A OneNote document may contain a number of images and other documents at locations that cannot be retained while converting the document to other formats. This can result in displacement of such content to next page, for example, if it lies on the page border.

This month’s release empowers users to specify the page splitting algorithm while converting the document to other formats. It can be done using the setPageSplittingAlgorithm method of _PdfSaveOptions_ class that can be set to the following values:

*   **AlwaysSplitObjectsAlgorithm** – Splits objects into several parts at pages’ bottom position
*   **KeepPartAndCloneSolidObjectToNextPageAlgorithm** – Adds objects up to the bottom of the page and clones full object to the next page in case it doesn’t fit in original page
*   **KeepSolidObjectsAlgorithm** – Shifts full object to the next page in case it doesn’t fit in original page

Our documentation article, [Setting Page Splitting Algorithm][3], demonstrates the usage of different page splitting options.

## API Resources

*   Documentation – Visit our documentation section for getting started with the API in no time
*   [API Reference Guide][4] – Gives detailed information about all the namespaces, classes and methods of the API
*   [Forum Support][5] – Post your queries on Aspose.Note forum to get assistance from our technical support team
*   [GitHub Examples][6] - Try the ready-to-use examples of the API by downloading from our GitHub repository




[1]: https://downloads.aspose.com/note/java
[2]: https://docs.aspose.com/display/notejava/Working+with+Images#WorkingwithImages-AddingImagetoaOneNoteDocumentPageandSavingasPDF
[3]: https://docs.aspose.com/display/notejava/Load+a+OneNote+Document#LoadaOneNoteDocument-SettingPageSplittingAlgorithm
[4]: http://www.aspose.com/api/java/note
[5]: https://forum.aspose.com/c/note
[6]: https://github.com/aspose-note/Aspose.Note-for-Java





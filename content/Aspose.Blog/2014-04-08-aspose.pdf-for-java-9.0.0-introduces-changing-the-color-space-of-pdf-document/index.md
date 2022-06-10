---
title: 'Aspose.Pdf for Java 9.0.0 Introduces Changing the Color Space of PDF Document'
date: Tue, 08 Apr 2014 13:12:48 +0000
draft: false
url: /2014/04/08/aspose.pdf-for-java-9.0.0-introduces-changing-the-color-space-of-pdf-document/
author: Tilal Ahmad
summary: ''
tags: []
categories: ['Aspose.Total Product Family', 'Aspose.PDF Product Family']
---

[![Aspose.Pdf for Java logo][1]](https://blog.aspose.com/wp-content/uploads/sites/2/2013/07/aspose-Pdf-for-Java_100.png)We are pleased to announce the release of [Aspose.Pdf for Java 9.0.0][2]. It includes some new exciting features, enhancements and fixes to issues reported in earlier versions of Aspose.Pdf for Java, along with a change of release numbering. As the Java version is ported from Aspose.Pdf for .NET, its version number has been changed to reflect the .NET version it comes from. You can download the latest release of Aspose.Pdf for Java from the [download section][3].

Changing color space of PDF document is one of the exiting features introduced in this version. The maximum number of columns limit in a table has been increased to 512 and we have made further progress on porting new classes and methods from Aspose.Pdf for .NET to the Aspose.Pdf for Java architecture. The complete details of these changes can be found in Public API Changes in Aspose.Pdf for Java 9.0.0.

Following are the some of the new features/enhancements this month’s release. For a full list of bug fixes and improvements please refer to the download pages in the link above.

## Export/Import Bookmarks

The methods exportBookmarksToXML(...) and importBookmarksWithXML(...) with Stream arguments are implemented in the PdfBookmarkEditor class. So now extracted bookmarks can be saved into stream object can be import into stream from XML file.

### Export  Bookmarks```
//Create PdfBookmarkEditor object
PdfBookmarkEditor bookmarkeditor = new PdfBookmarkEditor();
//Open PDF file
bookmarkeditor.bindPdf("Input.pdf");
OutputStream os = new FileOutputStream("bookmark.xml");
bookmarkeditor.exportBookmarksToXML(os);
bookmarkeditor.dispose();
```

### Import Bookmarks```
//Create PdfBookmarkEditor object
PdfBookmarkEditor bookmarkeditor = new PdfBookmarkEditor();
//Open PDF file
bookmarkeditor.bindPdf("Input.pdf");
InputStream is = new FileInputStream("bookmark.xml");
bookmarkeditor.importBookmarksWithXML(is);
bookmarkeditor.save("output.pdf");
```

For more information, please take a look at Working with Bookmarks.




[1]: https://blog.aspose.com/wp-content/uploads/sites/2/2013/07/aspose-Pdf-for-Java_100.png "Aspose.Pdf for Java logo"
[2]: http://www.aspose.com/community/files/72/java-components/aspose.pdf-for-java/default.aspx
[3]: http://www.aspose.com/community/files/72/java-components/aspose.pdf-for-java/default.aspx





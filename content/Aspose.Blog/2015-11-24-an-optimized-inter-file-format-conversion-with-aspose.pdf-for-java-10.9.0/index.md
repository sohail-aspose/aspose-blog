---
title: 'An optimized inter file format conversion with Aspose.Pdf for Java 10.9.0'
date: Tue, 24 Nov 2015 19:04:02 +0000
draft: false
url: /2015/11/24/an-optimized-inter-file-format-conversion-with-aspose.pdf-for-java-10.9.0/
author: Codewarior
summary: ''
tags: ['Nayyer Shahbaz']
categories: ['Aspose.PDF Product Family']
---

[![Aspose.Pdf for .NET logo][1]](https://blog.aspose.com/wp-content/uploads/sites/2/2013/07/aspose-Pdf-for-Java_100.png)This month's release of [Aspose.Pdf for Java 10.9.0 ][2] provides a stable and a reliable version which provides the capabilities to convert PDF documents to various output formats with great fidelity. PDF to other formats conversion has always been challenging but Aspose team has always made it possible by challenging themselves, by producing better API's as we believe **well done is better than well said**. We believe in delivering reliable API's rather than just making announcements. Aspose is one of the market leading File format conversion API provider and we are in this business for more than a decade. So who knows file formats better than us !

Each single release of API's created by our team of experts is competitive and steadfast enough to compete in market and it helps our customers to fulfill their requirements in a more professional and proficient manner. In short, our goal is to "make IT better". The new release of Aspose.Pdf for Java is published and the main focus in this release has been towards PDF file to other file formats conversion which includes HTML, DOCX, TIFF, PNG, PDF/A and Excel are some to be named. The complex CSS objects like underline text can easily be recognized during PDF to HTML conversion and similar formatting information can be stored in CSS file. To accomplish this requirement, please try using following code snippet.

```
Document doc = new Document(myDir+"Lorem+Ipsum.pdf");
HtmlSaveOptions options = new HtmlSaveOptions();
options.TrySaveTextUnderliningAndStrikeoutingInCss = true;
doc.save(myDir+"outline.html", options);
```

Please download and try the latest release of [Aspose.Pdf for Java 10.9.0][3].




[1]: https://blog.aspose.com/wp-content/uploads/sites/2/2013/07/aspose-Pdf-for-Java_100.png "Aspose.Pdf for .NET logo"
[2]: http://www.aspose.com/community/files/72/java-components/aspose.pdf-for-java/entry668742.aspx
[3]: http://www.aspose.com/community/files/72/java-components/aspose.pdf-for-java/entry668742.aspx





---
title: 'Create FreeTextAnnotations with Rich Text using Aspose.PDF for Java'
date: Sun, 18 Nov 2018 21:49:23 +0000
draft: false
url: /2018/11/18/create-freetextannotations-with-rich-text-using-aspose.pdf-for-java/
author: Asad Ali
summary: ''
tags: ['Asad Ali', 'Create free text annotations in PDF', 'PDF free text annotations with rich text', 'free text annotations in PDF using Java']
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/aspose-Pdf-for-Java.png" alt="create free text annotation in PDF">}}


We are gratified to announce that the latest version **Aspose.PDF for Java** 18.10 has been released. As per regular monthly revision, quite exciting features and enhancements have been included in the latest release in order to make API more user-friendly and usable while creating and manipulating PDF documents. Release notes page of **Aspose.PDF for Java** 18.10 contains detailed information of what has been changed and introduced new in the latest release. In case you are planning to use the latest version in your Java applications, it is strongly recommended to go through the release notes page of the API.

The following section includes insights into worth-mentioning features that latest version of the API includes:

## Create Free Text Annotation with Rich Text in PDF

RichText is now supported in FreeTextAnnotation. Please note that rich text is HTML-like text markup and in order to use this in FreeTextAnnotaiton, you need to use setRichText() method offered by the API as the following sample:

```
freeTextAnnot.setRichText("<?xml version=\"1.0\"?>" " + <br>"<body xmlns=\"http://www.w3.org/1999/xhtml\" " +
"xmlns:xfa=\"http://www.xfa.org/schema/xfa-data/1.0/\" xfa:APIVersion=\"Acrobat:11.0.23\" " +
"xfa:spec=\"2.0.2\"  style=\"font-size:12.0pt;color:#00eeff;font-weight:normal;font-style:normal;" +
"font-family:Arial;font-stretch:normal\"><p dir=\"ltr\">This <p style=\"color:#00ff00;" +
"font-style:italic\">is  a rich text</body>");
```

If you need just plain text, you should use Contents Property instead of RictText but, you may assign plain text to RichText and this would also work:

```
freeTextAnnot.setContents("Annotation Text");
// or
freeTextAnnot.setRichText("Annotation Text");
```

Please also notice that, using DefaultAppearance.FontSize can set the font size manually as shown below:

```
DefaultAppearance defaultAppearance = new DefaultAppearance();
defaultAppearance.setFontSize(12);
// or <br>DefaultAppearance defaultAppearance = <br>new DefaultAppearance("Arial", 12, java.awt.Color.BLACK);
```

## Miscellaneous Fixes

Along with the feature mentioned above, following are some useful improvement which have been made to the latest version of the API:

*   Support of custom fonts is tested and verified for IBM iSeries
*   HOCR to PDF conversion has been improved for multithreaded maven scenarios
*   Text Stamping has further been improved
*   PDF to PDF/A Conversion engine is further improved

As it is always recommended to use latest release of our API’s because they include latest features/improvements and fixes related to issues reported in earlier released versions. Therefore, please download the latest release of [Aspose.PDF for Java 18.10.][1]

*   [Home page for Aspose.PDF for Java][2]
*   [Download Aspose.PDF for Java 18.10][3]
*   [Aspose.PDF product family forum][4]– Post your technical questions and queries, or any other problem you faced while running Aspose.PDF APIs.
*   [Aspose.PDF for Java online documentation][5]– Help documentation and API reference documents.
*   [Enable Blog Subscription][6]– Do not limit yourself, you can keep yourself updated with the latest news on Aspose.PDF APIs, new features, fixes and other API related topics by subscribing to Aspose.PDF blog.




[1]: https://artifact.aspose.com/repo/com/aspose/aspose-pdf/18.10/
[2]: https://products.aspose.com/pdf/java
[3]: https://artifact.aspose.com/repo/com/aspose/aspose-pdf/18.10/
[4]: https://forum.aspose.com/c/pdf
[5]: https://docs.aspose.com/display/pdfjava/Home
[6]: https://blog.aspose.com/category/aspose-products/aspose-pdf-product-family/





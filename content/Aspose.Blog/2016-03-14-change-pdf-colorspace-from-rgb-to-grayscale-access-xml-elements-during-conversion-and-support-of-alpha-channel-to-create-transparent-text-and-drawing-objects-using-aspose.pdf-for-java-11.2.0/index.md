---
title: 'Change PDF colorspace from RGB to Grayscale,  access XML elements during conversion and support of Alpha channel to create transparent text and drawing objects using Aspose.Pdf for Java 11.2.0'
date: Mon, 14 Mar 2016 03:13:23 +0000
draft: false
url: /2016/03/14/change-pdf-colorspace-from-rgb-to-grayscale-access-xml-elements-during-conversion-and-support-of-alpha-channel-to-create-transparent-text-and-drawing-objects-using-aspose.pdf-for-java-11.2.0/
author: Tilal Ahmad
summary: ''
tags: ['Color PDF to Grayscale PDF', 'Convert PDF to Black and White', 'Convert PDF to Black and White in Java', 'Convert PDF to Grayscale in Java', 'Converting color PDF to greyscale PDF']
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/aspose_pdf-for-java1.jpg" alt="">}}


Aspose.PDF for Java 11.2.0 has been released. We are pleased to announce that the new version of Aspose.Pdf for Java not only includes all the features and enhancements introduced in [Aspose.PDF for .NET 11.2.0][1] but also contains the feature to change PDF document colorspace from RGB to Grayscale and set the background image of submit button. It also includes some important bug fixes along with above-stated enhancements. Please check release notes of Aspose.PDF for Java 11.2.0 for a complete list of bug fixed.

The following sections describe some details regarding these newly added features/enhancements.

## Convert PDF Document Colorspace from RGB to Grayscale

We received a requirement to [convert a PDF document colorspace from RGB to Grayscale][2], so that it would be faster while printing those PDF files. Also when a file is converted to Grayscale, the size of the document is reduced but with this change, the quality of the document may drop. The feature is already supported in Aspose.Pdf for .NET version and now it is also supported in Java version of Aspose.Pdf i.e. Aspose.Pdf for Java 11.2.0. In order to accomplish this requirement, the following code snippet can be used.

## Add background image of submit button

One of the customers wants to set the background image for submit button over form. We can set background image of submit button by using addImage() method in DOM approach as following.

```
Document doc = new Document("PdfWithAcroForm.pdf");
com.aspose.pdf.ButtonField button = (com.aspose.pdf.ButtonField) doc.getForm().get_Item("buttonField");
java.awt.image.BufferedImage img = ImageIO.read(new File("image.png"));
button.addImage(img);
doc.save("output.pdf");
```

## Other Enhancements & Improvements

The other most notable enhancements in this release are as follow:

*   [How to add Grouped ChekBoxes.][3]
*   [Convert XML file to PDF.][4]
*   How to add transparent text in PDF.
*   [How to add drawing with transparent Color.][5]

## Aspose.Pdf for Java Resources

The following resources will help you work with Aspose.Pdf for Java:

*   [Home page for Aspose.PDF for Java][6]
*   [Download Aspose.PDF for Java][7]
*   [Aspose.PDF product family forum][8] – Post your technical questions and queries, or any other problem you faced while running Aspose.PDF APIs.
*   [Aspose.PDF for Java online documentation][9] – help documentation and API reference documents.
*   [Enable Blog Subscription][10] – Do not limit yourself, you can keep yourself updated with the latest news on Aspose.Pdf APIs, new features, fixes and other API related topics by subscribing to Aspose.PDF blog.
*   [Aspose.PDF for Java Examples][11] – We have published our code examples on the social coding website GitHub.com. Anyone could explore the code examples for learning purposes.




[1]: https://downloads.aspose.com/pdf/java
[2]: https://docs.aspose.com/
[3]: http://docs.aspose.com/display/pdfjava/How+to+add+Grouped+CheckBoxes
[4]: https://docs.aspose.com/display/pdfjava/Home
[5]: http://docs.aspose.com/display/pdfjava/How+to+add+drawing+with+transparent+Color
[6]: http://products.aspose.com/pdf/java
[7]: https://downloads.aspose.com/pdf/java
[8]: https://forum.aspose.com/c/pdf
[9]: http://docs.aspose.com/display/pdfjava/Home
[10]: https://blog.aspose.com/category/pdf/
[11]: https://github.com/aspose-pdf/Aspose.PDF-for-Java





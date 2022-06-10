---
title: 'Support for Metered License and Inter-File Format Conversion'
date: Sun, 22 Jul 2018 23:50:19 +0000
draft: false
url: /2018/07/22/support-for-metered-license-and-inter-file-format-conversion/
author: Asad Ali
summary: ''
tags: ['Asad Ali']
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/aspose-Pdf-for-Android_100.png" alt="">}}


We at Aspose are honored to announce long awaited release of [Aspose.PDF for Android via Java 18.6][1]. This version of the API is now available for download and to be used in Android Applications. New features have been introduced as well as some fixes have also been made to the existing features of the API in this release. A detailed overview of enhancements and improvements in this release has been given in [release notes page][2] of the API. If you are planning to download and use latest version of the API, we strongly recommend you to please check Public API Changes section in release notes to know which new classes have been added and what changes have been made to existing methods and classes of the API. Please check following major features included in latest version.

## Create Named Destination in Existing PDF Documents

One of the exciting features introduced in this release is to create named destination in existing PDF documents. If you want to change a destination without effecting any internal/external link inside PDF document, you have to use named destinations. Since, creating named destinations is very tedious task when you are doing it manually, you can automate it using latest release of the API. Following example shows the implementation of the feature:

```
Document doc = new Document(getInputPath("input.pdf"));
PdfAction act = doc.getOutlines().getFirst().getAction();
NamedDestinationCollection destination = doc.getNamedDestinations();
IAppointment app1 = destination.get_Item("bm305");
IAppointment app2 = destination.get_Item("added");
destination.set_Item("aaa", new XYZExplicitDestination(1, 0, 0, 0.5));
String[] k = destination.getNames();
LinkAnnotation link = new LinkAnnotation(doc.getPages().get_Item(1), 
new Rectangle(0, 0, 100, 100));
GoToAction action = new GoToAction();
action.setDestination(new NamedDestination(doc, "aaa"));
link.setAction(action);
doc.getPages().get_Item(1).getAnnotations().add(link);
doc.save(getOutputPath("output.pdf"));
```

## Metered License Support

You can now take advantages of Metered License as latest release of Aspose.PDF for Android via Java 18.6 includes its support. In order to apply metered license in your application, you can use following code snippet:

```
Metered matered = new Metered();
matered.setMeteredKey(publicKey, privateKey);
Assert.assertTrue(Document.isLicensed()
```

## PDF to PDF/A Conversion

Expanding inter-file format conversion features of the API, a new output format has also been added to the API. Now you can generate PDF/A compliant documents from simple PDFs. In order to convert PDF into PDF/A format, please check following code snippet:

```
Document doc = new Document(inFile);
OutputStream logStream = 
new FileOutputStream(getOutputPath("log.xml"));
doc.convert(logStream, PdfFormat.PDF_A_1A, 
ConvertErrorAction.Delete);
doc.save(outFile);
```

## Miscellaneous Fixes

Along with the new features described above, some improvement and fixes have also been made to the API regarding font handling, stamp annotations and licensing feature. 

Please visit the following links for information regarding latest release of [Aspose.PDF for Android via Java][3] and [Release Notes][4] section. In case you have any question about Aspose.PDF for Android via Java, you can post your inquiry in [Aspose.PDF forums][5]. We will be more than happy to assist you there.

*   [Homepage for Aspose.PDF for Android via Java][6]
*   [Download Aspose.PDF for Android via Java][7]
*   [Aspose.PDF product family forum][8]– Post your technical questions and queries, or any other problem you face while running Aspose.PDF APIs.
*   [Aspose.PDF for Android via Java online documentation][9]– Help documentation on using Aspose.PDF for Android via Java API.
*   [Enable Blog Subscription][10]– Do not limit yourself, you can keep yourself updated with the latest news on Aspose.PDF APIs, new features, fixes and other API related topics by subscribing to Aspose.PDF blog.




[1]: https://artifact.aspose.com/webapp/#/artifacts/browse/tree/General/repo/com/aspose/aspose-pdf/18.6
[2]: https://docs.aspose.com/pdf/java/aspose-pdf-for-android-via-java-18-6-release-notes/
[3]: https://artifact.aspose.com/webapp/#/artifacts/browse/tree/General/repo/com/aspose/aspose-pdf/18.6
[4]: https://docs.aspose.com/pdf/java/aspose-pdf-for-android-via-java-18-6-release-notes/
[5]: https://forum.aspose.com/c/pdf
[6]: https://products.aspose.com/pdf/android-java
[7]: https://artifact.aspose.com/webapp/#/artifacts/browse/tree/General/repo/com/aspose/aspose-pdf/18.6
[8]: https://forum.aspose.com/c/pdf
[9]: https://docs.aspose.com/pdf/java/
[10]: https://blog.aspose.com/category/aspose-products/aspose-pdf-product-family/





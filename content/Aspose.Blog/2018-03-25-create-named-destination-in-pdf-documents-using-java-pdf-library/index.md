---
title: 'Create Named Destination in Existing PDF Documents using Java'
date: Sun, 25 Mar 2018 21:28:55 +0000
draft: false
url: /2018/03/25/create-named-destination-in-pdf-documents-using-java-pdf-library/
author: Asad Ali
summary: ''
tags: ['Asad Ali', 'Create Named Destination in PDF using Java']
categories: ['Aspose.PDF Product Family']
---



{{< figure align=center src="images/aspose-Pdf-for-Java.png" alt="">}}


We at Aspose are pleased to announce a new version of Aspose.PDF for Java. As per the regular monthly release process, [Aspose.PDF for Java 18.2][1] has been released and available for download on our [Maven][2] Repository. [Aspose.PDF for Java 18.2][3] is a balancing release in which we have ported features from Aspose.PDF for .NET 18.2 API, in order to offer the same set of features for both .NET and Java platforms. In order to have a look at what is new in this release of the API, we recommend you to visit [release notes][4] page of Aspose.PDF for Java 18.2. However, the following are some features that we would like to highlight.

## Create Named Destination in Existing PDF Documents using Java

With Aspose.PDF for Java 18.2, you can now create named destinations programmatically in your Java Application. We have implemented [getNamedDestinations()][5] method for [com.aspose.pdf.Document][6] Class, which allows you to manipulate Named Destinations in existing PDF documents. [NamedDestinationCollection][7] has the following properties:

*   public IAppointment get\_Item(String name); // Gets destination by its name
*   public void set\_Item(String name, IAppointment value); // Sets destination by its name
*   public int getCount(); // Returns count of the destinations.
*   public void remove(String name); // Removes destination by its name.
*   public void add(String name, IAppointment appointment); // Adds new named destination.

The following code snippet demonstrates the usage of **getNamedDestinations()** method:

```
Document pdf = new Document();
// Create document with 100 pages
for (int i = 1; i <= 100; i++)
{
 Page page = pdf.getPages().add();
 page.addStamp(new com.aspose.pdf.TextStamp("Page " + i));
 // Named Destinations for every page
 pdf.getNamedDestinations().add("Page" + i, <br>new com.aspose.pdf.XYZExplicitDestination(i, 0, 600, 0.5));
}
for (int i = 1; i <= 100; i++)
{<br> // Create outlines (two outlines for every page)
 com.aspose.pdf.OutlineItemCollection item1 = new <br>com.aspose.pdf.OutlineItemCollection(pdf.getOutlines());
 item1.setDestination (new <br>com.aspose.pdf.NamedDestination(pdf, "Page" + i));
 item1.setTitle ("Page  " + i + "(1)");
 pdf.getOutlines().add(item1);

 com.aspose.pdf.OutlineItemCollection item2 = <br>new com.aspose.pdf.OutlineItemCollection(pdf.getOutlines());
 item2.setDestination (new <br>com.aspose.pdf.NamedDestination(pdf, "Page" + i));
 item2.setTitle ("Page  " + i + "(2)");
 pdf.getOutlines().add(item2);
}
// Update on of the named destinations
pdf.getNamedDestinations().set_Item("Page50", <br>new com.aspose.pdf.XYZExplicitDestination(50, 0, 100, 2));
pdf.save(myDir+"result.pdf");
```

## Miscellaneous Fixes

As it is always recommended to use the latest release of our API’s as they include the latest features/improvements and fixes related to issues reported in earlier released versions. Therefore, please download the latest release of [Aspose.PDF for Java 18.2][8].

*   [Home page for Aspose.PDF for Java][9]
*   [Download Aspose.PDF for Java][10]
*   [Aspose.PDF product family forum][11]– Post your technical questions and queries, or any other problem you faced while running Aspose.PDF APIs.
*   [Aspose.PDF for Java online documentation][12]– Help documentation and API reference documents.
*   [Enable Blog Subscription][13]– Do not limit yourself, you can keep yourself updated with the latest news on Aspose.PDF APIs, new features, fixes, and other API related topics by subscribing to Aspose.PDF blog.




[1]: http://maven.aspose.com/repository/simple/ext-release-local/com/aspose/aspose-pdf/18.2/
[2]: http://maven.aspose.com/repository/simple/ext-release-local/com/aspose/
[3]: http://maven.aspose.com/repository/simple/ext-release-local/com/aspose/aspose-pdf/18.2/
[4]: https://docs.aspose.com/display/pdfjava/Aspose.PDF+for+Java+18.2+Release+Notes
[5]: https://apireference.aspose.com/java/pdf/com.aspose.pdf/IDocument#getNamedDestinations--
[6]: https://apireference.aspose.com/java/pdf/com.aspose.pdf/Document
[7]: https://apireference.aspose.com/java/pdf/com.aspose.pdf.nameddestinations/NamedDestinationCollection
[8]: http://maven.aspose.com/repository/simple/ext-release-local/com/aspose/aspose-pdf/18.2/
[9]: https://products.aspose.com/pdf/java
[10]: http://maven.aspose.com/repository/simple/ext-release-local/com/aspose/aspose-pdf/18.2/
[11]: https://forum.aspose.com/c/pdf
[12]: https://docs.aspose.com/display/pdfjava/Home
[13]: https://blog.aspose.com/category/aspose-products/aspose-pdf-product-family/




